Registro de alterações

Todas as alterações relevantes neste projeto serão documentadas neste arquivo.

O formato é baseado em Keep a Changelog,
e este projeto adere à Semântica de Versionamento.

[0.4.7] - 2024-12-01
Adicionado

✨ Autocompletar entrada de prompt: Digite um prompt e deixe a IA sugerir e completar suas entradas de forma inteligente. Basta pressionar 'Tab' ou deslizar para a direita no celular para confirmar. Disponível apenas com entrada de texto formatado (configuração padrão). Desative nas configurações de administrador para controle total.

🌍 Melhorias nas traduções: Localização aprimorada para vários idiomas, garantindo uma experiência mais refinada e acessível para usuários internacionais.

Corrigido

🛠️ Problema de exportação de ferramentas: Resolvido um problema crítico em que a exportação de ferramentas não estava funcionando, restaurando os recursos de exportação contínua.

🔗 Registro de ID do modelo: Corrigido um problema em que os IDs do modelo não estavam sendo registrados corretamente no editor de modelo, garantindo a configuração e o rastreamento confiáveis do modelo.

🖋️ Expansão automática de área de texto: Corrigido um bug em que as áreas de texto não se expandiam automaticamente em determinados navegadores, melhorando a usabilidade para entradas de várias linhas.

🔧 Endpoint de incorporação do Ollama: Endereço do mau funcionamento do endpoint /ollama/embed, garantindo desempenho e funcionalidade consistentes.

Alterado

🎨 Estilo da base de conhecimento: Visuais refinados da base de conhecimento para uma aparência mais limpa e moderna, preparando o terreno para novos aprimoramentos em versões futuras.

[0.4.6] - 2024-11-26
Adicionado

🌍 Melhorias nas traduções: Várias traduções de idiomas aprimoradas para tornar o DoctorAI mais acessível e amigável em todo o mundo.

Corrigido

✏️ Bug de deslocamento da área de texto: Resolvido o problema em que a área de texto se deslocava inesperadamente, garantindo uma experiência de digitação mais suave.

⚙️ Modal de configuração do modelo: Corrigido o problema em que o modal de configuração dos modelos introduzido em 0.4.5 não estava funcionando para alguns usuários.

🔍 Suporte a consultas legadas: Restaurada a funcionalidade para geração de consultas personalizadas em RAG ao usar prompts legados, garantindo que os modelos padrão e personalizado agora funcionem perfeitamente.

⚡ Melhoria da confiabilidade geral: Várias pequenas correções melhoram a estabilidade da plataforma e garantem uma experiência geral mais suave em todos os fluxos de trabalho.

[0.4.5] - 2024-11-26
Adicionado

🎨 Ordem/padrões do modelo reintroduzidos: Retornada a capacidade de definir a ordem do modelo e os modelos padrão, agora configuráveis por meio de Configurações de administrador > Modelos > Configurar (ícone de engrenagem).

Corrigido

🔍 Problema de geração de consulta: Resolvido um erro na geração de consulta de pesquisa na web, aprimorando a precisão da pesquisa e garantindo fluxos de trabalho de pesquisa mais suaves.

📏 Bug de altura automática da área de texto: Corrigido um problema de layout em que a altura da entrada da área de texto estava mudando de forma imprevisível, especialmente ao editar prompts do sistema.

🔑 Autenticação Ollama: Corrigido um problema com os cabeçalhos de autorização do Ollama, garantindo autenticação confiável em todos os endpoints.

⚙️ Salvamento Min_P ausente: Resolvido um problema em que o parâmetro 'min_p' não estava sendo salvo nas configurações.

🛠️ Descrição das ferramentas: Corrigido um problema chave que omitia as descrições das ferramentas no payload das ferramentas.

[0.4.4] - 2024-11-22
Adicionado

🌐 Atualizações de tradução: Traduções atualizadas para catalão, português brasileiro, alemão e ucraniano, aprimorando ainda mais a acessibilidade da plataforma e melhorando a experiência para usuários internacionais.

Corrigido

📱 Visibilidade dos controles móveis: Resolvido um problema em que o botão de controles não era exibido na nova página de bate-papos para usuários móveis, garantindo navegação e funcionalidade mais suaves em telas menores.

📷 Problema de imagem de perfil LDAP: Corrigido um bug de integração LDAP relacionado a imagens de perfil, garantindo autenticação perfeita e uma experiência de login confiável para os usuários.

⏳ Problema de geração de consulta RAG: Resolvido um problema significativo em que a geração de consulta RAG ocorria desnecessariamente sem arquivos anexados, melhorando drasticamente a velocidade e reduzindo atrasos durante os preenchimentos de bate-papo.

Alterado

⚙️ Suporte ao emissor de eventos legado: Reintroduzida a compatibilidade com tipos de "citação" legados para emissores de eventos em ferramentas e funções, fornecendo fluxos de trabalho mais suaves e suporte mais amplo de ferramentas para os usuários.

[0.4.3] - 2024-11-21
Adicionado

📚 Citações embutidas para resultados RAG: Obtenha citações embutidas perfeitas para respostas de geração aumentada por recuperação (RAG) usando o prompt RAG padrão. Observação: este recurso suporta apenas arquivos carregados recentemente, melhorando a rastreabilidade e fornecendo clareza de origem.

🎨 Melhor suporte de entrada de texto formatado: Desfrute de formatação de texto formatado mais suave e confiável para bate-papos, aprimorando a qualidade da comunicação.

⚡ Recuperação de modelo mais rápida: Implementadas otimizações de cache para carregamento mais rápido do modelo, fornecendo um aumento perceptível de velocidade nos fluxos de trabalho. Mais melhorias estão a caminho!

Corrigido

🔗 Recurso de pipelines restaurado: Resolvido um problema crítico que antes impedia o funcionamento dos pipelines, garantindo fluxos de trabalho perfeitos.

✏️ Campo de sufixo ausente no formulário Ollama: Adicionado o campo "sufixo" ausente ao formulário de geração Ollama, aprimorando as opções de personalização.

Alterado

🗂️ "Citações" renomeadas para "Fontes": Clareza e consistência aprimoradas ao renomear o campo "citações" para "fontes" nas mensagens.

[0.4.2] - 2024-11-20
Corrigido

📁 Problema de visibilidade dos arquivos de conhecimento: Resolvido o bug que impedia a exibição de arquivos individuais em coleções de conhecimento quando referenciados com '#'.

🔗 Prefixo do endpoint OpenAI: Corrigido o problema em que certas conexões OpenAI que se desviavam da especificação oficial da API não estavam funcionando corretamente com prefixos.

⚔️ Controle de acesso ao modelo Arena: Corrigido um problema em que as configurações de controle de acesso ao modelo Arena não estavam sendo salvas.

🔧 Seletor de capacidade de uso: Corrigido o seletor de recursos de uso quebrado no editor de modelo.

[0.4.1] - 2024-11-19
Adicionado

📊 Sistema de feedback aprimorado: Introduzida uma escala de classificação detalhada de 1 a 10 para feedback junto com positivo/negativo, preparando-se para um ajuste fino do modelo mais preciso e melhorando a qualidade do feedback.

ℹ️ Descrições da ferramenta ao passar o mouse: Acesse facilmente as descrições da ferramenta passando o mouse sobre a entrada da mensagem, fornecendo um fluxo de trabalho mais suave com mais contexto ao utilizar ferramentas.

Corrigido

🗑️ Tratamento adequado de usuários excluídos: Resolvido um problema em que usuários excluídos faziam com que itens do espaço de trabalho (modelos, conhecimento, prompts, ferramentas) falhassem, garantindo o carregamento confiável do espaço de trabalho.

🔑 Criação de chave de API: Corrigido um problema que impedia os usuários de criar novas chaves de API, restaurando o gerenciamento de API seguro e contínuo.

🔗 Correção de proxy HTTPS: Corrigidos problemas de proxy HTTPS que afetavam o endpoint '/api/v1/models/', garantindo um gerenciamento de modelo mais suave e ininterrupto.

[0.4.0] - 2024-11-19
Adicionado

👥 Grupos de usuários: Agora você pode criar e gerenciar grupos de usuários, tornando a organização do usuário perfeita.

🔐 Controle de acesso baseado em grupo: Defina acesso granular a modelos, conhecimento, prompts e ferramentas com base em grupos de usuários, permitindo ambientes mais controlados e seguros.

🛠️ Permissões de usuário baseadas em grupo: Gerencie facilmente as permissões do espaço de trabalho. Conceda aos usuários a capacidade de carregar arquivos, excluir, editar ou criar bate-papos temporários, bem como definir sua capacidade de criar modelos, conhecimento, prompts e ferramentas.

🔑 Suporte LDAP: A autenticação LDAP recém-introduzida adiciona segurança robusta e escalabilidade ao gerenciamento de usuários.

🌐 Conexões compatíveis com OpenAI aprimoradas: Adicionado suporte a ID de prefixo para evitar conflitos de ID de modelo, com suporte explícito a ID de modelo para APIs sem suporte ao endpoint '/models', garantindo uma operação suave com configurações personalizadas.

🔐 Suporte a chave de API Ollama: Agora gerencie credenciais para Ollama quando definido atrás de proxies, incluindo a opção de utilizar ID de prefixo para distinção adequada em várias instâncias Ollama.

🔄 Alternância de ativação/desativação de conexão: Ative ou desative facilmente conexões OpenAI e Ollama individuais conforme necessário.

🎨 Espaço de trabalho do modelo redesenhado: Recém-redesenhado para melhorar a usabilidade para gerenciar modelos entre usuários e grupos.

🎨 Espaço de trabalho do prompt redesenhado: Uma nova interface do usuário para organizar e gerenciar prompts convenientemente.

🧩 Espaço de trabalho de funções classificadas: As funções agora são categorizadas automaticamente por tipo (Ação, Filtro, Pipe), simplificando o gerenciamento.

💻 Espaço de trabalho colaborativo redesenhado: Suporte aprimorado para vários usuários contribuindo para modelos, conhecimento, prompts ou ferramentas, melhorando a colaboração.

🔧 Ferramentas selecionadas automaticamente no editor de modelo: As ferramentas habilitadas por meio do editor de modelo agora são selecionadas automaticamente, enquanto anteriormente ele apenas dava aos usuários a opção de habilitar a ferramenta, reduzindo as etapas manuais e aumentando a eficiência.

🔔 Indicador de pesquisa na web e ferramentas: Uma indicação clara agora mostra quando a pesquisa na web ou as ferramentas estão ativas, reduzindo a confusão.

🔑 Alternar autenticação de chave de API: Reforce a segurança habilitando ou desabilitando facilmente a opção de autenticação de chave de API para DoctorAI.

🗂️ Recuperação agêntica: Melhore a precisão do RAG por meio do pré-processamento inteligente do histórico de bate-papo para determinar as melhores consultas antes da recuperação.

📁 Texto grande como opção de arquivo: Converta opcionalmente texto colado grande em um upload de arquivo, mantendo a interface do bate-papo mais limpa.

🗂️ Alternar citações para modelos: A capacidade de desabilitar citações foi introduzida no editor de modelo.

🔍 Pesquisa de configurações do usuário: Pesquise rapidamente os campos de configurações, melhorando a facilidade de uso e a navegação.

🗣️ TTS SpeechT5 experimental: Suporte local do SpeechT5 adicionado para recursos aprimorados de texto para fala.

🔄 Redefinição unificada para modelos: Uma opção de um clique foi introduzida para redefinir e remover todos os modelos das Configurações de administrador.

🛠️ Assistente de configuração inicial: O processo de configuração agora informa explicitamente aos usuários que eles estão criando uma conta de administrador durante a configuração inicial, garantindo clareza. Anteriormente, os usuários encontravam a página de login imediatamente sem essa distinção.

🌐 Traduções aprimoradas: Várias traduções de idiomas, incluindo ucraniano, norueguês e português brasileiro, foram refinadas para melhor localização.

Corrigido

🎥 Anexos de vídeo do YouTube: Corrigidos problemas que impediam o carregamento e anexo adequados de vídeos do YouTube como arquivos.

🔄 Atualização de bate-papo compartilhado: Corrigidos problemas em que os bate-papos compartilhados não eram atualizados, melhorando a consistência da colaboração.

🔍 Correção de limite de taxa do DuckDuckGo: Resolvidos problemas com a integração de pesquisa do DuckDuckGo, aprimorando a estabilidade da pesquisa e o desempenho ao operar dentro dos limites de taxa.

🧾 Correção de relevância das citações: Ajustado o cálculo da porcentagem de relevância para citações, para que o DoctorAI reflita adequadamente a precisão de um documento recuperado em RAG, garantindo que os usuários obtenham insights mais claros sobre as fontes.

🔑 Requisito de chave de API de pesquisa Jina: Adicionada a opção de inserir uma chave de API para pesquisa Jina, garantindo uma funcionalidade suave, pois as chaves agora são obrigatórias.

Alterado

🛠️ Funções movidas para o painel de administração: Como as funções operam como plug-ins avançados, agora são acessíveis no painel de administração em vez do espaço de trabalho.

🛠️ Gerenciar conexões Ollama: A seção "Modelos" nas configurações de administrador foi movida para Configurações de administrador > "Conexões" > Conexões Ollama. Agora você pode gerenciar instâncias Ollama por meio de um modal "Gerenciar Ollama" dedicado em "Conexões", simplificando a configuração e configuração de modelos Ollama.

📊 Modelos básicos nas configurações de administrador: Os administradores agora podem encontrar todos os modelos básicos, conexões ou funções, na configuração de administrador "Modelos". A acessibilidade global do modelo pode ser habilitada ou desabilitada aqui. Os modelos são privados por padrão, exigindo atribuição explícita de permissão para acesso do usuário.

📌 Seleção de modelo fixo para novos bate-papos: O modelo escolhido em um bate-papo anterior agora persiste ao criar um novo bate-papo. Se você clicar em "Novo bate-papo" novamente na página do novo bate-papo, ele retornará ao seu modelo padrão.

🎨 Refatoração de design: Refinamentos gerais de design em toda a plataforma foram feitos, fornecendo uma experiência do usuário mais coesa e refinada.

Removido

📂 Reordenação da lista de modelos: Removida temporariamente e será reintroduzida em futuras melhorias nas configurações do grupo de usuários.

⚙️ Configuração do modelo padrão: Removida a capacidade de definir um modelo padrão para os usuários, que será reintroduzida com as configurações do grupo de usuários no futuro.

