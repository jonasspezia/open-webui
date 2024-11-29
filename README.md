# DoctorAI 👨‍⚕️🤖

[![Teledoc]([https://img.shields.io/badge/Discord-DoctorAI-blue?logo=discord&logoColor=white](https://i.postimg.cc/QCTzLfdH/wredccds.png))](https://teledocmedical.com)

O **DoctorAI** é uma inteligência artificial inovadora desenvolvida para médicos, dentistas, profissionais da saúde e acadêmicos. Nossa solução ajuda na pesquisa, economizando tempo e recursos, ao gerar e resumir evidências científicas com links de referência de bases confiáveis. Para mais informações, não deixe de conferir nossa [Documentação do DoctorAI](https://docs.teledocmedical.ai/).

![Demonstração do DoctorAI](./demo.gif)

## Principais Recursos do DoctorAI ⭐

- 🧠 **Pesquisa Inteligente e Rápida**: Realize pesquisas médicas eficientes com a ajuda da inteligência artificial, obtendo resultados relevantes em menos tempo.

- 📄 **Geração e Resumo de Evidências**: O DoctorAI gera e resume artigos científicos, facilitando o acesso às informações essenciais.

- 🔗 **Referências Confiáveis**: Todos os resumos incluem links para as fontes originais e bases de dados confiáveis, garantindo a qualidade das informações.

- 💾 **Armazenamento Seguro de Pesquisas**: Salve e organize suas pesquisas para acesso futuro, mantendo um histórico completo de estudos.

- 📱 **Interface Amigável e Responsiva**: Utilize o DoctorAI em diversos dispositivos, com uma interface pensada para facilitar a navegação e o uso.

- 🌎 **Multidisciplinaridade**: Suporte para diversas áreas da saúde, incluindo Medicina, Odontologia, Enfermagem, Fisioterapia, Farmácia e mais.

- 🔐 **Privacidade e Segurança**: Garantimos a segurança dos seus dados e confidencialidade das suas pesquisas, seguindo rigorosos padrões de proteção de informações.

- 🤝 **Integração Facilmente Personalizável**: Possibilidade de integração com sistemas de instituições de saúde e educação, adaptando-se às necessidades específicas de cada usuário ou organização.

- 💡 **Apoio ao Ensino e Aprendizado**: Ideal para acadêmicos, auxiliando na elaboração de trabalhos, estudos de caso e aprofundamento de conteúdos.

- 🌟 **Atualizações e Melhoria Contínua**: Estamos comprometidos em aprimorar constantemente o DoctorAI, adicionando novos recursos e melhorias baseadas no feedback dos usuários.

Quer saber mais sobre os recursos do DoctorAI? Confira a nossa [Documentação do DoctorAI](https://docs.teledocmedical.ai/) para uma visão detalhada!

## 🔗 Também Conheça o Lacia Vision LLM!

Explore nosso produto complementar, o **Lacia Vision LLM**, uma inteligência artificial multimodal que analisa e avalia acadêmicos por vídeo e voz em tempo real, gerando feedback avaliativo sem a necessidade da presença de um professor. O Lacia Vision LLM está revolucionando a educação na área da saúde! 🚀

## Como Instalar 🚀

### Instalação via Python pip 🐍

O DoctorAI pode ser instalado usando o pip, o instalador de pacotes do Python. Antes de iniciar, certifique-se de que está usando o **Python 3.11** para evitar problemas de compatibilidade.

1. **Instale o DoctorAI**:
   Abra o terminal e execute o comando:

   ```bash
   pip install doctorai
   ```

2. **Executando o DoctorAI**:
   Após a instalação, execute:

   ```bash
   doctorai start
   ```

   Isso iniciará o servidor do DoctorAI, que pode ser acessado em [http://localhost:8080](http://localhost:8080).

### Início Rápido com Docker 🐳

> **Nota**: Em alguns ambientes Docker, configurações adicionais podem ser necessárias. Se encontrar problemas de conexão, consulte nosso guia detalhado na [Documentação do DoctorAI](https://docs.teledocmedical.ai/).

> **Aviso**: Ao utilizar o Docker para instalar o DoctorAI, certifique-se de incluir `-v doctorai:/app/backend/data` no comando Docker. Isso é crucial para garantir que seu banco de dados seja montado corretamente e evitar perda de dados.

> **Dica**: Se deseja utilizar o DoctorAI com suporte a GPU, use nossas imagens oficiais marcadas como `:cuda`. Para habilitar o CUDA, instale o [Nvidia CUDA container toolkit](https://docs.nvidia.com/dgx/nvidia-container-runtime-upgrade/) no seu sistema Linux/WSL.

#### Instalação com Configuração Padrão

```bash
docker run -d -p 3000:8080 -v doctorai:/app/backend/data --name doctorai --restart always ghcr.io/teledoc/doctorai:latest
```

Após a instalação, acesse o DoctorAI em [http://localhost:3000](http://localhost:3000). Aproveite! 😄

### Outros Métodos de Instalação

Oferecemos várias alternativas de instalação, incluindo métodos sem Docker e uso de Docker Compose. Visite nossa [Documentação do DoctorAI](https://docs.teledocmedical.ai/) ou junte-se à nossa [Comunidade no Discord](https://teledocmedical.com) para obter mais orientações.

### Solução de Problemas

Enfrentando problemas de conexão? Nossa [Documentação do DoctorAI](https://docs.teledocmedical.ai/) está pronta para ajudar. Para suporte adicional e para fazer parte da nossa comunidade, visite o [Discord do DoctorAI](https://teledocmedical.com).

### Mantendo Sua Instalação Docker Atualizada

Para atualizar sua instalação local do Docker para a versão mais recente, utilize o [Watchtower](https://containrrr.dev/watchtower/):

```bash
docker run --rm --volume /var/run/docker.sock:/var/run/docker.sock containrrr/watchtower --run-once doctorai
```

No final do comando, substitua `doctorai` pelo nome do seu contêiner se for diferente.

Consulte nosso Guia de Atualização disponível na [Documentação do DoctorAI](https://docs.teledocmedical.ai/).

## O Que Vem a Seguir? 🌟

Descubra os próximos recursos e planos em nosso roadmap disponível na [Documentação do DoctorAI](https://docs.teledocmedical.ai/).

## Licença 📜

Este projeto está licenciado sob a [Licença MIT](LICENSE) - veja o arquivo [LICENSE](LICENSE) para mais detalhes. 📄

## Suporte 💬

Tem perguntas, sugestões ou precisa de assistência? Abra uma issue ou junte-se à nossa [Comunidade no Discord do DoctorAI](https://teledocmedical.com/) para entrar em contato conosco! 🤝

---

Criado por [Dr. Jonas Spezia](https://github.com/jonasspezia) - Vamos tornar o DoctorAI ainda mais incrível juntos! 💪
