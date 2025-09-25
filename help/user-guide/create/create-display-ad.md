---
title: Criar uma experiência de anúncio de exibição
description: Saiba como criar experiências de anúncio de exibição no Adobe [!DNL GenStudio] para Marketing de Desempenho.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 7d5e777b-7a30-48f4-b253-9823e38eecce
source-git-commit: 47195c08f500e50a01db127c6badc461c10afaf9
workflow-type: tm+mt
source-wordcount: '1131'
ht-degree: 0%

---

# Criar uma experiência de anúncio de exibição

Este tutorial demonstra como gerar experiências de anúncio de exibição [da marca](display-ad-experiences.md) usando o GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (ícone de pincel na área de navegação à esquerda).

Para criar uma experiência atraente de anúncio de exibição, é recomendável [adicionar diretrizes ao GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) e analisar as [noções básicas sobre como escrever prompts](/help/user-guide/effective-prompts.md) antes de começar.

## Escolher um modelo

Para criar uma experiência de anúncio de exibição, use um modelo disponível para fornecer a estrutura para o seu conteúdo. Consulte [Diretrizes de modelo de anúncio de exibição](/help/user-guide/templates/display-template.md) para obter informações sobre dimensões de anúncio de exibição com suporte.

**Para escolher um modelo de anúncio de exibição**:

1. Em _[!DNL Create]_, clique em **[!UICONTROL Exibir anúncios]**.
1. Use a opção de pesquisa, adjacente ao _Filtro_, para localizar um modelo de anúncio de exibição específico.
1. No modo de exibição _Selecionar modelo_, clique em um modelo de anúncio de exibição.
1. Clique em **[!UICONTROL Usar]**.

   A Tela, que serve como hub central para a criação de conteúdo, é exibida.

## Adicionar parâmetros

Adicionar [diretrizes](/help/user-guide/guidelines/overview.md) e ativos em _Parâmetros_ na gaveta de prompt sobrecarrega o processo de geração de conteúdo e é uma etapa preparatória integral para gerar uma experiência de exibição de anúncio.

Se você estiver usando um modelo com diretrizes predefinidas—[!DNL Brands], [!DNL Personas] ou [!DNL Products]—essas diretrizes se aplicam às suas variantes. Você pode alterá-los se desejar.

**Para adicionar parâmetros e ativos**:

