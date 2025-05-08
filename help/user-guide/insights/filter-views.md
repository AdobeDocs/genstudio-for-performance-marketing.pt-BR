---
title: Filtrar visualizações do Insights
description: Saiba como usar os recursos aprimorados de filtro com Insights.
level: Intermediate
feature: Reporting and Insights
exl-id: fbc53c2a-388c-4b51-94e2-626cd1e18e63
source-git-commit: 04bc6f911394d0f4c324abc347ce125203011960
workflow-type: tm+mt
source-wordcount: '868'
ht-degree: 0%

---

# Filtro para visualizações de Insights

O painel [!DNL Insights] fornece um conjunto abrangente de filtros para uma experiência eficiente de exploração de dados. Ao analisar canais, anúncios, mídia ou atributos específicos, as opções de filtro permitem personalizar sua visualização e simplificar seu fluxo de trabalho. Use filtros de palavra-chave para direcionamento preciso ou explore listas predefinidas para refinar sua pesquisa e se concentrar nos dados mais importantes.

## Noções básicas de filtro

Cada modo de exibição em [!DNL Insights] oferece uma lista de opções de filtro. O botão de alternância de filtro (funil) à esquerda abre o menu **[!UICONTROL Filtro]**. Se você estiver visualizando a tabela ou a galeria, os filtros aplicados aparecerão na lista **[!UICONTROL Filtrar por]** acima da tabela ou galeria. Por padrão, um canal e uma conta são selecionados.

![Filtrar por](/help/assets/insights-filter-by.png "Filtrar por"){width=600 zoomable="yes"}

Os filtros aplicados persistem em todas as exibições. Selecione **[!UICONTROL Limpar tudo]** acima da tabela ou galeria para remover todos os filtros selecionados.

### Campo de pesquisa

Clique no ícone de pesquisa (lupa) para digitar um termo de pesquisa para localizar itens específicos na tabela ou galeria. Por exemplo, inserir o termo `Gear` na tabela [!UICONTROL Anúncios] filtra os resultados para exibir somente anúncios usando o termo `Gear` no nome.

![Pesquisar exemplo de campo](/help/assets/insights-search.png "Pesquisar anúncios com engrenagem no nome"){width=600 zoomable="yes"}

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

Com o tempo, sua lista de campanhas e anúncios pode crescer exponencialmente. Considere o seguinte cenário para usar o filtro _[!UICONTROL Campanhas]_ para refinar a tabela [!UICONTROL Anúncios].

**Para refinar a tabela Anúncios usando o filtro Campanhas**:

1. Em _[!DNL Insights]_, selecione a exibição **[!UICONTROL Anúncios]**.

   ![Filtro de anúncios e tabela](/help/assets/insights-ads-filter.png "Exibição de anúncios com menu de filtro"){zoomable="yes"}

1. Clique na opção de filtro (funil) acima do lado esquerdo da tabela para abrir o menu **[!UICONTROL Filtro]**.

1. Verifique se o canal `Filter by` e a conta corretos estão selecionados.

1. Expanda o filtro **[!UICONTROL Campanhas]** e clique em **[!UICONTROL Selecionar]**.

   ![Filtrar campanhas](/help/assets/insights-filter-campaigns-expand.png "Expandir filtro de campanhas"){width=200}

1. No campo de pesquisa _[!UICONTROL Selecionar campanhas]_, insira palavras-chave separadas por vírgulas.

   Use palavras-chave para refinar sua pesquisa com filtragem lógica e precisa.

   - Para localizar nomes de campanha que contenham `adventure` **AND** `ready`, insira as duas palavras-chave separadas por vírgula:

     ![Pesquisar todas as palavras-chave](/help/assets/insights-select-campaigns-and.png "Pesquisar nomes de campanha que contenham ambas as palavras-chave"){width=500}

   - Para localizar nomes de campanha que contenham `adventure` **OU** `ready`, insira cada palavra-chave separadamente:

     ![Pesquise por palavras-chave](/help/assets/insights-select-campaigns-or.png "Pesquise nomes de campanha que contenham pelo menos uma palavra-chave"){width=500}

   - Para realizar pesquisas avançadas, combine vários conjuntos de palavras-chave. Por exemplo, pesquise nomes de campanha com `adventure` e `apparel` **OU** `sun` e `gear`:

     ![Pesquisar com vários conjuntos de palavras-chave](/help/assets/insights-advanced-or.png "Pesquisar nomes de campanha usando vários conjuntos de palavras-chave"){width=500}

1. Selecione uma ou mais campanhas da pesquisa resultante e clique em **[!UICONTROL Aplicar]**.

   ![Lista de campanhas](/help/assets/insights-select-campaigns-list.png "Selecionar campanhas a serem incluídas")

As campanhas selecionadas agora aparecem na lista _[!UICONTROL Filtrar por]_ acima da tabela de anúncios ou galeria. Você pode se concentrar exclusivamente nos anúncios vinculados às campanhas escolhidas. Neste exemplo, os resultados filtrados incluem 6 anúncios, fornecendo uma visualização mais direcionada para análise.

![Tabela filtrada por campanhas](/help/assets/insights-filter-by-campaigns.png "Tabela com filtro de campanhas"){zoomable="yes"}

Você pode filtrar ainda mais a tabela [!UICONTROL Mídia] de maneira semelhante para nomes de anúncios. Expanda o filtro **[!UICONTROL Anúncios]**, clique em **[!UICONTROL Selecionar]** e você poderá executar um filtro de palavra-chave semelhante para refinar sua exibição de tabela de mídia ou galeria.

## Baixar resultados da tabela

Você pode baixar os resultados filtrados da exibição de tabela para análise ou compartilhamento adicional. Clique no ícone de download (seta apontando para baixo) acima do lado direito da tabela para baixar um arquivo CSV com base na tabela visualizável. O download é iniciado automaticamente e coloca o arquivo CSV no local de download padrão.

Algumas tabelas podem ter várias páginas, que podem ser vistas abaixo do lado direito da tabela. O arquivo CSV inclui dados de _todas_ páginas da tabela.