[0.3.35] - 2024-10-26
Adicionado

🌐 Atualização de tradução: Adicionados rótulos de tradução nos componentes SearchInput e CreateCollection e tradução para português brasileiro atualizada (pt-BR)

📁 Manipulação robusta de arquivos: Manipulação aprimorada de entrada de arquivos para bate-papo. Se a extração do conteúdo falhar ou estiver vazia, os usuários agora receberão um aviso claro, evitando falhas silenciosas e garantindo que você sempre saiba o que está acontecendo com seus uploads.

🌍 Suporte a novo idioma: Introduzidas traduções para húngaro e atualizadas as traduções para francês, expandindo a acessibilidade de idiomas da plataforma para uma base de usuários mais global.

Corrigido

📚 Problema de carregamento da base de conhecimento: Resolvido um bug crítico em que a base de conhecimento não estava carregando, garantindo acesso suave aos seus documentos armazenados e melhorando a recuperação de informações nos fluxos de trabalho aprimorados por RAG.

🛠️ Problema de parâmetros da ferramenta: Corrigido um erro em que as ferramentas não estavam funcionando corretamente quando os parâmetros necessários estavam ausentes, garantindo o desempenho confiável da ferramenta e conclusões de tarefas mais eficientes.

🔗 Perda de resposta mesclada em bate-papos com vários modelos: Resolvido um problema em que as respostas nos fluxos de trabalho de bate-papo com vários modelos estavam sendo excluídas após consultas de acompanhamento, melhorando a consistência e garantindo interações mais suaves entre os modelos.

[0.3.34] - 2024-10-26
Adicionado

🔧 Melhorias na exportação de feedback: Os dados do histórico de feedback agora podem ser exportados para JSON, permitindo a integração perfeita no processamento RLHF e análises adicionais.

🗂️ Carregamento lento do modelo de incorporação: A funcionalidade de pesquisa para classificação de leaderboard agora é mais eficiente, pois os modelos de incorporação são carregados lentamente apenas quando necessário, otimizando o desempenho.

🎨 Alternância de entrada de texto formatado: Os usuários agora podem voltar para a entrada de área de texto legada para bate-papo se preferirem uma entrada de texto mais simples, embora o texto formatado ainda seja o padrão até a descontinuação.

🛠️ Mecanismo aprimorado de chamada de ferramenta: Método aprimorado para analisar e chamar ferramentas, melhorando a confiabilidade e robustez das chamadas de função de ferramenta.

🌐 Melhorias na globalização: Atualizações para o suporte à internacionalização (i18n), refinando ainda mais a compatibilidade e a precisão de vários idiomas.

Corrigido

🖥️ Correção de renomeação de pasta para Firefox: Resolvido um problema persistente em que os usuários não conseguiam renomear pastas pressionando enter no Firefox, agora garantindo o gerenciamento contínuo de pastas em todos os navegadores.

🔠 Problema do divisor de texto do modelo Tiktoken: Resolvido um problema em que o divisor de texto tiktoken não estava funcionando em instalações Docker, restaurando a funcionalidade completa para edição de texto tokenizado.

💼 Problema de upload de arquivo S3: Corrigido um problema que afetava os uploads de arquivo S3, garantindo operações suaves para aqueles que armazenam arquivos no armazenamento em nuvem.

🔒 Falha de segurança de transporte estrito: Resolvida uma falha ao definir o cabeçalho Strict-Transport-Security (HSTS), melhorando a estabilidade e os aprimoramentos de segurança.

🚫 Correção de acesso booleano OIDC: Resolvido um problema com valores booleanos que não eram acessados corretamente durante logins OIDC, garantindo a confiabilidade do login.

⚙️ Comportamento de colar texto formatado: Refinado o comportamento de colar na entrada de texto formatado para torná-lo mais suave e intuitivo ao colar vários tipos de conteúdo.

🔨 Correção de exclusão de modelo para Arena: Corrigida a função de filtro que não estava excluindo modelos adequadamente da arena, melhorando o gerenciamento de modelos.

🏷️ Correção de "Prompt de geração de tags": Resolvido um problema que impedia o registro adequado de "prompts de geração de tags" personalizados, garantindo que os prompts personalizados funcionem perfeitamente.

[0.3.33] - 2024-10-24
Adicionado

🏆 Leaderboard de avaliação: Acompanhe facilmente seu desempenho por meio de um novo sistema de leaderboard em que suas classificações contribuem para uma classificação em tempo real com base no sistema Elo. Respostas de irmãos (regenerações, muitos bate-papos de modelo) são necessárias para que suas classificações contem no leaderboard. Além disso, você pode optar por compartilhar seu histórico de feedback e fazer parte do leaderboard da comunidade. Espere mais melhorias conforme refinamos o algoritmo - nos ajude a construir o melhor leaderboard da comunidade!

⚔️ Avaliação do modelo Arena: Habilite o teste A/B cego de modelos diretamente em Configurações de administrador > Avaliação para uma verdadeira comparação lado a lado. Ideal para identificar o melhor modelo para suas necessidades.

🎯 Leaderboard baseado em tópicos: Descubra classificações mais precisas com a reclassificação experimental baseada em tópicos, que ajusta as posições do leaderboard com base na similaridade de tags no feedback. Obtenha insights mais relevantes com base em tópicos específicos!

📁 Suporte a pastas para bate-papos: Organize seus bate-papos melhor agrupando-os em pastas. Arraste e solte bate-papos entre pastas e exporte-os perfeitamente para fácil compartilhamento ou análise.

📤 Importação fácil de bate-papo por arrastar e soltar: Economize tempo simplesmente arrastando e soltando exportações de bate-papo (JSON) diretamente na barra lateral para importá-las para seu espaço de trabalho - simplificado, eficiente e intuitivo!

📚 Coleção de conhecimento aprimorada: Agora você pode referenciar arquivos individuais de uma coleção de conhecimento - ideal para consultas de geração aumentada por recuperação (RAG) mais precisas e análise de documentos.

🏷️ Sistema de marcação aprimorado: As tags agora ocupam menos espaço! Utilize o novo sistema de consulta 'tag:' para gerenciar, pesquisar e organizar suas conversas de forma mais eficaz sem sobrecarregar a interface.

🧠 Marcação automática para bate-papos: Suas conversas agora são marcadas automaticamente para melhor organização, espelhando a eficiência dos títulos gerados automaticamente.

🔍 Sistema de consulta de bate-papo de back-end: A filtragem de bate-papo se tornou mais eficiente, agora tratada pelo back-end ** em vez do seu navegador, melhorando o desempenho e a precisão da pesquisa.

🎮 Playground renovado: Experimente um Playground atualizado e otimizado para testes, ajustes e experimentação mais suaves de seus modelos e ferramentas.

🧩 Divisor de texto baseado em token: Introduzindo a divisão de texto baseada em token (tiktoken), dando a você um controle mais preciso sobre como o texto é processado. Anteriormente, apenas a divisão baseada em caracteres estava disponível.

🔢 Incorporações em lote Ollama: Aproveite o novo suporte a incorporações em lote para melhorar a eficiência e o desempenho com os modelos de incorporação Ollama.

🔍 Modal aprimorado de adicionar conteúdo de texto: Desfrute de um fluxo de trabalho mais limpo e intuitivo para adicionar e curar conteúdo de conhecimento com um modal de entrada atualizado de nosso espaço de trabalho de conhecimento.

🖋️ Entrada de texto formatado para bate-papos: Torne suas entradas de bate-papo mais dinâmicas com suporte para formatação de texto formatado. Suas conversas ficaram muito mais polidas e profissionais.

⚡ Configurabilidade mais rápida do modelo Whisper: Personalize seu modelo local mais rápido Whisper diretamente do DoctorAI.

☁️ Suporte experimental S3: Habilite instâncias DoctorAI sem estado com suporte S3, aumentando consideravelmente a escalabilidade e equilibrando cargas de trabalho pesadas.

🔕 Desativar brinde de atualização: Agora você pode simplificar ainda mais seu espaço de trabalho - escolha desativar as notificações de atualização para uma experiência mais focada.

🌟 Porcentagem de relevância da citação RAG: Avalie facilmente a precisão da citação com a adição de porcentagens de relevância nos resultados RAG.

⚙️ Botão de cópia Mermaid: Os diagramas Mermaid agora vêm com um prático botão de cópia, simplificando a extração e o uso do conteúdo do diagrama diretamente em seu fluxo de trabalho.

🎨 Redesenho da IU: Redesenho principal da interface que tornará a navegação mais suave, manterá seu foco onde é importante e garantirá uma aparência moderna.

Corrigido

🎙️ Problema de parada do microfone de nota de voz: Corrigido o problema em que o microfone permanecia ativo após o término da gravação de uma nota de voz, garantindo que seu fluxo de trabalho de áudio seja executado sem problemas.

Removido

👋 Adeus tags da barra lateral: A desordem das tags da barra lateral acabou. Mudamos os botões de tag para uma filtragem de tag baseada em consulta mais eficaz para uma interface mais elegante e ágil.

[0.3.32] - 2024-10-06
Adicionado

🔢 Melhorias no espaço de trabalho: Adicionada uma contagem de exibição para modelos, prompts, ferramentas e funções no espaço de trabalho, fornecendo uma visão geral clara e um gerenciamento mais fácil.

Corrigido

🖥️ Correção de anexo da Web e do YouTube: Resolvido um problema em que anexar links da Web e vídeos do YouTube estava com mau funcionamento, garantindo integração e exibição perfeitas nos bate-papos.

📞 Ativação do modo de chamada na página inicial: Corrigido um bug em que o modo de chamada não estava operacional na página inicial.

Alterado

🔄 Refinamento do parâmetro de URL: Atualizado o parâmetro de URL 'tool_ids' para 'tools' ou 'tool-ids' para uma experiência do usuário mais intuitiva e consistente.

🎨 Atualização de estilo dos botões flutuantes: Refatorado o estilo dos botões flutuantes para se ajustar de forma inteligente ao lado esquerdo quando não há espaço suficiente à direita, melhorando a usabilidade e a estética da interface.

🔧 Acessibilidade aprimorada para botões flutuantes: Implementada a capacidade de fechar botões flutuantes com a tecla 'Esc', tornando o fluxo de trabalho mais suave e eficiente para usuários que navegam pelo teclado.

🖇️ URL de informações atualizado: Os URLs de informações agora direcionam os usuários para uma página de versão geral em vez de um URL específico da versão, garantindo o acesso aos detalhes mais recentes e relevantes, tudo em um só lugar.

📦 Atualização de dependências da biblioteca: Dependências atualizadas para garantir compatibilidade e otimização de desempenho para instalações pip.

[0.3.31] - 2024-10-06
Adicionado

📚 Recurso de conhecimento: Recurso de documentos reinventado, agora mais eficiente com uma interface do usuário melhor para organização aprimorada; inclui integração de API simplificada para geração aumentada por recuperação (RAG). Documentação detalhada em breve: https://teledocmedical.com/

🌐 Nova página inicial: Página inicial recém-projetada; alterne entre a nova interface do usuário e a interface do usuário de bate-papo clássica em Configurações > Interface para uma experiência personalizada.

📁 Modo de recuperação de documento completo: Alterne entre a recuperação de documento completo ou snippets tradicionais clicando no item do arquivo. Este modo aprimora os recursos do documento e suporta tarefas abrangentes como sumarização, utilizando todo o conteúdo em vez de RAG.

📄 Exibição de conteúdo de arquivo extraído: Visualize o conteúdo extraído diretamente clicando no item do arquivo, simplificando a análise do arquivo.

🎨 Recurso de artefatos: Renderize conteúdo da web e SVGs diretamente na interface, suportando iterações rápidas e mudanças ao vivo.

🖊️ Blocos de código editáveis: Blocos de código aprimorados agora permitem edição ao vivo diretamente na resposta LLM, com recarregamentos ao vivo suportados por artefatos.

🔧 Melhorias no bloco de código: Introduzido um botão de cópia flutuante em blocos de código para facilitar a cópia do código sem rolagem.

🔍 Pan/zoom SVG: Interação aprimorada com imagens SVG, incluindo diagramas Mermaid, por meio de novos recursos de pan e zoom.

🔍 Ações rápidas de seleção de texto: Novos botões flutuantes aparecem quando o texto é destacado nas respostas LLM, oferecendo interações mais profundas como "Fazer uma pergunta" ou "Explicar".

🗃️ Configuração do pool de banco de dados: Manipulação aprimorada do banco de dados para suportar o crescimento escalável do usuário.

🔊 Compressão de áudio experimental: Compactar arquivos de áudio para navegar em torno do limite de 25 MB para o processamento de fala para texto do OpenAI.

🔍 Incorporação de consulta: Ajustado o comportamento de incorporação para aprimorar o desempenho do sistema, não repetindo a incorporação de consulta.

💾 Otimizações de carregamento lento: Implementado o carregamento lento de grandes dependências para minimizar o uso inicial de memória, aumentando o desempenho.

🍏 Suporte a ícone de toque da Apple: Otimiza a exibição de ícones para favoritos da web em dispositivos móveis Apple.

🔽 Suporte a markdown de conteúdo expansível: Introduzindo suporte a tags 'details', 'summary' para criar seções de conteúdo expansível em markdown, facilitando a exibição de conteúdo interativo e documentação mais limpa e organizada.

Corrigido

🔘 Problema do botão de ação: Resolvido um bug em que os botões de ação não estavam funcionando, aprimorando a confiabilidade da interface do usuário.

🔄 Loop de bate-papo com vários modelos: Corrigido um problema de loop infinito em ambientes de bate-papo com vários modelos, garantindo operações de bate-papo mais suaves.

📄 Problema de exportação de PDF/TXT do bate-papo: Resolvidos problemas com a exportação de registros de bate-papo para os formatos PDF e TXT.

🔊 Problemas de chamada para texto para fala: Corrigidos problemas com as funções de texto para fala para melhorar as interações de áudio.

Alterado

⚙️ Renomeação do endpoint: Endpoints 'rag' renomeados para 'retrieval' para uma descrição de função mais clara.

🎨 Atualizações de estilo e interface: Vários refinamentos em toda a plataforma para aprimorar o apelo visual e a interação do usuário.

Removido

🗑️ 'DOCS_DIR' descontinuado: Removida a variável 'docs_dir' desatualizada em favor de soluções de gerenciamento de arquivos mais diretas, com sincronização direta do diretório de arquivos e uploads de API para uma experiência mais integrada.