1. Clique no ícone _Parâmetros_ para expandir a gaveta do prompt.
1. Na seção _Parâmetros_, selecione as diretrizes—[!DNL Brands], [!DNL Personas] e [!DNL Products]—para informar sobre a criação de conteúdo.

   Se não houver marcas, personalidades ou produtos disponíveis nesses menus, [adicione diretrizes à sua GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Para adicionar conteúdo a ser usado na experiência *e* para influenciar a geração de conteúdo:
   * Clique em **[!UICONTROL Selecionar do Conteúdo]** para selecionar ativos (imagens) do repositório [!DNL Content], filtrar e selecionar uma ou mais imagens.

     Para usar ativos de um repositório [!DNL AEM Assets Content Hub] conectado, escolha um repositório no menu suspenso _Local_. Filtre e selecione uma ou mais imagens.

   * Ou arraste e solte ativos na seção **[!UICONTROL Selecionar do conteúdo]** para carregar um ou mais ativos novos.
1. Clique em **[!UICONTROL Usar]**.

Quando terminar de adicionar parâmetros, recolha a gaveta do prompt clicando novamente no ícone _Parâmetros_.

## Digite um prompt

Depois que as diretrizes forem selecionadas, crie um prompt usando a linguagem natural para começar a gerar conteúdo para a nova experiência de anúncio de exibição. Para aprimorar a qualidade das experiências de anúncio de exibição geradas, é fundamental criar prompts detalhados e descritivos.

![Inserir um prompt](/help/assets/prompt-displayad.png){width="650" zoomable="yes"}

Consulte [Gravar prompts efetivos](/help/user-guide/effective-prompts.md) para saber mais sobre a gravação de prompts.

**Para inserir um prompt**:

1. Digite um prompt na caixa de prompt _&quot;Descrever as experiências que você deseja gerar&quot;_.
1. Clique em **[!UICONTROL Gerar]**.

Por padrão, quatro variações, alimentadas pelo prompt, pelas diretrizes e pelo conteúdo adicionado, são geradas e exibidas na Tela de desenho.

## Revisar variantes geradas

Antes de selecionar o que enviar para aprovação ou publicação para [!DNL Content], você pode editar seções de anúncio de exibição e campos de texto ou excluir uma variante gerada.

Para realçar uma camada individual a ser revisada, clique em um campo ou imagem editável e clique em _[!UICONTROL Exibir Camadas]_.

**Para revisar variantes geradas**:

* **Para [editar o nome do rascunho do anúncio de exibição](/help/user-guide/create/manage-variants.md#change-draft-name)**, clique no título _Rascunho Sem Título_ na parte superior da Tela e insira um novo título.
* **Para [editar manualmente um anúncio de exibição](/help/user-guide/create/manage-variants.md#manually-edit-text)**, clique duas vezes em qualquer uma das seções ou campos do anúncio de exibição (como a linha de assunto, o cabeçalho ou a cópia do corpo) e edite conforme necessário.
* **Para [aplicar formatação de texto](/help/user-guide/create/manage-variants.md#manually-edit-text)** a uma variante, clique no texto da imagem ou no link embutido de uma variante e clique em **[!UICONTROL Formatar texto]**.
* **Para [regenerar uma seção de uma variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, clique em um campo de texto editável e use as opções de _[!UICONTROL Edições sugeridas]_ ou insira um novo prompt na _[!UICONTROL seção Gerar novo texto_] e clique em **[!UICONTROL Gerar]**.
* **Para [adicionar ou trocar imagens em uma variante](/help/user-guide/create/manage-variants.md#swap-image)**, clique em um ativo de imagem (ou na área do ativo de imagem, se uma imagem não existir no momento) e clique no ícone **[!UICONTROL Trocar do conteúdo]**.
* **Para [adicionar um link a uma imagem em uma variante](/help/user-guide/create/manage-variants.md#add-image-link)**, clique em um ativo de imagem (ou na área do ativo de imagem se uma imagem não existir no momento) e clique no ícone de link.
* **Para [adicionar texto alternativo para imagens em uma variante](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**, clique em um ativo de imagem e use a opção _Texto alternativo_ para adicionar ou gerar manualmente texto alternativo por imagem.
* **Para [adicionar rótulos de acessibilidade](/help/user-guide/create/manage-variants.md#add-accessibility-labels) às suas variantes**, clique em uma imagem ou em um link do call-to-action e forneça uma breve descrição que explique o que o link ou o botão faz.
* **Para [alterar o tamanho e a taxa de proporção do anúncio](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**, clique no botão _[!UICONTROL Redimensionar]_ (caixa com um ícone de botão no lado esquerdo da Tela de Pintura) e selecione um novo tamanho e uma nova taxa de proporção a serem aplicados a todas as variantes. As variantes são duplicadas e redimensionadas.
* **Para [cortar ou reposicionar imagens](/help/user-guide/create/manage-variants.md#crop-assets)**, clique em uma imagem, clique em **[!UICONTROL Editar]** (ícone de lápis) e em **[!UICONTROL Cortar]**. Ajuste o tamanho e a posição da imagem.
* **Para [usar a Expansão Gerativa para dimensionar e ajustar as imagens](/help/user-guide/create/manage-variants.md#use-generative-expand) ao seu modelo de trabalho**, clique em uma imagem, clique em **[!UICONTROL Editar]** (ícone de lápis) e em **[!UICONTROL Expandir]**. Ajuste a imagem para ajustar as proporções de tamanho e o modelo necessários.

<!-- # Preview for device
When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.
**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

## Enviar feedback de geração

Para [enviar comentários](/help/user-guide/create/manage-variants.md#generation-feedback) sobre a qualidade da saída de geração, clique no ícone de opções (três pontos) e selecione **[!UICONTROL Boa saída]** ou **[!UICONTROL Má saída]**.

## Verificar o alinhamento da verificação de conteúdo

Para otimizar as variantes geradas e garantir a estrita adesão à identidade da marca, às diretrizes da plataforma e aos padrões de acessibilidade, aproveite o potencial do painel [_Verificação de conteúdo_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Esse painel exibe detalhes abrangentes da verificação de conteúdo e ilumina áreas de aprimoramento.

**Para executar verificações de conteúdo em uma variante**:

1. Clique no ícone do painel _Verificação de conteúdo_, na barra de ações à direita, para abrir o painel [_Verificação de conteúdo_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Veja um resumo das *Verificações de Necessidades de revisão* e *Aprovadas* para ver quais seções e diretrizes precisam ser aprimoradas.

   ![_Verificação de conteúdo_ painel](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [Revise manualmente as variantes](#revise-generated-variants) para garantir que suas variantes estejam alinhadas às verificações de conteúdo realizadas.

Consulte [Validação da marca](/help/user-guide/guidelines/brand-validation.md).

## Obter revisões e aprovações

Use o painel Aprovações, acessível como um ícone na barra de ação direita da Tela, para obter revisões, rastrear comentários de revisão e obter aprovações das partes interessadas.

**Para obter revisões e aprovações**:

1. [Iniciar uma solicitação de aprovação](/help/user-guide/approvals/request-review.md) para solicitar uma [aprovação de experiências de anúncio de exibição rascunho](/help/user-guide/approvals/approve-content.md).
1. [Remover ou adicionar revisores](/help/user-guide/approvals/review-and-edit.md#manage-approvals) durante o processo de revisão.
1. [Acesse o conteúdo para revisão](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) e exiba as solicitações de revisão.
1. Edite os rascunhos por comentários de revisão e [publique suas experiências de anúncio de exibição](#publish-and-export-experience).

Consulte [Análises e aprovações](/help/user-guide/approvals/overview.md).

## Publicar e exportar experiência

Para disponibilizar os anúncios de exibição gerados para uso atual e futuro, publique-os no [!UICONTROL Conteúdo] e exporte-os para uso em suas campanhas de marketing.

1. **Para publicar sua(s) nova(s) experiência(s) de anúncio de exibição**, clique em **[!UICONTROL Publicar]** na barra de ferramentas superior ou no fluxo de aprovações.
   1. Selecione _[!UICONTROL [!DNL Campaigns]]_&#x200B;e adicione&#x200B;_[!UICONTROL &#x200B; Mais detalhes &#x200B;]_, se desejar.
   1. Clique em **[!UICONTROL Publicar]**.

      ![Publicar um anúncio de exibição](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **Para exportar sua(s) nova(s) experiência(s) de anúncio de exibição**, clique em **[!UICONTROL Exportar]** na barra de ferramentas superior.
   1. Selecione o formato (HTML e imagens, PNG ou JPG) e clique em **[!UICONTROL Exportar]**.

      O HTML exportado deve ser colocado em uma propriedade da Web predefinida, como um modelo ou contêiner `div`. Sem essas dimensões definidas, as imagens podem parecer distorcidas quando visualizadas independentemente.

Consulte [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
