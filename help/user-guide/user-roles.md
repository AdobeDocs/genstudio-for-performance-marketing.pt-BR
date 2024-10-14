---
title: Funções e permissões de usuário do Adobe GenStudio for Performance Marketing
description: Saiba mais sobre as funções e permissões de usuário do GenStudio for Performance Marketing.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
source-git-commit: 3e9a2a4f42ba79389691705c571bf6bbd0b990c5
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 2%

---

# Funções e permissões do usuário

A criação e a implantação de campanhas de marketing modernas exigem a colaboração entre as partes interessadas com diferentes responsabilidades e conjuntos de habilidades. _Funções do usuário_ controlam o acesso das partes interessadas aos vários recursos da GenStudio for Performance Marketing. Sua função de usuário atribuída determina as tarefas que você pode executar usando essa plataforma. Um administrador de sistema do Adobe atribui você a uma função no perfil de produto do GenStudio no Adobe Admin Console. O email de boas-vindas identifica a função atribuída.

>[!NOTE]
>
>Antes que qualquer usuário seja provisionado nessas funções, um administrador de sistema do Adobe deve ser designado no Adobe Admin Console para executar tarefas de configuração únicas. Essa função de administrador de Adobe opera somente no contexto do Adobe Admin Console. Ele não tem nenhuma função na interface da plataforma do GenStudio for Performance Marketing. Um administrador de sistema Adobe que precise de direitos de gerente de sistema deve provisionar-se como um gerente de sistema GenStudio no Adobe Admin Console. Consulte [Provisionar GenStudio for Performance Marketing](product-provisioning.md).

## Direitos

_Os direitos_ concedem permissão para executar tarefas específicas e acessar recursos protegidos. Os direitos são definidos na função de usuário no perfil do produto e os usuários recebem esses direitos quando atribuídos a essa função.

## Funções do usuário

Três tipos de funções de usuário do GenStudio for Performance Marketing oferecem suporte a essa diversidade de funções organizacionais. As permissões são personalizadas para cada um desses tipos de usuários e oferecem suporte às responsabilidades de cada usuário na organização de marketing. Esses três tipos de função de usuário são:

* **Os editores do GenStudio** usam os recursos de IA gerativa da GenStudio for Performance Marketing para criar ativos de campanha de marketing, solicitar revisão e aprovação de conteúdo e publicar rascunhos aprovados desse conteúdo. Todos os usuários do GenStudio for Performance Marketing podem acessar e usar um ativo depois que seu editor o salvar em [!DNL Content].

* **Os colaboradores do GenStudio** são o maior número de usuários do GenStudio for Performance Marketing. Os colaboradores podem visualizar e aprovar o conteúdo e são uma parte essencial do fluxo de trabalho, garantindo que o conteúdo gerado corresponda às necessidades e padrões da sua organização.

* **os gerenciadores de sistemas do GenStudio** têm o mais amplo conjunto de permissões da GenStudio for Performance Marketing. Os gerentes de sistema executam a tarefa essencial de integração de estabelecer as medidas de proteção fundamentais para a criação e implantação de ativos de campanha. Os gerentes de sistema implementam essas medidas de proteção fazendo upload das informações específicas da marca e da organização, como as [diretrizes da marca](./guidelines/overview.md). Os gerentes de sistema têm permissão para criar e publicar [!DNL Brands], mas não têm privilégios de administração de usuário.

### editores do GenStudio

Os _editores_ ou criadores de conteúdo têm as permissões principais necessárias para criar ativos do GenStudio for Performance Marketing [!DNL Brands], [!DNL Campaigns] e [!DNL Content]. Eles também podem editar e excluir os ativos que criaram. O GenStudio for Performance Marketing oferece suporte à criação rápida de centenas de conteúdo. Esses usuários podem gerar fragmentos de conteúdo ou experiências inteiras que orquestram partes distintas de conteúdo aprovado para atender às necessidades de campanhas de marketing específicas.

Os editores interagem com as tecnologias de IA gerativa da GenStudio for Performance Marketing por meio de _prompts_. A gaveta de prompts na Tela fornece ferramentas para colocar prompts no contexto das diretrizes de uma campanha específica. Como resultado, a qualidade e o sucesso do conteúdo gerado dependem parcialmente da qualidade das diretrizes de marca que sua organização carregou e da especificidade do seu prompt. Consulte [Gravar prompts efetivos](effective-prompts.md).

A tabela a seguir exibe as permissões padrão do editor:

| Destaque | Criar | Atualizar o | Excluir | Exibir |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | não | não | não | sim |
| [!DNL Campaigns] | sim | sim | sim | sim |
| [!DNL Content] | sim | sim | sim | sim |
| [!DNL Create] | sim | sim | sim | sim |
| [!DNL Insights] | pode configurar apenas conectores de anúncios |    |     | sim |
| [!DNL Personas] | sim | sim* | sim* | sim |
| [!DNL Products] | sim | sim* | sim* | sim |
| [!DNL Reviews and approvals] | sim | sim | sim | sim |

Editores podem editar e excluir [!DNL Personas] e [!DNL Products] criados por eles.

Os gerentes de sistema da GenStudio podem dar permissão aos editores para editar e excluir um [!DNL Brand].

### Colaboradores da GenStudio

_Os colaboradores_ podem exibir ativos na GenStudio for Performance Marketing, mas não podem criar, editar nem excluir esses ativos. Os colaboradores incluem participantes essenciais para o sucesso do processo de revisão e aprovação do conteúdo, mas que não precisam criar ou editar diretamente o conteúdo. Juristas e gerentes de criativos são exemplos de colaboradores potenciais. Os colaboradores da GenStudio for Performance Marketing podem ter permissão para criar e visualizar ativos em outros produtos Creative Cloud.

A tabela a seguir exibe as permissões padrão do colaborador:

| Destaque | Criar | Atualizar o | Excluir | Exibir |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | não | não | não | sim |
| [!DNL Campaigns] | não | não | não | sim |
| [!DNL Content] | não | não | não | sim |
| [!DNL Create] | não | não | não | sim |
| [!DNL Insights] | não | não | não | sim |
| [!DNL Personas] | não | não | não | sim |
| [!DNL Products] | não | não | não | sim |
| [!DNL Reviews and approvals] | não | não | não | sim |

### Gerenciadores de sistema da GenStudio

_os gerenciadores de sistemas do GenStudio_ têm o conjunto de permissões mais avançado da GenStudio for Performance Marketing. Os gerentes de sistema executam a tarefa essencial de integração de estabelecer as medidas de proteção fundamentais para a criação e implantação de ativos de campanha. Os gerentes de sistema implementam essas medidas de proteção fazendo upload das informações específicas da marca e da organização, como as [diretrizes da marca](./guidelines/overview.md). Os gerentes de sistema têm permissão para criar e publicar [!DNL Brands], mas não têm privilégios de administração de usuário.

A tabela a seguir exibe as permissões padrão do gerenciador de sistemas:

| Destaque | Criar | Atualizar o | Excluir | Exibir |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | sim | sim | sim | sim |
| [!DNL Campaigns] | sim | sim | sim | sim |
| [!DNL Content] | sim | sim | sim | sim |
| [!DNL Insights] | sim | sim | sim | sim |
| [!DNL Personas] | sim | sim | sim | sim |
| [!DNL Products] | sim | sim | sim | sim |
| [!DNL Reviews and approvals] | sim | sim | sim | sim |

Consulte [Introdução ao Adobe GenStudio for Performance Marketing](get-started.md) para obter uma visão geral das tarefas de configuração preliminares.