[0.3.30] - 2024-09-26
Corrigido

🍞 Rejeição de brinde de atualização disponível: Experiência do usuário aprimorada, garantindo que, uma vez que a notificação de atualização disponível seja rejeitada, ela não reaparecerá por 24 horas.

📋 Dados do formulário /embed do Ollama: Ajustadas as imprecisões de integração nos dados do formulário /embed para garantir que ele corresponda perfeitamente às especificações do Ollama.

🔧 Problema de tokens de preenchimento máximo O1: Resolvidos problemas de compatibilidade com o parâmetro max_completion_tokens dos modelos o1 do OpenAI para garantir uma operação suave.

🔄 Problema de banco de dados de instalação Pip: Corrigido um problema crítico em que as alterações do banco de dados durante as instalações pip estavam revertendo e não salvando registros de bate-papo, agora garantindo a persistência e confiabilidade dos dados nas operações de bate-papo.

🏷️ Atualização da guia Renomear bate-papo: Corrigida a funcionalidade para alterar o título da guia do navegador da web simultaneamente quando um bate-papo é renomeado, mantendo os títulos das guias consistentes.

[0.3.29] - 2023-09-25
Corrigido

🔧 Melhoria na renderização KaTeX: Resolvidos casos de canto específicos na renderização KaTeX para aprimorar a exibição de notação matemática complexa.

📞 Correção do parâmetro de URL 'Call': Corrigida a funcionalidade para o parâmetro de pesquisa de URL 'call', garantindo a ativação confiável de chamadas de voz por meio de gatilhos de URL.

🔄 Correção de redefinição de configuração: Corrigido o RESET_CONFIG_ON_START para garantir que as configurações retornem ao padrão corretamente após cada inicialização, melhorando a confiabilidade no gerenciamento de configuração.

🌍 Correção do gancho de saída do filtro: Resolvidos problemas no gancho de saída do filtro, garantindo que todas as funções de filtro operem conforme o pretendido.

[0.3.28] - 2024-09-24
Corrigido

🔍 Funcionalidade de pesquisa na web: Corrigido um problema em que a opção de pesquisa na web não estava funcionando corretamente.

[0.3.27] - 2024-09-24
Corrigido

🔄 Erro de limpeza periódica resolvido: Corrigido um RuntimeError crítico relacionado à corrotina 'periodic_usage_pool_cleanup', garantindo um desempenho suave e eficiente após a instalação do pip, corrigindo um problema persistente da versão 0.3.26.

📊 Renderização LaTeX aprimorada: Renderização aprimorada para conteúdo LaTeX, aprimorando a clareza e a apresentação visual em documentos e modelos matemáticos.

[0.3.26] - 2024-09-24
Corrigido

🔄 Resolução de erro de loop de eventos: Resolvido um erro crítico em que um loop de eventos de execução ausente fazia com que 'periodic_usage_pool_cleanup' falhasse com instalações pip. Esta correção garante atualizações e instalações mais suaves e confiáveis, aprimorando a estabilidade geral do sistema.

[0.3.25] - 2024-09-24
Corrigido

🖼️ Funcionalidade de geração de imagens: Resolvido um problema em que a geração de imagens não estava funcionando, restaurando a capacidade total de criação de conteúdo visual.

⚖️ Correções de resposta de taxa: Resolvido um problema em que as respostas de taxa não estavam funcionando, garantindo que mecanismos de feedback confiáveis estejam operacionais.

[0.3.24] - 2024-09-24
Adicionado

🚀 Otimização de renderização: Desempenho de renderização de mensagens significativamente aprimorado, aprimorando a experiência do usuário e a capacidade de resposta do DoctorAI.

💖 Recurso de resposta favorita na visão geral do bate-papo: Os usuários agora podem marcar respostas como favoritas diretamente da visão geral do bate-papo, aprimorando a facilidade de recuperação e organização das respostas preferidas.

💬 Criar pares de mensagens com atalho: Implementada a criação de novos pares de mensagens usando Cmd/Ctrl+Shift+Enter, tornando a edição de conversas mais rápida e intuitiva.

🌍 Variáveis de prompt do usuário expandidas: Adicionadas variáveis de informações de dia da semana, fuso horário e idioma aos prompts do usuário para corresponder às variáveis de prompt do sistema.

🎵 Suporte aprimorado a áudio: Agora inclui suporte para arquivos 'audio/x-m4a', ampliando a compatibilidade com conteúdo de áudio na plataforma.

🔏 Parâmetro de pesquisa de URL do modelo: Adicionada a capacidade de selecionar um modelo diretamente por meio de parâmetros de URL, simplificando a navegação e o acesso ao modelo.

📄 Citações de PDF aprimoradas: As citações de PDF agora abrem na página associada, simplificando as verificações de referência e o manuseio de documentos.

🔧Uso de Redis em soquetes: Implementação de soquete aprimorada para suportar totalmente Redis, permitindo instâncias sem estado eficazes adequadas para balanceamento de carga escalável.

🌍 Transmitir respostas de modelo individuais: Permite que modelos específicos tenham configurações de streaming individualizadas, aprimorando o desempenho e a personalização.

de streaming individualizadas, aprimorando o desempenho e a personalização.

🕒 Exibir hash do modelo e carimbo de data/hora da última modificação para modelos Ollama: Fornece detalhes críticos do modelo diretamente no espaço de trabalho Modelos para rastreamento aprimorado.

❗ Notificação de informações de atualização para administradores: Garante que os administradores recebam atualizações imediatas ao fazer login, mantendo-os informados sobre as alterações mais recentes e os status do sistema.

Corrigido

🗑️ Manipulação de arquivos temporários no Windows: Corrigido um problema que causava erros ao acessar um arquivo temporário que estava sendo usado por outro processo. Ferramentas e funções agora devem funcionar conforme o esperado.

🔓 Problema de alternância de autenticação: Resolvido o mau funcionamento em que definir 'WEBUI_AUTH=False' não desabilitava a autenticação adequadamente, garantindo que a experiência do usuário e as configurações de segurança do sistema funcionem conforme configurado.

🔧 Problema de salvar como cópia para muitos bate-papos de modelo: Resolvido um erro que impedia os usuários de salvar mensagens como cópias em muitos bate-papos de modelo.

🔒 Fechamento da barra lateral no celular: Resolvido um problema em que a barra lateral móvel permanecia aberta após o engajamento do menu, melhorando a capacidade de resposta e o conforto da interface do usuário.

🛡️ Vulnerabilidade XSS de dica de ferramenta: Resolvido um problema de script entre sites (XSS) nas dicas de ferramenta, garantindo segurança aprimorada e integridade dos dados durante as interações do usuário.

Alterado

↩️ Configurações de resposta de fluxo da interface descontinuadas: Movido para parâmetros avançados para simplificar as configurações da interface e aprimorar a clareza do usuário.

⚙️ 'speedRate' renomeado para 'playbackRate': Padroniza a terminologia, melhorando a usabilidade e a compreensão nas configurações de mídia.

[0.3.23] - 2024-09-21
Adicionado

🚀 Suporte a WebSocket Redis: Capacidades aprimoradas de balanceamento de carga para configurações de várias instâncias, promovendo melhor desempenho e confiabilidade no DoctorAI.

🔧 Controles de bate-papo ajustáveis: Introduzidos controles de bate-papo com largura ajustável, permitindo uma interface do usuário personalizada e mais confortável.

🌎 Atualizações i18n: Melhoria e atualização das traduções para chinês.

Corrigido

🌐 Problema de descarregamento do modelo de tarefa: Modificada a manipulação de tarefas para usar o endpoint /api/chat do Ollama em vez do endpoint compatível com OpenAI, garantindo que os modelos permaneçam carregados e prontos com parâmetros personalizados, minimizando atrasos na execução da tarefa.

📝 Correção de geração de título para APIs compatíveis com OpenAI: Resolvido um problema que impedia a geração de títulos, aprimorando a consistência e a confiabilidade ao usar vários provedores de API.

🗃️ Problema de coleção duplicada de RAG: Corrigido um bug que causava o processamento repetido do mesmo arquivo carregado. Agora utiliza arquivos indexados para evitar duplicações desnecessárias, otimizando o uso de recursos.

🖼️ Aprimoramento da geração de imagens: Endpoint de geração de imagens OpenAI refatorado para ser assíncrono, evitando que o DoctorAI fique sem resposta durante o processamento, aprimorando assim a experiência do usuário.

🔓 Downgrade do Authlib: Revertido o Authlib para a versão 1.3.1 para resolver problemas relacionados à funcionalidade OAuth.

Alterado

🔍 Interação de mensagem aprimorada: Interface do nó de mensagem aprimorada para permitir um redirecionamento de foco mais fácil com um simples clique, simplificando a interação do usuário.

✨ Refatoração de estilo: Estilo do DoctorAI atualizado para uma aparência mais limpa e moderna, aprimorando a experiência do usuário em toda a plataforma.

[0.3.22] - 2024-09-19
Adicionado

⭐ Visão geral do bate-papo: Introduzindo um diagrama de mensagens interativo baseado em nós para melhor visualização dos fluxos de conversação.

🔗 Suporte a vários bancos de dados vetoriais: Agora suporta vários bancos de dados vetoriais, incluindo o recém-adicionado suporte a Milvus. Contribuições da comunidade para suporte adicional ao banco de dados são altamente incentivadas!

📡 Conclusão de bate-papo sem streaming experimental: Recurso experimental que permite o uso de modelos OpenAI o1, que não suportam streaming, garantindo uma implantação de modelo mais versátil.

🔍 Integração experimental do reclassificador Colbert-AI: Adicionado suporte para "jinaai/jina-colbert-v2" como um reclassificador, aprimorando a relevância e a precisão da pesquisa. Observação: pode não funcionar em computadores com especificações baixas.

🕸️ ENABLE_WEBSOCKET_SUPPORT: Adicionada variável de ambiente para instâncias ignorarem atualizações de websocket, estabilizando conexões em plataformas com problemas de websocket.

🔊 Integração do Azure Speech Service: Adicionado suporte para serviços do Azure Speech para texto para fala (TTS).

🎚️ Velocidade de reprodução personalizável: O controle de velocidade de reprodução agora está disponível nas configurações do modo Chamada, permitindo que os usuários ajustem a velocidade de reprodução de áudio de acordo com suas preferências.

🧠 Mensagens de erro aprimoradas: O sistema agora exibe mensagens de erro úteis diretamente aos usuários durante problemas de preenchimento de bate-papo.

📂 Salvar modelo como PNG transparente: As imagens de perfil do modelo agora são salvas como PNGs, suportando transparência e melhorando a integração visual.

📱 Ajustes de compatibilidade com iPhone: Adicionada preenchimento para acomodar a barra de navegação do iPhone, melhorando a exibição da interface do usuário nesses dispositivos.

🔗 Cabeçalhos de resposta seguros: Implementados cabeçalhos de resposta de segurança, reforçando a segurança do aplicativo web.

🔧 Configurações aprimoradas do AUTOMATIC1111: Os usuários agora podem configurar os parâmetros 'Escala CFG', 'Amostrador' e 'Agendador' diretamente nas configurações de administrador, aprimorando a flexibilidade do fluxo de trabalho sem modificações no código-fonte.

🌍 Atualizações i18n: Traduções aprimoradas para chinês, ucraniano, russo e francês, promovendo uma experiência localizada melhor.

Corrigido

🛠️ Exclusão de mensagem de bate-papo: Resolvidos problemas com a exclusão de mensagem de bate-papo, garantindo uma interação mais suave do usuário e estabilidade do sistema.

🔢 Numeração de lista ordenada: Corrigida a ordenação incorreta em listas.

Alterado

🎨 Manipulação de ícone transparente: Permitido que os ícones do modelo sejam exibidos em fundos transparentes, melhorando a estética da interface do usuário.

📝 Modelo RAG aprimorado: Modelo de geração aumentada por recuperação aprimorado, otimizando o tratamento de contexto e a verificação de erros para uma operação mais precisa.

[0.3.21] - 2024-09-08
Adicionado

📊 Exibição da contagem de documentos: Agora exibe o número total de documentos diretamente no painel.

🚀 Endpoint da API de incorporação do Ollama: Habilitado o suporte a proxy do endpoint /api/embed.

Corrigido

🐳 Problema de inicialização do Docker: Resolvido o problema que impedia o DoctorAI de ser iniciado corretamente ao usar o Docker.

Alterado

🔍 Prompts de pesquisa aprimorados: Aprimorados os prompts de geração de consultas de pesquisa para melhor precisão e interação do usuário, aprimorando a experiência geral de pesquisa.

[0.3.20] - 2024-09-07
Adicionado

🌐 Atualização de tradução: Traduções catalãs atualizadas para melhorar a experiência do usuário para falantes de catalão.

Corrigido

📄 Download de PDF: Resolvido um problema de configuração com o diretório de fontes, garantindo que os PDFs agora sejam baixados com a formatação correta.

🛠️ Instalação de requisitos de ferramentas e funções: Corrigido um bug em que os requisitos necessários para ferramentas e funções não estavam sendo instalados corretamente.

🔗 Renderização de link de imagem embutida: Habilitada a renderização de imagens diretamente de links no bate-papo.

📞 Limpeza da interface do usuário pós-chamada: Ajustado o comportamento da interface do usuário para fechar automaticamente os controles de bate-papo após o término de uma chamada de voz, reduzindo a desordem da tela.

🎙️ Desativação do microfone pós-chamada: Resolvido um problema em que o microfone permanecia ativo após as chamadas.

✍️ Correção de espaçamento Markdown: Corrigido o espaçamento na renderização Markdown, garantindo que o texto apareça corretamente e conforme o esperado.

🔄 Renderização de mensagens: Corrigido um problema que fazia com que todas as mensagens de resposta fossem renderizadas novamente a cada nova mensagem, agora melhorando o desempenho do bate-papo.

Alterado

🌐 Integração de pesquisa na web refinada: Descontinuado o limite de prompt de geração de consulta de pesquisa; introduzido um botão de alternância para "Habilitar geração de consulta de pesquisa na web", permitindo que os usuários optem por usar a pesquisa na web de forma mais criteriosa.

📝 Atualização dos modelos de prompt padrão: Os modelos de variáveis ​​de ambiente esvaziados para pesquisa e geração de título agora usam como padrão os modelos de prompt padrão do DoctorAI, simplificando os esforços de configuração.

