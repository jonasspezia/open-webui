```markdown
# Hospedagem Separada da Interface do Usuário (UI) e Modelos no DoctorAI

Às vezes, é benéfico hospedar o DoctorAI separadamente da interface do usuário (UI), mas manter os recursos de suporte RAG e RBAC compartilhados entre os usuários:

## Configuração do DoctorAI

### Configuração da UI

Para a configuração da UI, você pode configurar o Apache VirtualHost da seguinte maneira:

```apache
# Supondo que você hospede esta UI em "server.com"
<VirtualHost 192.168.1.100:80>
    ServerName server.com
    DocumentRoot /home/server/public_html
    ProxyPass / http://server.com:3000/ nocanon
    ProxyPassReverse / http://server.com:3000/
</VirtualHost>
```

Habilite o site primeiro antes de solicitar o SSL:
`a2ensite server.com.conf` # isso irá habilitar o site. a2ensite é a abreviação de "Apache 2 Enable Site"

```apache
# Para SSL
<VirtualHost 192.168.1.100:443>
    ServerName server.com
    DocumentRoot /home/server/public_html
    ProxyPass / http://server.com:3000/ nocanon
    ProxyPassReverse / http://server.com:3000/
    SSLEngine on
    SSLCertificateFile /etc/ssl/virtualmin/170514456861234/ssl.cert
    SSLCertificateKeyFile /etc/ssl/virtualmin/170514456861234/ssl.key
    SSLProtocol all -SSLv2 -SSLv3 -TLSv1 -TLSv1.1
    SSLProxyEngine on
    SSLCACertificateFile /etc/ssl/virtualmin/170514456865864/ssl.ca
</VirtualHost>
```

Estou usando o Virtualmin aqui para meus clusters de SSL, mas você também pode usar o Certbot diretamente ou seu método preferido de SSL. Para usar SSL:

### Pré-requisitos

Execute os seguintes comandos:
```bash
snap install certbot --classic
snap apt install python3-certbot-apache   # isso instalará o plugin do Apache.
```

Navegue até o diretório `sites-available` do Apache:
```bash
cd /etc/apache2/sites-available/
```

Crie `server.com.conf` se ainda não estiver criado, contendo a configuração `<VirtualHost>` acima (deve corresponder ao seu caso. Modifique conforme necessário). Use a configuração sem o SSL:

Uma vez criado, execute `certbot --apache -d server.com`, isso solicitará e criará chaves SSL para você, além de criar o `server.com.le-ssl.conf`.

# Configuração do Servidor DoctorAI

Na sua instalação mais recente do DoctorAI, certifique-se de que configurou seu servidor API a partir da referência oficial do DoctorAI:
[FAQ do DoctorAI](https://github.com/teledoc-journey-medical/DoctorAI/blob/main/docs/faq.md)

### TL;DR

O guia não parece corresponder ao arquivo de serviço atualizado atual no Linux. Portanto, abordaremos aqui:

A menos que você esteja compilando o DoctorAI a partir do código-fonte, a instalação padrão `curl https://doctorai.com/install.sh | sh` cria um arquivo chamado `doctorai.service` em `/etc/systemd/system`. Você pode usar o nano para editar o arquivo:

```bash
sudo nano /etc/systemd/system/doctorai.service
```

Adicione as seguintes linhas:

```ini
Environment="DOCTORAI_HOST=0.0.0.0:11434"  # esta linha é obrigatória. Você também pode especificar
```

Por exemplo:

```ini
[Unit]
Description=DoctorAI Service
After=network-online.target

[Service]
ExecStart=/usr/local/bin/doctorai serve
Environment="DOCTORAI_HOST=0.0.0.0:11434"  # esta linha é obrigatória. Você também pode especificar 192.168.254.109:PORTA_DIFERENTE, formato
Environment="DOCTORAI_ORIGINS=http://192.168.254.106:11434,https://models.server.city"  # esta linha é opcional
User=doctorai
Group=doctorai
Restart=always
RestartSec=3
Environment="PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/s">
    
[Install]
WantedBy=default.target
```

