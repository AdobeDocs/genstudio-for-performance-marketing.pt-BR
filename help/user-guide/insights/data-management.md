---
title: Gestão de dados
description: Saiba mais sobre a assimilação e o armazenamento de dados para Insights no GenStudio for Performance Marketing.
feature: Insights
level: Experienced
role: Admin
last-substantial-update: 2025-1-7
source-git-commit: 5dbe645f2ccf033f515da22ffdcce86edcb9fb24
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Gestão de dados

O GenStudio for Performance Marketing usa o Adobe Experience Platform (AEP) para assimilação e armazenamento de dados das métricas e metadados que alimentam o [!DNL Insights]. A AEP usa _esquemas_ para definir as estruturas de dados e _conjuntos de dados_ para armazenar e gerenciar coleções de dados.

## Conexões de dados

O GenStudio for Performance Marketing usa o Customer Journey Analytics (CJA) para agregar várias fontes de dados criando uma conexão com um ou mais conjuntos de dados da AEP. O CJA usa essas conexões de dados para criar visualizações de dados para analisar métricas com [!DNL Insights].

>[!BEGINSHADEBOX]

**Informações importantes sobre conexões de dados**

Se você for um [administrador de sistema do Adobe](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager), poderá ter direitos que permitem acesso ao gerenciamento de sandbox da AEP e a componentes de data lake que oferecem suporte ao GenStudio for Performance Marketing.

>[!WARNING]
>
>Redefinir a sandbox de produção na AEP exclui todas as conexões de dados e faz com que [!DNL Insights] pare de funcionar.

Tenha cuidado e não exclua as seguintes conexões de dados necessárias para que o GenStudio for Performance Marketing opere de forma confiável:

- Conjuntos de dados da AEP prefixados com `GS Insights`
- Esquemas, classes e grupos de campos da AEP com o prefixo `GS Insights`
- Grupo de campos personalizado `timestamp for metadata`
- Conexões da AEP: fluxos de dados com o prefixo `GS Insights`
- Conexões da AEP: conta do GS Insights

Consulte [Excluir implicações](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/deletion) no guia _Customer Journey Analytics_ antes de excluir quaisquer componentes de dados na AEP.

>[!ENDSHADEBOX]

## Política de retenção de dados

O GenStudio for Performance Marketing retém os dados do canal por 13 meses. Essa política de retenção inclui os seis meses de dados assimilados durante a conexão inicial, garantindo uma análise e relatórios abrangentes de dados históricos.

Consulte [Conectar canal e conta](/help/user-guide/insights/connect-channel.md).
