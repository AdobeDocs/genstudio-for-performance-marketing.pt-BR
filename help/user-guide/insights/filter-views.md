---
title: Filtrar visualizações do Insights
description: Saiba como usar os recursos aprimorados de filtro com Insights.
level: Intermediate
feature: Reporting and Insights
source-git-commit: 656395e517fcb334b64865dcdbde09d8d982dc0a
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 0%

---

# Filtro para visualizações de Insights

O painel [!DNL Insights] fornece um conjunto abrangente de filtros para uma experiência eficiente de exploração de dados. Ao analisar canais, anúncios, mídia ou atributos específicos, as opções de filtro permitem personalizar sua visualização e simplificar seu fluxo de trabalho. Use filtros de palavra-chave para direcionamento preciso ou explore listas predefinidas para refinar sua pesquisa e se concentrar nos dados mais importantes.

## Noções básicas de filtro

Cada modo de exibição em [!DNL Insights] oferece uma lista de opções de filtro. O ícone de filtro (funil) acima do lado esquerdo da tabela abre o menu **[!UICONTROL Filtro]**. Se você estiver visualizando a tabela ou a galeria, os filtros aplicados aparecerão na lista **[!UICONTROL Filtrar por]** acima da tabela ou galeria. Por padrão, um canal e uma conta são selecionados.

![Filtrar por](/help/assets/insights-filter-by.png "Filtrar por"){width=600 zoomable="yes"}

Os filtros aplicados persistem em todas as exibições. Selecione **[!UICONTROL Limpar tudo]** acima da tabela ou galeria para remover todos os filtros selecionados.

### Campo de pesquisa

Clique no ícone de pesquisa (lupa) para usar um termo de pesquisa para localizar itens específicos na tabela ou galeria. Por exemplo, inserir o termo `pink` na tabela [!UICONTROL Anúncios] filtra os resultados para exibir somente anúncios usando o termo `pink` no nome.

![Exemplo de campo de pesquisa](/help/assets/insights-search.png "Pesquisar anúncios em rosa"){width=600 zoomable="yes"}

### Intervalo de datas

O seletor de intervalo de datas é uma ferramenta poderosa para alinhar os dados exibidos com seus objetivos de análise. Use o seletor de intervalo de datas para ajustar o intervalo de tempo dos dados exibidos na tabela ou exibição de galeria. Por padrão, o intervalo de datas é definido como os últimos 30 dias. Para incluir mais dados ou se concentrar em um período específico, expanda o intervalo de datas.

![Seletor de intervalo de datas](/help/assets/insights-date-range.png "Selecione um intervalo de datas"){width=400}

Se nenhum item aparecer na exibição de tabela ou galeria, talvez o intervalo de datas selecionado não inclua dados relevantes. Nesses casos, aumente o intervalo de datas para garantir que os dados desejados sejam incluídos.

### Páginas

Algumas tabelas podem abranger várias páginas, conforme indicado abaixo da tabela no lado direito. Use as opções versáteis de pesquisa e filtro para refinar os resultados. Para navegar entre páginas, use os controles de paginação direita (avançar) e esquerda (voltar). Aplique os filtros corretamente para incluir todos os dados relevantes nas páginas.

### Controle de slide

Algumas opções de filtro incluem um controle deslizante, que permite selecionar um valor dentro de um intervalo definido. Por exemplo, no controle deslizante _[!UICONTROL Atributos]_, a **[!UICONTROL Contagem de mídia]** permite filtrar atributos com base no número de imagens ou vídeos associados. Arraste o controle deslizante para especificar um intervalo, começando com um mínimo de 0 até um máximo que pode exceder 100.

## Filtragem avançada

Com os filtros _[!UICONTROL Campanhas]_ e _[!UICONTROL Anúncios]_, você pode utilizar palavras-chave precisas para refinar a lista. Os filtros de palavra-chave são particularmente úteis para filtrar campanhas ou anúncios que usam uma convenção de nomenclatura complexa com vários identificadores exclusivos. Por exemplo, um nome de campanha pode incluir o seguinte:

- Nome ou código de região específico: `NA`, `EMEA`
- Acrônimos de tipo de conteúdo: `EB`, `CHT` ou `DSP`
- Códigos de oferta ou acrônimos: `OFFER2023`, `PROMO`

Com o tempo, a lista de campanhas e anúncios cresce exponencialmente. Considere o seguinte cenário para usar o filtro _[!UICONTROL Campanhas]_ para refinar a tabela [!UICONTROL Anúncios].

**Para refinar a tabela Anúncios usando o filtro Campanhas**:

1. Em _[!DNL Insights]_, selecione a exibição **[!UICONTROL Anúncios]**.

   ![Filtro de anúncios e tabela](/help/assets/insights-ads-filter.png "Exibição de anúncios com lista de filtros"){zoomable="yes"}

1. Clique no ícone de filtro (funil) acima do lado esquerdo da tabela para abrir o menu **[!UICONTROL Filtro]**.

1. Verifique se o canal `Filter by` e a conta corretos estão selecionados.

1. Expanda o filtro **[!UICONTROL Campanhas]** e clique em **[!UICONTROL Selecionar]**.

   ![Filtrar campanhas](/help/assets/insights-filter-campaigns-expand.png "Expandir filtro de campanhas"){width=200}

1. No campo de pesquisa _[!UICONTROL Selecionar campanhas]_, insira palavras-chave separadas por vírgulas.

   - Use quantas palavras-chave forem necessárias para refinar a lista. O exemplo a seguir procura campanhas com `evergreen`, `ROI` e `Meta` no nome:

     ![Pesquisa por palavra-chave](/help/assets/insights-select-campaigns-keywords.png "Insira palavras-chave para pesquisar nomes de campanha"){width=500}

   - Você pode adicionar outro conjunto de palavras-chave para ampliar sua pesquisa. Usar vários conjuntos de palavras-chave permite incluir campanhas que correspondem ao primeiro conjunto de palavras-chave ou ao segundo conjunto de palavras-chave. Por exemplo, você pode pesquisar campanhas rotuladas `evergreen` e `web` _OU_ campanhas rotuladas `photoshop` e `roi`:

     ![Pesquisar com vários conjuntos de palavras-chave](/help/assets/insights-advanced-or.png "Pesquisar nomes de campanha usando vários conjuntos de palavras-chave"){width=500}

1. Selecione uma ou mais campanhas da pesquisa resultante e clique em **[!UICONTROL Aplicar]**.

   ![Lista de campanhas](/help/assets/insights-select-campaigns-list.png "Selecionar campanhas a serem incluídas")

As campanhas selecionadas agora aparecem na lista _[!UICONTROL Filtrar por]_ acima da tabela de anúncios ou galeria. Você pode se concentrar exclusivamente nos anúncios vinculados às campanhas escolhidas. Neste exemplo, os resultados filtrados incluem 28 anúncios, fornecendo uma visualização mais direcionada para análise.

![Tabela filtrada por campanhas](/help/assets/insights-filter-by-campaigns.png "Tabela com filtro de campanhas"){zoomable="yes"}

Você pode filtrar ainda mais a tabela [!UICONTROL Mídia] de maneira semelhante para nomes de anúncios. Expanda o filtro **[!UICONTROL Anúncios]**, clique em **[!UICONTROL Selecionar]** e você poderá executar um filtro de palavra-chave semelhante para refinar sua exibição de tabela de mídia ou galeria.

## Baixar resultados da tabela

Você pode baixar os resultados filtrados da exibição de tabela para análise ou compartilhamento adicional. Clique no ícone de download (seta apontando para baixo) acima do lado direito da tabela para baixar um arquivo CSV com base na tabela visualizável. O download é iniciado automaticamente e coloca o arquivo CSV no local de download padrão.

Algumas tabelas podem ter várias páginas, que podem ser vistas abaixo do lado direito da tabela. O arquivo CSV inclui dados de _todas_ páginas da tabela.
