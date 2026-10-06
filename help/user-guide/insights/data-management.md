---
title: Gerenciamento de dados
description: Saiba mais sobre a assimilação e o armazenamento de dados do [!DNL Insights] no GenStudio for Performance Marketing.
feature: Reporting and Insights
level: Experienced
role: Admin, Developer
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
TQID: 'https://experienceleague.adobe.com/HM2e0Yq2uwTpKtK-z8gHs0hDFrsJS6koQBqoNoKJK0Y'
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: e0aa398c-6185-4e77-8cf7-2561c578c181
    internal-label: Integrations
  - id: c5a86ad9-9158-4ab1-a7ea-9e29985087b8
    internal-label: Content lifecycle
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: e61505eb-ae0c-4fa0-a6cc-9f95313d4431
    internal-label: Reporting and insights
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: d3cdead0-685a-4489-9250-4bb709942f66
    internal-label: Data collection
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
    internal-label: Data management
source-git-commit: 4d35c796d2968255c3e1f525215cfe71434f8e23
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%
---
# Gestão de dados

O GenStudio for Performance Marketing usa o Adobe Experience Platform (AEP) para assimilação e armazenamento de dados das métricas e metadados que alimentam o [!DNL Insights]. O AEP usa _esquemas_ para definir as estruturas de dados e _conjuntos de dados_ para armazenar e gerenciar coleções de dados.

## Conexões de dados

O GenStudio for Performance Marketing usa o Customer Journey Analytics (CJA) para agregar várias fontes de dados criando uma conexão com um ou mais conjuntos de dados do AEP. O CJA usa essas conexões de dados para criar visualizações de dados para analisar métricas com [!DNL Insights].

>[!BEGINSHADEBOX]

**Informações importantes sobre conexões de dados**

Se você for um [administrador do sistema Adobe](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager), poderá ter direitos que permitem acesso ao gerenciamento de sandbox da AEP e a componentes do data lake que oferecem suporte ao GenStudio for Performance Marketing.

>[!WARNING]
>
>Redefinir a sandbox de produção no AEP exclui todas as conexões de dados e faz com que [!DNL Insights] pare de funcionar.

Tenha cuidado e não exclua as seguintes conexões de dados necessárias para que o GenStudio for Performance Marketing opere de forma confiável:

- Conjuntos de dados AEP com o prefixo `GS Insights`
- Esquemas, classes e grupos de campos do AEP com o prefixo `GS Insights`
- Grupo de campos personalizado `timestamp for metadata`
- Conexões do AEP: fluxos de dados com o prefixo `GS Insights`
- Conexões da AEP: conta do GS Insights

Consulte [Excluir implicações](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/deletion) no guia do _Customer Journey Analytics_ antes de excluir quaisquer componentes de dados no AEP.

>[!ENDSHADEBOX]

## Política de retenção de dados

O GenStudio for Performance Marketing retém os dados do canal por 13 meses. Essa política de retenção inclui os seis meses de dados assimilados durante a conexão inicial, garantindo uma análise e relatórios abrangentes de dados históricos.

Consulte [Conectar conta de mídia paga](/help/user-guide/connectors/connect-channel.md).
