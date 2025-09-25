---
title: Gerenciamento de dados
description: Saiba mais sobre a assimilação e o armazenamento de dados do  [!DNL Insights]  no GenStudio for Performance Marketing.
feature: Reporting and Insights
level: Experienced
role: Admin, Data Architect
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
source-git-commit: 44fedfdc3902b4f993d656ae6360a32e27a62520
workflow-type: tm+mt
source-wordcount: '242'
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

Consulte [Excluir implicações](https://experienceleague.adobe.com/pt-br/docs/analytics-platform/using/technotes/deletion) no guia do _Customer Journey Analytics_ antes de excluir quaisquer componentes de dados no AEP.

>[!ENDSHADEBOX]

## Política de retenção de dados

O GenStudio for Performance Marketing retém os dados do canal por 13 meses. Essa política de retenção inclui os seis meses de dados assimilados durante a conexão inicial, garantindo uma análise e relatórios abrangentes de dados históricos.

Consulte [Conectar conta de mídia paga](/help/user-guide/connectors/connect-channel.md).
