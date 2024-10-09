---
title: Criar uma experiência de email
description: Saiba como criar experiências de email no Adobe GenStudio para Marketing de desempenho.
feature: Content, Brands Service, Guidelines, Content Generation, Create, Experiences, Variant Generation
role: User
level: Beginner
type: Tutorial
recommendations: noDisplay
exl-id: 34446202-da98-45ff-869a-b43496a477f8
source-git-commit: 30cd73ba1beb582ea4ac73eca7e17715f9aafc66
workflow-type: tm+mt
source-wordcount: '955'
ht-degree: 0%

---

# Criar uma experiência de email

Este tutorial demonstra como gerar [experiências de email](/help/user-guide/create/email-experiences.md) com a marca usando o GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (ícone de pincel na área de navegação à esquerda).

Para criar uma experiência de email eficaz, é recomendável [adicionar diretrizes ao GenStudio para Marketing de Desempenho](/help/user-guide/guidelines/add-guidelines.md) e aprofundar as [noções básicas de criação de um prompt](/help/user-guide/effective-prompts.md) antes de começar.

## Escolher um modelo

Para criar uma nova experiência de email, use um modelo disponível para fornecer a estrutura para o seu conteúdo.

**Para escolher um modelo de email**:

1. Em _[!DNL Create]_, clique em **[!UICONTROL Email]**na_&quot;O que deseja criar hoje?&quot;seção _.
1. Use a opção de pesquisa, ao lado de _Filtro_, para localizar um modelo de email específico.
1. Clique para selecionar um modelo de email e clique em **[!UICONTROL Usar]**.

   A Tela, o epicentro da criação de conteúdo, é exibida.

## Adicionar parâmetros

Adicionar [diretrizes](/help/user-guide/guidelines/overview.md) e ativos em _Parâmetros_ na área de prompt sobrecarrega o processo de geração de conteúdo e é uma etapa preparatória integral para gerar uma experiência de email.

**Para adicionar parâmetros e ativos**:

1. Clique no ícone _Parâmetros_ para expandir a área de prompt.
1. Na seção _Parâmetros_, selecione as diretrizes—[!DNL Brands], [!DNL Personas] e [!DNL Products]—para informar sobre a criação de conteúdo.

   Se não houver marcas, personalidades ou produtos disponíveis nesses menus, [adicione diretrizes ao seu GenStudio para Marketing de Desempenho](/help/user-guide/guidelines/add-guidelines.md).

1. Clique em **[!UICONTROL Selecionar conteúdo]** para adicionar conteúdo a ser usado na experiência *e* para influenciar a geração de conteúdo.
   * Para selecionar ativos (imagens) do seu repositório [!DNL Content], clique em **[!UICONTROL Selecionar do conteúdo]**. Filtre e selecione uma ou mais imagens.

     Para usar ativos de um repositório [!DNL AEM Assets Content Hub] conectado, escolha um repositório no menu suspenso _Local_. Filtre e selecione uma ou mais imagens.

   * Para carregar um ou mais novos ativos, clique em **[!UICONTROL Carregar]**, navegue pelos arquivos e escolha os ativos a serem usados. Além de navegar em seu dispositivo, você pode importar do Microsoft OneDrive ou Dropbox. Clique em para selecionar as imagens desejadas.
   * Arraste e solte ativos na seção _Conteúdo_.
1. Clique em **[!UICONTROL Usar]**.

>[!NOTE]
>
>Se o seu modelo de email tiver várias seções, selecione [!DNL Products] e conteúdo (ativos visuais) para cada seção de email em _Emails de várias seções_. Emails de várias seções suportam um ativo visual por seção.

Quando terminar de adicionar parâmetros, você poderá recolher a área de prompt clicando no ícone _Parâmetros_ novamente.

## Digite um prompt

Depois que as diretrizes forem selecionadas, crie um prompt usando a linguagem natural para começar a gerar conteúdo para sua nova experiência de email. Prompts detalhados produzem uma saída de qualidade superior aos prompts vagos ou indescritivos.

Consulte [Gravar prompts efetivos](/help/user-guide/effective-prompts.md) para saber mais sobre a gravação de prompts.

**Para inserir um prompt**:

1. Digite um prompt na caixa de prompt _&quot;Descrever as experiências que você deseja gerar&quot;_.
1. Clique em **[!UICONTROL Gerar]**.

Por padrão, quatro variações — todas alimentadas pelo prompt, pelas diretrizes e pelo conteúdo adicionado — são geradas e mostradas na Tela.

