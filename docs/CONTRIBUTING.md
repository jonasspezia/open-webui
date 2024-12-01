# Contribuindo para DoctorAI
🚀 **Bem-vindo, Contribuidores!** 🚀  
Agradecemos profundamente o seu interesse em contribuir para o DoctorAI. Este documento está aqui para guiá-lo através do processo, garantindo que suas contribuições aprimorem o projeto de maneira eficaz. Vamos tornar o DoctorAI ainda melhor, juntos!

## 📌 Pontos Principais
### 🧑‍⚕️ DoctorAI vs. Tecnologia Base
É crucial distinguir entre DoctorAI e as tecnologias que a suportam:
- **DoctorAI** foca em fornecer uma interface intuitiva e responsiva para interações médicas.
- As **Tecnologias Base** (como IA e plataformas de telemedicina) são os fundamentos que alimentam essas interações.
Se sua questão ou contribuição refere-se diretamente à tecnologia subjacente, por favor direcione-a para o repositório apropriado. O repositório do DoctorAI está dedicado apenas ao aspecto da interface do usuário.

### 🚨 Relatando Problemas
Percebeu algo incorreto? Tem uma ideia? Verifique nossa [aba de Issues](https://github.com/teledoc-journey-medical/DoctorAI/issues) para ver se já foi reportado ou sugerido. Caso contrário, sinta-se à vontade para abrir uma nova issue. Ao reportar um problema, por favor siga nossos templates de issue. Esses templates são projetados para garantir que todos os detalhes necessários sejam fornecidos desde o início, permitindo que abordemos suas preocupações de forma mais eficiente.

> [!IMPORTANT]
>
> - **Conformidade com o Template:** Esteja ciente de que a não utilização do template fornecido, ou a não inclusão das informações solicitadas, provavelmente resultará no fechamento da sua issue sem consideração adicional. Essa abordagem é essencial para manter a gerenciabilidade e integridade do rastreamento de issues.
> - **Detalhamento é Fundamental:** Para garantir que sua issue seja entendida e possa ser efetivamente resolvida, é imperativo incluir detalhes abrangentes. As descrições devem ser claras, incluindo passos para reproduzir, resultados esperados e resultados atuais. A falta de detalhes suficientes pode dificultar nossa capacidade de resolver seu problema.

### 🧭 Escopo de Suporte
Notamos um aumento nas issues que não estão diretamente relacionadas ao DoctorAI, mas sim ao ambiente em que ele é executado, especialmente configurações de Docker. Embora nos esforcemos para suportar a implantação com Docker, entender os fundamentos do Docker é crucial para uma experiência tranquila.
- **Suporte à Implantação com Docker**: DoctorAI suporta implantação via Docker. Assume-se familiaridade com Docker. Para noções básicas de Docker, por favor, consulte a [documentação oficial do Docker](https://docs.docker.com/get-started/overview/).
- **Configurações Avançadas**: Configurar proxies reversos para HTTPS e gerenciar implantações com Docker requer conhecimento fundamental. Existem inúmeros recursos online disponíveis para aprender essas habilidades. Garantir que você possui esse conhecimento aprimorará grandemente sua experiência com o DoctorAI e projetos semelhantes.

## 💡 Contribuindo
Deseja contribuir? Ótimo! Veja como você pode ajudar:

### 🛠 Pull Requests
Recebemos com entusiasmo pull requests. Antes de submeter uma, por favor:
1. Abra uma discussão sobre suas ideias [aqui](https://github.com/teledoc-journey-medical/DoctorAI/discussions/new/choose).
2. Siga os padrões de codificação do projeto e inclua testes para novas funcionalidades.
3. Atualize a documentação conforme necessário.
4. Escreva mensagens de commit claras e descritivas.
5. É essencial completar seu pull request de maneira oportuna. Nós trabalhamos rapidamente, e ter PRs pendentes por muito tempo não é viável. Se você não conseguir finalizar dentro de um prazo razoável, poderemos fechá-lo para manter o projeto avançando.

### 📚 Documentação & Tutoriais
Ajude-nos a tornar o DoctorAI mais acessível melhorando a documentação, escrevendo tutoriais ou criando guias sobre como configurar e otimizar a interface do usuário.

### 🌐 Traduções e Internacionalização
Ajude-nos a disponibilizar o DoctorAI para um público mais amplo. Nesta seção, orientaremos você através do processo de adicionar novas traduções ao projeto.
Usamos arquivos JSON para armazenar traduções. Você pode encontrar os arquivos de tradução existentes no diretório `src/lib/i18n/locales`. Cada diretório corresponde a um idioma específico, por exemplo, `pt-BR` para Português (Brasil), `es-ES` para Espanhol (Espanha) e assim por diante. Você pode referir-se aos [Códigos de Idioma ISO 639](http://www.lingoes.net/en/translator/langcode.htm) para encontrar o código apropriado para um idioma específico.
Para adicionar um novo idioma:
- Crie um novo diretório no caminho `src/lib/i18n/locales` com o código de idioma apropriado como nome. Por exemplo, se você está adicionando traduções para Português (Portugal), crie um novo diretório chamado `pt-PT`.
- Copie os arquivos de tradução em inglês americano (do diretório `en-US` em `src/lib/i18n/locales`) para este novo diretório e atualize os valores das strings no formato JSON de acordo com o seu idioma. Certifique-se de preservar a estrutura do objeto JSON.
- Adicione o código do idioma e seu respectivo título ao arquivo de idiomas em `src/lib/i18n/locales/languages.json`.

### 🤔 Perguntas & Feedback
Tem perguntas ou feedback? Junte-se à nossa [comunidade no Discord](https://discord.gg/5rJgQTnV4s) ou abra uma issue. Estamos aqui para ajudar!

## 🙏 Obrigado!
Suas contribuições, grandes ou pequenas, têm um impacto significativo no DoctorAI. Estamos entusiasmados para ver o que você trará para o projeto!
Juntos, vamos criar uma ferramenta ainda mais poderosa para a comunidade médica. 🌟
