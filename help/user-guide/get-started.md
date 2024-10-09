---
title: Introdução ao Adobe GenStudio for Performance Marketing
description: Saiba como configurar seu GenStudio for Performance Marketing para gerar novo conteúdo de marketing alinhado à marca.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
exl-id: bcb03198-bbcb-45ae-af01-25c1e834b563
source-git-commit: ce08231cb723bec3d80a732837b72a435d3b552d
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 1%

---

# Introdução ao Adobe GenStudio for Performance Marketing

O Adobe GenStudio for Performance Marketing é uma plataforma abrangente para criar, avaliar e gerenciar experiências de marketing que refletem e seguem a identidade da sua marca.

O acesso das partes interessadas a seus vários recursos é controlado pelas _funções de usuário_ atribuídas. Sua função de usuário atribuída determina as tarefas que você pode executar no GenStudio for Performance Marketing. Um administrador de sistema do Adobe atribui suas permissões no perfil de produto do GenStudio for Performance Marketing no Adobe Admin Console. O email de boas-vindas identifica a função atribuída.

Se você é novo em ferramentas generativas baseadas em IA ou está simplesmente curioso sobre os princípios básicos do GenStudio for Performance Marketing, consulte [Conceitos](concepts.md) e [Gravar prompts efetivos](effective-prompts.md).

## Funções do usuário

A criação e a implantação de campanhas de marketing modernas exigem a colaboração entre as partes interessadas com diferentes responsabilidades e conjuntos de habilidades.

Três tipos de funções de usuário do GenStudio for Performance Marketing oferecem suporte a essa diversidade de funções organizacionais. As permissões são personalizadas para cada um desses tipos de usuários e oferecem suporte às responsabilidades de cada usuário na organização de marketing.

**Os três tipos de função de usuário são**:

* **Os editores** usam os recursos de IA gerativa da GenStudio for Performance Marketing para criar ativos de campanha de marketing, solicitar revisão e aprovação de conteúdo e publicar rascunhos aprovados desse conteúdo. Todos os usuários do GenStudio for Performance Marketing podem acessar e usar um ativo depois que seu criador o tiver salvo no conteúdo.

* **Colaboradores** são o maior número de usuários do GenStudio for Performance Marketing. Os colaboradores podem visualizar e aprovar o conteúdo e são uma parte essencial do fluxo de trabalho, garantindo que o conteúdo gerado corresponda às necessidades e padrões da sua organização.

* **Os gerenciadores de sistemas** têm o mais amplo conjunto de permissões no GenStudio for Performance Marketing. Os gerentes de sistema executam a tarefa essencial de integração de estabelecer as medidas de proteção fundamentais para a criação e implantação de ativos de campanha. Os gerentes de sistema implementam essas medidas de proteção fazendo upload das informações específicas da marca e da organização, como as [diretrizes da marca](/help/user-guide/guidelines/overview.md). Os gerentes de sistema da GenStudio for Performance Marketing têm permissão para criar e publicar marcas, mas não têm privilégios de administração do usuário.

>[!NOTE]
>Antes que qualquer usuário seja provisionado nessas funções, um administrador de sistema do Adobe deve ser designado no Adobe Admin Console para executar tarefas de configuração únicas. Essa função de administrador de Adobe opera somente no contexto do Adobe Admin Console. Ele não tem nenhuma função na interface da plataforma do GenStudio for Performance Marketing.

### editores do GenStudio for Performance Marketing

**Editores** têm as permissões principais necessárias para criar ativos do GenStudio for Performance Marketing [!DNL Brands], [!DNL Campaigns] e [!DNL Content]. Eles também podem editar e excluir os ativos que criaram. O GenStudio for Performance Marketing oferece suporte à criação rápida de centenas de conteúdo. Esses usuários podem gerar seções de conteúdo ou experiências completas que orquestram partes distintas de conteúdo aprovado para atender às necessidades de campanhas de marketing específicas.

Os editores interagem com as tecnologias de IA gerativa da GenStudio for Performance Marketing por meio de _prompts_. A área de prompt na Tela de Pintura fornece ferramentas para colocar prompts no contexto das diretrizes de uma campanha específica. Como resultado, a qualidade e o sucesso do conteúdo gerado dependem parcialmente da qualidade das diretrizes de marca que sua organização carregou e da especificidade do seu prompt.

Consulte [Gravar prompts efetivos](effective-prompts.md).

A tabela a seguir exibe as permissões padrão do editor:

| Destaque | Criar | Atualizar o | Excluir | Exibir |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | não | não | não | sim |
| [!DNL Campaigns] | sim | sim | sim | sim |
| [!DNL Content] | sim | sim | sim | sim |
| [!DNL Insights] | pode configurar apenas conectores de anúncios |    |     | sim |
| [!DNL Personas] | sim | sim | sim | sim |
| [!DNL Products] | sim | sim | sim | sim |
| [!DNL Reviews and approvals] | sim | sim | sim | sim |

### Colaboradores da GenStudio for Performance Marketing