[0.3.19] - 2024-09-05
Adicionado

🌐 Atualização de tradução: Traduções chinesas aprimoradas.

Corrigido

📂 Substituição de DATA_DIR: Corrigido um problema para evitar a substituição de DATA_DIR, evitando erros quando os diretórios são definidos de forma idêntica, garantindo uma operação e gerenciamento de dados mais suaves.

🛠️ Extração de Frontmatter: Corrigido o processo de extração para frontmatter em ferramentas e funções.

Alterado

🎨 Estilo da interface do usuário: Refinado o estilo da interface do usuário para melhor coerência visual e experiência do usuário.

[0.3.18] - 2024-09-04
Adicionado

🛠️ Execução direta de banco de dados para ferramentas e funções: Aprimorada a execução de arquivos Python para ferramentas e funções, agora carregando diretamente do banco de dados para um processo de back-end mais simplificado.

Corrigido

🔄 Reescrição automática de instruções de importação em ferramentas e funções: Scripts de ferramentas e funções que importam 'utils', 'apps', 'main', 'config' agora renomearão automaticamente estes com 'open_webui.', garantindo compatibilidade e consistência entre diferentes módulos.

🎨 Ajustes de estilo: Pequenas correções no estilo visual para melhorar a experiência do usuário e a consistência da interface.

[0.3.17] - 2024-09-04
Adicionado

🔄 Importar/exportar configuração: Os usuários agora podem importar e exportar configurações do DoctorAI das configurações de administrador > Banco de dados, simplificando a replicação da configuração em todos os sistemas.

🌍 Pesquisa na web por meio de parâmetro de URL: Adicionado suporte para ativar a pesquisa na web diretamente por meio de URL, definindo 'web-search=true'.

🌐 Integração SearchApi: Adicionado suporte para SearchApi como um provedor alternativo de pesquisa na web, aprimorando os recursos de pesquisa na plataforma.

🔍 Suporte ao tipo literal em ferramentas: As ferramentas agora suportam o tipo Literal.

🌍 Traduções atualizadas: Traduções aprimoradas para chinês, ucraniano e catalão.

Corrigido

🔧 Problema de instalação do Pip: Resolvido o problema em que a instalação do pip falhava devido à falta de 'alembic.ini', garantindo processos de instalação mais suaves.

🌃 Atualização automática do tema: Corrigido um problema em que o tema de cores não era atualizado dinamicamente com as alterações do sistema.

🛠️ Agente do usuário em ComfyUI: Adicionados cabeçalhos padrão em ComfyUI para corrigir problemas de acesso, melhorando a confiabilidade nas comunicações de rede.

🔄 Cabeçalhos de resposta de preenchimento de bate-papo ausentes: Garantido o retorno adequado dos cabeçalhos de resposta por proxy durante o preenchimento do bate-papo, melhorando a confiabilidade da API.

🔗 Priorização da conexão WebSocket: Modificada a configuração do socket.io para preferir websockets e fallback para polling de forma mais confiável, aprimorando a estabilidade da conexão.

🎭 Melhorias de acessibilidade: Adicionados rótulos ARIA ausentes para botões, melhorando a acessibilidade para usuários com deficiência visual.

⚖️ Parâmetro avançado: Corrigido um problema garantindo que os parâmetros avançados sejam aplicados corretamente em todos os cenários, garantindo o comportamento consistente das configurações definidas pelo usuário.

Alterado

🔁 Reorganização do namespace: Reorganizados todos os arquivos Python sob o namespace 'open_webui' para simplificar a estrutura do projeto e melhorar a manutenção. Ferramentas e funções que importam de 'utils' agora devem usar 'open_webui.utils'.

🚧 Atualizações de dependência: Atualizadas várias dependências de back-end, como 'aiohttp', 'authlib', 'duckduckgo-search', 'flask-cors' e 'langchain' para suas versões mais recentes, aprimorando o desempenho e a segurança.

[0.3.16] - 2024-08-27
Adicionado

🚀 Migração do banco de dados de configuração: Manipulação de configuração migrada de config.json para o banco de dados, permitindo configurações de alta disponibilidade e balanceamento de carga em várias instâncias do DoctorAI.

🔗 Ativação do modo de chamada via URL: Adicionado um parâmetro de pesquisa de URL 'call=true', permitindo atalhos diretos para ativar o modo de chamada, aprimorando a interação do usuário em dispositivos móveis.

✨ Controle de conteúdo TTS: Adicionada funcionalidade para controlar como o conteúdo da mensagem é segmentado para solicitações de geração de texto para fala (TTS), permitindo opções de saída de fala mais flexíveis.

😄 Mostrar status da pesquisa de conhecimento: Aprimorada a transparência do uso do modelo exibindo o status ao trabalhar com modelos aumentados por conhecimento, ajudando os usuários a entender o estado do sistema durante as consultas.

👆 Clique para copiar para Codespan: Experiência interativa aprimorada no DoctorAI, permitindo que os usuários cliquem para copiar o conteúdo de trechos de código diretamente.

🚫 Bloqueio de usuário de API por meio de filtro de modelo: Introduzida a capacidade de bloquear usuários de API com base em filtros de modelo personalizados, aprimorando a segurança e o controle sobre o acesso à API.

🎬 Estilo de sobreposição de chamada: Ajustado o estilo de sobreposição de chamada em telas grandes para não cobrir toda a interface, mas apenas a área de controle do bate-papo, para uma experiência de interação mais discreta.

Corrigido

🔧 Problema de renderização LaTeX: Resolvido um problema que afetava a renderização correta do LaTeX.

📁 Prevenção de vazamento de arquivo: Resolvido o problema de arquivos carregados serem acessíveis erroneamente em bate-papos de usuário.

🔧 Funções de pipe com o parâmetro 'files': Corrigidos problemas com o parâmetro 'files' não funcionando corretamente nas funções de pipe.

📝 Processamento Markdown para RAG: Corrigidos problemas com o processamento Markdown em arquivos.

🚫 Prompts de sistema duplicados: Corrigidos bugs que causavam a duplicação de prompts de sistema.

Alterado

🔋 Permissão Wakelock: Otimizada a ativação do wakelock para ser ativado apenas durante o modo de chamada, conservando os recursos do dispositivo e melhorando o desempenho da bateria durante os períodos de inatividade.

🔍 Tipo de conteúdo para bate-papos Ollama: Adicionado tipo de conteúdo 'application/x-ndjson' às respostas do endpoint '/api/chat' para corresponder às respostas brutas do Ollama.

✋ Desativar registros condicionalmente: Implementada lógica condicional para desativar registros quando 'ENABLE_LOGIN_FORM' estiver definido como falso.

[0.3.15] - 2024-08-21
Adicionado

🔗 Ativação temporária do bate-papo: Integrado um novo parâmetro de URL 'temporary-chat=true' para habilitar sessões de bate-papo temporárias diretamente pelo URL.

🌄 Suporte ao nó de semente ComfyUI: Introduzido o suporte ao nó de semente em ComfyUI para geração de imagens, permitindo que os usuários especifiquem IDs de nó para atribuição de semente aleatória.

Corrigido

🛠️ Ferramentas e funções: Resolvido um problema crítico em que as ferramentas e funções não estavam funcionando corretamente, restaurando a capacidade total e a confiabilidade desses recursos essenciais.

🔘 Botão de ação do bate-papo em muitos bate-papos de modelo: Corrigido o mau funcionamento dos botões de ação do bate-papo em muitos ambientes de bate-papo de modelo, garantindo uma interação do usuário mais suave e responsiva.

⏪ Compatibilidade com muitos bate-papos de modelo: Restaurada a compatibilidade com versões anteriores para muitos bate-papos de modelo.

[0.3.14] - 2024-08-21
Adicionado

🛠️ Fluxo de trabalho ComfyUI personalizado: Descontinuando várias variáveis ​​de ambiente mais antigas, este aprimoramento introduz um novo fluxo de trabalho personalizável para uma experiência do usuário mais personalizada.

🔀 Mesclar respostas em muitos bate-papos de modelo: Aprimora o diálogo mesclando respostas de vários modelos em uma única resposta coerente, melhorando a qualidade da interação em muitos bate-papos de modelo.

✅ Várias instâncias do mesmo modelo em bate-papos: Bate-papo com vários modelos aprimorado para suportar a adição de várias instâncias do mesmo modelo.

🔧 Ações rápidas no espaço de trabalho do modelo: Ações rápidas da tecla Shift aprimoradas para ocultar/exibir e excluir modelos, facilitando um fluxo de trabalho mais suave.

🗨️ Renderização Markdown em mensagens do usuário: As mensagens do usuário agora são renderizadas em Markdown, aprimorando a legibilidade e a interação.

💬 Recurso de bate-papo temporário: Introduzido um recurso de bate-papo temporário, descontinuando a antiga configuração do histórico de bate-papo para aprimorar a flexibilidade de interação do usuário.

🖋️ Edição de mensagem do usuário: Aprimorado o recurso de edição de bate-papo do usuário para permitir salvar alterações sem enviar, fornecendo mais flexibilidade no gerenciamento de mensagens.

🛡️ Melhorias de segurança: Várias melhorias de segurança implementadas em toda a plataforma para garantir experiências de usuário mais seguras.

🌍 Traduções atualizadas: Traduções aprimoradas para chinês, ucraniano e bahasa malaio, melhorando a localização e a compreensão do usuário.

Corrigido

📑 Problema de renderização Mermaid: Resolvidos problemas com a renderização do gráfico Mermaid para garantir a representação visual clara e limpa dos dados.

🎭 Mascaramento de ícone PWA: Corrigido o ícone do aplicativo web progressivo para ser mascarável, garantindo a exibição correta nas telas iniciais de vários dispositivos.

🔀 Problema de congelamento do bate-papo do modelo clonado: Corrigido um bug em que a clonagem de muitos bate-papos de modelo causava congelamento, aprimorando a estabilidade e a capacidade de resposta.

🔍 Tratamento de erros genéricos e refinamentos: Várias pequenas correções e refinamentos para resolver problemas não rastreados anteriormente, garantindo operações mais suaves.

Alterado

🖼️ Refatoração da geração de imagens: Processos de geração de imagens revisados ​​para melhorar a eficiência e a qualidade.

🔨 Refatorar chamada de ferramenta e função: Mecanismos de chamada de ferramenta e função refatorados para maior clareza e manutenção.

🌐 Atualizações da biblioteca de back-end: Bibliotecas críticas de back-end atualizadas, incluindo SQLAlchemy, uvicorn[standard], faster-whisper, bcrypt e boto3 para desempenho e segurança aprimorados.

Removido

🚫 Variáveis ​​de ambiente ComfyUI descontinuadas: Removidas várias variáveis ​​de ambiente desatualizadas relacionadas às configurações ComfyUI, simplificando o gerenciamento de configuração.

[0.3.13] - 2024-08-14
Adicionado

🎨 Renderização Markdown aprimorada: Melhorias significativas na renderização de markdown, garantindo a exibição suave e confiável de gráficos LaTeX e Mermaid, aprimorando a experiência do usuário com conteúdo visual mais robusto.

🔄 Instalar automaticamente dependências Python de ferramentas e funções: Para 'Ferramentas' e 'Funções', o DoctorAI agora instala automaticamente requisitos extras do Python especificados no frontmatter, simplificando os processos de configuração e personalização.

🌀 Personalização de reivindicação de e-mail OAuth: Introduzida uma variável 'OAUTH_EMAIL_CLAIM' para permitir a personalização da reivindicação padrão "email" nas configurações OAuth, fornecendo maior flexibilidade nos processos de autenticação.

📶 Reconexão WebSocket: Confiabilidade aprimorada com a capacidade de reconectar automaticamente quando um websocket é fechado, garantindo comunicação consistente e estável.

🤳 Feedback tátil em dispositivos de suporte: Dispositivos Android agora suportam feedback tátil para uma experiência tátil imersiva durante certas interações.

Corrigido

🛠️ Melhoria de desempenho ComfyUI: Resolvido um problema que fazia com que o FastAPI parasse quando a geração de imagens ComfyUI estava ativa; agora é executado em uma thread separada para evitar que a interface do usuário não responda.

🔀 Manipulação de sessão: Corrigido um problema que exigia session_id no lado do cliente para garantir um gerenciamento e transições de sessão mais suaves.

🖋️ Pequenas correções de bugs e correções de formato: Várias pequenas correções, incluindo correções de erros de digitação, melhorias na formatação do back-end e alterações de teste, aprimorando a estabilidade e o desempenho geral do sistema.

Alterado

🚀 Migração para SvelteKit 2: Framework subjacente atualizado para a versão 2 do SvelteKit, oferecendo velocidade aprimorada, melhor estrutura de código e recursos de implantação aprimorados.

🧹 Limpeza geral e refatoração: Realizada limpeza e refatoração amplas em toda a plataforma, melhorando a eficiência do código e mantendo altos padrões de integridade do código.

🚧 Melhorias no teste de integração: Modificada a forma como os testes de integração do Cypress detectam mensagens de bate-papo e testes de compartilhamento atualizados para melhor confiabilidade e precisão.

📁 Extensão de arquivo '.safetensors' padronizada: Extensão de arquivo '.sft' renomeada para '.safetensors' para fluxos de trabalho ComfyUI, padronizando formatos de arquivo em toda a plataforma.

Removido

🗑️ Funções de front-end descontinuadas: Removidas funções de front-end que foram migradas para o back-end para organizar a base de código e reduzir a redundância.

[0.3.12] - 2024-08-07
Adicionado

🔄 Rolagem infinita da barra lateral: Adicionado um recurso de rolagem infinita na barra lateral para uma navegação de bate-papo mais eficiente, reduzindo os tempos de carregamento e aprimorando a experiência do usuário.

🚀 Renderização Markdown aprimorada: Suporte para renderizar todos os blocos de código e tornar as imagens clicáveis ​​para visualização; o estilo codespan também é aprimorado para melhorar a legibilidade e a interação do usuário.

🔒 Visibilidade do bate-papo compartilhado do administrador: Os administradores não têm mais visibilidade padrão sobre os bate-papos compartilhados quando ENABLE_ADMIN_CHAT_ACCESS está definido como falso, reforçando as configurações de segurança e privacidade para os usuários.