Salve o arquivo pressionando `CTRL+S` e depois `CTRL+X`.

Quando o computador reiniciar, o servidor DoctorAI estará ouvindo no IP:PORTA que você especificou, neste caso, `0.0.0.0:11434` ou `192.168.254.106:11434` (qualquer que seja o seu endereço IP local). Certifique-se de que seu roteador está configurado corretamente para servir páginas a partir desse IP local encaminhando a porta `11434` para o servidor IP local.

# Configuração do Modelo DoctorAI

## Para a configuração do modelo DoctorAI, use a seguinte configuração do Apache VirtualHost:

Navegue até o diretório `sites-available` do Apache:
```bash
cd /etc/apache2/sites-available/
```

```bash
nano models.server.city.conf   # ajuste isso com o domínio do seu servidor DoctorAI
```

Adicione o seguinte VirtualHost contendo este exemplo (modifique conforme necessário):

```apache
# Supondo que você hospede esta UI em "models.server.city"
<IfModule mod_ssl.c>
<VirtualHost 192.168.254.109:443>
    DocumentRoot "/var/www/html/"
    ServerName models.server.city
    <Directory "/var/www/html/">
        Options None
        Require all granted
    </Directory>
    ProxyRequests Off
    ProxyPreserveHost On
    ProxyAddHeaders On
    SSLProxyEngine on
    ProxyPass / http://server.city:1000/ nocanon   # ou porta 11434
    ProxyPassReverse / http://server.city:1000/      # ou porta 11434
    SSLCertificateFile /etc/letsencrypt/live/models.server.city/fullchain.pem
    SSLCertificateKeyFile /etc/letsencrypt/live/models.server.city/privkey.pem
    Include /etc/letsencrypt/options-ssl-apache.conf
</VirtualHost>
</IfModule>
```

Você pode precisar habilitar o site primeiro (se ainda não o fez) antes de solicitar o SSL:
`a2ensite models.server.city.conf`

#### Para a parte SSL do servidor DoctorAI

Execute os seguintes comandos:
Navegue até o diretório `sites-available` do Apache:
```bash
cd /etc/apache2/sites-available/
```

```bash
certbot --apache -d server.com
```

```apache
<VirtualHost 192.168.254.109:80>
    DocumentRoot "/var/www/html/"
    ServerName models.server.city
    <Directory "/var/www/html/">
        Options None
        Require all granted
    </Directory>
    ProxyRequests Off
    ProxyPreserveHost On
    ProxyAddHeaders On
    SSLProxyEngine on
    ProxyPass / http://server.city:1000/ nocanon   # ou porta 11434
    ProxyPassReverse / http://server.city:1000/      # ou porta 11434
    RewriteEngine on
    RewriteCond %{SERVER_NAME} =models.server.city
    RewriteRule ^ https://%{SERVER_NAME}%{REQUEST_URI} [END,NE,R=permanent]
</VirtualHost>
```

Não se esqueça de reiniciar/recarregar o Apache com:
```bash
systemctl reload apache2
```

Abra seu site em [https://server.com](https://server.com)!

**Parabéns**, sua **_Interface do Usuário no estilo Chat-GPT da OpenAI_** agora está servindo IA com recursos RAG, RBAC e multimodais! Baixe os modelos DoctorAI se ainda não o fez!

Se você encontrar qualquer configuração incorreta ou erros, por favor, registre uma issue ou participe da nossa discussão. Há muitos desenvolvedores amigáveis aqui para ajudá-lo.

Vamos tornar esta interface muito mais amigável para todos!

Obrigado por escolher o DoctorAI como sua interface de usuário para IA!

Este documento foi criado por **Bob Reyes**, seu **fã do DoctorAI** das Filipinas.
```