**Os colaboradores** podem exibir ativos na GenStudio for Performance Marketing, mas não podem criar, editar nem excluir esses ativos. Os colaboradores incluem participantes essenciais para o sucesso do processo de revisão e aprovação do conteúdo, mas que não precisam criar ou editar diretamente o conteúdo. Juristas e gerentes de criadores são exemplos de colaboradores potenciais. Os colaboradores da GenStudio for Performance Marketing podem ter permissões para criar e visualizar ativos em outros produtos Creative Cloud.

A tabela a seguir exibe as permissões padrão do colaborador:

| Destaque | Criar | Atualizar o | Excluir | Exibir |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | não | não | não | sim |
| [!DNL Campaigns] | não | não | não | sim |
| [!DNL Content] | não | não | não | sim |
| [!DNL Insights] | não | não | não | sim |
| [!DNL Personas] | não | não | não | sim |
| [!DNL Products] | não | não | não | sim |
| [!DNL Reviews and approvals] | não | não | não | sim |

### Gerenciadores de sistema da GenStudio for Performance Marketing

Os **gerentes de sistema da GenStudio** concluem as tarefas iniciais que preparam sua organização para implantar o GenStudio for Performance Marketing.

A tabela a seguir exibe as permissões padrão do GenStudio for Performance Marketing System Manager:

| Destaque | Criar | Atualizar o | Excluir | Exibir |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | sim | sim | sim | sim |
| [!DNL Campaigns] | sim | sim | sim | sim |
| [!DNL Content] | sim | sim | sim | sim |
| [!DNL Insights] | sim | sim | sim | sim |
| [!DNL Personas] | sim | sim | sim | sim |
| [!DNL Products] | sim | sim | sim | sim |
| [!DNL Reviews and approvals] | sim | sim | sim | sim |


## Preparar o GenStudio for Performance Marketing para gerar conteúdo

Os gerentes de sistema da GenStudio for Performance Marketing preparam o ambiente GenStudio for Performance Marketing de sua organização para que editores e colaboradores criem ativos de campanha. Essas tarefas preliminares de configuração incluem:

1. [Adicionar diretrizes](./guidelines/overview.md) para [!DNL Brands], [!DNL Products] e [!DNL Personas]. Configurar os elementos fundamentais da identidade de marca de sua organização é um pré-requisito essencial para o trabalho de criadores e colaboradores. Você pode fazer upload de documentos de diretrizes da marca ou inserir manualmente as informações da marca.
   * **Prepare seus documentos de diretrizes**. Quanto mais descritivas e abrangentes forem as diretrizes da sua marca, melhor será o resultado. Inclua breves exemplos de recursos que você considera essenciais para sua marca e adicione descrições de comportamento que deseja excluir da criação de conteúdo. O GenStudio for Performance Marketing extrai informações desses documentos carregados e começa a criar sua marca. Informações como voz da marca, canal e diretrizes de imagem são preenchidas conforme a GenStudio for Performance Marketing monta cada diretriz dos documentos carregados.
   * **Edite ou preencha os campos de diretriz da marca conforme necessário**. As diretrizes abrangentes da marca formam a base para a GenStudio for Performance Marketing entender a marca da sua organização. Depois que a GenStudio for Performance Marketing tiver extraído as informações necessárias dos documentos de diretrizes da marca, você será solicitado a editar ou preencher manualmente os campos das informações extraídas. Especifique áreas de foco de produto individuais para criação de conteúdo adicionando um [!DNL Product]. As diretrizes do [!DNL Personas] ajudam a adaptar a criação de conteúdo para segmentos de clientes definidos.

   Embora a configuração das diretrizes de marca de uma organização possa ser uma ação única, talvez seja necessário revisar e aprimorar essas diretrizes com base na volatilidade, no crescimento e nas mudanças nas circunstâncias do mercado de sua organização.

1. **[Carregar modelos](./content/use-templates.md)**. Os modelos fornecem atalhos e aceleram a criação de conteúdo. Um modelo contém recursos aprovados, como cabeçalhos e rodapés, e estabelece medidas de proteção para a criação de conteúdo. Os gerentes de sistema normalmente fazem upload e gerenciam modelos para sua organização. Os criadores usam modelos para iniciar rapidamente o processo de criação de conteúdo dentro dos limites estabelecidos da marca organizacional.

1. **[Carregar ativos aprovados](./content/manage-assets.md)**. Os ativos aprovados em [!DNL Content] estão disponíveis para todos os criadores do GenStudio for Performance Marketing. Você pode propagar [!DNL Content] com ativos que os criadores podem usar para criar novas experiências ou ativos.

1. **[Conectar a uma conta Meta (Facebook)](./insights/connect-channel.md)**. Configure uma conexão entre o GenStudio for Performance Marketing e as contas sociais de sua organização para receber dados de suas campanhas de marketing ativas, ativos e experiências. [[!DNL Insights]](./insights/overview.md) fornece ferramentas para analisar dados derivados de canais.
