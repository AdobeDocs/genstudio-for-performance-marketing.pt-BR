---
title: Visão geral da mídia
description: Saiba como avaliar o desempenho da mídia no Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Media Performance, Content Attributes
exl-id: 1e93422b-2645-4e29-a216-fc1008afbfc7
source-git-commit: facc38b8afe8104e27a89ac3d9ec40d1209229a9
workflow-type: tm+mt
source-wordcount: '645'
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

{{filter-table}}

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
| **[!UICONTROL CTR &#x200B;]**<br>_Taxa de cliques_ | Porcentagem (%) de impressões que resultaram em cliques de mídia em um anúncio.<br>**Cálculo**: `clicks` dividido por `impressions` | Uma alta taxa de cliques indica que a mídia é altamente relevante e envolvente para o público-alvo. Ela sugere que as mensagens e o design estão capturando efetivamente o interesse do público e solicitando que eles tomem uma ação. Além disso, um CTR alto pode significar que a mídia é bem direcionada e reflete no público-alvo desejado, resultando em um melhor desempenho geral da campanha. |
| **[!UICONTROL CPM &#x200B;]**<br>_Custo por mil_ | O custo médio para cada mil impressões de mídia.<br>**Cálculo**: valor total `spent` dividido pelo número de impressões e multiplicado por 1000 | Um valor baixo de CPM pode indicar um desempenho de mídia econômico, especialmente quando combinado a uma alta taxa de cliques. |
| **[!UICONTROL CPA &#x200B;]**<br>_Custo por Ação_ | Custo médio gasto para realizar uma ação específica do cliente, como uma compra ou assinatura.<br>**Cálculo**: valor total `spent` dividido pelo número de ações de clientes concluídas | Ajuda a identificar a mídia que resulta em ações valiosas do cliente. |
| **[!UICONTROL CPC &#x200B;]**<br>_Custo por clique_ | Custo médio associado a cada clique na mídia.<br>**Cálculo**: valor total `spent` dividido por `clicks` | Custos médios mais baixos podem indicar anúncios e gastos econômicos, especialmente quando comparados a um aumento nas conversões. |
| **[!UICONTROL Gastar]** | O valor gasto com o orçamento relacionado a mídia individual durante um determinado período de tempo. | Um alto valor de gasto em um curto período pode indicar uso rápido, o que pode levar ao esgotamento antecipado de recursos. Acompanhe o valor gasto em relação às principais métricas de desempenho para ajudar a monitorar o retorno geral sobre o investimento. |
| **[!UICONTROL Usado nestes anúncios]** | O número de anúncios que usam essa mídia. | |
| **Atributos** | Lista de recursos inerentes presentes nesta mídia. | Os atributos ajudam a identificar elementos criativos que mais refletem em seu público-alvo. |
