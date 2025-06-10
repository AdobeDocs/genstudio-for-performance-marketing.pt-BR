---
title: Revisões e aprovações do Adobe GenStudio for Performance Marketing
description: Saiba mais sobre o processo de revisão e aprovação do GenStudio for Performance Marketing.
level: Beginner
feature: Content Review, Content Management
exl-id: c83f47c0-e8ae-4c54-84b3-c50f67d6b3c2
source-git-commit: 7955796949c17f7cd877b115cba45c58cdd614a7
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# Revisões e aprovações do Adobe GenStudio for Performance Marketing

O fluxo de trabalho de revisão e aprovação garante que todas as partes interessadas, desde equipes criativas até especialistas jurídicos, possam revisar e aprovar com eficiência ativos e experiências de campanha, incluindo ativos de marca produzidos por IA gerativa.

>[!NOTE]
>
> Este recurso também está disponível como uma [integração com o Adobe Workfront Proof](/help/user-guide/approvals/proof-integration.md). Essa integração fornece recursos de Prova na Tela do GenStudio for Performance Marketing. Com a integração do Workfront Proof, a GenStudio for Performance Marketing obtém um processo de revisão mais estruturado, transparente e colaborativo, ajudando as equipes a migrar do rascunho para o final com mais confiança e clareza.

## Vantagens do fluxo de trabalho de revisão e aprovação

* **Suporte para criação robusta e iterativa de conteúdo de IA generativa**. Criar e implantar conteúdo alinhado à marca em uma organização é um processo altamente iterativo. Os recursos de IA gerativa do GenStudio for Performance Marketing permitem a criação rápida de centenas de variantes de ativos. Cada revisor pode solicitar várias alterações em um rascunho de ativo antes de aprová-lo. Quanto mais revisores, maior será o número de iterações potenciais antes de todas as partes interessadas chegarem a acordo sobre uma variante final.

* **Suporte para integridade criativa**. As aprovações protegem a integridade criativa dos ativos da sua marca, mantendo os criadores de conteúdo envolvidos no processo de aprovação. Ao envolver as partes interessadas criativas (por exemplo, criadores de conteúdo e diretores criativos) no processo de revisão e aprovação, você garante que a saída final se alinhe à sua visão e identidade da marca.

* **Adesão às metas da campanha e aos requisitos legais**. O processo de aprovação ajuda a verificar se o conteúdo oferece suporte às metas da campanha. Ela garante que todo o material de marketing esteja em conformidade com os padrões legais e regulatórios, o que minimiza os riscos e possíveis problemas legais.

* **Integração com a Prova do Adobe Workfront**. Os usuários podem acessar os recursos robustos de revisão e aprovação da Workfront Proof no GenStudio for Performance Marketing. O conteúdo revisado no GenStudio for Performance Marketing é sincronizado com o Workfront Proof, e os comentários e o status da revisão são preservados. [Destaques da integração](/help/user-guide/approvals/proof-integration.md) identifica como o Proof estende o fluxo de trabalho de aprovação da GenStudio for Performance Marketing.

## Ciclo de vida de revisão e aprovação

As principais fases do fluxo de trabalho de revisão e aprovação incluem:

* [Solicitar revisão e aprovação do conteúdo criado](/help/user-guide/approvals/request-review.md). O GenStudio for Performance Marketing simplifica o processo de solicitação de aprovações e gerenciamento de aprovadores. Os modelos de aprovação do Workfront Proof podem simplificar ainda mais essa tarefa.

* [Revisar e editar conteúdo](/help/user-guide/approvals/review-and-edit.md). As notificações mantêm os criadores de conteúdo informados sobre as alterações e aprovações solicitadas. A revisão de conteúdo aciona um novo ciclo de aprovação automático.

* [Aprovar conteúdo](/help/user-guide/approvals/approve-content.md). Os aprovadores designados marcam o conteúdo como aprovado ou pronto para publicação.

* [Publicar conteúdo](/help/user-guide/approvals/publish-content.md). A publicação do conteúdo aprovado em [!DNL Content] o torna disponível para uso ou referência por outras pessoas na sua organização.

## Sobre rascunhos de conteúdo

_Rascunhos_ são versões preliminares de ativos ou experiências que não concluíram o processo de revisão e aprovação. O status de rascunho identifica onde o rascunho está no processo de revisão e aprovação. Uma ID de rascunho exclusiva identifica cada rascunho. Esta ID é válida até que um rascunho seja aprovado e publicado em [!DNL Content]. Comentários de revisão e aprovações para um rascunho são associados a essa ID de rascunho individual. Não há controle de versão para rascunhos de conteúdo do GenStudio.

Quando um rascunho conclui o processo de revisão e aprovação e é publicado em [!DNL Content], a ID do rascunho expira. O GenStudio for Performance Marketing não salva os comentários associados e o status de aprovação. O URL de rascunho não é mais válido.

O status Rascunho captura o estado do rascunho do conteúdo à medida que ele se move pelo processo de revisão e aprovação. O editor de conteúdo do GenStudio for Performance Marketing que criou o ativo sob revisão é notificado de qualquer alteração solicitada no rascunho ou nas aprovações. Os aprovadores alteram o status de rascunho para indicar se um rascunho precisa de revisão adicional ou se pode ser aprovado. Todos os aprovadores designados devem aprovar um ativo ou experiência antes que ela possa ser publicada.

Status de rascunho disponíveis:

**Notificado**: o editor de conteúdo iniciou o processo de revisão e aprovação notificando os aprovadores que um rascunho está pronto para revisão.
**Precisa do trabalho**: indica que um ou mais aprovadores solicitaram alterações no rascunho do conteúdo. O conteúdo neste status não pode ser salvo em [!DNL Content].
**Aprovado**: todos os aprovadores designados aprovaram o ativo ou a experiência. O editor de conteúdo agora pode adicionar metadados ao ativo ou experiência e salvá-los em [!DNL Content].

>[!NOTE]
>
> Os rascunhos correspondem a _provas_ para usuários da integração com o Workfront Proof. [Rascunhos e provas](/help/user-guide/approvals/proof-integration.md#drafts-and-proofs) diferem em termos de persistência e controle de versão.

## Funções de aprovação

_Revisores_ podem adicionar comentários, mas não podem aprovar conteúdo. A participação do revisor é útil, mas não essencial. _Os aprovadores_ devem aprovar o conteúdo para que ele possa avançar no processo de aprovação. A integração do Workfront Proof oferece suporte a uma variedade maior de funções de usuário.

## Notificações

As notificações no produto da GenStudio for Performance Marketing atualizam os aprovadores e editores de conteúdo em tempo real das alterações de status do ativo e `@mention` comentários. As notificações suportam iteração rápida por meio de vários ciclos de revisão, edição e aprovação.

Os editores de conteúdo e aprovadores podem se inscrever para receber essas notificações no Slack. Consulte [Assinar serviços no Experience Cloud](https://experienceleague.adobe.com/pt-br/docs/core-services/interface/services/customer-attributes/subscription).

As ações executadas pelos participantes da aprovação acionam notificações automáticas no produto e notificações por email. Ao iniciar um processo de aprovação, os aprovadores designados recebem notificações por email e no produto. Você é mantido no loop com notificações no produto e por email sempre que um aprovador adiciona `@mention` comentários ou toma uma decisão. As notificações incluem links para o rascunho do conteúdo.

Se tiver iniciado o processo de revisão e aprovação do conteúdo, você será notificado de todas as aprovações e revisará os comentários. No entanto, os aprovadores são notificados apenas de comentários que os incluem com um `@mention`.
