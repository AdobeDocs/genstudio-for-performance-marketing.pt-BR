---
title: Distribuir seu aplicativo
description: Distribua seu aplicativo ou Complemento para GenStudio for Performance Marketing.
feature: Extensibility
exl-id: 4935356b-08df-402c-b1a2-b89627afc188
source-git-commit: 6ba402e9cdfb62d71c9993457a6d9952c4877553
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Distribuir seu aplicativo

A distribuição do complemento o torna disponível para uso pela sua organização e por outras pessoas. O fluxo de trabalho de distribuição depende se o complemento se destina à distribuição pública ou privada.

Este tópico discute a distribuição privada. A distribuição privada restringe a implantação do complemento na organização, identificada pela organização IMS, para a qual foi desenvolvido.

A distribuição pública disponibiliza o Complemento como um aplicativo na Adobe Exchange. A [Distribuição pública](https://developer.adobe.com/app-builder/docs/guides/distribution/public/), na documentação do desenvolvedor do _App Builder_, descreve como disponibilizar seu aplicativo para qualquer organização da Adobe.

>[!BEGINSHADEBOX]

**Pré-requisitos**:

Confirme as seguintes permissões:

* Permissões de desenvolvedor na organização da qual você envia o aplicativo para aprovação

* Permissões do administrador do sistema para aprovar o aplicativo

Seu aplicativo App Builder deve ser implantado em um projeto App Builder.

>[!ENDSHADEBOX]

**Para distribuir seu aplicativo de forma privada**:

A distribuição privada disponibiliza seu aplicativo somente para membros de sua organização.

1. No [Adobe Developer Console](https://developer.adobe.com/console/), selecione a organização, o projeto e o espaço de trabalho em que o aplicativo será implantado.

1. Selecione [!UICONTROL Aprovação] na área _Visão geral do Workspace_. O painel _Aprovação de aplicativo_ é aberto.

1. Na área _Detalhes de Envio de Aplicativo_, adicione detalhes informativos sobre o Complemento. Os detalhes incluem nome do aplicativo, descrição e email de contato.

1. Após concluir todos os campos, clique em [!UICONTROL Enviar].

1. Faça logon no [Adobe Exchange](https://exchange.adobe.com/) usando a mesma Adobe ID usada para fazer logon no Developer Console. Se você não tiver permissões de administrador do sistema nesta organização, solicite a aprovação de um administrador do sistema da organização.

1. Selecione [!UICONTROL Gerenciar] > [!UICONTROL aplicativos App Builder] para acessar uma solicitação para revisar o aplicativo.

1. Depois de examinar o aplicativo, selecione [!UICONTROL Aprovar]. Você também pode adicionar notas informativas.

Seu complemento agora está visível na instância do GenStudio for Performance Marketing de sua organização.
