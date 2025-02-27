---
title: Recursos da imagem
description: Saiba mais sobre o recurso de imagem das categorias de atributo usadas no GenStudio for Performance Marketing.
feature: Insights, Attributes, Generative AI
source-git-commit: c15140ed3fe3d07e9112e9ad4781cb8fcf65045d
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 0%

---

# Recursos da imagem

Os recursos de imagem representam elementos ou padrões distintos e informativos em uma imagem que são usados para análise com [!DNL Insights]. Esses recursos ajudam a categorizar e entender o conteúdo visual, permitindo insights mais precisos e detalhados. Ao identificar vários atributos, como estilo, cor e objetos, a IA pode fornecer uma análise abrangente da imagem, auxiliando na melhor tomada de decisões e formulação de estratégia.

## Detecção de estilo

Determinar o _estilo da imagem_ serve como base para identificar outras características da imagem. A IA pode aplicar as técnicas de análise adequadas e reconhecer recursos relevantes, o que permite uma compreensão mais abrangente da imagem. Cada estilo tem características visuais distintas que influenciam como a imagem é percebida e analisada.

Se o estilo de imagem for identificado como `photograph`, a IA analisa características adicionais de `camera settings`, `camera proximity` e `Photography genres`. Essas características são específicas para fotografias e fornecem insights mais profundos sobre a composição e a qualidade da imagem. Consulte [28 tipos de estilos de fotografia](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html) no _Saiba mais sobre fotografia_ da Adobe e saiba mais sobre tipos populares de fotografia e terminologia fundamental.

Se o estilo de imagem for identificado como `sketch` ou `digital cartoon`, um conjunto diferente de características pode ser relevante. Essa abordagem hierárquica garante que a análise seja contextualmente precisa e adaptada ao tipo específico de imagem que está sendo examinado.

## Pesquisar recursos de imagem

**Para exibir imagens em uma categoria de atributo específica**:

1. Em _[!DNL Insights]_, selecione a exibição **[!UICONTROL Atributos]**.

1. Altere a exibição de tabela selecionando **[!UICONTROL Imagens]**.

1. Selecione um recurso de imagem na lista **[!UICONTROL Categoria do atributo]**, como `Scenes`.

1. Selecione um atributo para obter uma exibição detalhada das imagens que compartilham essa categoria.

   Como exemplo, a categoria `Scenes` pode ter `restaurant` como um atributo.

1. A página _Detalhes do atributo_ lista todas as imagens com esse atributo.

