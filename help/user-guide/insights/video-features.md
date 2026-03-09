---
title: Recursos de vídeo
description: Saiba mais sobre o recurso de vídeo das categorias de atributo usadas no GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Video Attributes, Generative AI
exl-id: 0dfdd735-b365-4a15-a6fd-e981697442cb
TQID: https://experienceleague.adobe.com/s-8h3ODnNuRyebiDTLZGQORJzPnPOcPzQjIhWBmpk-c
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 572
ht-degree: 1%

---

# Recursos de vídeo

Os recursos de vídeo representam elementos, sons ou padrões distintos e informativos em um vídeo para análise com o [!DNL Insights]. Esses recursos ajudam a categorizar e entender o conteúdo do vídeo, permitindo insights mais precisos e detalhados. Ao identificar vários atributos, como humor em áudio, gênero musical e objetos, a IA pode fornecer uma análise abrangente do vídeo, ajudando em uma melhor tomada de decisões e formulação de estratégia.

## Detecção de áudio

A detecção de áudio no GenStudio for Performance Marketing envolve a análise da trilha de áudio de um vídeo para identificar vários atributos. Esse processo de detecção determina o humor geral do áudio, identificando os tipos de áudio presentes, marcando gêneros ou categorias específicas de música e extraindo palavras-chave da fala. Ao entender esses elementos de áudio, a IA pode fornecer insights mais profundos sobre o conteúdo e o contexto do vídeo, aprimorando o processo geral de análise e categorização.

## Pesquisar recursos de vídeo

**Para visualizar um vídeo e ouvir um exemplo do áudio**:

1. Em _[!DNL Insights]_, selecione a exibição **[!UICONTROL Atributos]**.

1. Altere a exibição de tabela selecionando **[!UICONTROL Vídeo]**.

1. Selecione um recurso na lista **[!UICONTROL Categoria do atributo]**. Para um exemplo de áudio, selecione **Gênero de música**.

1. Selecione um atributo para obter uma visualização detalhada dos vídeos que compartilham essa categoria.

   Como exemplo, a categoria `Music genre` pode ter `electronic` como um atributo.

1. A página _Detalhes do atributo_ lista todos os vídeos com esse atributo. Mantenha o ponteiro do mouse sobre qualquer vídeo da lista para iniciar uma visualização de vídeo.

1. Alterne o botão **desativar som** (localizado no canto inferior esquerdo de uma visualização de vídeo) e ouça o áudio da visualização do vídeo.

A tabela a seguir lista as categorias de recursos de vídeo reconhecidas pela IA do GenStudio for Performance Marketing. A lista de atributos detectados para um conteúdo de mídia não é exaustiva. As mídias que contêm um conjunto avançado de recursos podem ser limitadas aos três recursos mais dominantes identificados pela IA.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Categoria | Descrição | Exemplo |
| ------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| Modo de áudio | Determina o tom emocional geral ou a atmosfera da faixa de áudio, como `calm`, `upbeat` ou `tense`. | `Energetic`, `Happy`, `Emotional Ambient/atmospheric`, `Relaxing`, `Dramatic`, `Expressive/characterful`, `Intense`, `Slow`, `Neutral` |
| Tipos de áudio | Marca o vídeo com um ou mais tipos de conteúdo de áudio presentes, como `music` ou `speech`. | `Music`, `Speech`, `Silence`, `Special effects`, `Ambience` |
| Categorias | Classifica o vídeo em uma ou mais categorias de conteúdo amplas. | `Entertainment`, `Sports`, `Music`, `Gaming`, `Howto tutorials`, `Fashion and style`, `Film and animation`, `Science and technology`, `Autos and vehicles`, `Pets and animals`, `People and blogs`, `News and politics`, `Social causes and activism`, `Travel and events`, `Education`, `Sales and offers` |
| Categoria de Música | Classificação ampla do gênero musical quando a música está presente no vídeo. O gênero ajuda a identificar o tipo geral de música, como os estilos `contemporary` ou `traditional`. | `Contemporary/pop music`, `Traditional/folk-based music`, `Instrumental/orchestral music`, `Rock music`, `Acoustic/unplugged music`, `Specialised/occasional music`, `Experimental/unique music` |
| Gênero de música | Classificação específica do estilo musical quando a música está presente no vídeo, o que fornece uma identificação mais detalhada da música, como `electronic` ou `jazz`. | `electronic`, `hip-hop`, `dance`, `novelty`, `rock`, `world`, `reggae`, `pop`, `film`, `jazz`, `background`, `latin` |
| Objetos | Identifica um ou mais itens, entidades e elementos que aparecem no vídeo. | Os valores são muito numerosos, mas alguns exemplos incluem: `backpack`, `book`, `hawk`, `glasses`, `fish`, `pencil`, `mountain bike`, `soap` |
| Orientação | O alinhamento do vídeo em relação à sua largura e altura. Detecta se é mais largo do que alto (paisagem), mais alto do que largo (retrato) ou igual em largura e altura (quadrado). | `landscape`, `portrait`, `square` |
| Pessoas | Quando houver pelo menos uma pessoa, um ou mais atributos podem descrever a pessoa ou as pessoas presentes no vídeo. | `person`, `woman`, `man`, `girl`, `boy`, `social group`, `kid`, `crowd`, `people` |
| Cenas | Identifica a configuração ou o ambiente em um vídeo, fornecendo contexto sobre onde o vídeo foi feito ou o tipo de local representado. | Os valores são muito numerosos, mas alguns exemplos incluem: `lake`, `underwater`, `highway`, `hill`, `log cabin`, `island`, `beach`, `lounge` |
| Estilos | Detecta tratamentos visuais aplicados a elementos de vídeo, como aqueles usados no After Effects ou no Lightroom. | `design`, `illustration`, `logo`, `square`, `cartoon`, `art`, `matte`, `neon` |
| Tags | Detecta outras características de vídeo que não se enquadram em uma classificação específica. As tags fornecem contexto e metadados adicionais sobre o vídeo. | Os valores são muito numerosos, mas alguns exemplos incluem: `construction`, `gothic`, `healing`, `military`, `selfie`, `football`, `typing`, `dancer`, `dancing` |
