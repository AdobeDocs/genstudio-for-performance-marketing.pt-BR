---
title: Visão geral da Ativação
description: Saiba como ativar conteúdo com o Adobe CX Enterprise e aplicativos de terceiros.
level: Beginner
feature: Ad Activation
exl-id: 365fe253-d189-467e-a723-f54cd74ff60b
TQID: https://experienceleague.adobe.com/-Nal0YqjTzKw4g2SM3IuMf0a13e87CWdTqBZPd0dBkU
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: d87258a7-722c-4afd-b632-adddc447c7aa
    internal-label: Ad activation
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%
---
# Adobe GenStudio for Performance Marketing Ativate

O GenStudio for Performance Marketing [!DNL Activate] é o local para onde você prepara e envia experiências de anúncios para canais de anúncios pagos, como Meta ou LinkedIn. A _Ativação_ pega uma experiência de anúncio aprovada e seus ativos, aplica a configuração de um canal específico e a entrega diretamente a esse canal em um status inativo e desativado. A partir daí, você pode fazer uma análise final no próprio gerenciador de anúncios do canal antes que seu anúncio seja publicado.

O [!DNL Activate] fornece sua experiência diretamente para o canal, portanto, você não precisa exportar arquivos ou carregá-los manualmente para o próprio gerenciador de anúncios do canal.

Um gerente de sistema ou editor do GenStudio deve conectar a conta de anúncio de cada canal de anúncio pago antes de ativar uma experiência de anúncio para esse canal.

## Ativar recursos

Use o [!DNL Activate] para preparar experiências de anúncio para seus canais de anúncios pagos de destino. [Ativar experiências em massa](create-activation.md) em vários canais de anúncios pagos em uma única tabela de ativação. Em seguida, [gerencie suas ativações](manage-activations.md) para ver o status e os detalhes de cada experiência ativada.

>[!VIDEO](https://video.tv.adobe.com/v/3503542?captions=por_br&learn=on)

### Ativar experiências aprovadas a partir do conteúdo

Selecione uma ou mais experiências aprovadas, publicadas de [!DNL Content] ou comece na página de aterrissagem [!DNL Activate]. Ao contrário das versões anteriores do [!DNL Activate], uma única tabela de ativação pode incluir experiências para vários canais de anúncios pagos de uma só vez, organizadas por formato de anúncio e canal.

>[!NOTE]
>
>[!DNL Content] chama um destino como Meta ou LinkedIn de um **canal**. [!DNL Activate] chama o mesmo destino de **plataforma** (por exemplo, em **[!UICONTROL Configuração de plataforma]**). Os dois termos se referem à mesma coisa.

### Definir detalhes de configuração do anúncio e da plataforma

Cada linha na tabela de ativação representa um anúncio. Os ativos criativos, as manchetes e a cópia do corpo aprovados estão bloqueados porque já passaram por revisão e aprovação. Você pode editar os campos restantes, como texto do call-to-action, URL de destino e detalhes de configuração da plataforma, como conta de anúncio, campanha e conjunto de anúncios. Edite campos para uma linha por vez ou selecione várias linhas para editar campos compartilhados em massa.

### Revise e publique suas experiências nos canais de publicidade deles

Confirme se cada linha mostra [!UICONTROL Pronto para Ativar]. [!DNL Activate] sinalizadores sem campos ou com campos inválidos, chamadas de ação incompatíveis e IDs de rastreamento duplicadas, pois [!UICONTROL Requer Atenção]. Quando cada linha estiver pronta, clique em **[!UICONTROL Enviar para a Platform]** para publicar todos os anúncios na tabela. [!DNL Activate] relata o status de cada anúncio em tempo quase real e os anúncios publicados com êxito incluem um deep link para o anúncio no gerenciador de anúncios nativo da plataforma de destino. Anúncios com falha retornam uma mensagem de erro e podem ser repetidos.
