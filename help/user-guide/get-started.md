---
title: Introdução ao Adobe GenStudio for Performance Marketing
description: Saiba como começar a usar o GenStudio for Performance Marketing para gerar novo conteúdo de marketing alinhado à marca.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
exl-id: bcb03198-bbcb-45ae-af01-25c1e834b563
source-git-commit: 3c391753ebd0d19ad7dcb17870915eeccc55cc05
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# Introdução ao Adobe GenStudio for Performance Marketing

O Adobe GenStudio for Performance Marketing oferece um conjunto abrangente de ferramentas projetadas para simplificar a criação, o gerenciamento e a análise de conteúdo. Ele integra o ciclo de vida da criação de conteúdo aos recursos de IA gerativa que transformam a forma como o conteúdo de marketing é criado, revisado, compartilhado e analisado.

## Comece a criar, compartilhar e revisar conteúdo

Se você é novo em ferramentas generativas baseadas em IA ou está simplesmente curioso sobre os princípios fundamentais do GenStudio for Performance Marketing, consulte [Conceitos](concepts.md) e [Gravar prompts efetivos](effective-prompts.md). Você pode conferir a [Adobe GenStudio Academy](https://learningmanager.adobe.com/genstudioacademy), plataforma de aprendizado online de Adobe sobre o uso de tecnologias de IA gerativa no processo criativo.

## Treinar o GenStudio for Performance Marketing

O GenStudio for Performance Marketing usa informações sobre sua marca e mercados para aprimorar a criação de conteúdo compatível com a marca. Os materiais de treinamento incluem exemplos, descrições de [personas](/help/user-guide/guidelines/personas.md) e [produtos](/help/user-guide/guidelines/products.md) do cliente e [diretrizes de marca](/help/user-guide/guidelines/overview.md).

Os gerentes de sistema configuram o Adobe GenStudio for Performance Marketing inserindo ou fazendo upload de informações específicas da organização. Essa preparação garante que editores de conteúdo e colaboradores possam usar efetivamente os recursos de IA gerativa para criar e revisar ativos de campanha. Depois que um administrador de sistema do Adobe provisiona a instância de produto da organização e atribui permissões de gerente de sistema da GenStudio, o gerente de sistema da GenStudio pode preparar a estrutura de IA gerativa subjacente do produto usando diretrizes.

### Etapa 1: adicionar diretrizes

Configurar os elementos fundamentais da identidade de marca de sua organização é um pré-requisito essencial para o trabalho de editores de conteúdo e colaboradores. As [diretrizes](./guidelines/overview.md) capturam as características da marca, como logotipos, tom de voz e paletas de cores. Você pode carregar [[!DNL Brands] diretrizes](./guidelines/brands.md) documentos ou inserir manualmente informações sobre a marca. [[!DNL Personas] diretrizes](./guidelines/personas.md) e [[!DNL Products] diretrizes](./guidelines/products.md) também são importantes. Os recursos subjacentes de IA gerativa do GenStudio for Performance Marketing usam essas diretrizes para estabelecer medidas de proteção que orientam a geração de conteúdo.

#### Preparar seus documentos de orientação

As diretrizes abrangentes e focalizadas do [[!DNL Brands]](./guidelines/brands.md), [[!DNL Products]](./guidelines/products.md) e [[!DNL Personas]](./guidelines/personas.md) definem os aspectos principais das campanhas de marketing da sua organização. A GenStudio for Performance Marketing extrai informações dessas diretrizes para começar a criar sua marca.

Siga estas práticas recomendadas ao preparar diretrizes:

* Use um idioma específico.

* Inclua os melhores exemplos que encontrar do estilo e tom que deseja que os ativos da campanha incorporem.

* Evite redundância. Você pode ser tentado a repetir uma diretiva várias vezes, mas a redundância em suas diretrizes não ajuda a capturar e implementar as diretrizes de marca subjacentes do LLM.

* Identifique os elementos que você deseja que o LLM exclua durante a geração do conteúdo (por exemplo, pontos de exclamação no texto).

Você pode fazer upload de documentos de orientação ou consultá-los à medida que insere informações manualmente no GenStudio for Performance Marketing. Consulte [Adicionar diretrizes](./guidelines/overview.md) para obter orientação sobre como carregar ou inserir essas informações.

#### Revisar diretrizes

Um gerente de sistema da GenStudio pode preparar a estrutura de IA gerativa subjacente do produto inserindo ou fazendo upload manualmente dos requisitos específicos da marca de sua organização. Embora a configuração das diretrizes de marca de uma organização seja uma ação única, você pode revisar e aprimorar essas diretrizes com base na volatilidade, no crescimento e na alteração das circunstâncias do mercado de sua organização.

## Etapa 2: configurar um projeto do Adobe Admin Console para o GenStudio [!DNL Brands]

Os administradores do sistema devem concluir tarefas adicionais de configuração antes que os colaboradores possam editar ou criar [!DNL Brands]. Os administradores de sistema do Adobe executam estas tarefas no Adobe Admin Console:

* Crie um novo grupo de usuários que inclua todos os usuários que precisem editar e crie [!DNL Brands] direitos.

* Crie um novo projeto na Adobe Admin Console.

Consulte [Atribuir permissões de marca](configure-brand-permissions.md).

### Etapa 3: Fazer upload de modelos

Os modelos aceleram a criação de conteúdo. Um modelo contém recursos aprovados, como cabeçalhos e rodapés, e é otimizado para canais específicos. Os gerentes de sistema normalmente fazem upload e gerenciam modelos para sua organização. Os editores de conteúdo usam modelos para iniciar rapidamente o processo de criação de conteúdo dentro dos limites estabelecidos da marca organizacional.

Consulte [Trabalhar com modelos](./content/use-templates.md).

### Etapa 4: Fazer upload de ativos aprovados

Os ativos aprovados em [!DNL Content] estão disponíveis para todos os editores do GenStudio for Performance Marketing. Você pode preencher [!DNL Content] com ativos para que os editores de conteúdo os usem na criação de novas experiências ou ativos.

Consulte [Carregar ativos aprovados](./content/manage-assets.md).

### Etapa 5: conectar-se a uma conta Meta (Facebook)

Configure uma conexão entre o GenStudio for Performance Marketing e as contas sociais de sua organização para receber dados de suas campanhas de marketing ativas, ativos e experiências. [[!DNL Insights]](./insights/overview.md) fornece ferramentas para analisar dados derivados de canais. Consulte [Conectar a uma conta Meta (Facebook)](./insights/connect-channel.md#meta-ads-connect).
