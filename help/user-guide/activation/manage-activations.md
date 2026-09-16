---
title: Gerenciar ativações
description: Saiba como gerenciar experiências ativadas com o Adobe GenStudio for Performance Marketing.
feature: Ad Activation
exl-id: 7cf340d4-37ab-4906-9aad-088a26db0818
TQID: https://experienceleague.adobe.com/ird0IiW8L5Axjj2FmEjlUcD1sPaNCNfxj9XNqGfQWiI
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 1%
---
# Gerenciar ativações

Suas tabelas de ativação aparecem na página de aterrissagem [!DNL Activate]. Cada tabela lista seus anúncios, juntamente com seus status:

| Status | Significado |
|---|---|
| [!UICONTROL Precisa de Atenção] | Pelo menos um anúncio na tabela de ativação tem um campo ausente ou inválido, como uma call to action incompatível, ou uma ID de rastreamento duplicada. |
| [!UICONTROL Pronto para Ativar] | Todos os anúncios na tabela de ativação passaram na validação e estão prontos para publicação. |
| [!UICONTROL Pendente] | A tabela de ativação inteira foi enviada e está sendo processada pela plataforma de destino. |
| [!UICONTROL Publicado] | A tabela de ativação inteira foi publicada com sucesso. |
| [!UICONTROL Falha] | A plataforma de destino rejeitou pelo menos um dos anúncios da tabela. Passe o mouse sobre a dica de ferramenta de status para ver a mensagem de erro da plataforma. |

Você pode repetir automaticamente as ativações com falha clicando em **[!UICONTROL Tentar novamente]** no canto superior direito.

As linhas publicadas são bloqueadas para reenvio e incluem um deep link para o anúncio no gerenciador de anúncios nativo da plataforma de destino, para que você possa ir diretamente para ele para revisá-lo ou iniciá-lo.

## Exibição de detalhes

Clique em uma linha de anúncio para abrir uma exibição focalizada dos detalhes de ativação. A visualização de detalhes somente leitura captura os detalhes de definição de um anúncio ativado, incluindo ativações com falha, com informações derivadas do GenStudio for Performance Marketing e da plataforma de destino:

* **Hora e data da publicação**: hora e data da publicação da plataforma de destino
* **ID do anúncio**: ID atribuída pela plataforma de destino e usada para rastreamento, com um deep link para o anúncio publicado no gerenciador de anúncios nativo da plataforma
* **Detalhes do anúncio**: os ativos, a cópia e os metadados aprovados usados para o anúncio
* **Configuração da plataforma**: a conta, a campanha e outros campos de configuração de plataforma usados para ativar o anúncio

A visualização de detalhes de uma ativação com falha inclui o motivo da falha.
