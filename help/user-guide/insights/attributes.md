---
title: Visão geral dos atributos
description: Saiba como avaliar o desempenho de atributos específicos no Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Content Attributes, Content Performance
exl-id: 9d05c128-50d5-415a-ae60-7023c36c06ad
source-git-commit: facc38b8afe8104e27a89ac3d9ec40d1209229a9
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Visão geral dos atributos

A exibição [!DNL Insights] _[!UICONTROL Atributos]_ mostra uma lista de atributos usados em campanhas de publicidade para a conta de canal selecionada.

{{connect-insights}}

A tabela _[!UICONTROL Atributos]_ é organizada com o nome [!UICONTROL Atributo]. Você pode alternar entre os tipos de lista usando os botões **[!UICONTROL Imagens]** e **[!UICONTROL Vídeo]**. Clique no ícone de configurações (cog) acima do lado direito da tabela para alternar as colunas visualizáveis.

![Filtro e tabela de atributos](/help/assets/insights-attributes-filter.png){zoomable="yes"}

{{filter-table}}

## Detalhes do atributo

Os atributos ajudam a identificar [anúncios](ads.md#ad-details) e [mídia](media.md#media-details) por seus detalhes inerentes, como cor, composição, elementos visuais e outras propriedades.

Na visualização de detalhes do atributo, é possível ver quais anúncios usam o atributo selecionado. Os detalhes incluem o desempenho total do atributo e uma análise das métricas de desempenho relacionadas a cada anúncio.

![Atribuir métricas de desempenho](/help/assets/insights-attribute-details.png){zoomable="yes"}

O GenStudio for Performance Marketing detecta determinados recursos e aplica o atributo apropriado ao conteúdo de mídia ou anúncio como uma tag. Consulte [Categorias](#categories) para ver exemplos dessas marcas. Para ver todos os atributos associados a um anúncio, clique no ícone de configurações (cog) acima do lado direito da tabela para selecionar a coluna **[!UICONTROL Atributos]**.

## Categorias

Um atributo _categoria_ é um grupo de classificação que organiza atributos relacionados que compartilham uma característica comum. Essas categorias ajudam a simplificar a descoberta, a identificação e a compreensão de atributos específicos, fornecendo maior contexto e facilitando sua aplicação e uso.

O GenStudio for Performance Marketing usa os recursos de IA e aprendizado de máquina do Adobe para estudar [imagens](image-features.md), [vídeos](video-features.md) e [texto](text-features.md) e aplicar atributos a anúncios e mídia com base em uma probabilidade de correção.

A lista de atributos detectados para anúncios e conteúdo de mídia não é exaustiva. O conteúdo que contém um conjunto avançado de recursos pode ser limitado aos três recursos mais dominantes identificados pela IA. Por exemplo, a ilustração a seguir contém vários atributos de imagem detectados, incluindo vários objetos, cores do primeiro plano e do plano de fundo:

![atributos de imagem](/help/assets/category/asset-attributes.png "A imagem de Toucan inclui vários atributos detectados"){width="300" zoomable="yes"}

>[!INFO]
>
>Não é possível editar tags detectadas e aplicadas automaticamente.

## Desempenho do atributo

As métricas de Insights podem ajudar você a avaliar quais atributos inspiram mais engajamento do cliente.

A tabela a seguir fornece definições e insights para as métricas principais de marketing digital na exibição de tabela [!UICONTROL Atributos]. Cada métrica inclui uma breve definição, pois se relaciona a atributos, como a métrica é calculada e um ou mais insights para ajudar a entender sua importância e impacto em uma campanha publicitária.

| Métrica | Definição | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Atributo]** | O nome do atributo. | Classifique a tabela clicando no cabeçalho da coluna para qualquer uma das métricas principais. |
| **[!UICONTROL Categoria]** | A [categoria](#categories) que representa a qualidade inerente de um atributo. |  |
| **[!UICONTROL # de imagens]** | O número de imagens que têm este atributo. | A contagem na tabela Atributos pode ser diferente da contagem na exibição Detalhes do atributo. Essa discrepância pode ocorrer se a origem do canal, como Meta e GenStudio, usar cálculos de resumo ligeiramente diferentes. |
| **[!UICONTROL # de vídeos]** | O número de vídeos com este atributo. | A contagem na tabela Atributos pode ser diferente da contagem na exibição Detalhes do atributo. Essa discrepância pode ocorrer se a origem do canal, como Meta e GenStudio, usar cálculos de resumo ligeiramente diferentes. |
| **[!UICONTROL Impressões]** | Uma contagem de cada vez que uma imagem ou vídeos com esse atributo são carregados no canal, independentemente da interação ou da visualização. | Uma contagem de alta impressão pode indicar ampla visibilidade, mas, para um verdadeiro desempenho do insight, considere-a em relação a outras métricas de envolvimento. |
| **[!UICONTROL Cliques]** | O número de vezes que os usuários interagem com uma imagem ou vídeo com esse atributo. | Uma alta contagem de cliques indica forte interesse e envolvimento com o conteúdo, que pode ser eficaz e alcançar o público-alvo correto. |
| **[!UICONTROL CTR &#x200B;]**<br>_Taxa de cliques_ | Porcentagem (%) de impressões que resultaram em cliques em imagens ou vídeos com esse atributo.<br>**Cálculo**: `clicks` dividido por `impressions` | Uma alta taxa de cliques indica que o conteúdo é altamente relevante e motivador para o público-alvo nas mensagens e no design e está efetivamente direcionando os interesses do público-alvo. |
| **[!UICONTROL CPM &#x200B;]**<br>_Custo por mil_ | Custo para cada mil impressões de anúncios de uma imagem ou vídeo com esse atributo.<br>**Cálculo**: valor total `spent` dividido pelo alcance, então multiplicado por 1000 | Um valor baixo pode indicar visibilidade com boa relação custo-benefício, especialmente quando combinado a uma alta taxa de cliques. |
| **[!UICONTROL CPA &#x200B;]**<br>_Custo por Ação_ | Custo médio gasto para realizar uma ação específica do cliente, como uma compra ou assinatura.<br>**Cálculo**: valor total `spent` dividido pelo número de ações de clientes concluídas | Ajuda a identificar atributos que resultam em ações valiosas do cliente. |
| **[!UICONTROL CPC &#x200B;]**<br>_Custo por clique_ | Custo médio associado a cada clique em imagens ou vídeos com este atributo.<br>**Cálculo**: valor total `spent` dividido por `clicks` | Custos médios mais baixos podem indicar anúncios e gastos econômicos, especialmente quando comparados a um aumento nas conversões. |
| **[!UICONTROL Gastar]** | O valor gasto com o orçamento em relação aos atributos em um determinado período. | Um alto valor de gasto em um curto período pode indicar uso rápido, o que pode levar ao esgotamento antecipado de recursos. Acompanhe o valor gasto em relação às principais métricas de desempenho para ajudar a monitorar o retorno geral sobre o investimento. |