O conteúdo gerado é carregado progressivamente — à medida que cada seção das experiências de email é gerada, elas são exibidas na Tela. Consulte [Experiências de email](/help/user-guide/create/meta-experiences.md#progressive-loading) para saber como essas alterações são carregadas na Tela.

## Revisar emails gerados

Antes de selecionar o que enviar para aprovação ou publicação para [!DNL Content], você pode editar seções de email ou excluir uma variante do conjunto de emails gerados.

**Para revisar variantes geradas**:

* **Para [editar o nome do rascunho do email](/help/user-guide/create/manage-variants.md#change-draft-name)**, clique no título _Rascunho Sem Título_ na parte superior da Tela e insira um novo título.
* **Para [editar um email manualmente](/help/user-guide/create/manage-variants.md#manually-edit-text)**, clique duas vezes em qualquer campo de texto editável (como linha de assunto, cabeçalho ou cópia de corpo) e edite conforme necessário
<!-- * **To [regenerate a section of a variant](/help/user-guide/create/manage-variants.md#re-generate-sections)**, click an editable text field and use the _[!UICONTROL Suggested edits]_ options or enter a new prompt and click **[!UICONTROL Generate]**. -->
* **Para [adicionar ou trocar imagens em uma variante](/help/user-guide/create/manage-variants.md#swap-image)**, clique em um ativo de imagem (ou na área do ativo de imagem se uma imagem não existir no momento) e clique em **[!UICONTROL Selecionar/trocar conteúdo]** ou **[!UICONTROL Carregar nova imagem]** para adicionar ou trocar uma imagem em uma variante individual.
* **Para [excluir um email](/help/user-guide/create/manage-variants.md#delete-variant)**, clique para selecionar o título do email (por exemplo, &quot;Email 1/4&quot;) e clique em **[!UICONTROL Excluir variante]**.

## Enviar feedback de geração

Para [enviar comentários](/help/user-guide/create/manage-variants.md#generation-feedback) sobre a qualidade da saída de geração, clique no ícone de opções (três pontos) e selecione **[!UICONTROL Boa saída]** ou **[!UICONTROL Má saída]**.

## Visualizar para dispositivo

Ao revisar e preparar experiências de email, você pode [alternar entre visualizações para desktop e dispositivos móveis](/help/user-guide/create/manage-variants.md#preview-for-device) para garantir a coerência e o apelo visual de variantes de rascunho.

## Verificar o alinhamento da marca

Para otimizar os emails gerados e garantir a adesão estrita à identidade da marca, aproveite o potencial da [_Verificação das diretrizes da marca_](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check)—fornecendo um resumo do alinhamento da marca para uma variante—e do [_painel Validação da marca_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel)—exibindo detalhes abrangentes da validação da marca e áreas de aprimoramento esclarecedoras.

**Para verificar o alinhamento da marca**:

1. Clique no ícone de verificação]**](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) das diretrizes de [**[!UICONTROL [!DNL Brand] para uma variante e veja um resumo de como essa variante é executada quando marcada em relação à sua marca.
1. Para obter os detalhes das seções e diretrizes que precisam ser aprimoradas, clique em **[!UICONTROL Revisão]** _ou_ clique no ícone Validação da marca na barra de menu superior para abrir o [_Painel de validação da marca_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel).

1. Alternar em cada email para ver como você pode melhorar o conteúdo gerado para estar mais alinhado à marca.
1. [Revise emails manualmente](#revise-generated-emails) para garantir que seus emails estejam alinhados à sua marca.

Consulte [Validação da marca](/help/user-guide/guidelines/brand-validation.md).

## Obter revisões e aprovações

Use o painel Aprovações, acessível na barra de menu superior da Tela, para obter revisões, rastrear comentários de revisão e obter aprovações das partes interessadas.

**Para obter revisões e aprovações**:

1. [Iniciar uma solicitação de aprovação](/help/user-guide/approvals/request-review.md) para solicitar uma [aprovação de experiências de email em rascunho](/help/user-guide/approvals/approve-content.md).
1. [Remover ou adicionar revisores](/help/user-guide/approvals/review-and-edit.md#manage-approvals) durante o processo de revisão.
1. [Acesse o conteúdo para revisão](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) e exiba as solicitações de revisão.
1. Edite os rascunhos de acordo com os comentários de revisão e [publique suas experiências de email](#publish-and-export-experience).

Consulte [Revisões e aprovações](/help/user-guide/approvals/overview.md) para obter mais informações.

## Experiência do Publish e de exportação

Para disponibilizar os emails gerados para uso atual e futuro, publique-os no [!UICONTROL Conteúdo] e exporte-os para uso em suas campanhas de marketing.

1. **Para publicar sua(s) nova(s) experiência(s) de email**, clique em **[!UICONTROL Publish]** na barra de ferramentas superior.
1. **Para exportar sua(s) nova(s) experiência(s) de email**, clique em **[!UICONTROL Exportar]** na barra de ferramentas superior.
   1. Selecione o formato (somente CSV e imagens ou HTML) e clique em **[!UICONTROL Exportar]**.

Consulte [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) para obter mais informações.