🌍 Atualizações de idioma: Adicionada tradução para malaio (Bahasa Malaysia) e traduções atualizadas para catalão e chinês tradicional para melhorar a acessibilidade para mais usuários.

Corrigido

📊 Problemas de renderização Markdown: Resolvidos problemas com a renderização de markdown para garantir a exibição consistente e correta em todos os componentes.

🛠️ Problemas de estilo: Várias correções aplicadas ao estilo em todo o aplicativo, melhorando a experiência visual geral e a consistência da interface.

🗃️ Manipulação modal: Corrigido um problema em que os modais não estavam fechando corretamente em vários cenários de bate-papo de modelo, aprimorando a usabilidade e a confiabilidade da interface.

📄 Informações de uso do OpenAI ausentes: Resolvidos problemas em que as estatísticas de uso dos serviços OpenAI não estavam sendo exibidas corretamente, garantindo que os usuários tenham acesso a dados cruciais para gerenciar e monitorar seu consumo de API.

🔧 Suporte de streaming não para o plugin de funções: Corrigido um problema de funcionalidade com o plugin de funções em que as operações sem streaming não estavam funcionando conforme o esperado, restaurando os recursos completos para integração assíncrona e síncrona na plataforma.

🔄 Correção de tipo de variável de ambiente (COMFYUI_FLUX_FP8_CLIP): Corrigido o tipo de dados da variável de ambiente 'COMFYUI_FLUX_FP8_CLIP' de string para booleano, garantindo que as configurações de ambiente sejam aplicadas corretamente e aprimorando o gerenciamento de configuração.

Alterado

🔧 Atualizações de dependência de back-end: Atualizadas várias dependências de back-end, como boto3, pypdf, python-pptx, validadores e preto, garantindo otimizações de segurança e desempenho atualizadas.

[0.3.11] - 2024-08-02
Adicionado

📊 Exibição de informações do modelo: Adicionados recursos visuais para seleção de modelo, incluindo imagens ao lado dos nomes dos modelos para navegação mais intuitiva.

🗣 Adaptações de voz ElevenLabs: Aprimoramentos de voz, incluindo suporte para ID de voz ElevenLabs por nome para interações vocais personalizadas.

⌨️ Seleção de modelo com teclas de seta: Os usuários agora podem usar as teclas de seta para uma seleção de modelo mais rápida, aprimorando a acessibilidade.

🔍 Pesquisa difusa no seletor de modelo: Seletor de modelo aprimorado com pesquisa difusa para localizar modelos rapidamente, incluindo descrições.

🕹️ Geração de imagens ComfyUI Flux: Adicionado suporte para o novo modelo de geração de imagens Flux; introduz controles de ambiente como precisão de peso e opções de modelo CLIP em Configurações.

💾 Exibir tamanho do arquivo para uploads: A interface de arquivo aprimorada agora exibe o tamanho do arquivo, preparando-se para as próximas restrições de upload.

🎚️ Parâmetros avançados "Min P": Adicionado o parâmetro 'Min P' nas configurações avançadas para controle de precisão personalizado do modelo.

🔒 OAuth aprimorado: Introduzido suporte a URI de redirecionamento personalizado para OAuth atrás de proxies reversos, permitindo processos de autenticação mais seguros.

🖥 Renderização aprimorada de Latex: Ajustes feitos aos processos de renderização de latex, agora detectando e apresentando com precisão entradas de latex de texto.

🌐 Internacionalização: Aprimorado com novas traduções para romeno e traduções atualizadas para vietnamita e ucraniano, ajudando a ampliar a acessibilidade para usuários internacionais.

Corrigido

🔧 Manipulação de tags no upload de documentos: As tags agora são enviadas corretamente para o manipulador de upload de documentos, resolvendo problemas com metadados ausentes.

🖥️ Campos de entrada confidenciais: Corrigida a interpretação incorreta do navegador dos campos de entrada segura, evitando a classificação incorreta como campos de senha.

📂 Resolução de caminho estático na geração de PDF: Corrigidos caminhos estáticos que se ajustam dinamicamente para evitar problemas em vários ambientes.

Alterado

🎨 Melhorias de estilo UI/UX: Várias pequenas atualizações de estilo para uma interface de usuário mais limpa e intuitiva.

🚧 Refatoração de vários componentes: Numerosas alterações de refatoração em estilo, manipulação de arquivos e simplificações de função para maior clareza e desempenho.

🎛️ Gerenciamento de válvulas do usuário: Movidas as válvulas do usuário das configurações para os controles diretos do bate-papo para um acesso mais amigável durante as interações.

Removido

⚙️ Registro de verificação de integridade: Removido o registro detalhado dos processos de verificação de integridade para organizar os registros e melhorar o desempenho do back-end.

[0.3.10] - 2024-07-17
Corrigido

🔄 Upload de arquivo aprimorado: Resolvido o problema em que os uploads de arquivo não tinham animação.

💬 Continuidade do bate-papo: Corrigido um problema em que os bate-papos existentes não estavam funcionando corretamente em alguns casos.

🗂️ Redefinição do arquivo de bate-papo: Resolvido o problema de arquivos de bate-papo que não eram redefinidos para novas conversas, agora garantindo uma nova página para cada sessão de bate-papo.

📁 Uploads do espaço de trabalho do documento: Corrigida a manipulação de uploads de documentos no espaço de trabalho usando a API de arquivos.

[0.3.9] - 2024-07-17
Adicionado

📁 Controles de bate-papo de arquivos: Retomamos o antigo comportamento de manipulação de arquivos em que os arquivos carregados são sempre incluídos. Agora você pode gerenciar arquivos diretamente na seção de controles de bate-papo, permitindo que você remova arquivos conforme necessário.

🔧 Suporte à função "Ação": Introduzindo uma nova função "Ação" para gravar botões personalizados na barra de ferramentas da mensagem. Este recurso permite mensagens mais interativas, com documentação em breve.

📜 Manipulação de citações: Para arquivos recém-carregados no espaço de trabalho de documentos, as citações agora exibirão o nome do arquivo real. Além disso, você pode clicar nesses nomes de arquivo para abrir o arquivo em uma nova guia para facilitar o acesso.

🛠️ Atualizações do emissor de eventos e chamadas: 'event_emitter' aprimorado para permitir a substituição de mensagens e 'event_call' para suportar entrada de texto para ferramentas e funções. Documentação detalhada será fornecida em breve.

🎨 Refatoração de estilo: Várias atualizações de estilo para uma interface de usuário mais limpa e coesa.

🌐 Traduções aprimoradas: Traduções aprimoradas para catalão, ucraniano e português brasileiro.

Corrigido

🔧 Prioridade dos controles de bate-papo: Resolvido um problema em que os valores dos controles de bate-papo estavam sendo substituídos pelos parâmetros de informações do modelo. A prioridade agora é Controles de bate-papo, seguidos por Configurações globais e, em seguida, Configurações do modelo.

🪲 Registros de depuração: Corrigido um problema em que os registros de depuração não estavam sendo registrados corretamente.

🔑 Chave de autenticação Automatic1111: A chave de autenticação para Automatic1111 não é mais necessária.

📝 Geração de título: Garantido que a geração de título seja executada apenas uma vez, mesmo quando vários modelos estão em um bate-papo.

✅ Valores booleanos em parâmetros: Adicionado suporte para valores booleanos em parâmetros.

🖼️ Estilo de sobreposição de arquivos: Corrigido o problema de estilo com a sobreposição de arquivos.

Alterado

⬆️ Atualizações de dependência

'pydantic' atualizado da versão 2.7.1 para 2.8.2.

'sqlalchemy' atualizado da versão 2.0.30 para 2.0.31.

'unstructured' atualizado da versão 0.14.9 para 0.14.10.

'chromadb' atualizado da versão 0.5.3 para 0.5.4.

[0.3.8] - 2024-07-09
Adicionado

💬 Controles de bate-papo: Ajuste facilmente os parâmetros para cada sessão de bate-papo, oferecendo um controle mais preciso sobre suas interações.

📌 Bate-papos fixados: Suporte para bate-papos fixados, permitindo que você mantenha conversas importantes facilmente acessíveis.

📄 Integração Apache Tika: Adicionado suporte para usar Apache Tika como um carregador de documentos, aprimorando os recursos de processamento de documentos.

🛠️ Ambiente personalizado para reivindicações OpenID: Permite definir reivindicações personalizadas para OpenID, fornecendo mais flexibilidade nos processos de autenticação do usuário.

🔧 API aprimorada de ferramentas e funções: Introduzido 'event_emitter' e 'event_call', agora você também pode adicionar citações para melhor documentação e rastreamento. Documentação detalhada será fornecida em nosso site de documentação.

↔️ Rolagem lateral em configurações: O contêiner de guias de configurações agora suporta rolagem horizontal para facilitar a navegação.

🌑 Tema OLED mais escuro: Inclui um novo tema OLED mais escuro e estilo aprimorado para o tema claro, aprimorando o apelo visual.

🌐 Atualizações de idioma: Traduções atualizadas para indonésio, alemão, francês e catalão, expandindo a acessibilidade.

Corrigido

⏰ Tempo limite de streaming OpenAI: Resolvidos problemas com a resposta de streaming OpenAI usando a configuração 'AIOHTTP_CLIENT_TIMEOUT', garantindo um desempenho confiável.

💡 Válvulas do usuário: Corrigidas válvulas do usuário com mau funcionamento, garantindo a funcionalidade adequada.

🔄 Componentes recolhíveis: Resolvidos problemas com componentes recolhíveis que não funcionavam, restaurando o comportamento esperado.

Alterado

🗃️ Back-end do banco de dados: Alternado de Peewee para SQLAlchemy para suporte aprimorado à simultaneidade, aprimorando o desempenho do banco de dados.

⬆️ Atualização do ChromaDB: Atualizado para a versão 0.5.3. Certifique-se de que sua instância remota do ChromaDB corresponda a esta versão.

🔤 Estilo da fonte primária: Fonte primária atualizada para Archivo para melhor consistência visual.

🔄 Alteração de fonte para Windows: Fonte Arimo substituída por fonte Inter para usuários do Windows, melhorando a legibilidade.

ando a legibilidade.

🚀 Carregamento lento: implementado carregamento lento para 'faster_whisper' e 'sentence_transformers' para reduzir o uso de memória na inicialização.

📋 Carga útil de geração de tarefas: as gerações de tarefas agora incluem apenas o campo "tarefa" no corpo em vez de "título".

[0.3.7] - 2024-06-29
Adicionado

🌐 Internacionalização aprimorada (i18n): Nova tradução para indonésio introduzida e traduções atualizadas para turco, chinês e catalão para melhorar a acessibilidade do usuário.

Corrigido

🕵️‍♂️ Detecção de idioma do navegador: corrigido o problema em que o aplicativo não detectava e se adaptava corretamente às configurações de idioma do navegador.

🔐 Atribuição de função de administrador OIDC: corrigido um bug em que a função de administrador não estava sendo atribuída ao primeiro usuário que se inscreveu via OpenID Connect (OIDC).

💬 Endpoint de bate-papo/conclusões: resolvido um problema em que o endpoint de bate-papo/conclusões não estava funcional quando a opção de fluxo estava definida como Falsa.

🚫 Configuração 'WEBUI_AUTH': resolvido o problema em que a definição de 'WEBUI_AUTH' como Falso não estava sendo aplicada corretamente.

Alterado

📦 Atualização de dependência: atualizado 'authlib' da versão 1.3.0 para 1.3.1 para garantir melhor segurança e aprimoramentos de desempenho.

[0.3.6] - 2024-06-27
Adicionado

✨ Recurso "Funções": agora você pode utilizar "Funções" como filtros (middleware) e funções de pipe (modelo) diretamente no DoctorAI. Embora amplamente compatíveis com Pipelines, essas funções nativas podem ser executadas facilmente no DoctorAI. Os casos de uso de exemplo para funções de filtro incluem monitoramento de uso, tradução em tempo real, moderação e memória automática. Para funções de pipe, o escopo varia da integração Cohere e Anthropic diretamente no DoctorAI, permitindo "Válvulas" para o uso da chave de API OpenAI por usuário e muito mais. Se você encontrar problemas, o SAFE_MODE foi introduzido.

📁 API de arquivos: compatível com OpenAI, este recurso permite a Geração Aumentada por Recuperação (RAG) personalizada em conjunto com a Função de Filtro. Mais exemplos serão compartilhados em nossa plataforma da comunidade e site de documentação oficial.

🛠️ Aprimoramentos de ferramentas: as ferramentas agora suportam citações e "válvulas". A documentação estará disponível em breve.

🔗 Suporte a Iframe via API de arquivos: permite renderizar HTML diretamente na interface do bate-papo usando funções e ferramentas. Os casos de uso incluem jogar jogos como DOOM e Snake, exibir um applet de clima e implementar recursos semelhantes a "artefatos" antrópicos. Fique ligado para atualizações em nossa plataforma da comunidade e documentação.

🔒 Suporte experimental a OAuth: novo suporte experimental a OAuth. Consulte nossa documentação para obter mais detalhes.

🖼️ Suporte a plano de fundo personalizado: defina um plano de fundo personalizado em Configurações > Interface para personalizar sua experiência.

🔑 Suporte AUTOMATIC1111_API_AUTH: segurança aprimorada para a API AUTOMATIC1111.

🎨 Otimização de destaque de código: recursos aprimorados de destaque de código.

🎙️ Recurso de interrupção de voz: reintroduzido e agora alternável em Configurações > Interface.

💤 API Wakelock: agora em uso para evitar o escurecimento da tela durante tarefas importantes.

🔐 Privacidade da chave de API: todas as chaves de API agora estão ocultas por padrão para melhor segurança.

🔍 Novo provedor de pesquisa na web: adicionado jina_search como uma nova opção.

🌐 Internacionalização aprimorada (i18n): traduções chinesas, ucranianas e brasileiras aprimoradas.

Corrigido

🔧 Problema do modo de conversação: corrigido o problema em que o modo de conversação permanecia ativo após ser removido das configurações.

📏 Obstrução do botão de rolagem: resolvido o problema em que o contêiner do botão scrollToBottom obstruía os cliques nos botões abaixo dele.

Alterado

⏲️ AIOHTTP_CLIENT_TIMEOUT: agora definido como 'Nenhum' por padrão para maior flexibilidade de configuração.

📞 Aprimoramentos de chamadas de voz: aprimorado ignorando blocos de código e expressões durante as chamadas.

