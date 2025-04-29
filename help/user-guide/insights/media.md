---
title: Visão geral da mídia
description: Saiba como avaliar o desempenho da mídia no Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Media Performance, Content Attributes
exl-id: 1e93422b-2645-4e29-a216-fc1008afbfc7
source-git-commit: 817a7bf425732cefd57da55e6bb41154567bca46
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# Visão geral da mídia

A exibição [!DNL Insights] _[!UICONTROL Mídia]_ mostra uma lista de mídias usadas em anúncios e campanhas publicitárias para a conta selecionada. A _Mídia_ representa uma imagem, vídeo, texto ou outro conteúdo criativo aprovado para uso em suas iniciativas de marketing.

{{connect-insights}}

A tabela _[!UICONTROL Mídia]_ é organizada com a **[!UICONTROL ID de Mídia]**. Você pode alternar entre as exibições usando o ícone lista de exibições (tabela) e o ícone exibição de galeria (grade). Clique no ícone de configurações (cog) acima do lado direito da tabela para alternar as colunas visualizáveis.

![Filtro de mídia e tabela](/help/assets/insights-media-filter.png){zoomable="yes"}

A exibição de galeria _[!UICONTROL Mídia]_ mostra uma intercalação de visualizações de mídia e uma métrica, como taxa de cliques. Clique no ícone de configurações (cog) acima do lado direito da galeria para abrir **[!UICONTROL Configurações de cartão]** e alternar uma das três métricas visualizáveis:

- CPA (Custo por ação)
- CTR (taxa de cliques)
- CPC (Custo por clique)
- Gastos

{{empty-table}}

## Filtrar mídia

O ícone de filtro (funil) acima do lado esquerdo abre o menu **[!UICONTROL Filtro]**, onde você pode selecionar em várias listas. Selecione **[!UICONTROL Limpar tudo]** acima da tabela de anúncios ou galeria para remover todos os filtros selecionados.

Com alguns filtros, você pode aproveitar palavras-chave precisas para refinar a lista de critérios. Os filtros de palavra-chave são particularmente úteis para campanhas e anúncios que seguem uma convenção de nomenclatura complexa com vários identificadores exclusivos, como os seguintes:

- Nome ou código de região específico: `NA`, `EMEA`
- Acrônimos de tipo de conteúdo: `EB`, `CHT` ou `DSP`
- Códigos de oferta ou acrônimos: `OFFER2023`, `PROMO`

**Para filtrar por campanhas**:

1. Expanda o filtro **[!UICONTROL Campanhas]** e clique em **[!UICONTROL Selecionar]**.
1. No campo de pesquisa, digite palavras-chave separadas por vírgulas.

   Use quantas palavras-chave forem necessárias para refinar a lista:

   ![Selecionar campanhas](/help/assets/insights-select-campaign.png){width=400}

1. Selecione uma ou mais campanhas da pesquisa resultante e clique em **[!UICONTROL Aplicar]**.

   As campanhas selecionadas agora aparecem na lista _[!UICONTROL Filtrar por]_ acima da tabela ou galeria de anúncios, permitindo que você se concentre na mídia associada às campanhas selecionadas.

1. _Opcional_: para filtrar ainda mais a mídia, execute um filtro de palavra-chave semelhante em **[!UICONTROL Anúncios]**.

>[!NOTE]
>
>O filtro aplicado persiste em todas as exibições em [!DNL Insights]. Selecione **[!UICONTROL Limpar tudo]** acima da tabela de anúncios ou galeria para remover todos os filtros selecionados.

### Baixar resultados da tabela

{{$include /help/_includes/download-insights.md}}

## Detalhes da mídia

Na exibição _Detalhes da mídia_, você pode ver quais anúncios usam a mídia selecionada. Os detalhes incluem desempenho total da mídia, Anúncios usando a mídia, atributos definidos pelo usuário e recursos detectados pela IA associados à mídia.

![Detalhes da mídia](/help/assets/insights-media-details.png){zoomable="yes"}

### Atributos de mídia

{{$include /help/_includes/generated-attributes.md}}

## Desempenho da mídia

As métricas de insights podem ajudar a avaliar quais mídias contribuem para o sucesso de uma campanha e quais atributos de mídia são mais eficazes.

A tabela a seguir fornece definições e insights para as métricas principais de marketing digital na exibição de tabela [!UICONTROL Mídia]. Cada métrica inclui uma breve definição, pois se relaciona à mídia, como a métrica é calculada e um ou mais insights para ajudar a entender sua importância e impacto.

| Métrica | Definição | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL ID de Mídia]** | O nome associado a uma imagem, vídeo, texto ou outro conteúdo criativo. | Classifique a tabela clicando no cabeçalho da coluna para qualquer uma das métricas principais. |
| **[!UICONTROL Impressões]** | Uma contagem de cada vez que a mídia é carregada no canal, independentemente da interação ou da visualização. | Uma contagem de alta impressão pode indicar ampla visibilidade, mas, para um verdadeiro desempenho do insight, considere-a em relação a outras métricas de envolvimento. |
| **[!UICONTROL Cliques]** | O número de vezes que os usuários interagem com um elemento clicável, como um link, na mídia. | Uma alta contagem de cliques indica forte interesse e envolvimento com o conteúdo, que pode ser eficaz e alcançar o público-alvo correto. |
| **[!UICONTROL CTR ]**<br>_Taxa de cliques_ | Porcentagem (%) de impressões que resultaram em cliques de mídia em um anúncio.<br>**Cálculo**: `clicks` dividido por `impressions` | Uma alta taxa de cliques indica que a mídia é altamente relevante e envolvente para o público-alvo. Ela sugere que as mensagens e o design estão capturando efetivamente o interesse do público e solicitando que eles tomem uma ação. Além disso, um CTR alto pode significar que a mídia é bem direcionada e reflete no público-alvo desejado, resultando em um melhor desempenho geral da campanha. |
| **[!UICONTROL CPM ]**<br>_Custo por mil_ | O custo médio para cada mil impressões de mídia.<br>**Cálculo**: valor total `spent` dividido pelo número de impressões e multiplicado por 1000 | Um valor baixo de CPM pode indicar um desempenho de mídia econômico, especialmente quando combinado a uma alta taxa de cliques. |
| **[!UICONTROL CPA ]**<br>_Custo por Ação_ | Custo médio gasto para realizar uma ação específica do cliente, como uma compra ou assinatura.<br>**Cálculo**: valor total `spent` dividido pelo número de ações de clientes concluídas | Ajuda a identificar a mídia que resulta em ações valiosas do cliente. |
| **[!UICONTROL CPC ]**<br>_Custo por clique_ | Custo médio associado a cada clique na mídia.<br>**Cálculo**: valor total `spent` dividido por `clicks` | Custos médios mais baixos podem indicar anúncios e gastos econômicos, especialmente quando comparados a um aumento nas conversões. |
| **[!UICONTROL Gastar]** | O valor gasto com o orçamento relacionado a mídia individual durante um determinado período de tempo. | Um alto valor de gasto em um curto período pode indicar uso rápido, o que pode levar ao esgotamento antecipado de recursos. Acompanhe o valor gasto em relação às principais métricas de desempenho para ajudar a monitorar o retorno geral sobre o investimento. |
| **[!UICONTROL Usado nestes anúncios]** | O número de anúncios que usam essa mídia. | |
| **Atributos** | Lista de recursos inerentes presentes nesta mídia. | Os atributos ajudam a identificar elementos criativos que mais refletem em seu público-alvo. |
