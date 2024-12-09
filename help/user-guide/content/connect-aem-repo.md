---
title: 'Conectar-se a um repositório  [!DNL AEM Assets Content Hub] '
description: Saiba como conectar o Adobe GenStudio for Performance Marketing a um repositório do Adobe Experience Manager (AEM) [!DNL Content Hub] e aproveitar o conteúdo aprovado existente.
level: Experienced
feature: Assets, Content
exl-id: abb587fd-593c-4b9f-baad-993d92400d9b
source-git-commit: abe1de42b81bff63d473a67632d27f96db7c1c7d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Conectar a um repositório [!DNL AEM Assets Content Hub]

Se você tiver ativos no Adobe Experience Manager (AEM), poderá seguir essas etapas para torná-los acessíveis no GenStudio for Performance Marketing.

>[!BEGINSHADEBOX]

**Pré-requisitos**:

As etapas a seguir exigem acesso administrativo ao Admin Console e AEM Assets as a Cloud Service.

>[!ENDSHADEBOX]

## Etapa 1: Habilitar [!DNL AEM Assets Content Hub]

Siga o processo de autoatendimento **Implantar Content Hub** para habilitar o [!DNL Content Hub] para sua AEM Assets existente no Cloud Manager. Consulte [Implantar [!DNL Content Hub]](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub) na documentação do _AEM as a Cloud Service_.

Depois de habilitar [!DNL AEM Assets Content Hub], você tem uma nova instância com o sufixo `contenthub` em [!DNL AEM Assets as a Cloud Service] no Admin Console.

>[!IMPORTANT]
>
>Os administradores devem verificar se o repositório [!DNL AEM Assets Content Hub] está na mesma organização que o GenStudio for Performance Marketing.

## Etapa 2: integrar usuários do GenStudio

No [!DNL Admin Console], adicione um usuário ou grupo de usuários do GenStudio for Performance Marketing ao perfil de produto [!DNL AEM Assets Content Hub]. Se um revisor de conteúdo não tiver acesso à mesma organização do repositório [!DNL AEM Assets Content Hub], ele poderá ter dificuldades para revisar e aprovar o conteúdo.

- [Integrar [!DNL Content Hub] administrador](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-administrator)
- [Integrar [!DNL Content Hub] usuários](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-users)

## Etapa 3: Aprovar ativos

Aprove ativos para uso no [!DNL AEM Assets Content Hub], que os disponibiliza no GenStudio for Performance Marketing.

Consulte [Aprovar ativos no Experience Manager](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/approve-assets) na documentação do _AEM as a Cloud Service_.

## Etapa 4: configurar a visibilidade do ativo

Nas opções de configuração do _[!DNL AEM Assets Content Hub]_, analise cada conjunto de opções de configuração para filtros, detalhes de ativos, pesquisa e identidade visual.

Consulte [Configurar interface do usuário do Content Hub](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/configure-content-hub-ui-options) na documentação do _AEM as a Cloud Service_.

## Etapa 5: verificar a conexão

Em Conteúdo do GenStudio for Performance Marketing, a lista _[!UICONTROL Local]_ está disponível acima da galeria, no lado direito. A lista não estará disponível se você não tiver acesso ou se sua organização não tiver implantado e conectado um repositório do [!DNL AEM Assets Content Hub].

Consulte [Local do Assets](manage-assets.md#assets-location) para ler sobre a lista Local e alterar repositórios.
