---
title: Visão geral dos atributos
description: Saiba como avaliar o desempenho de atributos específicos no Adobe GenStudio for Performance Marketing.
feature: Insights, Assets
source-git-commit: 87a8833549569aaeaa60f5760b4e9a8b710a6033
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Visão geral dos atributos

A exibição [!DNL Insights] _[!UICONTROL Atributos]_ mostra uma lista de atributos usados em campanhas de publicidade para a conta de canal selecionada.

A tabela _[!UICONTROL Atributos]_ é organizada com o nome [!UICONTROL Atributo]. Você pode alternar entre os tipos de lista usando os botões **[!UICONTROL Imagens]** e **[!UICONTROL Vídeo]**. Clique no ícone de configurações (cog) acima do lado direito da tabela para alternar as colunas visualizáveis.

O ícone de filtro (funil) acima do lado esquerdo da tabela abre o menu **[!UICONTROL Filtro]**, no qual você pode selecionar da [!UICONTROL Conta] e da [!UICONTROL Categoria de atributo] para filtrar os atributos na tabela. O exemplo a seguir mostra uma lista de atributos na categoria `Lighting Condition`.

![Filtro e tabela de atributos](/help/assets/insights-attributes-filter.png){zoomable="yes"}

## Detalhes do atributo

Os atributos ajudam a identificar ativos por seus detalhes inerentes, como cor, composição, elementos visuais e outras propriedades.

Na visualização de detalhes do atributo, você pode ver quais experiências usam o atributo selecionado. Os detalhes incluem o desempenho total do atributo e um detalhamento das métricas de desempenho relacionadas a cada experiência.

![Atribuir métricas de desempenho](/help/assets/insights-attribute-details.png){zoomable="yes"}

