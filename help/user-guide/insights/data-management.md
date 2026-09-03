---
title: Gerenciamento de dados
description: Saiba mais sobre a assimilação e o armazenamento de dados do  [!DNL Insights]  no GenStudio for Performance Marketing.
feature: Reporting and Insights
level: Experienced
role: Admin, Developer
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
TQID: https://experienceleague.adobe.com/HM2e0Yq2uwTpKtK-z8gHs0hDFrsJS6koQBqoNoKJK0Y
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: e0aa398c-6185-4e77-8cf7-2561c578c181
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: d3cdead0-685a-4489-9250-4bb709942f66
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 249
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
