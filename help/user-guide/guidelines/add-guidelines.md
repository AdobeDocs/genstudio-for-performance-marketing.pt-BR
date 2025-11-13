---
title: Adicionar diretrizes ao Adobe GenStudio for Performance Marketing
description: Saiba como adicionar diretrizes como parâmetros para seus prompts no Adobe GenStudio for Performance Marketing.
feature: Brand Personalization, Product Personalization, Persona Personalization, Variant Generation, Generative AI
role: User
level: Beginner
exl-id: cb893b5d-b535-42f6-8dd8-8bd779d80a4f
source-git-commit: a4df9c81339a8fe5197200d58abc8b48df59da6f
workflow-type: tm+mt
source-wordcount: '2476'
ht-degree: 0%

---

# Adicionar diretrizes

O GenStudio for Performance Marketing permite definir diretrizes definidas pelo usuário que garantem que qualquer conteúdo gerado por IA seja personalizado para se alinhar à identidade de uma marca. Esta página oferece instruções para definir e usar cada diretriz específica disponível. Para obter uma explicação geral, consulte a [visão geral das diretrizes](/help/user-guide/guidelines/overview.md).

Adicionar diretrizes ao GenStudio for Performance Marketing é uma etapa importante no processo de criação. As diretrizes informam o processo de criação de conteúdo, juntamente com prompts definidos pelo usuário, [verificações de acessibilidade e conteúdo](overview.md#compliance) e a tecnologia de IA gerativa da Adobe, para criar ativos impactantes.

As diretrizes podem ser definidas pelo usuário ou podem existir como diretrizes padrão, como as [diretrizes padrão [!DNL Brand] do canal](/help/user-guide/guidelines/brands.md#default-channel-guidelines).

Ao criar variantes de um modelo com diretrizes de canal predefinidas (como [!DNL Brands], [!DNL Personas] ou [!DNL Products]), essas diretrizes se aplicam às variantes. Você pode alterá-los se desejar.

{{in-academy}}

## Adicionar marcas

Para adicionar uma [!DNL Brand], [carregue um guia de marca](#upload-a-brand) ou [crie uma marca manualmente](#manually-add-brand) selecionando diretrizes e inserindo detalhes da sua marca. [Publique um [!DNL Brand]](#publish-brand) em [!DNL Content] para torná-lo disponível para uso na geração de conteúdo futura.

Na área de navegação esquerda, clique em **[!DNL Brands]** na lista _Compartilhado_.

![Diretrizes no GenStudio for Performance Marketing](/help/assets/guidelines.png){width="650" zoomable="yes"}

Se você fizer upload das diretrizes da marca redigidas em um idioma diferente do inglês, ou criar uma marca manualmente usando um idioma diferente do inglês, o GenStudio for Performance Marketing exibirá essas diretrizes nesse mesmo idioma.

>[!TIP]
>
>Cada marca opera independentemente sem relações hierárquicas. Para criar submarcas em uma marca principal, inclua as informações da marca principal durante o processo de criação.

### Carregar uma marca

Você pode fazer upload de seus próprios documentos de diretrizes de marca (até três arquivos PDF ou DOC) para a GenStudio for Performance Marketing para criar uma marca automaticamente.

Consulte [[!DNL Brands]](/help/user-guide/guidelines/brands.md).

**Para carregar documentos da marca**:

1. No painel _[!DNL Brands]_, selecione o botão **[!UICONTROL Adicionar marca]**.
1. Escolha **[!UICONTROL Carregar PDFs]** e insira um nome de marca no pop-up _Escolher uma maneira de adicionar sua marca_.
1. Selecione **[!UICONTROL Continuar]**.
1. Procure e anexe ou arraste seus documentos de diretrizes de marca para o pop-up _[!UICONTROL Adicionar sua marca]_.

   É possível anexar até cinco arquivos PDF a um máximo de 500 MB.

1. Selecione **[!UICONTROL Adicionar marca]**.

   Usando a tecnologia de IA generativa da Adobe, a GenStudio for Performance Marketing extrai informações de seus documentos carregados e começa a criar sua marca. As informações da marca, como voz da marca, canal e diretrizes de imagem, são preenchidas à medida que cada diretriz dos documentos da marca é montada.

A visualização da nova marca é aberta, mostrando os detalhes das diretrizes da marca extraídos de seus documentos. Um pop-up notifica você _&quot;Sua marca está pronta para ser revisada&quot;_ e lembra você de revisar o conteúdo extraído e fazer as edições necessárias.

### Adicionar marca manualmente

Você pode adicionar detalhes da marca manualmente, em vez de carregar documentos de marcas existentes, para preencher uma nova [marca](brands.md).

**Para adicionar manualmente uma marca**:

1. Selecione o botão **[!UICONTROL Adicionar marca]**.
1. Escolha **[!UICONTROL Carregar manualmente]** e insira um nome de marca no pop-up _Escolher uma maneira de adicionar sua marca_.
1. Selecione **[!UICONTROL Adicionar marca]**.

   Uma nova marca em branco é criada e exibida.

1. Preencha várias informações, diretrizes e imagens da marca para criar sua marca nas seções apropriadas (exibições de guias na parte superior).

   Você pode adicionar diretrizes diretamente da exibição da página inicial da sua nova marca _ou_ você pode adicioná-las nas seções com guias individuais (que incluem _Exibir exemplos_ para orientá-lo) na parte superior.

   ![Marcas](/help/assets/brands.png){width="600" zoomable="yes"}

   - _Quando usar esta marca_: clique em **[!UICONTROL Adicionar]** (ou clique no campo de texto para alterar o texto existente) e insira a visão geral e as informações de uso sobre a marca. Clique em **[!UICONTROL Salvar alterações]**.
   - [_[!DNL Brand] diretrizes de voz _](brands.md#brand-voice-guidelines): adicione as informações aplicáveis em cada campo de diretrizes.

     ![Adicionar [!DNL Brand] diretrizes de voz ](/help/assets/brand-voice-add.png){width="500" zoomable="yes"}

   - [_Diretrizes de imagem_](brands.md#image-guidelines): clique em **[!UICONTROL Adicionar categoria]** para adicionar categorias de diretriz, como &quot;Diretrizes gerais de arte&quot; ou &quot;Fotografia do produto&quot;. Preencha as diretrizes em cada categoria adicionada.
   - [_Diretrizes do canal_](brands.md#channel-guidelines): clique em cada canal disponível e adicione as diretrizes apropriadas.
   - [_Logotipos_](brands.md#logos): clique em **[!UICONTROL Adicionar logotipo]** para arrastar e soltar ou procure e carregue um logotipo.
   - [_Cores_](brands.md#colors): clique em **[!UICONTROL Adicionar cor]** para usar um código de cor hexadecimal ou RGB, ou o seletor de cores, para adicionar cores individuais.

     ![Cores da marca](/help/assets/colors.png){width="600" zoomable="yes"}

Para ver a [!DNL Brands] criada, clique na seta para trás próxima à parte superior do painel _[!UICONTROL Marcas]_ para navegar de volta para a página inicial das _[!UICONTROL Marcas]_.

Você não precisa [publicar](#publish-brand) seu [!DNL Brand] para tornar as informações acessíveis. Qualquer informação adicionada manualmente fica disponível imediatamente após ser adicionada. Para que outras pessoas na sua organização usem as informações de [!DNL Brand] no GenStudio for Performance Marketing, você deve publicá-las. Um [!DNL Brand] criado estará no formato de rascunho até ser publicado.

### Alterar miniatura da marca

Depois de adicionar manualmente um [!DNL Brand], você pode alterar a imagem da miniatura para garantir que ela seja facilmente distinguível na lista [!DNL Brands].

Se um [!DNL Brand] for criado com extração de documento (em vez de ser adicionado manualmente), um logotipo disponível nesses documentos será implementado automaticamente como a imagem em miniatura.

**Altere manualmente a imagem em miniatura de[!DNL Brand]**:

1. Selecione **[!UICONTROL Alterar miniatura]** no menu de ações.
1. Carregue uma nova imagem na guia _Upload_.
1. Em _[!UICONTROL Alterar miniatura]_, altere a imagem carregada.
1. Selecione **[!UICONTROL Atualizar]** para salvar a imagem como sua imagem em miniatura [!DNL Brand].

Você pode selecionar um logotipo [!DNL Brand] existente na exibição de guia [!UICONTROL Logotipos] para um [!DNL Brand]. Clique para abrir um logotipo e selecione **[!UICONTROL Usar como miniatura da marca]** no menu de ações.

### Publicar marca

Antes de publicar um rascunho [!DNL Brand], clique em todas as seções de diretrizes para revisar todas as informações preenchidas. Faça as alterações necessárias nas diretrizes da marca.

Em _[!DNL Brands]_, qualquer rascunho ou [!DNL Brands] publicado aparece como mosaico. Uma medalha de status-_ Publicada _ou_ Rascunho _—e a última vez que a marca foi modificada é exibida na parte inferior de cada bloco.

>[!TIP]
>
>Para ver apenas as marcas criadas por você, selecione **[!UICONTROL Criado por você]** no filtro [!DNL Brands] (ícone do funnel).

**Para publicar um rascunho da Marca**:

1. Na área de navegação esquerda, clique em **[!UICONTROL [!DNL Brands]]**.
1. Clique em um bloco de miniaturas para abrir um rascunho existente do [!DNL Brand].
1. Clique no botão **[!UICONTROL Publicar]** (disponível somente para rascunhos).
1. No pop-up _Publicar marca_, verifique quem tem acesso para exibir e usar o [!DNL Brand] publicado.
1. Na janela pop-up _Publicar marca_ exibida, selecione **[!UICONTROL Publicar]**.

   O pop-up confirma que [!DNL brand] foi publicado—&quot;{Brand} está pronto&quot;.

1. Clique em **[!UICONTROL Concluído]** para sair do pop-up.

O [!DNL brand] mostra um ponto verde e &quot;Publicado&quot; adjacente ao nome, e um botão **[!UICONTROL Editar[!DNL brand]]** é exibido no lugar do botão **[!UICONTROL Publicar]**.

**Para desfazer a publicação de um[!DNL brand]** publicado, clique na marca para abri-lo e clique em **[!UICONTROL Desfazer publicação]** no menu de ações (ícone de três pontos).

A marca publicada agora está disponível para uso em [_[!DNL Create]_](/help/user-guide/create/overview.md) e [_[!DNL Content]_](/help/user-guide/content/overview.md).

### Gerenciar marcas

Na página inicial do _[!DNL Brands]_, você pode clicar em para abrir uma marca já criada para gerenciá-la ou publicá-la.

Para **exibir informações sobre a marca**, clique em **[!UICONTROL [!DNL Brands]]** na área de navegação à esquerda e clique em para abrir uma marca existente.

**Para modificar uma marca** na exibição [!DNL Brands]:

1. Em **[!DNL Brands]**, clique para abrir uma marca definida.
1. Para exibir detalhes individuais ou modificar diretrizes, clique em [**[!UICONTROL Diretrizes de voz da marca]**](brands.md#brand-voice-guidelines), [**[!UICONTROL Diretrizes de imagem]**](brands.md#image-guidelines), [**[!UICONTROL Diretrizes de canal]**](brands.md#channel-guidelines), [**[!UICONTROL Logotipos]**](brands.md#logos) ou [**[!DNL Colors]**](brands.md#colors) na parte superior.
1. Para gerenciar um logotipo de marca, clique em [**[!UICONTROL Logotipos]**](brands.md#logos) na parte superior e clique no menu de ações (três pontos).
   1. Selecione **[!UICONTROL Exibir detalhes]** para ver informações para o [!DNL Brand], como _Formato_ e _Tamanho_.
   1. Selecione **[!UICONTROL Baixar]** para baixar o logotipo.
   1. Selecione [**[!UICONTROL Usar como miniatura da marca]](#change-brand-thumbnail) para definir o logotipo como a imagem em miniatura.
   1. Selecione **[!UICONTROL Renomear]** para renomear o logotipo.
   1. Selecione **[!UICONTROL Excluir]** para excluir o logotipo.
1. Para renomear uma marca existente, clique no título e insira um novo título.
1. Para duplicar uma marca existente, selecione **[!UICONTROL Duplicar]** no menu de ações _[!DNL Brands]_.
   1. Insira um nome de marca no pop-up _Duplicar marca_ e clique em **[!UICONTROL Duplicar marca]**.

      O pop-up confirma que a marca foi duplicada — &quot;Nova marca criada&quot;. A marca duplicada está inicialmente no modo _Não publicado_.

   1. Personalize a marca duplicada e [publique-a](#publish-brand) para disponibilizá-la para uso.
1. Para excluir uma marca, selecione **[!UICONTROL Excluir]** no menu de ações [!DNL Brands].

## Adicionar [!DNL Personas]

Para adicionar um perfil, [carregue um perfil](#upload-a-persona) ou [crie um perfil manualmente](#manually-add-persona) selecionando diretrizes e inserindo seus detalhes pessoais.

Na área de navegação esquerda, clique em **[!DNL Personas]** na lista _Compartilhado_.

![Diretrizes no GenStudio for Performance Marketing](/help/assets/guidelines.png){width="650" zoomable="yes"}

Você pode adicionar um [!DNL Persona] no GenStudio for Performance Marketing para ajudar a direcionar o conteúdo que você cria para o seu público-alvo ideal.

Consulte [[!DNL Personas]](personas.md).

### Carregar um perfil

Você pode fazer upload de seus próprios documentos pessoais para preencher novos perfis.

Consulte [[!DNL Personas]](/help/user-guide/guidelines/personas.md).

1. No painel _[!DNL Personas]_, selecione o botão **[!UICONTROL Adicionar persona]**.
1. Escolha **[!UICONTROL Carregar arquivos]** e insira um nome de persona no pop-up _Escolher uma maneira de adicionar sua persona_.
1. Selecione **[!UICONTROL Continuar]**.
1. Procure e anexe ou arraste seus documentos de diretrizes de persona para o pop-up _[!UICONTROL Adicionar sua persona]_.

   É possível anexar até cinco arquivos PDF ou DOC de no máximo 500 MB.

1. Selecione **[!UICONTROL Adicionar personas]**.

   Usando a tecnologia de IA generativa da Adobe, o GenStudio for Performance Marketing extrai informações de seus documentos carregados e começa a criar sua persona. À medida que cada diretriz de seus documentos de persona for montada, você verá detalhes como voz de persona, canal e diretrizes de imagem serem preenchidos.

   A visualização da nova persona é aberta, mostrando os detalhes das diretrizes de persona extraídos de seus documentos. Um pop-up notifica você _&quot;Sua pessoa está pronta para revisar&quot;_ e lembra você de revisar o conteúdo extraído e fazer as edições necessárias.

### Adicionar persona manualmente

Você pode adicionar detalhes de persona manualmente, em vez de carregar documentos de persona existentes, para preencher uma nova [persona](personas.md).

**Para adicionar um perfil manualmente**:

1. Selecione o botão **[!UICONTROL Adicionar persona]** e escolha **[!UICONTROL Adicionar manualmente]**.
1. Clique em **[!UICONTROL Continuar]**.

   É possível preencher várias diretrizes e imagens opcionais para criar sua persona.

1. Clique em **[!UICONTROL Novo nome de persona]** e insira um nome para [!DNL Persona].
1. Adicione informações sobre [!DNL Persona] na seção _Descrição_.

   ![Adicionar um [!DNL Persona]](/help/assets/personas-add.png){width="650" zoomable="yes"}

1. Clique em _Descrição_ e insira uma descrição desta [!DNL Persona].
1. Clique em _Preferências de mensagens_ e insira os detalhes de mensagens de [!DNL Persona].
1. Para editar a miniatura, passe o mouse sobre a miniatura da imagem e, no menu de ações, selecione **[!UICONTROL Editar miniatura]**.
   1. Escolha uma imagem da galeria na guia _Galeria_ ou _para carregar uma nova imagem na guia_ Carregar _._

      Você também pode excluir ou recortar uma imagem em miniatura existente na guia _Carregar_.

   1. Clique em **[!UICONTROL Usar imagem]**.
1. Para editar a imagem da capa, passe o mouse sobre a capa e, no menu de ações, selecione **[!UICONTROL Editar capa]**.
   1. Escolha uma imagem da galeria na guia _Galeria_ ou _para carregar uma nova imagem na guia_ Carregar _._
   1. Clique em **[!UICONTROL Usar imagem]**.
   1. Para reposicionar a imagem da capa, clique em **[!UICONTROL Reposicionar]** no menu de ações, arraste a imagem para a posição desejada e clique em **[!UICONTROL Salvar]**.

   Para ver a [!DNL Personas] criada, clique na seta para trás próxima à parte superior da exibição _Persona_ para voltar à página inicial do _[!DNL Personas]_.

### Gerenciar [!DNL Personas]

Na página inicial de _[!DNL Personas]_, você pode **abrir um[!DNL Persona]**já criado para editá-lo ou revisá-lo, ou **excluir um**da lista:

- Selecione **[!UICONTROL Abrir]** no menu de ações [!DNL Personas] para revisar e revisar um perfil existente.
- Selecione **[!UICONTROL Excluir]** do menu de ações [!DNL Personas] para **Excluir** um perfil.
- Selecione **[!UICONTROL Renomear]** no menu de ações [!DNL Personas] para **Renomear** uma persona.

## Adicionar [!DNL Products]

Para adicionar um produto:

1. Na área de navegação esquerda, clique em **[!DNL Products]** na lista _Compartilhado_.
   ![Diretrizes no GenStudio for Performance Marketing](/help/assets/guidelines.png){width="650" zoomable="yes"}
1. No painel _[!DNL Products]_, selecione **Adicionar produto**.
1. Opte por [carregar um produto](#upload-a-product) ou [criar um produto manualmente](#manually-add-product) selecionando diretrizes e inserindo os detalhes do seu produto.

![Adicionar um [!DNL Product]](/help/assets/products-add.png){width="650" zoomable="yes"}

Você pode incluir um [!DNL Product] no GenStudio for Performance Marketing para melhor adaptar o conteúdo criado para um produto específico.

Consulte [[!DNL Products]](products.md).

### Carregar um produto

Você pode fazer upload de seus próprios documentos de produtos para preencher novos produtos.

Consulte [[!DNL Products]](/help/user-guide/guidelines/products.md).

1. Selecione o botão **[!UICONTROL Adicionar produto]**.
1. Escolha **[!UICONTROL Carregar arquivos]** e digite um nome de produto no pop-up _Escolher uma maneira de adicionar seu produto_.
1. Selecione **[!UICONTROL Continuar]**.
1. Procure e anexe ou arraste seus documentos de diretrizes do produto para a janela pop-up _[!UICONTROL Adicionar seu produto]_.

   É possível anexar até cinco arquivos PDF ou DOC de no máximo 500 MB.

1. Selecione **[!UICONTROL Adicionar produtos]**.

   Usando a tecnologia de IA gerativa da Adobe, a GenStudio for Performance Marketing analisa os documentos carregados para criar o perfil do produto. À medida que cada diretriz dos documentos do produto for processada, você verá informações como descrições de produtos, propostas de valor e preferências de mensagens preenchidas.

   A exibição do novo produto é aberta, mostrando os detalhes das diretrizes do produto extraídos de seus documentos. Um pop-up notifica você _&quot;Seu produto está pronto para ser revisado&quot;_ e o lembra de revisar o conteúdo extraído e fazer as edições necessárias.

### Adicionar um produto manualmente

Você pode adicionar detalhes do produto manualmente, em vez de carregar documentos de produtos existentes, para preencher um novo [produtos](products.md).

**Para adicionar manualmente um produto**:

1. Selecione o botão **[!UICONTROL Adicionar produto]** e escolha **[!UICONTROL Adicionar manualmente]**.
1. Clique em **[!UICONTROL Continuar]**.

   É possível preencher várias informações opcionais para criar seu produto.

1. Clique em **[!UICONTROL Novo nome do produto]** e digite um nome para o [!DNL product].
1. Adicione informações sobre [!DNL product] na seção _Descrição_.
1. Clique em _Descrição_ e insira uma descrição desta [!DNL Product].
1. Clique em _Proposta de valor_ e insira os detalhes da proposta de valor para posicionar corretamente a [!DNL Product].
1. Clique em _Preferências de mensagens_ e insira os detalhes de mensagens de [!DNL product].
1. Para editar a miniatura, passe o mouse sobre a miniatura da imagem e, no menu de ações, selecione **[!UICONTROL Editar miniatura]**.
   1. Escolha uma imagem da galeria na guia _Galeria_ ou _para carregar uma nova imagem na guia_ Carregar _._

      Você também pode excluir ou recortar uma imagem em miniatura existente na guia _Carregar_.

   1. Clique em **[!UICONTROL Usar imagem]**.
   1. Para editar a imagem da capa, passe o mouse sobre a capa e, no menu de ações, selecione **[!UICONTROL Editar capa]**.
   1. Escolha uma imagem da galeria na guia _Galeria_ ou _para carregar uma nova imagem na guia_ Carregar _._
   1. Clique em **[!UICONTROL Usar imagem]**.
   1. Para reposicionar a imagem da capa, clique em **[!UICONTROL Reposicionar]** no menu de ações, arraste a imagem para a posição desejada e clique em **[!UICONTROL Salvar]**.

   Para ver o [!DNL Products] criado, clique na seta para trás próxima à parte superior da exibição do _Produto_ para navegar de volta para a página inicial do _[!DNL Products]_.

### Gerenciar [!DNL Products]

Na página inicial de _[!DNL Products]_, você pode **abrir um[!DNL Product]**já criado para editá-lo ou revisá-lo, ou **excluir um produto**da lista:

- Selecione **[!UICONTROL Abrir]** no menu de ações [!DNL Products] para revisar e analisar um produto existente.
- Selecione **[!UICONTROL Excluir]** do menu de ações [!DNL Products] para **Excluir** um produto.
- Selecione **[!UICONTROL Renomear]** no menu de ações [!DNL Products] para **Renomear** um produto.

## Adicionar [!DNL Audiences]

>[!NOTE]
>
>O recurso [!DNL Audiences] exige integração da equipe do Adobe para ser exibido no GenStudio. Se _[!DNL Audiences]_não aparecer nos parâmetros do modelo, contate o representante da Adobe.

O [!DNL Audiences] fornece segmentos de clientes direcionados do Adobe Real-Time Customer Data Platform (RTCDP), trazendo dados precisos de direcionamento para o fluxo de trabalho de geração de conteúdo. O GenStudio for Performance Marketing aproveita as definições de público-alvo para ajudar você a criar conteúdo de marketing personalizado alinhado a segmentos de clientes específicos.

[!DNL Audiences] aparecem como uma lista suspensa no painel de parâmetros, no [fluxo de trabalho _[!DNL Create]_](../create/overview.md#templates)._[!DNL Audiences]_ pode adicionar especificidade a _[!DNL Personas]_quando ambas as diretrizes são usadas, mas também pode ser efetivamente usada de forma independente.

Durante a integração, as definições de público-alvo são importadas e transformadas em um formato compatível com o GenStudio. Normalmente, esse processo leva alguns dias para ser concluído. Entre em contato com a equipe do Adobe para iniciá-lo.

**Pré-requisitos**:

- Acesso organizacional ao Adobe Real-Time Customer Data Platform
- Públicos-alvo existentes já configurados em sandboxes do RTCDP
- A integração do _[!DNL Audience]_requer um processo de integração manual pela equipe do Adobe

**Para selecionar uma audiência**:

1. Em [o fluxo de trabalho _[!DNL Create]_](../create/overview.md#templates), selecione um modelo e clique no botão **[!UICONTROL Usar]**para abrir o rascunho.
1. Na lista de parâmetros, clique na lista suspensa _[!UICONTROL Público-alvo]_ para exibir todos os públicos-alvo disponíveis.
   ![Lista suspensa de público-alvo no painel Parâmetros de persona](./audience-dropdown.png){width=450}
1. Selecione um público a ser atribuído na lista. O sistema sugere públicos-alvo recomendados que se alinhem com o [!DNL Persona] selecionado, se um [!DNL Persona] for selecionado.
1. Clique em **[!UICONTROL Ver detalhes do público-alvo]** para exibir a descrição expandida e as preferências de mensagens geradas para o público-alvo selecionado. Os detalhes do público-alvo informam a geração de conteúdo, garantindo que a criação se alinhe às características e preferências específicas do segmento do público-alvo.
   ![Painel de detalhes do público-alvo](./audience-details.png){width=450}