O GenStudio for Performance Marketing detecta determinados recursos e aplica o atributo apropriado a um ativo ou experiência como uma tag. Consulte [Categorias](#categories) para ver exemplos dessas marcas. Para ver todos os atributos associados a uma experiência, clique no ícone de configurações (cog) acima do lado direito da tabela para selecionar a coluna **[!UICONTROL Atributos]**.

## Categorias

A GenStudio for Performance Marketing reconhece determinados recursos de imagens, vídeos e texto e aplica uma tag de recurso ao ativo. Uma _categoria_ é um conjunto de recursos que compartilham uma característica específica. Um exemplo de valor de _orientação da imagem_ é `landscape`.

Os atributos detectados e aplicados automaticamente não podem ser editados.

<!--
Select any of the following to open a detailed list of feature categories:

+++**Image features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Background Colors      | 14 colors |
| Camera Position        | - `low angle`, `high angle`, `dutch angle`<br>- `overhead view`, `eye level`,`bird's eye view` |
| Camera Proximity       | `close up`, `mid shot`, `long shot` |
| Camera Setting         | - `fast shutter speed`, `long exposure`, `double exposure`<br>- `normal mode`, `flash`, `macro`, `wide-angle`<br>- `black and white`, `surreal`<br>- `bokeh blur`, `motion blur`, `tilt-shift blur` |
| Foreground Colors      | 14 colors |
| Image Type             | `photograph`, `sketch`, `painting`, `digital cartoon`, `infographics`, `graphic design`, `collage`, `screenshot` |
| Lighting Condition     | golden hour, blue hour, midday, overcast, night, high-key, low-key, daylight, incandescent, fluorescent, colorful, studio |
| Objects                | The items, entities, and elements that are visible, such as `lighthouse`, `orchid`, or `tunnel`. |
| Orientation            | Examples: `landscape`, `portrait`, `square` |
| Overall Tone           | `warm`, `cool`, `neutral` |
| People Categories      | Examples: `person`, `social group`, `people`, `kid` |
| Photography Styles     | `aerial photography`, `aerial photography`, `architectural photography`, `astrophotography`, `black and white photography`, `business photography`, `cityscape photography`, `commercial photography`, `composite photography`, `creative photography`, `editorial photography`, `event photography`, `family photography`, `fashion photography`, `fine art photography`, `food photography`, `holiday photography`, `indoor photography`, `landscape photography`, `lifestyle photography`, `macro photography`, `minimalist photography`, `night photography`, `outdoor photography`, `pet photography`, `portrait photography`, `product photography`, `real estate photography`, `seascape photography`, `sports photography`, `still-life photography`, `street photography`, `travel photography`, `underwater photography`, `wildlife photography` |
| Scenes                 | Examples: `city`, `island`, `living room` |
| Tags                   | Examples: `gaming`, `law`, `yoga` |
| Visual Attention Spread| The level of viewer attention spread across an image: `high`, `low` |
| Visual Content Density | The amount of information or detail in an image: `high`, `low` |

+++

+++**Video features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Audio Genre  | |
| Audio Genre Category  | |
| Audio Mood  | |
| Audio Types| |
| Objects  | |
| Orientation  | |
| People Categories  | |
| Scenes  | |
| Styles  | |
| Tags   | |
| Video Category  | |
| Video Type  | |

+++

+++**Text features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Emojis Count  | |
| HashTags Count  | |
| Keywords  | |
| Marketing Emotions  | |
| Narratives  |  |
| Persuasion Strategies  |  |
| Readability  | |
| Sentences Count  | |
| Stop Words Ratio  | |
| Text Quotes Count  | |
| Tones  | |
| Words Count  | |
| Words Count Per Sentence  | |

+++

-->

## Métricas de atributo

As métricas de Insights podem ajudar você a avaliar quais atributos inspiram mais engajamento do cliente.

### Detalhes das métricas

A tabela a seguir fornece definições e insights para as métricas principais de marketing digital na exibição de tabela [!UICONTROL Atributos]. Cada métrica inclui uma breve definição, pois se relaciona a um ativo, como a métrica é calculada, e um ou mais insights para ajudar a entender sua importância e impacto em uma campanha publicitária.

| Métrica | Definição | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Atributo]** | O nome do atributo. | Classifique a tabela clicando no cabeçalho da coluna para qualquer uma das métricas principais. |
| **[!UICONTROL Categoria]** | A [categoria](#categories) que representa a qualidade inerente de um atributo. |  |
| **[!UICONTROL # de imagens]** | Uma contagem de imagens com este atributo. |  |
| **[!UICONTROL # de vídeos]** | Uma contagem de vídeos com este atributo. |  |
| **[!UICONTROL Impressões]** | Uma contagem de cada vez que uma imagem ou vídeos com esse atributo são carregados no canal, independentemente da interação ou da visualização. | Uma contagem de alta impressão pode indicar ampla visibilidade, mas, para obter um verdadeiro insight sobre o desempenho, considere com outras métricas de envolvimento. |
| **[!UICONTROL Cliques]** | Número de vezes que os usuários interagem com uma imagem ou vídeo com esse atributo. | Uma alta contagem de cliques indica forte interesse e envolvimento com o conteúdo, que pode ser eficaz e alcançar o público-alvo correto. |
| **[!UICONTROL CTR ]**<br>_Taxa de cliques_ | Porcentagem (%) de impressões que resultaram em cliques em imagens ou vídeos com esse atributo.<br>**Cálculo**: `clicks` dividido por `impressions` | Uma alta taxa de cliques indica que o conteúdo é altamente relevante e motivador para o público-alvo nas mensagens e no design e está efetivamente direcionando os interesses do público-alvo. |
| **[!UICONTROL CPM ]**<br>_Custo por mil_ | Custo ($) para cada mil impressões de anúncios de uma imagem ou vídeo com esse atributo.<br>**Cálculo**: valor total `spent` dividido pelo alcance, então multiplicado por 1000 | Um valor baixo pode indicar visibilidade com boa relação custo-benefício, especialmente quando combinado a uma alta taxa de cliques. |
| **[!UICONTROL CPA ]**<br>_Custo por Ação_ | Custo médio ($) gasto para realizar uma ação específica do cliente, como uma compra ou assinatura.<br>**Cálculo**: valor total `spent` dividido pelo número de ações de clientes concluídas | Ajuda a identificar atributos que resultam em ações valiosas do cliente. |
| **[!UICONTROL CPC ]**<br>_Custo por clique_ | Custo médio ($) associado a cada clique em imagens ou vídeos com este atributo.<br>**Cálculo**: valor total `spent` dividido por `clicks` | Custos médios mais baixos podem indicar anúncios e gastos econômicos, especialmente quando comparados a um aumento nas conversões. |
| **[!UICONTROL Gastar]** | O valor ($) gasto com o orçamento relacionado aos atributos em um determinado período. | Um alto valor de gasto em um curto período pode indicar uso rápido, o que pode levar ao esgotamento antecipado de recursos. Acompanhe o valor dos gastos em relação às principais métricas de desempenho para ajudar a monitorar o retorno geral sobre o investimento. |