🚫 Manipulação de mensagens de erro: desativada a continuação das operações com mensagens de erro.

🗂️ Relocação do playground: movido o playground do espaço de trabalho para o menu do usuário para uma melhor experiência do usuário.

[0.3.5] - 2024-06-16
Adicionado

📞 Chamada de voz aprimorada: o retorno de chamada de texto para fala (TTS) agora opera em tempo real para cada frase, reduzindo a latência por não esperar a conclusão total.

👆 Toque para interromper: durante uma chamada, agora você pode impedir que o assistente fale simplesmente tocando, em vez de usar a voz. Isso resolve o problema da voz do alto-falante ser registrada incorretamente como entrada.

😊 Chamada de emoji: ative esse recurso em Configurações > Interface, permitindo que LLMs expressem emoções usando emojis durante chamadas de voz para uma interação mais dinâmica.

🖱️ Arquivar/excluir rápido: use a tecla Shift + passar o mouse sobre a lista de bate-papo para arquivar ou excluir itens rapidamente.

📝 Suporte a Markdown em descrições de modelo: agora você pode formatar descrições de modelo com markdown, permitindo texto em negrito, links, etc.

🧠 Memórias editáveis: adiciona a capacidade de modificar memórias.

📋 Classificação do painel de administração: introduz a capacidade de classificar usuários/bate-papos no painel de administração.

🌑 Modo escuro para seletores rápidos: modo escuro agora disponível para seletores rápidos de bate-papo (prompts, modelos, documentos).

🔧 Parâmetros avançados: adiciona 'num_keep' e 'num_batch' aos parâmetros avançados para personalização.

📅 Prompts de sistema dinâmicos: novas variáveis ​​'{{CURRENT_DATETIME}}', '{{CURRENT_TIME}}', '{{USER_LOCATION}}' adicionadas para prompts de sistema. Certifique-se de que '{{USER_LOCATION}}' esteja ativado em Configurações > Interface.

🌐 Pesquisa na web Tavily: inclui Tavily como uma opção de provedor de pesquisa na web.

🖊️ Nomes de usuário de autenticação federada: capacidade de definir nomes de usuário para autenticação federada.

🔗 Limpar URLs automaticamente: ao adicionar URLs de conexão, as barras finais agora são removidas automaticamente.

🌐 Traduções aprimoradas: traduções chinesas e suecas aprimoradas.

Corrigido

⏳ AIOHTTP_CLIENT_TIMEOUT: introduzida uma nova variável de ambiente 'AIOHTTP_CLIENT_TIMEOUT' para solicitações ao Ollama com duração superior a 5 minutos. O padrão é 300 segundos; defina como em branco ('') para nenhum tempo limite.

❌ Congelamento de exclusão de mensagem: resolvido um problema em que a exclusão de mensagem às vezes fazia com que a interface do usuário congelasse.

[0.3.4] - 2024-06-12
Corrigido

🔒 Problema de conteúdo misto com HTTPS: resolvido um problema em que o conteúdo misto (HTTP e HTTPS) estava causando avisos de segurança e bloqueando recursos em sites HTTPS.

🔍 Problema de pesquisa na web: resolvido o problema em que a funcionalidade de pesquisa na web não estava funcionando corretamente. A opção 'ENABLE_RAG_LOCAL_WEB_FETCH' foi reintroduzida para restaurar os recursos adequados de pesquisa na web.

💾 Modelo RAG não sendo salvo: corrigido um problema em que o modelo RAG não estava sendo salvo corretamente, garantindo que seus modelos personalizados agora sejam preservados conforme o esperado.

[0.3.3] - 2024-06-12
Adicionado

🛠️ Chamada de função Python nativa: introduzindo a chamada de função Python nativa no DoctorAI. Também incluímos um editor de código integrado para desenvolver e integrar perfeitamente o código da função no espaço de trabalho 'Ferramentas'. Com isso, você pode aprimorar significativamente os recursos do seu LLM criando pipelines RAG personalizados, ferramentas de pesquisa na web e até recursos semelhantes a agentes, como o envio de mensagens do Discord.

🌐 Integração DuckDuckGo: adicionado DuckDuckGo como um provedor de pesquisa na web, oferecendo mais opções de pesquisa.

🌏 Traduções aprimoradas: traduções aprimoradas para os idiomas vietnamita e chinês, tornando a interface mais acessível.

Corrigido

🔗 Manipulação de erros de URL de pesquisa na web: corrigido o problema em que um único erro de URL interrompia o processo de carregamento de dados no modo de pesquisa na web. Agora, esses erros serão tratados normalmente para garantir o carregamento ininterrupto dos dados.

🖥️ Responsividade do front-end: resolvido o problema em que o front-end parava de responder se o back-end encontrasse um erro ao baixar um modelo. Tratamento de erros aprimorado para manter a estabilidade do front-end.

🔧 Problemas de dependência no pip: corrigidos problemas relacionados às instalações do pip, garantindo que todas as dependências sejam gerenciadas corretamente para evitar erros de instalação.

[0.3.2] - 2024-06-10
Adicionado

🔍 Status da consulta de pesquisa na web: a consulta de pesquisa na web agora persistirá na seção de resultados para ajudar na depuração e rastreamento mais fáceis das consultas de pesquisa.

🌐 Novo provedor de pesquisa na web: adicionamos o Serply como uma nova opção para provedores de pesquisa na web, oferecendo mais opções para suas necessidades de pesquisa.

🌏 Traduções aprimoradas: aprimoramos as traduções para chinês e português.

Corrigido

🎤 Problema de upload de arquivo de áudio: o bug que impedia o upload de arquivos de áudio na entrada do bate-papo foi corrigido, garantindo uma comunicação tranquila.

💬 Manipulação de entrada de mensagem: aprimorada a manipulação de entradas de mensagem limpando imagens e texto instantaneamente após o envio, juntamente com indicações visuais imediatas quando uma mensagem de resposta está carregando, aprimorando o feedback do usuário.

⚙️ Registro e validação de parâmetros: corrigido o problema em que os parâmetros não eram registrados em certos casos e resolvido o problema em que os usuários não conseguiam salvar devido a erros de entrada inválidos.

[0.3.1] - 2024-06-09
Corrigido

💬 Funcionalidade de bate-papo: resolvido o problema em que a funcionalidade de bate-papo não estava funcionando para modelos específicos.

[0.3.0] - 2024-06-09
Adicionado

📚 Suporte a conhecimento para modelos: anexe documentos diretamente aos modelos do espaço de trabalho de modelos, aprimorando as informações disponíveis para cada modelo.

🎙️ Recurso de chamada de voz mãos-livres: inicie chamadas de voz sem precisar usar as mãos, tornando as interações mais perfeitas.

📹 Recurso de videochamada: ative videochamadas com modelos de visão suportados como Llava e GPT-4o, adicionando uma dimensão visual às suas comunicações.

🎛️ Interface do usuário aprimorada para gravação de voz: interface do usuário aprimorada para o recurso de gravação de voz, tornando-o mais intuitivo e amigável.

🌐 Suporte externo a STT: agora suporta serviços externos de fala para texto, fornecendo mais flexibilidade na escolha do seu provedor de STT.

⚙️ Configurações unificadas: configurações consolidadas, incluindo configurações de documento em uma nova seção de configurações de administrador para facilitar o gerenciamento.

🌑 Tela inicial do modo escuro: uma nova tela inicial para o modo escuro, garantindo uma experiência consistente e visualmente atraente para os usuários do modo escuro.

📥 Pipeline de upload: carregue pipelines diretamente das configurações de administrador > seção de pipelines, simplificando o processo de gerenciamento de pipeline.

🌍 Suporte a idiomas aprimorado: suporte aprimorado para os idiomas chinês e ucraniano, atendendo melhor a uma base de usuários global.

Corrigido

🛠️ Problema do playground: corrigido o playground que não funcionava corretamente, garantindo uma experiência de usuário mais tranquila.

🔥 Problema do parâmetro de temperatura: corrigido o problema em que o valor de temperatura '0' não estava sendo passado corretamente.

📝 Limpeza da entrada do prompt: resolvido o problema da área de texto de entrada do prompt não ser limpa imediatamente, garantindo uma nova página para novas entradas.

✨ Vários problemas de estilo da interface do usuário: corrigidos vários problemas de estilo da interface do usuário para uma aparência mais coesa.

👥 Exibição de usuários ativos: corrigido o problema de usuários ativos mostrando sessões ativas em vez de usuários reais, agora refletindo a atividade precisa do usuário.

🌐 Compatibilidade da plataforma da comunidade: a plataforma da comunidade está de volta online e totalmente compatível com o DoctorAI.

Alterado

📝 Implementação RAG: implementação RAG (Geração Aumentada por Recuperação) atualizada para usar um prompt do sistema para contexto, em vez de substituir o prompt do usuário.

🔄 Relocação de configurações: movidas as configurações de Modelos, Conexões, Áudio e Imagens para as configurações de administrador para melhor organização.

✍️ Geração de título aprimorada: prompt padrão aprimorado para geração de título, produzindo melhores resultados.

🔧 Gerenciamento de tarefas de back-end: tarefas como geração de título e geração de consulta de pesquisa agora são gerenciadas no lado do back-end e controladas apenas pelo administrador.

🔍 Prompt de consulta de pesquisa editável: agora você pode editar o prompt de geração de consulta de pesquisa, oferecendo mais controle sobre como as consultas são geradas.

📏 Limite de comprimento do prompt: defina o limite de comprimento do prompt para geração de consulta de pesquisa nas configurações de administrador, oferecendo mais opções de personalização.

📣 Consolidação de configurações: mesclada a configuração de administrador de banners com a configuração de administrador de interface para uma área de configurações mais simplificada.

[0.2.5] - 2024-06-05
Adicionado

👥 Indicador de usuários ativos: agora você pode ver quantas pessoas estão ativas atualmente e o que estão executando. Isso ajuda você a avaliar quando o desempenho pode diminuir devido a um grande número de usuários.

🗂️ Criar arquivo de modelo Ollama: a opção de criar um arquivo de modelo para Ollama foi reintroduzida em Configurações > seção Modelos, facilitando o gerenciamento de seus modelos.

⚙️ Configuração do modelo padrão: adicionada uma opção para definir o modelo padrão em Configurações > Interface. Este recurso agora é facilmente acessível, especialmente conveniente para usuários móveis, pois estava oculto anteriormente.

🌐 Traduções aprimoradas: aprimoramos as traduções para chinês e adicionamos suporte para os idiomas turcomeno e norueguês para tornar a interface mais acessível globalmente.

Corrigido

📱 Melhorias na visualização móvel: a interface do usuário agora usa dvh (altura dinâmica da janela de visualização) em vez de vh (altura da janela de visualização), proporcionando uma experiência melhor e mais responsiva para usuários móveis.

[0.2.4] - 2024-06-03
Adicionado

👤 Página de conta pendente aprimorada: a página de conta pendente agora exibe os detalhes do administrador por padrão para evitar confusão. Você pode desativar esse recurso nas configurações de administrador, se necessário.

🌐 Suporte a proxy HTTP: habilitamos o uso da variável de ambiente 'http_proxy' nas chamadas de API OpenAI e Ollama, facilitando a configuração das configurações de rede.

❓ Acesso rápido à documentação: agora você pode acessar facilmente os documentos do DoctorAI por meio de um botão de ponto de interrogação localizado no canto inferior direito da tela (disponível em telas maiores, como PCs).

🌍 Tradução aprimorada: melhorias foram feitas nas traduções.

Corrigido

🔍 Pesquisa na web SearxNG: corrigido o problema em que a funcionalidade de pesquisa na web SearxNG não estava funcionando corretamente.

[0.2.3] - 2024-06-03
Adicionado

📁 Exportar bate-papo como JSON: agora você pode exportar bate-papos individuais como arquivos JSON no menu da barra de navegação, navegando até 'Download > Exportar bate-papo'. Isso facilita o compartilhamento de conversas específicas.

✏️ Editar títulos com duplo clique: clique duas vezes nos títulos para renomeá-los de forma rápida e eficiente.

🧩 Incorporações múltiplas em lote: introduzido 'RAG_EMBEDDING_OPENAI_BATCH_SIZE' para processar várias incorporações em um lote, aprimorando o desempenho para grandes conjuntos de dados.

🌍 Traduções aprimoradas: qualidade da tradução aprimorada em vários idiomas para uma melhor experiência do usuário.

Corrigido

🛠️ Script de migração de arquivo de modelo: corrigido um problema em que o script de migração de arquivo de modelo falhava se um arquivo de modelo inválido fosse encontrado.

💬 Método de entrada Zhuyin no Mac: resolvido um problema em que o uso do método de entrada Zhuyin na interface do usuário da Web em um Mac fazia com que o texto fosse enviado imediatamente ao pressionar a tecla Enter, levando à entrada incorreta.

🔊 Seleção de voz TTS local: corrigido o problema em que a voz local de texto para fala (TTS) selecionada não estava sendo exibida nas configurações.

[0.2.2] - 2024-06-02
Adicionado

🌊 Suporte à renderização Mermaid: incluímos suporte para renderização Mermaid. Isso permite que você crie belos diagramas e fluxogramas diretamente no DoctorAI.

🔄 Nova variável de ambiente 'RESET_CONFIG_ON_START': introduzindo uma nova variável de ambiente: 'RESET_CONFIG_ON_START'. Defina esta variável para redefinir suas configurações de configuração ao iniciar o aplicativo, tornando mais fácil reverter para as configurações padrão.

Corrigido

🔧 Problema de filtro de pipelines: resolvemos um problema com os pipelines em que os filtros não estavam funcionando conforme o esperado.

[0.2.1] - 2024-06-02
Adicionado

🖱️ Botão de exportação de modelo único: exporte modelos facilmente com apenas um clique usando o novo botão de exportação de modelo único.

🖥️ Suporte a parâmetros avançados: adicionado suporte para os parâmetros 'num_thread', 'use_mmap' e 'use_mlock' para Ollama.

🌐 Tradução vietnamita aprimorada: suporte aprimorado ao idioma vietnamita para uma melhor experiência do usuário para nossa comunidade de língua vietnamita.

Corrigido

🔧 Problema de salvamento da API de URL OpenAI: corrigido um problema que impedia o salvamento das configurações da API de URL OpenAI.