A tabela a seguir lista as categorias de recursos de imagem reconhecidas pela IA do GenStudio for Performance Marketing. A lista de atributos detectados de um ativo não é exaustiva. O Assets que contém um conjunto avançado de recursos pode ser limitado aos três recursos mais dominantes identificados pela IA.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Categoria | Descrição | Exemplo |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Distribuição de atenção | O nível de atenção do visualizador se espalha por uma imagem, indicando quanto foco as diferentes áreas da imagem podem receber. Uma distribuição mais alta significa que nenhuma área domina o foco do visualizador, enquanto uma distribuição mais baixa significa que um ou dois pontos focais capturam a atenção do visualizador. | `high`, `medium`, `low`<p>Exemplo de distribuição `low` à esquerda e distribuição `high` à direita:<p>![bola de baixa e alta distribuição](/help/assets/category/image-attn-lowhigh.png "Diferença na baixa e alta distribuição"){width="200" zoomable="yes"} |
| Ângulo da câmera | A perspectiva a partir da qual a câmera captura o assunto, que afeta a percepção e interpretação da imagem pelo espectador. Se o estilo da Imagem for `photograph`, essa característica será identificada. | `Low angle`, `High angle`, `Eye level`, `Overhead view`, `Dutch angle`, `Bird's eye view`<p>Exemplo de `eye level`:<p>![nível dos olhos](/help/assets/category/image-camera-angle.png "Pessoas sentadas em ângulos diferentes"){width="200" zoomable="yes"} |
| Configuração da câmera | Os ajustes e configurações específicos dos controles da câmera que influenciam a aparência final e a qualidade da imagem. Se o estilo da Imagem for `photograph`, essa característica será identificada. | `Fast shutter speed`, `Long exposure`, `Bokeh blur`, `Motion blur`, `Tilt-shift blur`, `Flash`, `Wide-angle`, `Black and white`, `Surreal`, `Double-exposure`, `Macro`, `Normal mode`<p>Exemplo de uma configuração `macro`:<p>![Imagem de close-up da macro](/help/assets/category/image-subject-distance.png "Configuração da macro para flor de close-up e abelha ornamentada"){width="200" zoomable="yes"} |
| Cor e tom | As cores e as qualidades de tons em uma imagem. Identifica até três cores de um conjunto predefinido de 40 cores em diferentes camadas de imagem:<p>**[!UICONTROL Cores do primeiro plano]**—cores na camada da frente da imagem<br>**[!UICONTROL Cores do plano de fundo ]**—cores na camada de fundo da imagem | Valores de cor: `Red`, `Dark Red`, `Green`, `Bright Green`, `Dark Green`, `Light Green`, `Mud Green`, `Blue`, `Dark Blue`, `Light Blue`, `Royal Blue`, `Black`, `White`, `Off White`, `Gray`, `Dark Gray`, `Silver`, `Cream`, `Magenta`, `Cyan`, `Yellow`, `Mustard`, `Khaki`, `Brown`, `Dark Brown`, `Violet`, `Pink`, `Dark Pink`, `Maroon`, `Tan`, `Purple`, `Lavender`, `Turquoise`, `Plum`, `Gold`, `Emerald`, `Orange`, `Beige`, `Lilac`, `Olive` |
| Temperatura de cor | Descreve o calor geral ou a frieza das cores na imagem. | Valores de tom ou temperatura: `warm`, `cool`, `neutral`<br>![cores e tons frios](/help/assets/category/image-color-temp.png "Temperatura de cor com plano de fundo frio e vários objetos coloridos"){width="200" zoomable="yes"} |
| Densidade do conteúdo | A concentração de elementos visuais e detalhes em uma imagem, indicando quanta informação está compactada no espaço visual.<p>Diferentemente da distribuição de atenção, que mede como o foco do visualizador é distribuído em diferentes áreas de uma imagem, a densidade do conteúdo foca na quantidade de informações visuais presentes. Uma densidade de conteúdo mais alta significa que mais elementos estão presentes. | `high`, `medium`, `low`<p>Exemplo de densidade `low` à esquerda e densidade `high` à direita:<p>![bola de baixa e alta densidade](/help/assets/category/image-attn-lowhigh.png "Diferença entre alta e baixa densidade"){width="200" zoomable="yes"} |
| Estilo da imagem | O tratamento visual de uma imagem, como uma fotografia ou rascunho. Depois que a IA determinar o estilo da imagem, outras características poderão ser identificadas. Por exemplo, se a imagem for uma fotografia, as configurações da câmera, a proximidade da câmera e as condições de iluminação poderão ser aplicadas. | `Photograph`, `Sketch`, `Painting`, `Digital cartoon`, `Infographics`, `Graphic design`, `Collage`, `Software screenshot`<p>Exemplo de um `digital cartoon` estilo de imagem![estilo de imagem de desenho animado](/help/assets/category/image-style.png "Desenho animado de estilo de imagem de um gato"){width="200" zoomable="yes"} |
| Condição de iluminação | Descreve a qualidade e as características da luz em uma imagem, afetando seu humor, tom e visibilidade. | `Golden hour`, `Blue hour`, `Midday`, `Overcast`, `Night`, `High-key`, `Low-key`, `Daylighting`, `Incandescent`, `Fluorescent`, `Colorful`, `Studio`<p>Exemplo de condição `daylighting`:<p>![Pessoa e cachorro na calçada em condição de luz do dia](/help/assets/category/image-lighting.png "condição de luz do dia"){width="200" zoomable="yes"} |
| Objetos | Identifica um ou mais itens, entidades e elementos que compõem a imagem. | Os valores são muito numerosos, mas alguns exemplos incluem: `backpack`, `book`, `hawk`, `glasses`, `fish`, `pencil`, `mountain bike`, `soap`<p>Exemplo de objetos `toucan` e `bird`:<p>![pássaro, objeto tucano](/help/assets/category/image-objects-bird.png "Design gráfico do objeto pássaro tucano"){width="200" zoomable="yes"} |
| Orientação | O alinhamento da imagem em relação à sua largura e altura. Detecta se é mais largo do que alto (paisagem), mais alto do que largo (retrato) ou igual em largura e altura (quadrado). | `landscape`, `portrait`, `square`<p>Exemplo de orientação `square`:<p>![rascunho quadrado](/help/assets/category/image-orientation-square.png "Rascunho de flor com orientação quadrada"){width="200" zoomable="yes"} |
| Pessoas | Quando pelo menos uma pessoa estiver presente, um ou mais atributos podem descrever a pessoa ou as pessoas na imagem. | `person`, `woman`, `man`, `girl`, `boy`, `social group`, `kid`, `crowd`, `people`<p>Exemplo de pessoas `woman` e `person` categorias:<p>![mulher com câmera](/help/assets/category/image-people.png "Pessoa gerenciando uma câmera"){width="200" zoomable="yes"} |
| Gêneros de fotografia | Detecta o assunto e a técnica usada para capturar uma imagem, como `abstract` ou `landscape` (não a mesma que a orientação paisagem). | `Architecture`, `Astro`, `Landscape`, `Pet`, `Interior`, `Wildlife`, `Night`, `Cityscape`, `Seascape`, `Underwater`, `Storm`, `Adventure sports`, `Fashion`, `Portrait`, `Sports`, `Food`, `Street`, `Event`, `Lifestyle`, `Commercial`, `Group`, `Abstract`, `Minimalist`, `Composite`<p>Ver [Tipos de fotografia](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html) |
| Cenas | Identifica a configuração ou o ambiente em uma imagem, fornecendo contexto sobre onde a imagem foi capturada ou o tipo de local representado. | Os valores são muito numerosos, mas alguns exemplos incluem: `lake`, `underwater`, `highway`, `hill`, `log cabin`, `island`, `beach`, `lounge`<p>Exemplos de cenas `snow`, `sky`, `winter`, e `mountain` refletidas em um capacete:<p>![Cena de neve do inverno](/help/assets/category/image-scenes.png "Reflexão de cenas de inverno, neve, céu e montanha"){width="200" zoomable="yes"} |
| Distância do assunto | A distância entre a câmera e o assunto de uma imagem. | `close up`, `mid shot`, `long shot`<p>Exemplo de um `closeup shot`:<p>![close-up shot](/help/assets/category/image-subject-distance.png "Close-up, flor e abelha ornamentada"){width="200" zoomable="yes"} |
| Estilos | Detecta tratamentos visuais aplicados a elementos de imagem, como aqueles usados no Lightroom ou no Photoshop. | `design`, `illustration`, `logo`, `square`, `cartoon`, `art`, `circle`, `circular`<p>Exemplo de estilo `circular`:<p>![gateway circular em recife de coral](/help/assets/category/image-styles-circular.png "Portal circular em recife de coral"){width="200" zoomable="yes"} |
| Tags | Detecta outras características de imagem que não se enquadram em uma classificação específica. As tags fornecem contexto e metadados adicionais sobre a imagem. Por exemplo, a IA pode detectar objetos `helmet` e `motorobike` em uma imagem e incluir `riding` como uma marca. | Os valores são muito numerosos, mas alguns exemplos incluem: `construction`, `gothic`, `healing`, `military`, `selfie`, `football`, `typing`, `dancer`, `dancing`<p>Exemplo das marcas `dancer` e `dancing`:<p>![marcas para dançarino e dançarino](/help/assets/category/image-tags.png "Pessoa dançante"){width="200" zoomable="yes"} |
