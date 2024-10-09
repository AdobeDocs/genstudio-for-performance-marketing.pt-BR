---
title: Criar uma experiência de meta-anúncio
description: Saiba como criar experiências de meta anúncios na marca, para Facebook ou Instagram, com o Adobe GenStudio para Marketing de desempenho.
feature: Content, Brands Service, Guidelines, Content Generation, Create, Experiences, Variant Generation
role: User
level: Beginner
type: Tutorial
recommendations: noDisplay
exl-id: 42111bbf-70cd-4fd2-a7a9-15abe072d720
source-git-commit: 30cd73ba1beb582ea4ac73eca7e17715f9aafc66
workflow-type: tm+mt
source-wordcount: '1074'
ht-degree: 0%

---

# Criar uma experiência de meta-anúncio

Este tutorial demonstra como gerar experiências de [Metadados](/help/user-guide/create/meta-experiences.md) com a marca usando o GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (ícone de pincel na área de navegação à esquerda).

Antes de começar a gerar uma experiência de metadados, é importante [incorporar diretrizes](/help/user-guide/guidelines/add-guidelines.md) ao GenStudio para Marketing de Desempenho e familiarizar-se com as noções básicas de [criação de um prompt](/help/user-guide/effective-prompts.md).

## Escolher um modelo

Para começar a gerar uma nova experiência de Metadados, use um modelo disponível para fornecer a estrutura para o seu conteúdo.

**Para escolher um modelo de meta-anúncio**:

1. Em _[!DNL Create]_, clique em **[!UICONTROL Meta anúncios]**na_&quot;O que você deseja criar hoje?&quot;seção _.
1. Use a opção de pesquisa, adjacente ao _Filtro_, para localizar um Modelo de Metadados específico.
1. Clique para selecionar um modelo e clique em **[!UICONTROL Usar]**.

   Essa ação abre a Tela, que é o hub central para a criação de conteúdo.

## Adicionar parâmetros

Adicionar [diretrizes](/help/user-guide/guidelines/overview.md) e ativos em _Parâmetros_ na área de prompt melhora o processo de geração de conteúdo e é uma etapa crucial na preparação para gerar um Metadado.

**Para adicionar parâmetros e ativos**:

1. Clique no ícone _Parâmetros_ para expandir a área de prompt.
1. Na seção _Parâmetros_, selecione as diretrizes—[!DNL Brands], [!DNL Personas] e [!DNL Products]—para informar sobre a criação de conteúdo.

   Se não houver marcas, personalidades ou produtos disponíveis nesses menus, [adicione diretrizes ao seu GenStudio para Marketing de Desempenho](/help/user-guide/guidelines/add-guidelines.md).

1. Clique em **[!UICONTROL Selecionar conteúdo]** para adicionar conteúdo a ser usado na experiência *e* para influenciar a geração de conteúdo.
   * Para selecionar ativos (imagens) já publicados em [!DNL Content], clique em **[!UICONTROL Selecionar do conteúdo]** e clique em para selecionar as imagens desejadas. Use os filtros para restringir ainda mais os resultados da pesquisa.

     Se quiser usar ativos já presentes em um repositório conectado do AEM Content Hub, selecione o local aplicável no menu suspenso _Local_ e clique para selecionar as imagens desejadas.

   * Clique em **[!UICONTROL Carregar]** para procurar seus arquivos e escolher os ativos a serem usados. Além de navegar em seu dispositivo, você também pode importar do Microsoft OneDrive ou Dropbox. Clique em para selecionar as imagens desejadas.
   * Arraste e solte ativos na seção _Conteúdo_.
1. Clique em **[!UICONTROL Usar]**.

Quando terminar de adicionar parâmetros, você poderá recolher a área de prompt clicando no ícone _Parâmetros_ novamente.

## Digite um prompt

Depois que as diretrizes forem selecionadas, crie um prompt usando a linguagem natural para começar a gerar conteúdo para sua nova experiência de Meta ad. Prompts detalhados produzem uma saída de qualidade superior aos prompts vagos ou indescritivos.

Consulte [Gravar prompts efetivos](/help/user-guide/effective-prompts.md) para saber mais sobre a gravação de prompts.

**Para inserir um prompt**:

1. Digite um prompt na caixa de prompt _&quot;Descrever as experiências que você deseja gerar&quot;_.
1. Clique em **[!UICONTROL Gerar]**.

Por padrão, quatro variações — todas alimentadas pelo prompt, pelas diretrizes e pelo conteúdo adicionado — são geradas e mostradas na Tela.