🚫 Problema de exibição com API Ollama desativada: corrigido o bug de exibição que fazia com que os modelos aparecessem nas configurações quando a API Ollama estava desativada.

Alterado

💡 Atualização de versão: como um lembrete de nossa atualização anterior, a versão 0.2.y se concentrará principalmente em correções de bugs, enquanto as principais atualizações serão designadas como 0.x a partir de agora para melhor rastreamento de versão.

[0.2.0] - 2024-06-01
Adicionado

🔧 Suporte a Pipelines: DoctorAI agora inclui uma estrutura de plugins para personalização e funcionalidade aprimoradas (https://teledocmedical.com/). Adicione lógica personalizada e integre bibliotecas Python facilmente, de agentes de IA a APIs de automação residencial.

🔗 Chamada de função via Pipelines: integre a chamada de função perfeitamente por meio de Pipelines.

⚖️ Limitação de taxa do usuário via Pipelines: implemente limites de taxa específicos do usuário para gerenciar o uso da API com eficiência.

📊 Monitoramento de uso com Langfuse: rastreie e analise estatísticas de uso com a integração Langfuse por meio de Pipelines.

🕒 Limites de turnos de conversação: defina limites nos turnos de conversação para gerenciar melhor as interações por meio de Pipelines.

🛡️ Filtragem de mensagens tóxicas: filtre automaticamente mensagens tóxicas para manter um ambiente seguro usando Pipelines.

🔍 Suporte à pesquisa na web: introduzindo recursos integrados de pesquisa na web via API RAG, permitindo que os usuários pesquisem usando SearXNG, Google Programmatic Search Engine, Brave Search, serpstack e serper. Ative-o sem esforço adicionando as variáveis ​​necessárias de Configurações do documento > Parâmetros da web.

🗂️ Espaço de trabalho de modelos: crie e gerencie predefinições de modelo para API Ollama/OpenAI. Observação: o antigo espaço de trabalho Modelfiles está obsoleto.

🛠️ Recurso Construtor de modelos: crie e edite todos os modelos com o modo construtor persistente.

🏷️ Suporte à marcação de modelo: organize os modelos com recursos de marcação no espaço de trabalho de modelos.

📋 Suporte à ordenação de modelos: organize os modelos sem esforço arrastando e soltando-os nas posições desejadas no espaço de trabalho de modelos.

📈 Estatísticas de geração OpenAI: acesse estatísticas detalhadas de geração para modelos OpenAI.

📅 Variáveis ​​de prompt do sistema: novas variáveis ​​adicionadas: '{{CURRENT_DATE}}' e '{{USER_NAME}}' para prompts dinâmicos.

📢 Suporte a banner global: gerencie banners globais em configurações de administrador > banners.

🗃️ Modal aprimorado de bate-papos arquivados: pesquise e exporte bate-papos arquivados facilmente.

📂 Botão Arquivar tudo: arquive rapidamente todos os bate-papos em configurações > bate-papos.

🌐 Traduções aprimoradas: traduções adicionadas e aprimoradas para francês, croata, cebuano e vietnamita.

Corrigido

🔍 Visibilidade de bate-papos arquivados: resolvido o problema com bate-papos arquivados que não eram exibidos no painel de administração.

💬 Estilo de mensagem: corrigidos problemas de estilo que afetavam a aparência da mensagem.

🔗 Respostas de bate-papo compartilhado: corrigido o problema em que as mensagens de resposta de bate-papo compartilhado não eram somente leitura.

🖥️ Aprimoramento da interface do usuário: corrigido o problema de sobreposição da barra de rolagem com a caixa de mensagem na interface do usuário.

Alterado

💾 Armazenamento de configurações do usuário: as configurações do usuário agora são salvas no back-end, garantindo consistência em todos os dispositivos.

📡 Solicitações de API unificadas: a solicitação de API para obter modelos agora é unificada para '/api/models' para facilitar o uso.

🔄 Atualização de versão: nossa versão agora seguirá o formato 0.x para atualizações principais e 0.x.y para patches.

📦 Exportar todos os bate-papos (todos os usuários): moveu esta funcionalidade para as configurações do Painel de administração para melhor organização e acessibilidade.

Removido

🚫 Suporte LiteLLM empacotado descontinuado: migre seu config.yaml LiteLLM para uma instância LiteLLM auto-hospedada. LiteLLM ainda pode ser adicionado via OpenAI Connections. Baixe o config.yaml LiteLLM em configurações de administrador > banco de dados > exportar config.yaml LiteLLM.

[0.1.125] - 2024-05-19
Adicionado

🔄 Interface do usuário atualizada: interface do bate-papo renovada com bolhas de bate-papo. Alterne facilmente para o estilo antigo em configurações > interface > interface do usuário de bolha de bate-papo.

📂 Interface do usuário da barra lateral aprimorada: arquivos de modelo, documentos, prompts e playground mesclados no espaço de trabalho para acesso simplificado.

🚀 Interação aprimorada com vários modelos: todas as respostas agora são exibidas simultaneamente para uma experiência mais tranquila.

🐍 Execução de código Python: execute código Python localmente no navegador com bibliotecas como 'requests', 'beautifulsoup4', 'numpy', 'pandas', 'seaborn', 'matplotlib', 'scikit-learn', 'scipy', 'regex'.

🧠 Recurso de memória experimental: insira manualmente as informações pessoais que deseja que os LLMs lembrem em configurações > personalização > memória.

💾 Configurações persistentes: configurações agora salvas como config.json para conveniência.

🩺 Endpoint de verificação de integridade: adicionado para implantação do Docker.

↕️ Suporte RTL: alterne a direção do bate-papo em configurações > interface > direção do bate-papo.

🖥️ Suporte ao PowerPoint: o pipeline RAG agora suporta documentos do PowerPoint.

🌐 Atualizações de idioma: ucraniano, turco, árabe, chinês, sérvio, vietnamita atualizados; Punjabi adicionado.

Alterado

👤 Atualização de bate-papo compartilhado: o bate-papo compartilhado agora inclui informações do usuário criador.

[0.1.124] - 2024-05-08
Adicionado

🖼️ Barra lateral de bate-papo aprimorada: agora exibe convenientemente intervalos de tempo e organiza os bate-papos por hoje, ontem e muito mais.

📜 Citações no recurso RAG: rastreie facilmente o contexto fornecido ao LLM com citações adicionadas no recurso RAG.

🔒 Opção de desativação de autenticação: introduzindo a capacidade de desativar a autenticação. Defina 'WEBUI_AUTH' como Falso para desativar a autenticação. Observação: aplicável apenas para novas instalações sem usuários existentes.

📹 Pipeline RAG do YouTube aprimorado: agora suporta vídeos que não estão em inglês para uma experiência enriquecida.

🔊 Especificar modelos TTS OpenAI: personalize sua experiência TTS especificando modelos TTS OpenAI.

🔧 Variáveis ​​de ambiente adicionais: descubra mais variáveis ​​de ambiente em nossa documentação abrangente em Documentação do DoctorAI (https://teledocmedical.com).

🌐 Suporte a idiomas: árabe, finlandês e hindi adicionados; suporte aprimorado para alemão, vietnamita e chinês.

Corrigido

🛠️ Estilo do seletor de modelo: resolvidos problemas de estilo para melhorar a experiência do usuário.

⚠️ Mensagens de aviso: resolvidas mensagens de aviso do backend.

Alterado

📝 Geração de título: saída limitada a 50 tokens.

📦 Helm Charts: Helm charts removidos, agora disponíveis em um repositório separado (https://teledocmedical.com).

[0.1.123] - 2024-05-02
Adicionado

🎨 Novo design da página inicial: design atualizado para uma aparência mais moderna e uso otimizado do espaço na tela.

📹 Pipeline RAG do Youtube: introduz pipeline RAG dedicado para vídeos do Youtube, permitindo a interação com transcrições de vídeo diretamente.

🔧 Painel de administração aprimorado: gerenciamento de usuário simplificado com opções para adicionar usuários diretamente ou em massa por meio da importação de CSV.

👥 Integração do modelo '@': alterne facilmente para modelos específicos durante as conversas; recurso de bate-papo colaborativo antigo descontinuado.

🌐 Aprimoramentos de idioma: tradução para sueco adicionada, além de melhorias para o alemão, espanhol e adição da tradução Doge.

Corrigido

🗑️ Atalho para excluir bate-papo: resolvido o problema em que o atalho não estava funcionando.

🖼️ Bug de fechamento modal: resolvido o fechamento inesperado do modal ao arrastar de dentro.

✏️ Estilo do botão Editar: corrigida a inconsistência de estilo com os botões de edição.

🌐 Problema de compatibilidade de geração de imagens: corrigido o problema de compatibilidade de geração de imagens com APIs de terceiros.

📱 Correção do ícone PWA do iOS: corrigido o formato do ícone da tela inicial do PWA do iOS.

🔍 Bug de gesto de rolagem: ajustada a sensibilidade do gesto para evitar ativação acidental ao rolar pelo código no celular; agora requer rolagem do lado esquerdo para abrir a barra lateral.

Alterado

🔄 Comprimento de contexto ilimitado: as configurações avançadas agora permitem comprimento de contexto máximo ilimitado (anteriormente limitado a 16000).

👑 Atribuição de super administrador: a primeira inscrição recebe automaticamente uma função de super administrador, inalterável por outros administradores.

🛡️ Restrições do usuário administrador: os botões de ação do usuário no painel de administração agora estão desativados para usuários com funções de administrador.

🔝 Seletor de modelo padrão: definir como opção de modelo padrão agora disponível exclusivamente na página inicial.

[0.1.122] - 2024-04-27
Adicionado

🌟 Pipeline RAG aprimorado: agora com pesquisa híbrida via 'BM25', reclassificação por 'CrossEncoder' e limites de pontuação de relevância configuráveis.

🛢️ Suporte a banco de dados externo: conecte-se perfeitamente a bancos de dados SQLite ou Postgres personalizados usando a variável de ambiente 'DATABASE_URL'.

🌐 Suporte remoto ao ChromaDB: introduzindo a capacidade de se conectar a servidores remotos do ChromaDB.

👨‍💼 Painel de administração aprimorado: os administradores agora podem verificar convenientemente as listas de bate-papo dos usuários e o status da última atividade diretamente do painel de administração.

🎨 Tela inicial: introduzindo uma tela inicial de carregamento para uma experiência de usuário mais tranquila.

🌍 Expansão do suporte a idiomas: adicionado suporte para Bangla (bn-BD), juntamente com aprimoramentos nas traduções para chinês, espanhol e ucraniano.

💻 Desempenho de renderização LaTeX aprimorado: aproveite tempos de renderização mais rápidos para equações LaTeX.

🔧 Mais variáveis ​​de ambiente: explore variáveis ​​de ambiente adicionais em nossa documentação (https://teledocmedical.com), incluindo a opção 'ENABLE_LITELLM' para gerenciar o uso de memória.

Corrigido

🔧 Compatibilidade Ollama: resolvidos erros que ocorriam quando a versão do servidor Ollama não era um inteiro, como compilações SHA ou RCs.

🐛 Vários problemas de API OpenAI: resolvidos vários problemas relacionados à API OpenAI.

🛑 Problema de sequência de parada: corrigido o problema em que a sequência de parada com uma barra invertida '' não estava funcionando.

🔤 Fallback de fonte: corrigido o problema de fallback de fonte.

Alterado

⌨️ Comportamento de entrada do prompt no celular: envio do prompt da tecla Enter desativado em dispositivos móveis para melhorar a experiência do usuário.

[0.1.121] - 2024-04-24
Corrigido

🔧 Problemas de tradução: resolvidas várias discrepâncias de tradução.

🔒 Correção de segurança LiteLLM: versão LiteLLM atualizada para resolver uma vulnerabilidade de segurança.

🖥️ Exibição de tag HTML: corrigido o problema em que a tag '< br >' não estava sendo exibida corretamente.

🔗 Conexão WebSocket: resolvida a falha da conexão WebSocket sob segurança HTTPS para o servidor ComfyUI.

📜 Otimização FileReader: implementada a inicialização FileReader por imagem em arrastar e soltar de vários arquivos para garantir a reusabilidade.

🏷️ Exibição de tag: corrigidas inconsistências de exibição de tag.

📦 Estilo de bate-papo arquivado: corrigidos problemas de estilo no bate-papo arquivado.

🔖 Bug do botão Copiar do Safari: resolvido o bug em que o botão copiar não copiava links no Safari.

[0.1.120] - 2024-04-20
Adicionado

📦 Recurso Arquivar bate-papo: arquive bate-papos facilmente com um novo botão na barra lateral e acesse bate-papos arquivados através do botão de perfil > bate-papos arquivados.

🔊 Endpoint de texto para fala configurável: personalize sua experiência de texto para fala com endpoints OpenAI configuráveis.

🛠️ Tratamento de erros aprimorado: tratamento aprimorado de mensagens de erro para falhas de conexão.

⌨️ Atalho aprimorado: ao editar mensagens, use ctrl/cmd+enter para salvar e enviar e esc para fechar.

🌐 Suporte a idiomas: adicionado suporte ao idioma georgiano e traduções aprimoradas para português e vietnamita.

Corrigido

🔧 Seletor de modelo: resolvido o problema em que a seleção do modelo padrão não estava sendo salva.

🔗 Botão Copiar link de compartilhamento: corrigido o bug em que o botão copiar não estava copiando links no Safari.

🎨 Estilo do tema claro: resolvido o problema de estilo com o tema claro.

[0.1.119] - 2024-04-16
Adicionado

🌟 Suporte aprimorado para incorporação RAG: modelos Ollama e OpenAI agora podem ser usados ​​para modelo de incorporação RAG.

🔄 Integração perfeita: copie 'ollama run <nome do modelo>' diretamente da página Ollama para selecionar e extrair modelos facilmente.

🏷️ Recurso de marcação: adicione tags aos bate-papos diretamente na barra lateral do menu de bate-papo.

📱 Acessibilidade móvel: deslize para a esquerda e para a direita no celular para abrir e fechar a barra lateral sem esforço.

🔍 Navegação aprimorada: o painel de administração agora suporta paginação para a lista de usuários.

🌍 Suporte adicional ao idioma: adicionado suporte ao idioma polonês.

Corrigido

🌍 Aprimoramentos de idioma: as traduções em vietnamita e espanhol foram aprimoradas.

🔧 Correções do Helm: resolvidos problemas com a barra final do Helm e manifest.json.

Alterado

🐳 Otimização do Docker: processo de compilação de imagem do docker atualizado para utilizar 'uv' para compilações significativamente mais rápidas em comparação com 'pip3'.

[0.1.118] - 2024-04Adicionado

🦙 Imagens Ollama e CUDA: Adicionado suporte para imagens marcadas com ':ollama' e ':cuda'.

👍 Classificação de resposta aprimorada: agora você pode anotar suas classificações para um feedback melhor.

👤 Foto de perfil com iniciais do usuário: as iniciais do usuário agora são a foto de perfil padrão.

🔍 Atualizar modelo de incorporação RAG: personalize o modelo de incorporação RAG diretamente nas configurações do documento.

🌍 Suporte adicional ao idioma: adicionado suporte ao idioma turco.

Corrigido

🔒 Permissão de bate-papo de compartilhamento: resolvido o problema com as permissões de compartilhamento de bate-papo.

🛠 Fechamento modal: os modais agora podem ser fechados usando a tecla Esc.

Alterado

🎨 Estilo do painel de administração: estilo atualizado para o painel de administração.

🐳 Compilação de imagem do Docker: processo de compilação de imagem do docker atualizado para maior eficiência.

[0.1.117] - 2024-04-03
Adicionado

🗨️ Compartilhamento de bate-papo local: compartilhe links de bate-papo perfeitamente entre os usuários.

🔑 Suporte à geração de chave de API: gere chaves secretas para aproveitar o DoctorAI com bibliotecas OpenAI.

📄 Download do bate-papo como PDF: baixe bate-papos facilmente em formato PDF.

📝 Registro aprimorado: aprimoramentos na funcionalidade de registro.

📧 Autenticação de e-mail confiável: autentique usando um cabeçalho de e-mail confiável.

Corrigido

🌷 Tradução holandesa aprimorada: tradução aprimorada para usuários holandeses.

⚪ Estilo do tema branco: resolvido o problema de estilo com o tema branco.

📜 Estouro de tela de bate-papo LaTeX: corrigido o problema de estouro de tela com a renderização LaTeX.

🔒 Patches de segurança: patches de segurança necessários aplicados.

[0.1.116] - 2024-03-31
Adicionado

🔄 Interface do usuário aprimorada: o seletor de modelo agora está convenientemente localizado na barra de navegação, permitindo a alternância perfeita entre vários modelos durante as conversas.

🔍 Seletor de modelo aprimorado: extraia um modelo diretamente do seletor/os modelos agora exibem informações detalhadas para melhor compreensão.

💬 Suporte a Webhook: agora compatível com o Google Chat e o Microsoft Teams.

🌐 Localização: tradução coreana (I18n) agora disponível.

🌑 Tema escuro: tema escuro OLED introduzido para reduzir o cansaço visual durante o uso prolongado.

🏷️ Autocompletar de tag: recurso suspenso adicionado para marcação de bate-papo sem esforço.

Corrigido

🔽 Rolagem automática: resolvido o problema de rolagem automática do OpenAI.

🏷️ Validação de tag: implementada a validação de tag para evitar tags de string vazias.

🚫 Lista de permissões de modelo: resolvido o problema de lista de permissões de modelo LiteLLM.

✅ Ortografia: corrigidos vários erros ortográficos para melhorar a legibilidade.

[0.1.115] - 2024-03-24
Adicionado

🔍 Seletor de modelo personalizado: encontre e selecione modelos personalizados facilmente com o novo recurso de filtro de pesquisa.

🛑 Cancelar download do modelo: adicionada a capacidade de cancelar downloads de modelo.

🎨 Geração de imagens ComfyUI: a geração de imagens agora suporta ComfyUI.

🌟 Tema claro atualizado: tema claro atualizado para uma nova aparência.

🌍 Suporte adicional a idiomas: agora com suporte para búlgaro, italiano, português, japonês e holandês.

Corrigido

🔧 Upload GGUF quebrado experimental corrigido: resolvidos problemas com a funcionalidade experimental de upload GGUF.

Alterado

🔄 Botão Redefinir armazenamento vetorial: movido o botão redefinir armazenamento vetorial para as configurações do documento.

[0.1.114] - 2024-03-20
Adicionado

🔗 Integração de Webhook: agora você pode assinar novos eventos de inscrição de usuário via webhook. Basta navegar até o painel de administração > configurações de administrador > URL do webhook.

🛡️ Filtragem de modelo aprimorada: além da lista de permissões de modelo proxy OpenAI, Ollama, adicionamos funcionalidade de filtragem de modelo para proxy LiteLLM.

🌍 Suporte a idiomas expandido: os idiomas espanhol, catalão e vietnamita agora estão disponíveis, com melhorias feitas em outros.

Corrigido

🔧 Ortografia do campo de entrada: resolvido o problema com erros ortográficos nos campos de entrada.

🖊️ Estilo do modo claro: corrigido o problema de estilo com o modo claro na adição de documento.

Alterado

🔄 Classificação de idiomas: os idiomas agora são classificados em ordem alfabética por seu código para melhor organização.

[0.1.113] - 2024-03-18
Adicionado

🌍 Localização: agora você pode alterar o idioma da interface do usuário em Configurações > Geral. Oferecemos suporte a traduções para ucraniano, alemão, farsi (persa), chinês tradicional e simplificado e francês. Você pode nos ajudar a traduzir a interface do usuário para o seu idioma! Mais informações em nosso CONTRIBUTION.md.

🎨 Tema de todo o sistema: introduzindo um novo tema de todo o sistema para uma experiência visual aprimorada.

Corrigido

🌑 Fundo escuro em campos de seleção: legibilidade aprimorada adicionando um fundo escuro aos campos de seleção, resolvendo problemas em determinados navegadores/dispositivos.

Problema de vários OPENAI_API_BASE_URLS: resolvido o problema em que vários URLs base causavam conflitos quando um não estava funcionando.

Problema de codificação RAG: corrigido o problema de codificação em RAG.

Correção de auditoria npm: resultados de auditoria npm abordados.

Limite de rolagem reduzido: experiência de rolagem automática aprimorada, reduzindo o limite de rolagem de 50px para 5px.

Alterado

🔄 Atualização da interface do usuário da barra lateral: interface do usuário da barra lateral atualizada para apresentar um menu suspenso de bate-papo, substituindo dois ícones para melhorar a navegação.

[0.1.112] - 2024-03-15
Corrigido

🗨️ Resolvido o mau funcionamento do bate-papo após a geração de imagens.

🎨 Corrigidos vários problemas de RAG.

🧪 Corrigida a lógica experimental de upload GGUF quebrada.

[0.1.111] - 2024-03-10
Adicionado

🛡️ Lista de permissões de modelo: os administradores agora têm a capacidade de incluir modelos na lista de permissões para usuários com a função 'usuário'.

🔄 Atualizar todos os modelos: adicionado um botão conveniente para atualizar todos os modelos de uma vez.

📄 Alternar OCR de PDF: os usuários agora podem alternar a opção OCR de PDF para melhorar o desempenho da análise.

🎨 Integração DALL-E: introduzida a integração DALL-E para geração de imagens juntamente com automatic1111.

🛠️ Refatoração da API RAG: lógica RAG refatorada e sua API exposta, com documentação adicional a seguir.

Corrigido

🔒 Configurações de token máximo: adicionadas configurações de token máximo para antrópico/claude-3-soneto-20240229 (Problema #1094).

🔧 Problema de desalinhamento: corrigido o desalinhamento dos ícones Editar e Excluir quando o título do bate-papo está vazio (Problema #1104).

🔄 Correção de perda de contexto: resolvido o problema de RAG perdendo contexto na regeneração da resposta do modelo com modelos Groq via chave de API (Problema #1105).

📁 Bug de manipulação de arquivo: resolvido o problema de notificação de arquivo não encontrado ao descartar um elemento de conversação (Problema #1098).

🖱️ Estilo de arquivo arrastado: corrigido o problema de estilo de sobreposição de arquivo arrastado.

[0.1.110] - 2024-03-06
Adicionado

🌐 Suporte a vários servidores OpenAI: desfrute de integração perfeita com várias APIs compatíveis com OpenAI, agora suportadas nativamente.

Corrigido

🔍 Problema de OCR: resolvido o problema de análise de PDF causado por mau funcionamento do OCR.

🚫 Problema de RAG: corrigida a funcionalidade RAG, garantindo que ela funcione sem problemas.

📄 Botão de modelo "Adicionar documentos": resolvido o comportamento não funcional do botão de modelo "Adicionar documentos".

[0.1.109] - 2024-03-06
Adicionado

🔄 Suporte a vários servidores Ollama: desfrute de escalabilidade e desempenho aprimorados com suporte para vários servidores Ollama em uma única interface do usuário da Web. Os recursos de balanceamento de carga agora estão disponíveis, proporcionando maior eficiência (#788, #278).

🔧 Suporte para Claude 3 e Gemini: respondendo às solicitações do usuário, expandimos nosso conjunto de ferramentas para incluir Claude 3 e Gemini, oferecendo uma gama mais ampla de funcionalidades em nossa plataforma (#1064).

🔍 Funcionalidade OCR para carregador de PDF: aumentamos nosso carregador de PDF com recursos de reconhecimento óptico de caracteres (OCR). Agora, extraia texto de documentos digitalizados e imagens em PDFs, ampliando o escopo do processamento de conteúdo (#1050).

Corrigido

🛠️ Coleção RAG: implementado um mecanismo dinâmico para recriar coleções RAG, garantindo que os usuários tenham dados atualizados e precisos (#1031).

📝 Cabeçalhos do agente do usuário: corrigido o problema de solicitações da web RAG sendo enviadas com cabeçalhos user_agent vazios, reduzindo rejeições de determinados sites. Cabeçalhos realistas agora são utilizados para essas solicitações (#1024).

⏹️ Funcionalidade Cancelar do Playground: introduzindo uma nova opção "Cancelar" para interromper a geração do Ollama no Playground, aprimorando o controle e a usabilidade do usuário (#1006).

🔤 Erro tipográfico no campo 'ASSISTENTE': corrigido um erro tipográfico no campo 'ASSISTENTE' no modelo de upload GGUF para precisão e consistência (#1061).

Alterado

🔄 Lógica de exclusão de mensagem refatorada: processo de exclusão de mensagem simplificado para maior eficiência e experiência do usuário, simplificando as interações na plataforma (#1004).

⚠️ Descontinuação de OLLAMA_API_BASE_URL: variável de ambiente OLLAMA_API_BASE_URL descontinuada; recomenda-se usar OLLAMA_BASE_URL em vez disso. Consulte nossa documentação para obter mais detalhes.

[0.1.108] - 2024-03-02
Adicionado

🎮 Recurso Playground (Beta): explore todo o potencial da API bruta por meio de uma interface do usuário intuitiva com nosso novo recurso de playground, acessível aos administradores. Basta clicar na área do nome inferior da barra lateral para acessá-lo. O recurso playground oferece dois modos: preenchimento de texto (notebook) e preenchimento de bate-papo. Como está em versão beta, relate quaisquer problemas que encontrar.

🛠️ Download direto do banco de dados para administradores: os administradores agora podem baixar o banco de dados diretamente da interface do usuário da Web por meio das configurações de administrador.

🎨 Configurações RAG adicionais: personalize seu processo RAG com a capacidade de editar o valor TOP K. Navegue até Documentos > Configurações > Geral para fazer alterações.

🖥️ Melhorias na interface do usuário: dicas de ferramentas agora disponíveis na área de entrada e na alça da barra lateral. Mais dicas de ferramentas serão adicionadas em outras partes da interface do usuário.

Corrigido

Resolvido o problema de foco automático de entrada no celular quando a barra lateral está aberta, tornando mais fácil de usar.

Corrigido o problema de exibição da lista numerada no Safari (#963).

Capacidade restrita do usuário de excluir bate-papos sem as permissões adequadas (#993).

Alterado

Configurações simplificadas do Ollama: as configurações do Ollama agora não exigem o sufixo /api. Agora você pode utilizar o URL base do Ollama diretamente, por exemplo, http://localhost:11434. Além disso, uma variável de ambiente OLLAMA_BASE_URL foi adicionada.

Renomeação do banco de dados: a partir desta versão, ollama.db será renomeado automaticamente para webui.db.

[0.1.107] - 2024-03-01
Adicionado

🚀 Makefile e script de atualização LLM: incluídos Makefile e um script para atualizações LLM no repositório.

Corrigido

⚫ Ícones da interface do usuário: ícones da interface do usuário corrigidos que não eram exibidos corretamente.

🎤 Problema de carregamento de arquivo: resolvido o problema que impedia o upload de arquivos de áudio para modelos de fala para texto.

💬 Respostas vazias: corrigido o problema de respostas vazias ao usar modelos de bate-papo.

🛠 Título da guia: o título da guia agora é atualizado dinamicamente com base no título do bate-papo ativo.

[0.1.106] - 2024-02-26
Adicionado

🎨 Modo de conversação: introduzido um modo de conversação para interações mais longas e contextuais, permitindo que os usuários alternem entre os modos de bate-papo único e de conversação.

Corrigido

🔃 Problema de loop infinito: corrigido um problema de loop infinito encontrado em cenários específicos.

💾 Problema de salvamento do modelo: resolvido o problema em que as configurações do modelo não eram salvas corretamente.

🎤 Suporte a WAV: adicionado suporte para arquivos WAV, expandindo as opções de entrada de áudio.

[0.1.105] - 2024-02-25
Adicionado

🚀 Suporte a modelos GGUF: agora você pode fazer upload e usar arquivos GGUF no DoctorAI, expandindo as opções de modelo disponíveis.

🎨 Aprimoramentos da interface do usuário: várias melhorias na interface do usuário foram implementadas com base no feedback do usuário.

Corrigido

🐞 Bugs de upload de arquivo: corrigidos vários bugs que afetavam o processo de upload de arquivo.

💬 Problemas de bate-papo: resolvidos problemas que causavam mau funcionamento do bate-papo em determinadas circunstâncias.

🛠 Outras pequenas correções: várias pequenas correções e melhorias foram feitas para melhorar a estabilidade e o desempenho geral.

[0.1.104] - 2024-02-24

Esta versão marca o lançamento inicial do DoctorAI, uma interface de usuário da Web de código aberto para LLMs. Ele fornece uma plataforma amigável para interagir com modelos de linguagem grandes, oferecendo vários recursos e integrações.
