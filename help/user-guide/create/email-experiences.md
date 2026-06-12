---
title: Experiências de email
description: Saiba mais sobre experiências de email no Adobe GenStudio for Performance Marketing, incluindo o comportamento da Tela e a troca de fragmento de conteúdo de bibliotecas aprovadas.
feature: Create Canvas, Media Templates
role: User
level: Beginner
exl-id: e2bddd02-914e-43a8-92b6-fdcbced94a6a
TQID: https://experienceleague.adobe.com/-lwSfvc0TnVd8byNT-5OfoEsXz7yaeIifcHOJtp-n4c
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2: id: a8b28c00-da6e-4d27-8667-80f790ad8972id: be495d08-ecd1-455f-951e-c22de504e667id: dee4e9a9-78d1-4953-8179-f8da6117027did: ee4b6e5f-5b7a-421b-9859-0f964841a866
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 3890f933a4cccae2e5dbe7ef2184e1dfd089b20b
workflow-type: tm+mt
source-wordcount: 600
ht-degree: 0%

---

# Experiências de email

Com o Adobe GenStudio for Performance Marketing, você pode usar a IA gerativa para simplificar a [criação de experiências de email de alto impacto](/help/user-guide/create/create-email-experience.md).

O [!DNL Create] permite que profissionais de marketing modernos usem [diretrizes](/help/user-guide/guidelines/overview.md), ativos de imagem e um [prompt bem montado](/help/user-guide/effective-prompts.md) para [criar rapidamente experiências de email alinhadas à marca](/help/user-guide/create/create-email-experience.md).

Ao gerar experiências de email, quatro variações são criadas e mostradas na Tela.

As seções editáveis de uma experiência de email incluem:

* Pré-cabeçalho
* Título
* Subtítulo
* Corpo
* Call to action (CTA)
* Imagem

Consulte [Elementos do modelo](/help/user-guide/templates/use-templates.md#template-elements).

<!-- 
## Email capabilities

Content creators and marketers can produce brand-consistent email experiences in GenStudio for Performance Marketing. 
-->

## Emails de várias seções

As experiências de email podem apresentar várias seções, permitindo personalização completa para se alinhar à sua marca e objetivos. [Selecione [!DNL Products] e ativos visuais para cada seção](/help/user-guide/create/create-email-experience.md#add-parameters) e use [prompts estruturados](/help/user-guide/effective-prompts.md#structured-prompts) para criar conteúdo exclusivo. Cada seção suporta um ativo visual.

Consulte [personalização de modelos com seções](/help/user-guide/templates/customize-template.md#sections-or-groups) para saber como criar um modelo de várias seções.

## Carregamento progressivo

Quando o processo de geração de conteúdo é iniciado, cada seção do conteúdo gerado nas variantes de email é carregada progressivamente na Tela. Experiências, ativos e campos e seções nas experiências são exibidos individualmente na Tela à medida que são gerados.

Ao clicar em **[!UICONTROL Gerar]**, um indicador de carregamento é exibido na parte inferior da Tela, atualizando você sobre o progresso da geração.

Cada campo e seção de experiências de email são carregados progressivamente nesta sequência:

1. Nomes de variantes
1. Linhas de assunto para todas as variações
1. Pré-cabeçalhos
1. Manchetes, corpo do email (para emails de seção única) e planos de ação
1. Corpo do email para seções subsequentes (para emails de várias seções)
1. Validação da marca

   O processo de validação de marca e verificação de conteúdo ocorre e o [_resumo da verificação de conteúdo_](/help/user-guide/guidelines/brand-validation.md#content-check-summary) é preenchido para cada variante.

## Contagens de caracteres

Depois de gerar um conjunto de variantes de email, você pode ver a contagem de caracteres exibida para cada seção. Passe o mouse sobre ou clique em uma seção gerada, como a linha de assunto ou o corpo, e veja o nome da seção e a contagem de caracteres para essa seção.

![Contagem de caracteres](/help/assets/character-count.png){width="500" zoomable="yes"}

## Troca de fragmento de conteúdo {#content-fragment-swap}

>[!NOTE]
>
>A troca de fragmento de conteúdo está disponível para experiências de **email** na Tela hoje. O suporte ao canal **Horizon** será lançado em breve.

O conteúdo de e-mail corporativo geralmente precisa de uma cópia recém-gerada e de blocos modulares aprovados (como avisos de isenção de responsabilidade, idioma de segurança, ofertas e avisos de sinistro regulamentados), juntamente com o conteúdo que você cria para os modelos. As equipes que armazenam conteúdo modular no [!DNL Adobe Experience Manager] podem localizar e trocar esse conteúdo para usar em experiências de email sem sair do [!DNL GenStudio for Performance Marketing]. Isso pode ser útil para:

* **Conteúdo com reconhecimento de conformidade:** a IA pode preencher slots criativos, enquanto fragmentos aprovados para conformidade substituem slots injetáveis; as áreas legais bloqueadas permanecem inalteradas durante a exportação.
* **Componentes de conteúdo aprovado reutilizáveis:** títulos aprovados, avisos de isenção de responsabilidade regionais ou descrições de produtos podem permanecer no sistema de registro em [!DNL Adobe Experience Manager], enquanto os autores os colocam em variantes sem soluções alternativas de copiar e colar.

Os criadores reúnem experiências na Canvas; as equipes de conformidade e marca mantêm fluxos de trabalho de aprovação no [!DNL Adobe Experience Manager]; as equipes de TI e de integração conectam repositórios e permissões exigidos por sua organização.

![Troca de fragmento de conteúdo](./cf-swap.png){width="500" zoomable="yes"}

Quando sua organização habilita a troca de fragmento de conteúdo, você pode esperar:

* Os campos de fragmento de conteúdo podem ser preenchidos a partir de uma biblioteca de conteúdo conectada, em vez de somente digitação manual ou geração de IA.
* Navegue, pesquise e filtre fragmentos usando metadados como campanha, persona, canal, idioma e marca.
* Um seletor de repositório está disponível quando vários repositórios são configurados.
* Visualização de um fragmento antes da substituição do texto do campo.
* Propagação de uma seleção de fragmento em todas as variantes em uma ação.

![Painel da interface do usuário de fragmentos de conteúdo](./cf-pane.png){width="500" zoomable="yes"}

Sua organização escolhe quais fontes e repositórios de fragmento de conteúdo estão disponíveis. Consulte [Localizar extensão de fragmento de conteúdo](/help/extensibility/deploy-app.md#find-content-fragment-extension) para saber como os administradores configuram fontes e como os autores trocam cópias da Tela com o **[!UICONTROL Swap]**.

Você também pode traduzir uma experiência de email aprovada em vários idiomas na tela do HTML. Consulte [Traduzir e traduzir experiências](/help/user-guide/create/translate-experiences.md).
