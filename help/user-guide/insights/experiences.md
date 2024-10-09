---
title: Visão geral das experiências
description: Consulte uma visão geral do envolvimento do cliente, orçamento e despesas para obter experiências e desempenho no posicionamento de anúncios no Adobe GenStudio for Performance Marketing.
feature: Insights, Experiences
source-git-commit: ce08231cb723bec3d80a732837b72a435d3b552d
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# Visão geral das experiências

A exibição [!DNL Insights] _[!UICONTROL Experiências]_ mostra uma lista de experiências para a conta de anúncio do canal conectado. Para o Facebook, as experiências são nomes de Metadados.

A tabela _[!UICONTROL Experiências]_ é organizada com [!UICONTROL Nomes de anúncios]. Clique no ícone de configurações (cog) acima do lado direito da tabela para alternar as colunas visualizáveis. O ícone de filtro (funil) acima do lado esquerdo da tabela abre o menu **[!UICONTROL Filtro]**, onde você pode selecionar nas listas [!UICONTROL Conta] e [!UICONTROL Campanha] para filtrar os nomes de anúncios na tabela.

![Filtro e tabela de experiências](/help/assets/insights-experiences-filter.png){zoomable="yes"}

## Detalhes da experiência

Uma _experiência_ é um ativo promocional que inclui conteúdo visual e interativo destinado à distribuição para um público específico como parte de uma campanha de marketing.

Selecione uma experiência (nome do anúncio) e visualize as métricas de desempenho, os atributos de texto e os posicionamentos associados a cada anúncio. Na visualização de detalhes, é possível analisar as métricas de uma experiência com base em seus esforços de posicionamento de anúncios e marketing em um intervalo de datas especificado.

A exibição de detalhes inclui uma métrica para o anúncio geral `click-through rate`, `cost per click`, e quanto do orçamento foi `spent` no anúncio. Como os anúncios podem ter vários posicionamentos, como um feed ou um banner, você pode ver um detalhamento das mesmas métricas para cada posicionamento de anúncio. Use as setas para a esquerda e para a direita em **[!UICONTROL Desempenho por posicionamento de anúncio]** para percorrer as métricas de posicionamento de anúncios.

![Detalhes do anúncio com métricas e posicionamentos de anúncios](/help/assets/insights-experience-details.png){zoomable="yes"}

### Atributos de texto

Abaixo da visualização da experiência está uma lista de [!UICONTROL Atributos de texto] associados ao anúncio. Quando ativos e experiências são aprovados e armazenados no [!DNL Content], a GenStudio for Performance Marketing gera tags com base em seus recursos inerentes. Consulte [detalhes do ativo](../content/asset-details.md#system-metadata) para obter detalhes sobre metadados do sistema.

### Posicionamentos de anúncios

No momento em que você criou uma campanha com Meta ads, você pode ter selecionado onde executar seus anúncios com base no [objetivo](channels.md#objectives) da campanha. Os posicionamentos de anúncios ampliam o alcance do público-alvo do seu anúncio.

O GenStudio for Performance Marketing é compatível com formatos de anúncios, como feeds de ativos, anúncios de links e imagem ou vídeo únicos. Veja a seguir uma lista de formatos de anúncios por plataforma:

| Instagram | Facebook/Meta | Messenger | Rede de público-alvo |
| ------------ | ---------------- | ------------ | ---------------- |
| Explorar<br>Explorar Página Inicial<br>Explorar Página Inicial Do Grid<br>Feed<br>Rolos<br>Feed De Perfil<br>Pesquisa<br>Compras<br>Histórias | Business Explore<br>Feed<br>Vídeo em fluxo<br>Marketplace<br>Reels<br>Sobreposição de Reels<br>Coluna direita<br>Resultados da pesquisa<br>Histórias<br>Feeds de vídeo<br>Anúncios no Facebook Reels | Caixa de entrada<br>Histórias | Nativo, banner e intersticial<br>Vídeo recompensado |

## Métricas de experiência

As métricas de Insights podem ajudar a avaliar quais experiências contribuem para o sucesso de uma campanha e quais posicionamentos de anúncios são mais eficazes.

<!-- For example, -->

### Detalhes das métricas

A tabela a seguir fornece definições e insights para as métricas principais de marketing digital na exibição [!UICONTROL Experiências]. Cada métrica inclui uma breve definição, pois se relaciona a nomes de anúncios, como a métrica é calculada, e um ou mais insights para ajudar a entender sua importância e impacto em uma experiência.

| Métrica | Definição | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Nome do anúncio]** | Uma lista de experiências para a conta de canal conectada. Filtre anúncios selecionando uma campanha. | Classifique a lista de anúncios clicando em qualquer uma das métricas principais. |
| **[!UICONTROL Campanha]** | Uma campanha é um conjunto de experiências projetadas para atingir um objetivo específico. | |
| **[!UICONTROL Posicionamentos de anúncios]** | Uma contagem de [posicionamentos de anúncios](#ad-placements)—onde executar o anúncio—para o anúncio ou experiência. | Os posicionamentos de anúncios aumentam o alcance do público-alvo. |
| **[!UICONTROL Assets]** | Uma contagem dos ativos usados no anúncio ou na experiência. | |
| **[!UICONTROL Impressões]** | Uma contagem de cada vez que o posicionamento do anúncio ou a experiência são carregados no canal, independentemente da interação ou da visualização. | Uma contagem de alta impressão pode indicar ampla visibilidade, mas, para obter um verdadeiro insight sobre o desempenho, considere com outras métricas de envolvimento. |
| **[!UICONTROL Cliques]** | Número de vezes que os usuários interagem com um elemento clicável, como um link ou um botão de chamada para ação, em uma experiência. | Uma alta contagem de cliques indica forte interesse e envolvimento com o conteúdo, que pode ser eficaz e alcançar o público-alvo correto. |
| **[!UICONTROL CTR ]**<br>_Taxa de cliques_ | Porcentagem (%) de impressões que resultaram em cliques de experiência em uma campanha.<br>**Cálculo**: `clicks` dividido por `impressions` | Uma alta taxa de cliques indica que o conteúdo é altamente relevante e motivador para o público-alvo nas mensagens e no design e está efetivamente direcionando os interesses do público-alvo. |
| **[!UICONTROL CPM ]**<br>_Custo por mil_ | Custo ($) para cada mil impressões de anúncios para a experiência ou posicionamento de anúncios.<br>**Cálculo**: valor total `spent` dividido pelo alcance, então multiplicado por 1000 | Um valor baixo pode indicar visibilidade com boa relação custo-benefício, especialmente quando combinado a uma alta taxa de cliques. |
| **[!UICONTROL CPC ]**<br>_Custo por clique_ | Custo médio ($) associado a cada clique em uma experiência ou posicionamento de anúncio.<br>**Cálculo**: valor total `spent` dividido por `clicks` | Custos médios mais baixos podem indicar anúncios e gastos econômicos, especialmente quando comparados a um aumento nas conversões. |
| **[!UICONTROL Gastar]** | O valor ($) gasto no orçamento durante um determinado período. | Um alto valor de gasto em um curto período pode indicar uso rápido, o que pode levar ao esgotamento antecipado de recursos. Acompanhe o valor dos gastos em relação às principais métricas de desempenho para ajudar a monitorar o retorno geral sobre o investimento. |
