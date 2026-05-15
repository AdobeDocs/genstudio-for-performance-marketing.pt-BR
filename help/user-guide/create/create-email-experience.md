---
title: Criar uma experiência de email
description: Saiba como criar experiências de email no Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 34446202-da98-45ff-869a-b43496a477f8
TQID: https://experienceleague.adobe.com/RPeJQ02q9HXBSpn-uFqjzLCYbbzv5eNnFBXkFn9j5JI
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2: id: a8b28c00-da6e-4d27-8667-80f790ad8972id: be495d08-ecd1-455f-951e-c22de504e667id: de1f9646-abd3-4e21-9de2-df62ce55c8dcid: dee4e9a9-78d1-4953-8179-f8da6117027did: e3878dde-4b87-4290-9e81-ed7ee6eb83feid: f54ee13b-9545-4d68-9842-a12026e60aaf
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
source-git-commit: ecda1f61abaafe858629fc4700f61d89e2ab9e3e
workflow-type: tm+mt
source-wordcount: 1132
ht-degree: 0%

---

# Criar uma experiência de email

Este tutorial demonstra como gerar [experiências de email](/help/user-guide/create/email-experiences.md) com a marca usando o GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (ícone de pincel na área de navegação à esquerda).

Para criar uma experiência de email eficaz, é recomendável [adicionar diretrizes ao GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) e aprofundar as [noções básicas de criação de um prompt](/help/user-guide/effective-prompts.md) antes de começar.

## Escolher um modelo

Para criar uma nova experiência de email, use um modelo disponível para fornecer a estrutura para o seu conteúdo.

**Para escolher um modelo de email**:

1. Em _[!DNL Create]_, clique em **[!UICONTROL Email]**.
1. Use a opção de pesquisa, ao lado de _Filtro_, para localizar um modelo de email específico.
1. Clique para selecionar um modelo de email e clique em **[!UICONTROL Usar]**.

   A Tela, o epicentro da criação de conteúdo, é exibida.

## Adicionar parâmetros

Adicionar [diretrizes](/help/user-guide/guidelines/overview.md) e ativos em _Parâmetros_ na gaveta de prompt sobrecarrega o processo de geração de conteúdo e é uma etapa preparatória integral para gerar uma experiência de email.

Se você estiver usando um modelo com diretrizes predefinidas (como [!DNL Brands], [!DNL Personas] ou [!DNL Products]), essas diretrizes se aplicam às suas variantes. Você pode alterá-los se desejar.

**Para adicionar parâmetros e ativos**:

1. Clique no ícone _Parâmetros_ para expandir a gaveta do prompt.
1. Na seção _Parâmetros_, selecione as diretrizes—[!DNL Brands], [!DNL Personas] e [!DNL Products]—para informar sobre a criação de conteúdo.

   ![Escolher persona](/help/assets/persona-select-email2.png){width="50%" align="center"}

   Se não houver marcas, personalidades ou produtos disponíveis nesses menus, [adicione diretrizes à sua GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Adicione conteúdo para usar na experiência *e* para influenciar a geração de conteúdo:
   * Clique em **[!UICONTROL Selecionar do Conteúdo]** para selecionar ativos (imagens) do repositório [!DNL Content], filtrar e selecionar uma ou mais imagens.

     ![Escolher conteúdo visual](/help/assets/content-select-email.png){width="500" zoomable="yes"}

     Para usar ativos de um repositório [!DNL AEM Assets Content Hub] conectado, escolha um repositório no menu suspenso _Local_. Filtre e selecione uma ou mais imagens.

   * Ou arraste e solte ativos na seção **[!UICONTROL Selecionar do conteúdo]** para carregar um ou mais ativos novos.
1. Clique em **[!UICONTROL Usar]**.

   >[!NOTE]
   >Se o seu modelo de email tiver várias seções, selecione [!DNL Products] e conteúdo (ativos visuais) para cada seção de email em _Emails de várias seções_. Emails de várias seções suportam um ativo visual por seção. Você só pode adicionar ativos visuais a emails de várias seções do [!DNL Content]; não é possível arrastar e soltar ou carregar ativos da sua origem local.
   >![Adicionar conteúdo e parâmetros para cada seção de email](/help/assets/parameters-multisection-email.png){width="450" zoomable="yes"}

Quando terminar de adicionar parâmetros, você poderá recolher a gaveta do prompt clicando novamente no ícone _Parâmetros_.

## Digite um prompt

Depois que as diretrizes forem selecionadas, crie um prompt usando a linguagem natural para começar a gerar conteúdo para sua nova experiência de email. Prompts detalhados produzem uma saída de qualidade superior aos prompts vagos ou ambíguos.

Consulte [Gravar prompts efetivos](/help/user-guide/effective-prompts.md) para saber mais sobre a gravação de prompts.

**Para inserir um prompt**:

1. Digite um prompt na caixa de prompt _&quot;Descrever as experiências que você deseja gerar&quot;_.
1. Clique em **[!UICONTROL Gerar]**.

Por padrão, quatro variações — todas alimentadas pelo prompt, pelas diretrizes e pelo conteúdo adicionado — são geradas e mostradas na Tela.

O conteúdo gerado é carregado progressivamente — à medida que cada seção das experiências de email é gerada, elas são exibidas na Tela. Consulte [Experiências de email](/help/user-guide/create/meta-experiences.md#progressive-loading) para saber como essas alterações são carregadas na Tela.

## Revisar variantes geradas

Antes de selecionar o que enviar para aprovação ou publicação para [!DNL Content], você pode editar seções de email ou excluir uma variante do conjunto de emails gerados.

**Para revisar variantes geradas**:

* **Para [editar o nome do rascunho do email](/help/user-guide/create/manage-variants.md#change-draft-name)**, clique no título _Rascunho Sem Título_ na parte superior da Tela e insira um novo título.
* **Para [editar um email manualmente](/help/user-guide/create/manage-variants.md#manually-edit-text)**, clique em qualquer um dos campos de texto editáveis (como a linha de assunto, o cabeçalho ou a cópia do corpo) e edite conforme necessário
* **Para usar [fragmentos de conteúdo aprovados em variantes de email](/help/user-guide/create/email-experiences.md#content-fragment-swap)**, saiba como o [!DNL GenStudio for Performance Marketing] combina campos gerativos, campos de fragmento de conteúdo injetável e campos bloqueados em uma Tela. Os administradores configuram as origens de fragmento conforme descrito em [Localizar extensão de fragmento de conteúdo](/help/extensibility/deploy-app.md#find-content-fragment-extension).
* **Para [alterar ou selecionar o Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)**, clique no botão call-to-action e selecione _[!UICONTROL Refrase]_ ou _[!UICONTROL Adicionar link]_.
* **Para [aplicar a formatação do texto](/help/user-guide/create/manage-variants.md#manually-edit-text)** a uma variante, clique no texto da imagem de uma variante e clique em **[!UICONTROL Formatar texto]**.
* **Para [regenerar uma seção de uma variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, clique em um campo de texto editável e use as opções de _[!UICONTROL Edições sugeridas]_ ou insira um novo prompt e clique em **[!UICONTROL Gerar]**.
* **Para [adicionar ou trocar imagens em uma variante](/help/user-guide/create/manage-variants.md#swap-image)**, clique em um ativo de imagem (ou na área do ativo de imagem, se uma imagem não existir no momento) e clique no ícone **[!UICONTROL Trocar do conteúdo]**.
* **Para [adicionar um link a uma imagem em uma variante](/help/user-guide/create/manage-variants.md#add-image-link)**, clique em um ativo de imagem (ou na área do ativo de imagem se uma imagem não existir no momento) e clique no ícone de link.
* **Para [adicionar texto alternativo para imagens em uma variante](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**, clique em um ativo de imagem e use a opção _Texto alternativo_ para adicionar ou gerar manualmente texto alternativo por imagem.
* **Para [adicionar rótulos de acessibilidade](/help/user-guide/create/manage-variants.md#add-accessibility-labels) às suas variantes**, clique em uma imagem ou em um link do call-to-action e forneça uma breve descrição que explique o que o link ou o botão faz.
* **Para [excluir um email](/help/user-guide/create/manage-variants.md#delete-variant)**, clique para selecionar o título do email (por exemplo, &quot;Email 1/4&quot;) e clique em **[!UICONTROL Excluir variante]**.

## Enviar feedback de geração

Para [enviar comentários](/help/user-guide/create/manage-variants.md#generation-feedback) sobre a qualidade da saída de geração, clique no ícone de opções (três pontos) e selecione **[!UICONTROL Boa saída]** ou **[!UICONTROL Má saída]**.

## Visualizar para dispositivo

Ao revisar e preparar experiências de email, você pode [alternar entre visualizações para desktop e dispositivos móveis](/help/user-guide/create/manage-variants.md#preview-for-device) para garantir a coerência e o apelo visual de variantes de rascunho.

## Verificar o alinhamento da verificação de conteúdo

Para otimizar as variantes geradas e garantir a estrita adesão à identidade da marca, às diretrizes da plataforma e aos padrões de acessibilidade, aproveite o potencial do painel [_Verificação de conteúdo_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Esse painel exibe detalhes abrangentes da verificação de conteúdo e ilumina áreas de aprimoramento.

**Para executar verificações de conteúdo em uma variante**:

1. Clique no ícone do painel _Verificação de conteúdo_, na barra de ações à direita, para abrir o painel [_Verificação de conteúdo_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Veja um resumo das *Verificações de Necessidades de revisão* e *Aprovadas* para ver quais seções e diretrizes precisam ser aprimoradas.

   ![_Verificação de conteúdo_ painel](/help/assets/content-check-panel.png){width="300"}

2. [Revise manualmente as variantes](#revise-generated-variants) para garantir que suas variantes estejam alinhadas às verificações de conteúdo realizadas.

Consulte [Validação da marca](/help/user-guide/guidelines/brand-validation.md).

## Obter revisões e aprovações

Use o painel Aprovações, acessível como um ícone na barra de ação direita da Tela, para obter revisões, rastrear comentários de revisão e obter aprovações das partes interessadas.

**Para obter revisões e aprovações**:

1. [Iniciar uma solicitação de aprovação](/help/user-guide/approvals/request-review.md) para solicitar uma [aprovação de experiências de email em rascunho](/help/user-guide/approvals/approve-content.md).
1. [Remover ou adicionar revisores](/help/user-guide/approvals/review-and-edit.md#manage-approvals) durante o processo de revisão.
1. [Acesse o conteúdo para revisão](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) e exiba as solicitações de revisão.
1. Edite os rascunhos de acordo com os comentários de revisão e [publique suas experiências de email](#publish-and-export-experience).

Consulte [Revisões e aprovações](/help/user-guide/approvals/overview.md) para obter mais informações.

## Publicar e exportar experiência

Para disponibilizar os emails gerados para uso atual e futuro, publique-os no [!UICONTROL Conteúdo] e exporte-os para uso em suas campanhas de marketing.

1. **Para publicar sua(s) nova(s) experiência(s) de email**, clique em **[!UICONTROL Publicar]** na barra de ferramentas superior ou no fluxo de aprovações.
1. **Para exportar sua(s) nova(s) experiência(s) de email**, clique em **[!UICONTROL Exportar]** na barra de ferramentas superior.
   1. Selecione o formato (somente CSV e imagens ou HTML) e clique em **[!UICONTROL Exportar]**.

Consulte [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) para obter mais informações.
