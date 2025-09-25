---
title: Criar uma experiência de anúncio do Meta
description: Saiba como criar experiências de anúncio de Meta na marca, para Facebook ou Instagram, com o Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 42111bbf-70cd-4fd2-a7a9-15abe072d720
source-git-commit: 47195c08f500e50a01db127c6badc461c10afaf9
workflow-type: tm+mt
source-wordcount: '1392'
ht-degree: 0%

---

# Crie uma experiência de anúncio do Meta

Este tutorial demonstra como gerar [experiências de anúncio do Meta](/help/user-guide/create/meta-experiences.md) usando o GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (ícone de pincel na área de navegação esquerda).

Antes de começar a gerar uma experiência de anúncio do Meta, é importante [incorporar as diretrizes](/help/user-guide/guidelines/add-guidelines.md) no GenStudio for Performance Marketing e familiarizar-se com as noções básicas do [criação de um prompt](/help/user-guide/effective-prompts.md).

## Escolher um modelo

Para começar a gerar uma nova experiência de anúncio do Meta, use um modelo disponível para fornecer a estrutura para o seu conteúdo. Consulte [diretrizes de modelos de anúncios do Meta](/help/user-guide/templates/meta-template.md) para obter informações sobre as taxas de proporção de anúncios do Meta com suporte.

Ao selecionar um modelo, você tem a opção de usar um dos modelos carregados ou um modelo inicial.

**Para escolher um modelo de anúncio do Meta**:

1. Em _[!DNL Create]_, clique em **[!UICONTROL Meta ads]**.
1. Selecione **[!UICONTROL Modelos personalizados]** para procurar os modelos carregados ou **[!UICONTROL Modelos iniciais]** para procurar os modelos pré-criados.

   Se você planeja adicionar ativos de vídeo às variantes do Meta, é necessário escolher um modelo inicial. Eles são pré-carregados com áreas de conteúdo definidas pelo sistema que facilitam o uso de vídeos.

1. Clique para selecionar um modelo e clique em **[!UICONTROL Usar]**.

   Essa ação abre a Tela, que é o hub central para a criação de conteúdo.

## Adicionar parâmetros

Adicionar [diretrizes](/help/user-guide/guidelines/overview.md) e ativos em _Parâmetros_ na gaveta de prompts melhora o processo de geração de conteúdo e é uma etapa crucial na preparação para gerar um anúncio do Meta.

Se você estiver usando um modelo com diretrizes predefinidas—[!DNL Brands], [!DNL Personas] ou [!DNL Products]—essas diretrizes se aplicam às suas variantes. Você pode alterá-los se desejar.

**Para adicionar parâmetros e ativos**:

1. Clique no ícone _Parâmetros_ para expandir a gaveta do prompt.
1. Na seção _Parâmetros_, selecione as diretrizes—[!DNL Brands], [!DNL Personas] e [!DNL Products]—para informar sobre a criação de conteúdo.

   ![Escolher persona](/help/assets/persona-select.png){width="600" zoomable="yes"}

   Se não houver marcas, personalidades ou produtos disponíveis nesses menus, [adicione diretrizes à sua GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Adicione conteúdo (imagens ou vídeos) para usar na experiência *e* para influenciar a geração de conteúdo:
   * Clique em **[!UICONTROL Selecionar do Conteúdo]** para selecionar ativos do repositório [!DNL Content], filtrar e selecionar uma ou mais imagens.

     Se você estiver usando um modelo que tenha uma seção para vídeos, o conteúdo de vídeo (.mp4) será pré-selecionado e filtrado para você. Passe o mouse sobre um vídeo para ter uma visualização reproduzida automaticamente.

     ![Escolher conteúdo visual](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

     Para usar ativos de um repositório [!DNL AEM Assets Content Hub] conectado, escolha um repositório no menu suspenso _Local_. Filtre e selecione uma ou mais imagens.

   * Ou arraste e solte imagens na seção **[!UICONTROL Selecionar do conteúdo]** para carregar um ou mais ativos novos.

1. Clique em **[!UICONTROL Usar]**.

Quando terminar de adicionar parâmetros, você poderá recolher a gaveta do prompt clicando no ícone _Parâmetros_ novamente.

## Digite um prompt

Depois que as diretrizes forem selecionadas, crie um prompt usando a linguagem natural para começar a gerar conteúdo para sua nova experiência de anúncio do Meta. Prompts detalhados produzem uma saída de qualidade superior aos prompts vagos ou ambíguos.

Consulte [Gravar prompts efetivos](/help/user-guide/effective-prompts.md) para saber mais sobre a gravação de prompts.

**Para inserir um prompt**:

1. Digite um prompt na caixa de prompt _&quot;Descrever as experiências que você deseja gerar&quot;_.
1. Clique em **[!UICONTROL Gerar]**.

   Consulte [Gerenciar vídeos](#manage-videos) para entender como eles são gerados e como gerenciá-los.

Por padrão, quatro variações — todas alimentadas pelo prompt, pelas diretrizes e pelo conteúdo adicionado — são geradas e mostradas na Tela.

O conteúdo gerado é carregado progressivamente — à medida que cada seção das experiências do Meta é gerada, elas aparecem na Tela. Consulte [Experiências do Meta](/help/user-guide/create/meta-experiences.md#progressive-loading) para saber como essas alterações são carregadas na Tela.

## Escolher canal de anúncios do Meta

Ao gerar um anúncio do Meta, você pode escolher entre anúncios do Facebook ou do Instagram.

Alterne a opção de canal de anúncios do Meta (entre **Facebook** e **Instagram**) na barra de menu direita (ícones do Facebook e do Instagram) para ver e gerenciar variantes de cada canal.

Ao [revisar os anúncios do Meta](#revise-generated-variants), você pode alterar a proporção dos anúncios do Facebook e do Instagram.

## Revisar variantes geradas

Antes de selecionar o que enviar para aprovação ou publicação para [!DNL Content], você pode editar os anúncios do Meta ou excluir uma variante do conjunto de anúncios gerados.

Para realçar uma camada individual a ser revisada, clique em um campo ou imagem editável e clique em _[!UICONTROL Exibir Camadas]_.

**Para revisar variantes geradas**:

* **Para [editar o nome do rascunho do anúncio do Meta](/help/user-guide/create/manage-variants.md#change-draft-name)**, clique no título _Rascunho Sem Título_ na parte superior da Tela e insira um novo título.
* **Para [editar manualmente um anúncio do Meta](/help/user-guide/create/manage-variants.md#manually-edit-text)**, clique em qualquer uma das seções de anúncio (como a linha de assunto,
cabeçalho ou cópia do corpo) e edite conforme necessário.
* **Para alterar ou selecionar o call to action**, clique no botão call-to-action e selecione entre as opções de texto do botão disponíveis. Em _Link_, insira uma URL para o texto do call-to-action.
* **Para [aplicar formatação de texto](/help/user-guide/create/manage-variants.md#manually-edit-text)** a uma variante, clique no texto da imagem ou no link embutido de uma variante e clique em **[!UICONTROL Formatar texto]**.
<!-- **To [change or select the Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)**, click the call-to-action button and select _[!UICONTROL Rephrase]_ or _[!UICONTROL Add link]_. -->
* **Para [adicionar um link a uma imagem em uma variante](/help/user-guide/create/manage-variants.md#add-image-link)**, clique em um ativo de imagem (ou na área do ativo de imagem se uma imagem não existir no momento) e clique no ícone de link.
* **Para [alterar o tamanho e a taxa de proporção do anúncio](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**, clique no botão _[!UICONTROL Redimensionar]_ (caixa com um ícone de botão no lado esquerdo da Tela de Pintura) e selecione um novo tamanho e uma nova taxa de proporção a serem aplicados a todas as variantes. As variantes são duplicadas e redimensionadas.
* **Para [regenerar uma seção de uma variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, clique em um campo de texto editável e use as opções de _[!UICONTROL Edições sugeridas]_ ou insira um novo prompt e clique em **[!UICONTROL Gerar]**.
* **Para [adicionar ou trocar imagens em uma variante](/help/user-guide/create/manage-variants.md#swap-image)**, clique em um ativo de imagem (ou na área do ativo de imagem, se uma imagem não existir no momento) e clique no ícone **[!UICONTROL Trocar do conteúdo]**.
* **Para [cortar ou reposicionar imagens](/help/user-guide/create/manage-variants.md#crop-assets)**, clique em uma imagem, clique em **[!UICONTROL Editar]** (ícone de lápis) e em **[!UICONTROL Cortar]**. Ajuste o tamanho e a posição da imagem.
* **Para [usar a Expansão Gerativa para dimensionar e ajustar as imagens](/help/user-guide/create/manage-variants.md#use-generative-expand) ao seu modelo de trabalho**, clique em uma imagem, clique em **[!UICONTROL Editar]** (ícone de lápis) e em **[!UICONTROL Expandir]**. Ajuste a imagem para ajustar as proporções de tamanho e o modelo necessários.
* **Para [adicionar texto alternativo para imagens em uma variante](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**, clique em um ativo de imagem e use a opção _Texto alternativo_ para adicionar ou gerar manualmente texto alternativo por imagem.
* **Para [adicionar rótulos de acessibilidade](/help/user-guide/create/manage-variants.md#add-accessibility-labels) às suas variantes**, clique em uma imagem ou em um link do call-to-action e forneça uma breve descrição que explique o que o link ou o botão faz.
* **Para [excluir um anúncio do Meta](/help/user-guide/create/manage-variants.md#delete-variant)**, clique no menu de opções de uma variante e clique em **[!UICONTROL Excluir variante]**.

### Gerenciar vídeos

Passe o mouse sobre cada um dos vídeos para ver a reprodução automática em loop.

Os vídeos são reformulados para se ajustarem à taxa de proporção selecionada durante a geração. Reverta para o vídeo original não reformulado clicando em **[!UICONTROL Reformatar Vídeo]** e desativando-o.

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

1. [Iniciar uma solicitação de aprovação](/help/user-guide/approvals/request-review.md) para solicitar uma [aprovação de experiências de anúncio de rascunho do Meta](/help/user-guide/approvals/approve-content.md).

   ![Enviar rascunhos para revisão e aprovação](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. [Remover ou adicionar revisores](/help/user-guide/approvals/review-and-edit.md#manage-approvals) durante o processo de revisão.
1. [Acesse o conteúdo para revisão](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) e exiba as solicitações de revisão.
1. Edite os rascunhos por comentários de revisão e [publique suas experiências de anúncio do Meta](#publish-and-export-experience).

Consulte [Revisões e aprovações](/help/user-guide/approvals/overview.md) para obter mais informações.

## Publicar e exportar experiência

Para disponibilizar os anúncios gerados do Meta para uso atual e futuro, publique-os no [!UICONTROL Conteúdo] e exporte-os para uso em suas campanhas de marketing.

1. **Para publicar sua(s) nova(s) experiência(s) de anúncio do Meta**, clique em **[!UICONTROL Publicar]** na barra de ferramentas superior ou no fluxo de aprovações.
1. **Para exportar sua(s) nova(s) experiência(s) de anúncio do Meta**, clique em **[!UICONTROL Exportar]** na barra de ferramentas superior.
   1. Selecione o formato — HTML e imagens ou CSV e imagens (JPG ou PNG) — clique em **[!UICONTROL Exportar]**.

Consulte [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) para obter mais informações.

## Conectar o Meta

Você pode conectar o GenStudio for Performance Marketing ao Meta para receber análises e insights avançados sobre o desempenho do conteúdo.

Consulte [Meta ads connect](/help/user-guide/connectors/meta-ads.md).
