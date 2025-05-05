---
title: Visão geral de anúncios e posicionamento de anúncios
description: Consulte uma visão geral do envolvimento do cliente, orçamento e despesas para desempenho de anúncios e disposição de anúncios no Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Ad Performance, Text Attributes, Reporting and Insights
exl-id: e3827b1a-53d0-465c-8125-15b0e298ef3a
source-git-commit: e053c91ebb40a9625ce22281a89feaa9cccab956
workflow-type: tm+mt
source-wordcount: '1536'
ht-degree: 0%

---

# Visão geral de anúncios e posicionamento de anúncios

A exibição [!DNL Insights] _[!UICONTROL Anúncios]_ mostra uma lista de anúncios para a conta de anúncio do canal conectado. Um _anúncio_ é um ativo promocional que inclui conteúdo visual e interativo destinado à distribuição para um público específico como parte de uma campanha de marketing.

{{connect-insights}}

A tabela _[!UICONTROL Anúncios]_ é organizada com o uso de [!UICONTROL Nomes de anúncios]. Clique no ícone de configurações (cog) acima do lado direito da tabela para alternar as colunas visualizáveis.

![Filtro de anúncios e tabela](/help/assets/insights-ads-filter.png){zoomable="yes"}

A exibição de galeria _[!UICONTROL Anúncio]_ mostra uma colagem de visualizações de anúncios e uma métrica, como taxa de cliques. Clique no ícone de configurações (cog) acima do lado direito da galeria para abrir **[!UICONTROL Configurações de cartão]** e alternar uma das três métricas visualizáveis:

- CPA (Custo por ação)
- CTR (taxa de cliques)
- CPC (Custo por clique)
- Gastos

{{empty-table}}

## Filtrar anúncios

O ícone de filtro (funil) acima do lado esquerdo abre o menu **[!UICONTROL Filtro]**, onde você pode selecionar em várias listas. Com alguns filtros, você pode aproveitar palavras-chave precisas para refinar a lista de critérios. Os filtros de palavra-chave são particularmente úteis para campanhas que seguem uma convenção de nomenclatura complexa com vários identificadores exclusivos, como os seguintes:

- Nome ou código de região específico: `NA`, `EMEA`
- Acrônimos de tipo de conteúdo: `EB`, `CHT` ou `DSP`
- Códigos de oferta ou acrônimos: `OFFER2023`, `PROMO`

**Para filtrar por campanhas**:

1. Expanda o filtro **[!UICONTROL Campanhas]** e clique em **[!UICONTROL Selecionar]**.
1. No campo de pesquisa, digite palavras-chave separadas por vírgulas.

   Use quantas palavras-chave forem necessárias para refinar a lista:

   ![Selecionar campanhas](/help/assets/insights-select-campaign.png){width=400}

1. Selecione uma ou mais campanhas da pesquisa resultante e clique em **[!UICONTROL Aplicar]**.

   As campanhas selecionadas agora aparecem na lista _[!UICONTROL Filtrar por]_ acima da tabela ou galeria de anúncios, permitindo que você se concentre nos anúncios associados às campanhas selecionadas.

>[!NOTE]
>
>O filtro aplicado persiste em todas as exibições em [!DNL Insights]. Selecione **[!UICONTROL Limpar tudo]** acima da tabela de anúncios ou galeria para remover todos os filtros selecionados.

### Baixar resultados da tabela

{{$include /help/_includes/download-insights.md}}

## Detalhes do anúncio

Selecione um anúncio e visualize as métricas de desempenho, os atributos de texto e os posicionamentos associados a cada anúncio. A _[!UICONTROL Página de detalhes do anúncio]_ inclui métricas para o anúncio `click-through rate`, `cost per action` e `spend`—quanto do orçamento foi gasto no anúncio. Como os anúncios podem ter vários posicionamentos, como um feed ou um banner, você pode ver um detalhamento das mesmas métricas para cada posicionamento de anúncio. Use as setas para a esquerda e para a direita em **[!UICONTROL Desempenho por posicionamento de anúncio]** para percorrer as métricas de posicionamento.

![Detalhes do anúncio com métricas e posicionamentos de anúncios](/help/assets/insights-ad-details.png){zoomable="yes"}

### Atributos do anúncio

Abaixo da visualização do anúncio há uma lista de atributos associados ao anúncio.

{{$include /help/_includes/generated-attributes.md}}

### Formatos de publicidade

Os formatos de anúncios se referem a vários elementos criativos e layouts usados para alinhar-se aos objetivos da campanha, engajar o público-alvo e ajudar a rastrear as métricas de desempenho.

[!DNL Insights] no GenStudio for Performance Marketing atualmente suporta os seguintes formatos de anúncios disponíveis.

