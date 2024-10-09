---
title: Gerenciar ativos e experiências
description: Simplifique e aprimore o gerenciamento de ativos aprovados pela marca para uso e reutilização em sua jornada de marketing digital.
feature: Content, Assets, Experiences
exl-id: e2ce8797-6d3b-46d4-b12f-f5f80e26c669
source-git-commit: ce08231cb723bec3d80a732837b72a435d3b552d
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 0%

---

# Gerenciar ativos e experiências

O Adobe GenStudio for Performance Marketing [!DNL Content] simplifica e aprimora o gerenciamento de ativos aprovados pela marca para uso e reutilização em sua jornada de marketing digital.

## Galeria do Assets

A galeria [!UICONTROL Assets] mostra um inventário de ativos aprovados. O ícone de filtro (funil) acima do lado esquerdo da tabela abre o menu **[!UICONTROL Filtro]**, onde você pode selecionar entre várias categorias para filtrar os ativos mostrados na galeria. Clique no ícone de pesquisa (lupa) para usar uma palavra-chave para localizar um ativo.

A seguir, uma pesquisa sobre o termo `dog` na galeria [!UICONTROL Assets]:

![exibição do Assets com pesquisa no cachorro](../../assets/content-assets.png)

### Localização do Assets

Por padrão, os ativos adicionados a [!DNL Content] por meio do processo [!DNL Create] ou através de upload são armazenados no repositório `GenStudio assets`. O repositório `GenStudio assets` é um repositório leitura-gravação no GenStudio for Performance Marketing. Isso significa que você pode salvar, editar e excluir ativos no repositório `GenStudio assets`.

A lista **[!UICONTROL Local]** acima da galeria no lado direito permite selecionar entre repositórios do Adobe Experience Manager (AEM) [!DNL Assets Content Hub] conectados. Quando você seleciona um repositório AEM, a galeria mostra um inventário de ativos desse repositório, permitindo que você aproveite os ativos aprovados desses repositórios como entradas para a criação de conteúdo. As opções de filtro são alteradas para refletir as categorias configuradas em [!DNL AEM Assets Content Hub].

O repositório AEM é somente leitura, o que significa que não é possível salvar rascunhos, novos ativos ou metadados no repositório AEM. Todos os rascunhos e atualizações finais para ativos, experiências e modelos são salvos no repositório do `GenStudio assets` com os novos [metadados do sistema](asset-details.md#system-metadata).

Consulte [Conectar um repositório AEM](connect-aem-repo.md) para obter orientação sobre como adicionar seu repositório [!DNL AEM Assets Content Hub] ao GenStudio for Performance Marketing.

## Gerenciamento do Assets

No [!UICONTROL Conteúdo], os profissionais de marketing de desempenho podem armazenar, recuperar e gerenciar facilmente seus ativos digitais. Ao utilizar os repositórios `GenStudio assets` e AEM, os usuários podem garantir que seus ativos estejam bem organizados e acessíveis para várias campanhas de marketing. Essa abordagem de vários repositórios oferece flexibilidade e controle sobre o uso de ativos em todos os ambientes, garantindo que somente ativos aprovados e atualizados sejam usados em esforços de marketing.

### Adicionar ativos

Ao adicionar ativos ao [!DNL Content], eles são armazenados por padrão no repositório `GenStudio assets`. O botão _[!UICONTROL Adicionar ativos]_ está disponível somente quando o _[!UICONTROL Local]_ é o repositório `GenStudio assets`.

![Campo de localização](../../assets/content-location.png){width="350" align="center"}

**Para adicionar um ou mais ativos**:

1. Em _[!DNL Content]_, clique em **[!UICONTROL Adicionar ativos]**.

1. No modo de exibição _Adicionar ativos aprovados_, solte um ou mais arquivos no espaço. Como opção, você pode selecionar arquivos locais usando o **[!UICONTROL Procurar]** ou importar arquivos do Dropbox ou do Microsoft OneDrive.

1. Na seção _Adicionar detalhes_, selecione um **[!UICONTROL nome da campanha]** ou insira um novo nome.

1. Para melhorar a descoberta, adicione detalhes opcionais, como _Marca_, _Personas_, _Região_ e _Palavras-chave_, na seção **Mais detalhes**.

   Quanto mais detalhes você fornecer, mais conhecerá os recursos avançados do GenStudio for Performance Marketing. Selecione um ou mais detalhes na lista ou insira um novo, onde aplicável, como com palavras-chave. Cada detalhe adicionado aparece abaixo da lista. Clique em **`x`** para remover um detalhe.

   Todos os detalhes adicionados se aplicam a todos os ativos adicionados nesta ação.

   Consulte [detalhes de metadados](/help/user-guide/content/asset-details.md#system-metadata).

1. Clique em **[!UICONTROL Adicionar ativos]**.

1. Quando o carregamento do ativo for concluído, clique em **Concluído**.

1. Para exibir os novos ativos carregados, clique em **[!UICONTROL Atualizar]** na notificação _Novos ativos disponíveis_, na parte inferior da Tela.

<!-- 
In the future, need guidance on template upload errors. For now, the UI just says error.
-->

### Pesquisar conteúdo

O filtro e a interface de pesquisa são rápidos e responsivos e fornecem uma experiência produtiva de pesquisa. Cada exibição do [!DNL Content] fornece opções de Filtro para restringir sua pesquisa pelo ativo, experiência ou modelo ideal. Para ativos e experiências, você pode selecionar uma campanha e diretrizes específicas, como o conteúdo criado para um produto específico.

Há filtros baseados em [palavras-chave](asset-details.md#user-defined-metadata) e [atributos](/help/user-guide/insights/attributes.md) para restringir os resultados da pesquisa. Por exemplo, talvez você queira encontrar um ativo de um tipo de arquivo ou assunto específico para ajudá-lo a criar uma nova experiência para sua campanha.

Ao pesquisar por _Experiências_, você pode usar o filtro **[!UICONTROL Criado por]** para limitar a lista a fim de mostrar apenas as experiências criadas por você ou por uma pessoa específica.

**Para pesquisar conteúdo a ser reutilizado**:

1. Em _[!DNL Content]_, selecione a seção **[!UICONTROL Assets]**.

1. Selecione um repositório de ativos na lista **[!UICONTROL Local]** ou verifique se você está observando o repositório de ativos correto. `GenStudio assets` é o repositório padrão.

   >[!IMPORTANT]
   >
   >A lista _Local_ está disponível somente quando você [se conecta a um repositório AEM](connect-aem-repo.md).

1. Clique em **[!UICONTROL Pesquisar]** (lupa) para inserir uma palavra-chave ou descrição.

1. Restrinja sua pesquisa selecionando uma categoria na lista _[!UICONTROL Filtro]_. Por exemplo, se você estiver procurando um arquivo PNG, clique em **[!UICONTROL Formato de arquivo]** e escolha **PNG**.

   Quanto mais você limitar sua pesquisa, menos opções de filtro estarão disponíveis. Clique em **[!UICONTROL Limpar tudo]** para remover todos os filtros.

1. Selecione um ativo para obter uma visualização completa e uma lista de detalhes.

   Clique em **[!UICONTROL Baixar]** (seta para baixo) para usar o ativo na sua estação de trabalho local.
