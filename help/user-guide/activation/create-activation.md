---
title: Fluxo de trabalho de ativação
description: Saiba mais sobre o fluxo de trabalho de ativação para experiências de anúncio.
feature: Ad Activation
exl-id: 17e1bade-d52a-4953-a85c-c10d093e73d6
source-git-commit: 8db25ba42a8eebc2d17f8b8b1a5f5fbede1a6e0f
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

# Fluxo de trabalho de ativação

O _[!DNL Activate]_oferece suporte à ativação de experiências de anúncio na forma de um criativo em formatos específicos de canal, como uma experiência de anúncio Meta ou Google Campaign Manager 360.

Uma experiência do GenStudio for Performance Marketing é um componente de campanha de marketing, como um anúncio, preparado como criativo para um público específico em um canal de anúncio pago ou email. A criação contém três componentes principais:

* **Ativos de mídia**: os ativos de mídia são as imagens (GIFs, PNG, JPEG) incluídas na sua experiência com anúncios. A ativação atualmente suporta imagens estáticas.
A seleção de um ativo de imagem para sua experiência de anúncio requer a escolha de uma taxa de proporção apropriada. As taxas de proporção definem a relação proporcional entre a largura e a altura de uma imagem e são cruciais para a eficácia dos posicionamentos de anúncios. Os canais de mídia paga especificam cuidadosamente as taxas de aspecto válidas para cada posicionamento de anúncio em suas plataformas. Ao adicionar ativos de imagem à sua ativação, você deve selecionar a taxa de proporção com base nos posicionamentos finais dos anúncios para sua experiência. Os tipos de arquivos são restritos ao JPEG, PNG e GIF.

* **Texto**: o texto compreende todas as formas de cópia incluídas no anúncio, incluindo títulos, corpo de texto e elementos de chamada para ação.

* **Metadados**: atributos definidos pelo usuário que você pode atribuir ao conteúdo. Os metadados aprimoram a análise, a filtragem e o rastreamento do desempenho. Normalmente, não é visível para usuários.

A criação de uma ativação envolve o refinamento de cada um desses componentes de anúncio para uma campanha de marketing e inserção de canal designada. O GenStudio for Performance Marketing permite ativar uma experiência para um canal pago.

## Fases do fluxo de trabalho

Embora requisitos exclusivos de posicionamento definam cada canal pago, todas as ativações de anúncios compartilham as mesmas etapas de alto nível. A ativação de uma experiência para qualquer canal pago tem três fases principais:

* **Conecte o GenStudio for Performance Marketing ao seu canal de destino**. Um gerente de sistema da GenStudio deve conectar suas contas de canal antes que você possa ativar uma experiência.

* **Prepare sua experiência para ativação**. A preparação inclui selecionar os ativos de mídia na proporção apropriada para o posicionamento específico do anúncio e atribuir o texto aos elementos de chamada para ação e cópia do corpo. Você também pode adicionar metadados informativos que ajudam os usuários a pesquisar a experiência após a ativação. Cada posicionamento de canal de anúncio especifica taxas de proporção válidas para ativos visuais incluídos no posicionamento.

>[!TIP]
>
>Você pode selecionar experiências de anúncio aprovadas diretamente da galeria de experiências _[!DNL Content]_para se preparar para as criações do Google Campaign Manager 360. Depois de selecionar uma experiência na galeria_[!DNL Content]_, não é possível editar nem adicionar ativos ao criativo.

* **Revise e publique sua experiência no canal de destino**. Use o painel _Visualização_ durante a configuração criativa para avaliar sua escolha de posicionamento de anúncio e elementos de texto antes de finalizar sua ativação. Sua revisão final antes da publicação ocorre no aplicativo de gerenciamento de anúncios do canal de destino. Por exemplo, depois de ativar uma experiência de anúncio Meta no GenStudio for Performance Marketing, você deve fazer logon no Gerenciador de anúncios Meta, revisar o criativo e selecionar os atributos específicos antes de publicá-lo.

Depois que um criativo estiver no seu canal de mídia paga de destino, _[!DNL Insights]_poderá acompanhar e analisar seus dados de desempenho.

## Canais compatíveis

Cada canal de mídia paga tem um fluxo de trabalho de ativação exclusivo. Selecione o canal pago para as diretrizes de ativação:

* [Meta](activate-meta-ad.md)
* [Google Campaign Manager 360](activate-cm360-ad.md)