O conteúdo gerado é carregado progressivamente — à medida que cada seção das metaexperiências é gerada, elas aparecem na Tela. Consulte [Metaexperiências](/help/user-guide/create/meta-experiences.md#progressive-loading) para saber como essas alterações são carregadas na Tela.

## Escolher canal de metadados

Ao gerar um meta anúncio, você pode escolher entre anúncios do Facebook ou do Instagram.

Alterne a opção de canal de Metadados (entre **Facebook** e **Instagram**) para a barra de menu direita (ícones do Facebook e do Instagram) para ver e gerenciar as variantes de cada canal.

Ao [revisar os Metadados](#revise-generated-meta-ads), é possível alterar a proporção da Facebook e dos anúncios do Instagram.

## Revisar metadados gerados

Antes de selecionar o que enviar para aprovação ou publicação para [!DNL Content], você pode editar os Metadados ou excluir uma variante do conjunto de anúncios gerados.

**Para revisar variantes geradas**:

* **Para [editar o nome do rascunho do Metaanúncio](/help/user-guide/create/manage-variants.md#change-draft-name)**, clique no título _Rascunho Sem Título_ na parte superior da Tela e insira um novo título.
* **Para [editar um Metadado manualmente](/help/user-guide/create/manage-variants.md#manually-edit-text)**, clique duas vezes em qualquer seção do anúncio (como a linha de assunto, o cabeçalho ou a cópia do corpo) e edite conforme necessário.
* **Para alterar ou selecionar a chamada para ação**, clique no botão de chamada para ação e selecione nas opções de texto disponíveis do botão. Em _[!UICONTROL Link]_, insira uma URL para o texto de chamada para ação.
* **Para [alterar o tamanho e a taxa de proporção do anúncio](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**, clique no botão _[!UICONTROL Redimensionar]_ (caixa com um ícone de botão no lado esquerdo da Tela de Pintura) e selecione um novo tamanho e uma nova taxa de proporção a serem aplicados a todas as variantes. As variantes são duplicadas e redimensionadas.
<!-- * **To [regenerate a section of a variant](/help/user-guide/create/manage-variants.md#re-generate-sections)**, click an editable text field and use the _[!UICONTROL Suggested edits]_ options or enter a new prompt and click **[!UICONTROL Generate]**. -->
* **Para [cortar ou reposicionar imagens](/help/user-guide/create/manage-variants.md#crop-assets)**, passe o mouse sobre uma imagem, clique no ícone de recorte exibido e ajuste o tamanho e o posicionamento da imagem.
* **Para [excluir um Metadado](/help/user-guide/create/manage-variants.md#delete-variant)**, clique no título do anúncio (por exemplo, &quot;Meta 4&quot;) e clique em **[!UICONTROL Excluir variante]**.

## Enviar feedback de geração

Para [enviar comentários](/help/user-guide/create/manage-variants.md#generation-feedback) sobre a qualidade da saída de geração, clique no ícone de opções (três pontos) e selecione **[!UICONTROL Boa saída]** ou **[!UICONTROL Má saída]**.

## Verificar o alinhamento da marca

Para otimizar os anúncios gerados e garantir a adesão estrita à identidade da marca, aproveite o potencial da [_Verificação das diretrizes da marca_](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check)—fornecendo um resumo do alinhamento da marca para uma variante—e do [_painel Validação da marca_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel)—exibindo detalhes abrangentes da validação da marca e áreas de aprimoramento mais claras.

**Para verificar o alinhamento da marca**:

1. Clique no ícone de verificação]**](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) das diretrizes de [**[!UICONTROL [!DNL Brand] para uma variante e veja um resumo de como essa variante é executada quando marcada em relação à sua marca.
1. Para obter os detalhes das seções e diretrizes que precisam ser aprimoradas, clique em **[!UICONTROL Revisão]** _ou_ clique no ícone Validação da marca na barra de menu superior para abrir o [_Painel de validação da marca_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel).

1. Alterne cada anúncio para ver como você pode melhorar o conteúdo gerado para torná-lo mais alinhado à marca.
1. [Revise os anúncios manualmente](#revise-generated-meta-ads) para garantir que seus anúncios estejam alinhados à sua marca.

Consulte [Validação da marca](/help/user-guide/guidelines/brand-validation.md).

## Obter revisões e aprovações

Use o painel Aprovações, acessível na barra de menu superior da Tela, para obter revisões, rastrear comentários de revisão e obter aprovações das partes interessadas.

**Para obter revisões e aprovações**:

1. [Iniciar uma solicitação de aprovação](/help/user-guide/approvals/request-review.md) para solicitar uma [aprovação de experiências de Metadados rascunhados](/help/user-guide/approvals/approve-content.md).
1. [Remover ou adicionar revisores](/help/user-guide/approvals/review-and-edit.md#manage-approvals) durante o processo de revisão.
1. [Acesse o conteúdo para revisão](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) e exiba as solicitações de revisão.
1. Edite os rascunhos por comentários de revisão e [publique suas experiências de Metadados](#publish-and-export-experience).

Consulte [Revisões e aprovações](/help/user-guide/approvals/overview.md) para obter mais informações.

## Experiência do Publish e de exportação

Para disponibilizar os Metadados gerados para uso atual e futuro, publique-os no [!UICONTROL Content] e exporte-os para uso em suas campanhas de marketing.

1. **Para publicar sua(s) nova(s) experiência(s) de Metadados**, clique em **[!UICONTROL Publish]** na barra de ferramentas superior.
1. **Para exportar sua(s) nova(s) experiência(s) de Metadados**, clique em **[!UICONTROL Exportar]** na barra de ferramentas superior.
   1. Selecione o formato (somente CSV e imagens ou HTML) e clique em **[!UICONTROL Exportar]**.

Consulte [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) para obter mais informações.

## Conectar Meta

Você pode conectar o GenStudio for Performance Marketing ao Meta para receber análises avançadas e [insights](/help/user-guide/insights/overview.md) sobre o desempenho do conteúdo.

Consulte [Conectar conta de canal](/help/user-guide/insights/connect-channel.md) para obter mais informações.
