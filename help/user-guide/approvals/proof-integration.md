---
title: Integração do Workfront Proof com análise e aprovações
description: Integração do Workfront Proof com o Adobe GenStudio for Performance Marketing.
feature: Content Review, Content Management
source-git-commit: f8508ee9440714137141e933cfe0f5761a510c7a
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Integração do Workfront Proof com o GenStudio for Performance Marketing

A integração com o Workfront Proof aprimora o ciclo de vida de revisão e aprovação do GenStudio for Performance Marketing com recursos avançados, incluindo modelos de aprovação, fluxos de trabalho de vários estágios e a capacidade de [comparar versões de prova](https://experienceleague.adobe.com/pt-br/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs). Esse controle de versão estruturado garante transparência, responsabilidade e colaboração simplificada por todo o ciclo de vida da análise do conteúdo.

>[!BEGINSHADEBOX]

**Pré-requisitos**:

Instalar a [extensão do Adobe Workfront Web Viewer](https://experienceleague.adobe.com/pt-br/docs/workfront/using/review-and-approve-work/proofing/review-proofs-in-workfront/review-a-proof/review-proof-in-web-viewer-extension)

>[!ENDSHADEBOX]

O [!DNL Proofing Viewer] da Workfront Proof é um espaço de trabalho avançado para exibir, comentar e comparar provas. De [!DNL Proofing Viewer], você pode

* Comparar diferentes versões do conteúdo
* Adicionar comentários e marcações de desenho a uma prova
* Aprovar a prova

O [!DNL Proofing Viewer] é carregado quando você clica na URL da prova no email de solicitação de aprovação ou na notificação no produto. A exibição [!DNL Proofing Viewer] _Minha nova aprovação_ é aberta. Nesta exibição, você pode revisar o conteúdo e fornecer comentários usando as ferramentas de anotação principais do [!DNL Proofing Viewer].

Para sair de [!DNL Proofing Viewer], clique em **[!UICONTROL Retornar ao GenStudio]**.

## Genstudio para Marketing de desempenho e Workfront Proof: comparação de recursos

A tabela abaixo compara os recursos padrão de revisão e aprovação do GenStudio for Performance Marketing com os recursos mais avançados disponíveis por meio da integração com o Workfront Proof.

| Recurso        | GenStudio for Performance Marketing                                                                 | Workfront Proof                                                                 |
|-------------------------------|------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|
| **Ciclo de vida de rascunho/prova**        | O conteúdo de rascunho expira após a publicação. | Cadeias de aprovação de vários estágios, baseadas em função, com registros persistentes com carimbo de data e hora.<br> Todas as versões são retidas indefinidamente. |
| **Comentários**                | Os comentários são vinculados à ID de rascunho e descartados após a publicação.                                           | Comentários e anotações persistentes são retidos para auditoria e conformidade.     |
| **Versões**           | Os rascunhos são tratados como instâncias exclusivas.<br>Nenhuma comparação lado a lado.                                      | Controle completo da versão com ferramentas de comparação lado a lado e de sobreposição.        |
| **Gerenciamento de projetos** | Gerenciamento básico de campanhas. | Gerenciamento completo do ciclo de vida da campanha, incluindo personalização, modelos, relatórios e auditorias detalhadas. |

### Licenças e funções de usuário

As licenças identificam o conjunto de direitos do usuário em um produto. O Workfront Proof fornece mais tipos de licença ou funções de usuário do que o GenStudio for Performance Marketing. [Visão geral das funções de prova](https://experienceleague.adobe.com/pt-br/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles) apresenta as funções de usuário associadas ao fluxo de trabalho de revisão e aprovação do Workfront Proof.

| Licença do GenStudio for Performance Marketing       | Licença do Workfront                 | Descrição                                                                                                                                                      |
|---------------------------------------------------|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| GenStudio System Manager                          | Administrador do Workfront/Usuário avançado | Acesso total aos recursos de Marketing de desempenho do GenStudio, como gerenciamento de marca, persona e produto. Gerencia fluxos de trabalho e configurações. Cria modelos de aprovação. |
| Criador e editor de conteúdo (licença de usuário avançado)   | Criador da prova (licença Standard)  | Gera e envia rascunhos de conteúdo. No Visualizador de provas, carrega ativos e inicia provas. Exige uma licença do Workfront Proof.                              |
| Revisor / Aprovador (licença do Collaborator)        | Revisor/Aprovador                 | Participa de revisões de vários estágios, adiciona comentários e aprova ou rejeita conteúdo.                                                                             |

Os administradores de sistema da Adobe gerenciam o provisionamento de usuários e os direitos para ambos os produtos na Adobe Admin Console.

>[!NOTE]
>
> A Workfront Proof fornece [funções de usuário adicionais](https://experienceleague.adobe.com/pt-br/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles). Nem todas as funções estão visíveis no Marketing de desempenho. No entanto, o sistema respeita qualquer função definida em um modelo do Workfront Proof.

### Rascunhos e provas

O Workfront [!DNL Proofing Viewer] estende o processo básico de revisão e aprovação da GenStudio for Performance Marketing com recursos de revisão e aprovação mais estruturados. As provas revisadas nesta integração estão limitadas aos formatos compatíveis com o GenStudio for Performance Marketing.

### Controle de versão

O GenStudio for Performance Marketing não oferece suporte a modelos de aprovação, mas o Workfront Proof oferece. Os recursos de controle de versão do Proof melhoram significativamente o processo de revisão e aprovação de conteúdo do GenStudio. Cada envio no fluxo de trabalho de Prova é tratado como uma versão distinta do rascunho do conteúdo ou _prova_. Provas são salvas automaticamente e podem ser comparadas lado a lado com iterações anteriores. As partes interessadas podem rastrear as alterações, fornecer feedback preciso e manter o alinhamento durante todo o ciclo de revisão. A prova preserva um histórico completo de todos os comentários, decisões e versões, oferecendo suporte aos requisitos de conformidade e disponibilidade de auditoria. Cada versão também é compatível com fluxos de trabalho de aprovação em vários estágios com base em funções, com cada ação (aprovação, rejeição ou comentário) claramente registrada e carimbada com data e hora.

### Modelos de aprovação

Os modelos de aprovação do Workfront Proof fornecem etapas pré-formatadas que podem simplificar o fluxo de trabalho de aprovação de prova. Esses modelos incluem revisores e aprovadores selecionados, funções de prova e prazos, garantindo consistência e eficiência. Os criadores de conteúdo que iniciam uma revisão podem selecionar entre um conjunto de modelos predefinidos para fluxos de trabalho de aprovação de fase única e de várias fases.

Cada estágio do modelo de fluxo de trabalho identifica revisores atribuídos. Todas as atualizações de status e comentários do fluxo de trabalho do Workfront Proof estão visíveis no Visualizador de provas, melhorando a transparência e a colaboração.

Os modelos de aprovação são compatíveis com aprovações em vários estágios, que oferecem suporte à coordenação de revisões de diferentes grupos de participantes.

### Comentários

Os revisores podem clicar diretamente em áreas específicas da prova para deixar comentários precisos e contextuais. Todos os comentários recebem carimbo de data e hora e são salvos como parte do histórico de versões da prova. O histórico de comentários não está disponível no GenStudio for Performance Marketing.

Você pode [comparar duas versões de uma prova](https://experienceleague.adobe.com/pt-br/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs) para avaliar comentários de revisão e conteúdo.

## Notificações e lembretes

Revisores e aprovadores recebem notificações por email quando uma nova prova está disponível para revisão ou quando uma revisão em andamento mudou o status.
[Notificações e lembretes de prova](https://experienceleague.adobe.com/pt-br/docs/workfront/using/workfront-proof/proof-notifications-and-reminders/proof-notifications-and-reminders/proof-notifications-and-reminders) incluem um link personalizado para a prova, detalhes sobre a prova e seu progresso pelo processo de aprovação e informações sobre controle de versão.
