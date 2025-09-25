---
title: Fluxo de trabalho de ativação
description: Saiba mais sobre o fluxo de trabalho de ativação para experiências de anúncio.
feature: Ad Activation
exl-id: 17e1bade-d52a-4953-a85c-c10d093e73d6
source-git-commit: 72cd93d9d6fdd99d5a524d05cba923e9c0191960
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Fluxo de trabalho de ativação

O [!DNL Activate] oferece suporte à ativação de experiências de anúncio em formatos específicos de canal, como uma experiência de anúncio do Meta ou do Google Campaign Manager 360.

Uma experiência do GenStudio for Performance Marketing é um componente de campanha de marketing, como um anúncio, que é preparado como uma experiência de anúncio para um público específico em um canal de anúncio pago ou email. As experiências para ativação contêm três componentes principais:

* **Ativos de mídia**: os ativos de mídia são as imagens (GIFs, PNG, JPEG) incluídas na sua experiência com anúncios. A ativação atualmente suporta imagens estáticas.

  A seleção de um ativo de imagem para sua experiência de anúncio requer a escolha de uma taxa de proporção apropriada. As taxas de proporção definem a relação proporcional entre a largura e a altura de uma imagem e são cruciais para a eficácia dos posicionamentos de anúncios. Os canais de mídia paga especificam cuidadosamente as taxas de aspecto válidas para cada posicionamento de anúncio em suas plataformas. Ao adicionar ativos de imagem à sua ativação, você deve selecionar a taxa de proporção com base nos posicionamentos finais dos anúncios para sua experiência. Os tipos de arquivos são restritos ao JPEG, PNG e GIF.

* **Texto**: o texto compreende todas as formas de cópia incluídas no anúncio, incluindo títulos, corpo de texto e elementos call-to-action.

* **Metadados**: atributos definidos pelo usuário que você pode atribuir ao conteúdo. Os metadados aprimoram a análise, a filtragem e o rastreamento do desempenho. Normalmente, não é visível para usuários.

A criação de uma ativação envolve o refinamento de cada um desses componentes de anúncio para uma campanha de marketing e inserção de canal designada. O GenStudio for Performance Marketing permite ativar uma experiência para um canal pago.

## Fases do fluxo de trabalho

Embora requisitos exclusivos de posicionamento definam cada canal pago, todas as ativações de anúncios compartilham as mesmas etapas de alto nível. A ativação de uma experiência para qualquer canal pago tem três fases principais:

1. **Conecte o GenStudio for Performance Marketing ao seu canal de destino**. Um gerente de sistema da GenStudio deve conectar suas contas de canal antes que você possa ativar uma experiência.

1. **Prepare sua experiência para ativação**. Você pode preparar experiências para ativação de duas maneiras:

   * Ativar uma experiência aprovada com configurações predefinidas diretamente do [!DNL Content]. Essa maneira simplificada de ativar uma ou mais experiências de anúncio em um único canal. Depois de selecionar uma experiência na galeria [!DNL Content], não é possível editar nem adicionar ativos à sua experiência com anúncios. Ativar de [!DNL Content] está disponível para experiências de anúncio do Meta e do Google Campaign Manager 360.

   * Combine sua experiência de anúncio selecionando ativos visuais de [!DNL Content], adicionando elementos de texto e selecionando taxas de proporções. Esse método envolve mais etapas, mas oferece maior flexibilidade criativa. A preparação inclui selecionar os ativos de mídia na proporção apropriada para seu posicionamento de anúncio específico e atribuir texto aos elementos e à cópia do corpo do call-to-action. Você pode adicionar metadados informativos que ajudam os usuários a pesquisar a experiência após a ativação. Cada posicionamento de canal de anúncio especifica taxas de proporção válidas para ativos visuais incluídos no posicionamento.

1. **Revise e publique sua experiência no canal de destino**. Use o painel _Visualização_ durante a configuração da experiência para avaliar sua escolha de posicionamento de anúncio e elementos de texto antes de finalizar sua ativação. Sua revisão final antes da publicação ocorre no aplicativo de gerenciamento de anúncios do canal de destino. Por exemplo, depois de ativar uma experiência de anúncio do Meta no GenStudio for Performance Marketing, você deve fazer logon no Meta Ads Manager, revisar a experiência de anúncio e selecionar os atributos específicos antes de publicá-la.

Quando uma experiência de anúncio estiver ativa em seu canal de mídia paga de destino, o [!DNL Insights] poderá acompanhar e analisar seus dados de desempenho.

## Canais compatíveis

Cada canal de mídia paga tem um fluxo de trabalho de ativação exclusivo. Selecione o canal pago para as diretrizes de ativação:

* [Google Campaign Manager 360](activate-cm360-ad.md)
* [LinkedIn](activate-linkedin-ad.md)
* [Meta](activate-meta-ad.md)
