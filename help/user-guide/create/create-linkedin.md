---
title: Criar uma experiência do LinkedIn
description: Saiba como criar experiências do LinkedIn compatíveis com a marca com o Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
badgeBeta: label="Beta" tooltip="No momento, esse recurso está no Beta, portanto, algumas funcionalidades podem estar limitadas ou sujeitas a alterações."
recommendations: noDisplay
exl-id: abe10fc8-d6d5-4cad-9273-400b622f22b7
source-git-commit: d82891b2347c6b97bf8f6eef9cffe363ea341725
workflow-type: tm+mt
source-wordcount: '1224'
ht-degree: 0%

---

# Criar uma experiência do LinkedIn

Este tutorial demonstra como gerar [experiências do LinkedIn](/help/user-guide/create/meta-experiences.md) que seguem as diretrizes da sua marca usando o GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (ícone de pincel na área de navegação esquerda).

Antes de começar a gerar um anúncio do LinkedIn, é importante [adicionar diretrizes](/help/user-guide/guidelines/add-guidelines.md) no GenStudio for Performance Marketing e saber mais sobre as noções básicas de [criação de um prompt](/help/user-guide/effective-prompts.md).

## Escolher um modelo

Para gerar uma nova experiência no LinkedIn, você precisa de um modelo para fornecer a estrutura para o seu conteúdo. Consulte [diretrizes do modelo do LinkedIn](/help/user-guide/templates/linkedin-template.md) para obter informações sobre as taxas de proporção do LinkedIn com suporte.

Você pode selecionar na lista de modelos personalizados ou escolher um modelo inicial.

**Para escolher um modelo do LinkedIn**:

1. Em _[!DNL Create]_, clique em **[!UICONTROL LinkedIn]**.
1. Selecione **[!UICONTROL Modelos personalizados]** para procurar os modelos carregados ou **[!UICONTROL Modelos iniciais]** para procurar os modelos pré-criados.

   Se você planeja adicionar ativos de vídeo às suas Variantes Meta, é necessário escolher um modelo inicial. Eles são pré-carregados com áreas de conteúdo definidas pelo sistema que facilitam o uso de vídeos.

1. Clique para selecionar um modelo e clique em **[!UICONTROL Usar]**.

   Essa ação abre a Tela, que é o hub central para a criação de conteúdo.

## Adicionar parâmetros

Adicionar [diretrizes](/help/user-guide/guidelines/overview.md) e ativos em _Parâmetros_ na gaveta de prompts melhora o processo de geração de conteúdo e é uma etapa crucial na preparação para gerar uma experiência do LinkedIn.

**Para adicionar parâmetros e ativos**:

1. Clique no ícone _Parâmetros_ para expandir a gaveta do prompt.
1. Na seção _Parâmetros_, selecione as diretrizes—[!DNL Brands], [!DNL Personas] e [!DNL Products]—para informar sobre a criação de conteúdo.

   ![Escolher persona](/help/assets/persona-select.png){width="600" zoomable="yes"}

   Se não houver marcas, personalidades ou produtos disponíveis nesses menus, [adicione diretrizes à sua GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Adicione conteúdo (imagens ou vídeos) para usar na experiência *e* para influenciar a geração de conteúdo clicando em **[!UICONTROL Selecionar do Conteúdo]**. Ou arraste e solte imagens na seção **[!UICONTROL Selecionar do conteúdo]** para carregar um ou mais ativos novos.

   Use o filtro para pesquisar o conteúdo e selecione uma ou mais imagens.

   Se você estiver usando um modelo que tenha uma seção para vídeos, o conteúdo de vídeo (.mp4) será pré-selecionado e filtrado para você. Passe o mouse sobre um vídeo para ter uma visualização reproduzida automaticamente.

   ![Escolher conteúdo visual](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

   Para usar ativos de um repositório [!DNL AEM Assets Content Hub] conectado, escolha um repositório no menu suspenso _Local_. Filtre e selecione uma ou mais imagens.

1. Clique em **[!UICONTROL Usar]**.

Quando terminar de adicionar parâmetros, você poderá recolher a gaveta do prompt clicando no ícone _Parâmetros_ novamente.

## Digite um prompt

Depois de selecionar as diretrizes, crie um prompt usando a linguagem natural para começar a gerar conteúdo para a sua nova experiência do LinkedIn. Solicitações detalhadas garantem que você receba boa qualidade e resultados úteis.

Consulte [Gravar prompts efetivos](/help/user-guide/effective-prompts.md) para saber mais sobre a gravação de prompts.

**Para inserir um prompt**:

1. Digite um prompt na caixa de prompt _&quot;Descrever as experiências que você deseja gerar&quot;_.
1. Clique em **[!UICONTROL Gerar]**.

   Consulte [Gerenciar vídeos](#manage-videos) para entender como eles são gerados e como gerenciá-los.

Por padrão, quatro variações — todas alimentadas pelo prompt, pelas diretrizes e pelo conteúdo adicionado — são geradas e mostradas na Tela.

O conteúdo gerado é carregado progressivamente — à medida que cada seção das experiências do LinkedIn é gerada, elas são exibidas na Tela. Consulte [experiências do LinkedIn](/help/user-guide/create/linkedin-experiences.md#progressive-loading) para saber como essas alterações são carregadas na Tela.

## Revisar anúncios gerados do LinkedIn

Antes de enviar variantes para aprovação ou publicação para [!DNL Content], edite os anúncios do LinkedIn ou exclua uma variante do conjunto de anúncios gerados.

**Para revisar variantes geradas**:

* **Para [editar o nome do rascunho do anúncio do LinkedIn](/help/user-guide/create/manage-variants.md#change-draft-name)**, clique no título _Rascunho Sem Título_ na parte superior da Tela e insira um novo título.
* **Para [editar manualmente um anúncio do LinkedIn](/help/user-guide/create/manage-variants.md#manually-edit-text)**, clique em qualquer uma das seções do anúncio (como a linha de assunto, o cabeçalho ou a cópia do corpo) e edite conforme necessário.
* **Para alterar ou selecionar o plano de ação**, clique no botão call-to-action e selecione entre as opções de texto de botão disponíveis. Em _Link_, insira uma URL para o texto do call-to-action.
* **Para [aplicar a formatação do texto](/help/user-guide/create/manage-variants.md#manually-edit-text)** a uma variante, clique no texto da imagem de uma variante e clique em **[!UICONTROL Formatar texto]**.
* **Para [regenerar uma seção de uma variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, clique em um campo de texto editável e use as opções de _[!UICONTROL Edições sugeridas]_ ou insira um novo prompt na _[!UICONTROL seção Gerar novo texto_] e clique em **[!UICONTROL Gerar]**.
* **Para [usar a Expansão Gerativa para dimensionar e ajustar as imagens](/help/user-guide/create/manage-variants.md#use-generative-expand) ao seu modelo de trabalho**, clique em uma imagem, clique em **[!UICONTROL Editar]** (ícone de lápis) e em **[!UICONTROL Expandir]**. Ajuste a imagem para ajustar as proporções de tamanho e o modelo necessários.
* **Para [cortar ou reposicionar imagens](/help/user-guide/create/manage-variants.md#crop-assets)**, passe o mouse sobre uma imagem, clique no ícone de recorte exibido e ajuste o tamanho e o posicionamento da imagem.
* **Para [alterar o tamanho e a taxa de proporção do anúncio](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**, clique no botão _[!UICONTROL Redimensionar]_ (caixa com um ícone de botão no lado esquerdo da Tela de Pintura) e selecione um novo tamanho e uma nova taxa de proporção a serem aplicados a todas as variantes. As variantes são duplicadas e redimensionadas.
* **Para [adicionar ou trocar ativos (imagem ou vídeo) em uma variante](/help/user-guide/create/manage-variants.md#swap-image)**, clique em um ativo (ou na área de ativo) e clique no ícone **[!UICONTROL Trocar do conteúdo]**.
* **Para [adicionar texto alternativo para imagens em uma variante](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**, clique em um ativo de imagem e use a opção _Texto alternativo_ para adicionar ou gerar manualmente texto alternativo por imagem.
* **Para [adicionar rótulos de acessibilidade](/help/user-guide/create/manage-variants.md#add-accessibility-labels) às suas variantes**, clique em uma imagem ou em um link do call-to-action e forneça uma breve descrição que explique o que o link ou o botão faz.
* **Para [excluir um anúncio do LinkedIn](/help/user-guide/create/manage-variants.md#delete-variant)**, clique no menu de opções de uma variante e clique em **[!UICONTROL Excluir variante]**.

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

1. [Revise manualmente as variantes](#revise-generated-linkedin-ads) para garantir que suas variantes estejam alinhadas às verificações de conteúdo concluídas.

Consulte [Validação da marca](/help/user-guide/guidelines/brand-validation.md).

## Obter revisões e aprovações

Use o painel Aprovações, acessível na barra de menu superior da Tela, para obter revisões, rastrear comentários de revisão e obter aprovações das partes interessadas.

**Para obter revisões e aprovações**:

1. [Iniciar uma solicitação de aprovação](/help/user-guide/approvals/request-review.md) para solicitar uma [aprovação de experiências de Metadados rascunhados](/help/user-guide/approvals/approve-content.md).

   ![Enviar rascunhos para revisão e aprovação](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. [Remover ou adicionar revisores](/help/user-guide/approvals/review-and-edit.md#manage-approvals) durante o processo de revisão.
1. [Acesse o conteúdo para revisão](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) e exiba as solicitações de revisão.
1. Edite os rascunhos por comentários de revisão e [publique suas experiências de Metadados](#publish-and-export-experience).

Consulte [Revisões e aprovações](/help/user-guide/approvals/overview.md) para obter mais informações.

## Publicar e exportar experiência

Para disponibilizar os anúncios gerados do LinkedIn para uso atual e futuro, publique-os no [!UICONTROL Content] e exporte-os para uso em suas campanhas de marketing.

1. **Para publicar sua(s) nova(s) experiência(s)**, clique em **[!UICONTROL Publicar]** na barra de ferramentas superior ou no fluxo de aprovações.
1. **Para exportar sua(s) nova(s) experiência(s)**, clique em **[!UICONTROL Exportar]** na barra de ferramentas superior.
   1. Selecione o formato (JPG, PNG ou GIF) e clique em **[!UICONTROL Exportar]**.

Consulte [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) para obter mais informações.
