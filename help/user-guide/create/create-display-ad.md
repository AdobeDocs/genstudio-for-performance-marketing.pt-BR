---
title: Criar uma experiência de anúncio de exibição
description: Saiba como criar experiências de anúncio de exibição no Adobe [!DNL GenStudio] para Marketing de desempenho.
feature: Brands Service, Guidelines, Content Generation, Generative AI, Create, Experiences, Variant Generation
role: User
level: Beginner
recommendations: noDisplay
source-git-commit: 885900eb259246c2d86a07791a1b7070e0dbf12a
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 0%

---

# Criar uma experiência de anúncio de exibição

Este tutorial demonstra como gerar experiências de anúncio de exibição [da marca](display-ad-experiences.md) usando o GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (ícone de pincel na área de navegação à esquerda).

Para criar uma experiência atraente de anúncio de exibição, é recomendável [adicionar diretrizes ao GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) e analisar as [noções básicas sobre como escrever prompts](/help/user-guide/effective-prompts.md) antes de começar.

## Escolher um modelo

Para criar uma experiência de anúncio de exibição, use um modelo disponível para fornecer a estrutura para o seu conteúdo.

**Para escolher um modelo de anúncio de exibição**:

1. Em _[!DNL Create]_, clique em **[!UICONTROL Exibir anúncios]**na_&quot;O que deseja criar hoje?&quot;seção _.
1. Use a opção de pesquisa, adjacente ao _Filtro_, para localizar um modelo de anúncio de exibição específico.
1. No modo de exibição _Selecionar modelo_, clique em um modelo de anúncio de exibição.
1. Clique em **[!UICONTROL Usar]**.

   A Tela, que serve como hub central para a criação de conteúdo, é exibida.

## Adicionar parâmetros

Adicionar [diretrizes](/help/user-guide/guidelines/overview.md) e ativos em _Parâmetros_ na gaveta de prompt sobrecarrega o processo de geração de conteúdo e é uma etapa preparatória integral para gerar uma experiência de exibição de anúncio.

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

## Revisar anúncios de exibição gerados

Antes de selecionar o que enviar para aprovação ou publicação para [!DNL Content], você pode editar seções de anúncio de exibição e campos de texto ou excluir uma variante gerada.

**Para revisar variantes geradas**:

* **Para [editar o nome do rascunho do anúncio de exibição](/help/user-guide/create/manage-variants.md#change-draft-name)**, clique no título _Rascunho Sem Título_ na parte superior da Tela e insira um novo título.
* **Para [editar manualmente um anúncio de exibição](/help/user-guide/create/manage-variants.md#manually-edit-text)**, clique duas vezes em qualquer uma das seções ou campos do anúncio de exibição (como a linha de assunto, o cabeçalho ou a cópia do corpo) e edite conforme necessário.
* **Para [alterar o tamanho e a taxa de proporção do anúncio](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**, clique no botão _[!UICONTROL Redimensionar]_ (caixa com um ícone de botão no lado esquerdo da Tela de Pintura) e selecione um novo tamanho e uma nova taxa de proporção a serem aplicados a todas as variantes. As variantes são duplicadas e redimensionadas.
* **Para [cortar ou reposicionar imagens](/help/user-guide/create/manage-variants.md#crop-assets)**, passe o mouse sobre a imagem, clique no ícone de recorte exibido e ajuste o tamanho e o posicionamento da imagem. Clique em **[!UICONTROL Aplicar]**.

<!-- # Preview for device
When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.
**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

## Enviar feedback de geração

Para [enviar comentários](/help/user-guide/create/manage-variants.md#generation-feedback) sobre a qualidade da saída de geração, clique no ícone de opções (três pontos) e selecione **[!UICONTROL Boa saída]** ou **[!UICONTROL Má saída]**.

## Verificar o alinhamento da marca

Para otimizar os anúncios gerados e garantir a estrita adesão à identidade da marca, aproveite o poder do [_Painel de validação de marca_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel), que exibe detalhes abrangentes sobre a validação de marca e ilumina áreas de aprimoramento.

**Para verificar o alinhamento da marca**:

1. Clique no ícone Validação de marca na barra de menu superior para abrir o [_Painel de validação de marca_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel). Você pode ver detalhes dos fragmentos e diretrizes que precisam ser aprimorados.

1. Alterne cada anúncio para ver como você pode melhorar o conteúdo gerado para torná-lo mais alinhado à marca.
1. [Revise os anúncios manualmente](#revise-generated-display-ads) para garantir que seus emails estejam alinhados à sua marca.

Consulte [Validação da marca](/help/user-guide/guidelines/brand-validation.md).

## Obter revisões e aprovações

Use o painel Aprovações, acessível na barra de menu superior da Tela, para obter revisões, rastrear comentários de revisão e obter aprovações das partes interessadas.

**Para obter revisões e aprovações**:

1. [Iniciar uma solicitação de aprovação](/help/user-guide/approvals/request-review.md) para solicitar uma [aprovação de experiências de email em rascunho](/help/user-guide/approvals/approve-content.md).
1. [Remover ou adicionar revisores](/help/user-guide/approvals/review-and-edit.md#manage-approvals) durante o processo de revisão.
1. [Acesse o conteúdo para revisão](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) e exiba as solicitações de revisão.
1. Edite os rascunhos por comentários de revisão e [publique suas experiências de anúncio de exibição](#publish-and-export-experience).

Consulte [Análises e aprovações](/help/user-guide/approvals/overview.md).

## Experiência do Publish e de exportação

Para disponibilizar os anúncios de exibição gerados para uso atual e futuro, publique-os no [!UICONTROL Conteúdo] e exporte-os para uso em suas campanhas de marketing.

1. **Para publicar sua(s) nova(s) experiência(s) de anúncio de exibição**, clique em **[!UICONTROL Publish]** na barra de ferramentas superior ou no fluxo de aprovações.
   1. Selecione _[!UICONTROL [!DNL Campaigns]]_e adicione_[!UICONTROL  Mais detalhes ]_, se desejar.
   1. Clique em **[!UICONTROL Publicar]**.

      ![Publish um anúncio de exibição](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **Para exportar sua(s) nova(s) experiência(s) de anúncio de exibição**, clique em **[!UICONTROL Exportar]** na barra de ferramentas superior.
   1. Selecione o formato—somente JPG—e clique em **[!UICONTROL Exportar]**.

      O HTML exportado deve ser colocado em uma propriedade da Web predefinida, como um modelo ou contêiner `div`. Sem essas dimensões definidas, as imagens podem parecer distorcidas quando visualizadas independentemente.

Consulte [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