| Compatível | Não compatível |
|-----------|-------------|
| Especificação do feed de ativos (otimização de posicionamento)<br>Imagem ou vídeo individual<br>Link | Carrossel<br>Colaborativo<br>Catálogo<br>Experiência Instantânea<br>Especificação do Feed de Ativos (além da otimização de posicionamento)<br>Chamada (imagem e vídeo)<br>Aplicativo (imagem e vídeo)<br>Mensagens<br>Lead (imagem e vídeo)<br>Apresentação de slides (vídeo)<br>Coleção (ativo de imagem e vídeo herói)<br>Loja (imagem e vídeo)<br>Foto ou vídeo de Publicação de Página, Publicação no Instagram<br>Conteúdo de Marca<br>Flexível<br>Catálogo+ de Vantagens |

### Posicionamentos de anúncios

Os posicionamentos de anúncios se referem a locais ou plataformas específicas em que seus anúncios aparecem em uma campanha. Esses posicionamentos determinam como e onde o público-alvo interage com o conteúdo. Os posicionamentos de anúncios ampliam o alcance do público, o que ajuda a maximizar a visibilidade, o engajamento e a eficácia geral da campanha.

Ao criar uma campanha com Meta ads, você pode ter selecionado onde executar seus anúncios com base no [objetivo](channels.md#objectives) da campanha.

Veja a seguir uma lista dos posicionamentos de anúncios compatíveis:

| Rede de público-alvo | Facebook/Meta \* | Instagram | Messenger |
|--------------------|--------------------|-------------------------|---------------------|
| Vídeo premiado | Feed<br>Feeds de vídeo<br>Histórias<br>Marketplace<br>Coluna direita<br>Sobreposição de bobinas<br>Vídeo em fluxo<br>Pesquisa<br>Feed de discoteca de negócios<br>Feed de perfil<br> | Histórias<br>Feed<br>Explorar<br>Bobinas<br>Explorar Página Inicial da grade<br>Feed do perfil<br>Pesquisa<br>Fluxo | Histórias<br>Caixa de entrada |

\* Consulte [Sobre posicionamentos de anúncios em Metatecnologias](https://www.facebook.com/business/help/407108559393196?id=369787570424415) na _Central de Ajuda do Meta Business_.

## Desempenho do anúncio

As métricas de Insights podem ajudar a avaliar quais anúncios contribuem para o sucesso de uma campanha e quais posicionamentos de anúncios são mais eficazes.

A tabela a seguir fornece definições e insights para as métricas principais de marketing digital na exibição de tabela [!UICONTROL Anúncios]. Cada métrica inclui uma breve definição, pois se relaciona a nomes de anúncios, como a métrica é calculada, e um ou mais insights para ajudar a entender sua importância e impacto em um anúncio.

| Métrica | Definição | Insight |
| ---------------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Nome do anúncio]** | Uma lista de anúncios para a conta de canal conectada. Filtre anúncios selecionando uma campanha. | Classifique a lista de anúncios clicando em qualquer uma das métricas principais. |
| **[!UICONTROL Campanha]** | Uma campanha é um conjunto de anúncios projetados para atingir um objetivo específico. | Ao filtrar a tabela Anúncios por campanha, as métricas de resumo de todos os anúncios da campanha podem ser diferentes da linha de resumo da campanha na exibição [!UICONTROL Canais]. Essa discrepância pode ocorrer se a origem do canal, como Meta e GenStudio, usar cálculos de resumo ligeiramente diferentes. |
| **[!UICONTROL Posicionamentos]** | Uma contagem de [posicionamentos](#ad-placements) de anúncios, locais em que um anúncio apareceu na campanha. | Os posicionamentos aumentam o alcance do público-alvo.<p>Anúncios que mostram zero posicionamento e mídia zero podem indicar um [tipo de anúncio sem suporte](#unsupported-placements).</p> |
| **[!UICONTROL Mídia]** | O número de ativos usados nos posicionamentos de anúncios e anúncios | A contagem na tabela Anúncios pode ser diferente da contagem na visualização Detalhes do anúncio. Essa discrepância pode ocorrer se a origem do canal, como Meta e GenStudio, usar cálculos de resumo ligeiramente diferentes. |
| **[!UICONTROL Impressões]** | Uma contagem de cada vez que o posicionamento do anúncio ou o anúncio é carregado no canal, independentemente da interação ou da visualização. | Uma contagem de alta impressão pode indicar ampla visibilidade, mas, para um verdadeiro desempenho do insight, considere-a em relação a outras métricas de envolvimento. |
| **[!UICONTROL Cliques]** | O número de vezes que os usuários interagem com um elemento clicável, como um link ou um botão do call-to-action, em um posicionamento de anúncio. | Uma alta contagem de cliques indica forte interesse e envolvimento com o conteúdo, que pode ser eficaz e alcançar o público-alvo correto. |
| **[!UICONTROL CTR &#x200B;]**<br>_Taxa de cliques_ | Porcentagem (%) de impressões que resultaram em cliques no anúncio em uma campanha.<br>**Cálculo**: `clicks` dividido por `impressions` | Uma alta taxa de cliques indica que o conteúdo é altamente relevante e motivador para o público-alvo nas mensagens e no design e está efetivamente direcionando os interesses do público-alvo. |
| **[!UICONTROL CPM &#x200B;]**<br>_Custo por mil_ | O custo médio para cada mil impressões de anúncios.<br>**Cálculo**: valor total `spent` dividido pelo alcance, então multiplicado por 1000 | Um valor baixo pode indicar visibilidade com boa relação custo-benefício, especialmente quando combinado a uma alta taxa de cliques. |
| **[!UICONTROL CPA &#x200B;]**<br>_Custo por Ação_ | O custo médio gasto para realizar uma ação específica do cliente, como uma compra ou assinatura.<br>**Cálculo**: valor total `spent` dividido pelo número de ações de clientes concluídas | Use para monitorar os gastos com anúncios que resultam em ações valiosas do cliente. |
| **[!UICONTROL CPC &#x200B;]**<br>_Custo por clique_ | O custo médio associado a cada clique em um posicionamento de anúncio.<br>**Cálculo**: valor total `spent` dividido por `clicks` | Custos médios mais baixos podem indicar anúncios e gastos econômicos, especialmente quando comparados a um aumento nas conversões. |
| **[!UICONTROL Gastar]** | O valor gasto com o orçamento da campanha durante um determinado período para fazer esse anúncio. | Um alto valor de gasto em um curto período pode indicar uso rápido, o que pode levar ao esgotamento antecipado de recursos. Acompanhe o valor gasto em relação às principais métricas de desempenho para ajudar a monitorar o retorno geral sobre o investimento. |
| **Atributos** | Lista de recursos inerentes presentes neste anúncio. | Os atributos ajudam a identificar elementos criativos que mais refletem em seu público-alvo. Consulte [Categorias](/help/user-guide/insights/attributes.md#categories). |

## Desempenho de posicionamento

Na exibição da _[!UICONTROL página de detalhes do anúncio]_, as três métricas principais refletem o desempenho geral do anúncio selecionado. No entanto, a seção _Desempenho por posicionamento_ mostra as métricas detalhadas para cada posicionamento de anúncio. Use as setas para a direita e para a esquerda para navegar pelos diferentes posicionamentos de anúncios.

A tabela a seguir fornece definições para as métricas de desempenho de posicionamento de anúncios:

| Métrica | Definição | Insight |
| ---------------------------- | ----------------------------- | --------------------------------- |
| **[!UICONTROL CTR &#x200B;]**<br>_Taxa de cliques_ | A porcentagem (%) de impressões para um único posicionamento de anúncio que resultou em cliques.<p>**Cálculo**:`clicks` dividido por `impressions`<p>Essa métrica ajuda a determinar a eficácia do posicionamento do anúncio em envolver o público-alvo. | Um CTR alto indica que o posicionamento do anúncio é relevante e atraente para o público-alvo, resultando em mais interações. |
| **[!UICONTROL CPA &#x200B;]**<br>_Custo por Ação_ | O custo médio gasto em um único posicionamento de anúncio para atingir a ação desejada do cliente, como uma compra ou assinatura.<p>**Cálculo**: valor total `spent` dividido pelo número de ações de clientes concluídas<p>Essa métrica ajuda a avaliar a relação custo-eficiência do posicionamento do anúncio ao gerar ações valiosas. | Um CPA mais baixo sugere que a inserção de anúncios é eficaz na conversão de interações de público-alvo em ações desejadas a um custo mais baixo. |
| **[!UICONTROL CPC &#x200B;]**<br>_Custo por clique_ | O custo médio associado a cada clique em um único posicionamento de anúncio.<p>**Cálculo**: valor total `spent` dividido por `clicks`<p>Essa métrica ajuda a avaliar a relação custo-eficácia do posicionamento do anúncio na geração de cliques. | Um CPC menor indica que o posicionamento do anúncio está gerando cliques a um custo menor, o que pode ser benéfico para maximizar o retorno sobre o investimento. |
| **[!UICONTROL Gastar]** | O valor gasto em um único posicionamento de anúncio, representando uma fração do valor total gasto em todo o anúncio. Essa métrica ajuda a rastrear a alocação de orçamento e a eficiência dos gastos para cada posicionamento de anúncio. | O monitoramento dos gastos pode ajudar a garantir que os recursos estejam sendo usados de maneira eficaz em diferentes posicionamentos. |
| **Atributos** | Lista de recursos inerentes presentes neste posicionamento de anúncio. | Os atributos ajudam a identificar elementos criativos que mais refletem em seu público-alvo. Consulte [Categorias](/help/user-guide/insights/attributes.md#categories). |
