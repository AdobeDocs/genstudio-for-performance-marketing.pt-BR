---
title: Criar uma experiência de anúncio no ChatGPT
description: Saiba como criar, revisar, publicar e ativar experiências de mídia paga no ChatGPT no Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 8%
---

# Criar uma experiência de anúncio no ChatGPT

Use o [[!DNL Create]](/help/user-guide/create/overview.md) no [!DNL GenStudio for Performance Marketing] para criar **anúncios de ChatGPT** como experiências de mídia paga, desde diretrizes e ativos até geração, verificações de marca e canal, aprovação, publicação no [!DNL Content] e ativação no mesmo fluxo do [!DNL Activate] usado para canais como o Meta e o Google Campaign Manager 360.

Antes de começar, [adicione diretrizes](/help/user-guide/guidelines/add-guidelines.md) onde necessário e revise [solicitações efetivas](/help/user-guide/effective-prompts.md) para que suas solicitações de título produzam variantes fortes.

## Pré-requisitos

Você precisará ser configurado de acordo com esses pré-requisitos para criar ou ativar anúncios de ChatGPT no [!DNL GenStudio for Performance Marketing].

### Acesso e funções

* Você tem uma função de **Editor** ou superior em [!DNL GenStudio for Performance Marketing]. Consulte [Funções e permissões de usuário](/help/user-guide/user-roles.md).
* Você tem uma **Conta de anúncio OpenAI** e uma **Chave de API** dessa conta.
* Uma conta do **ChatGPT Ads** está conectada ao [!DNL GenStudio for Performance Marketing].

Para criar uma chave de API no OpenAI Ads Manager:

1. No OpenAI Ads Manager, vá para **[!UICONTROL Configurações]** > **[!UICONTROL Chaves de API]** > **[!UICONTROL Criar nova chave]**.

Para conectar sua conta do ChatGPT Ads em [!DNL GenStudio for Performance Marketing]:

1. Na área inferior esquerda, clique em **[!UICONTROL Mais]** > **[!UICONTROL Configurações]** > **[!UICONTROL ChatGPT]** > **[!UICONTROL Conectar]** > **[!UICONTROL Adicionar Conta]**.
1. Insira o nome da sua conta de anúncio OpenAI, cole sua chave de API e clique em **[!UICONTROL Adicionar conta]**.

Sua conta de anúncio é conectada quando o fluxo é concluído com sucesso.

### Criar configuração

* **[!DNL Brands]**, **[!DNL Products]** e **[!DNL Personas]** estão configurados para que o aplicativo possa gerar uma cópia da marca. Consulte [Visão geral das diretrizes](/help/user-guide/guidelines/overview.md).
* As imagens que você deseja usar estão disponíveis em [[!DNL Content]](/help/user-guide/content/overview.md).

## Gerar um anúncio de ChatGPT

Você cria anúncios ChatGPT como experiências de mídia paga no espaço de trabalho [!DNL Create].

### Iniciar uma experiência de ChatGPT

Para abrir a criação do ChatGPT:

1. Vá para **[!UICONTROL Criar]** > **[!UICONTROL ChatGPT]**. Você não seleciona modelos para o ChatGPT; um único layout de anúncio é usado.
   ![Bloco ChatGPT no Criar fluxo de trabalho](./create-chatgpt-clp.png){width="60%"}
1. Na _Tela_, faça seleções para **[!DNL Brand]**, **[!DNL Product]**, **[!DNL Persona]** e **Idioma**.
1. Selecione uma imagem de [!DNL Content].
1. Digite um prompt para a cópia do título do ChatGPT.
1. Clique em **[!UICONTROL Gerar]**.

[!DNL GenStudio for Performance Marketing] **gera quatro** variantes criativas.

É possível:

* Use **[!UICONTROL Regenerar]** ou **[!UICONTROL Refinar]** para ajustar o tom, o comprimento ou a ênfase.
* Editar texto diretamente na _Tela_.
* Use **[!UICONTROL Swap]** para escolher uma imagem alternativa de [!DNL Content].

Consulte [Gerenciar variantes](/help/user-guide/create/manage-variants.md) para saber mais sobre como editar experiências geradas.

### Executar verificações de marca e canal

Antes de salvar ou enviar a experiência para revisão, valide a cópia e o layout em relação às regras de marca e canal.

Para executar verificações de conteúdo:

1. Clique em **[!UICONTROL Verificação de conteúdo]** (verificações de marca e canal).
1. Revise os resultados da validação no painel [_Verificação de conteúdo_](/help/user-guide/guidelines/brand-validation.md#content-check-panel).
1. Resolva quaisquer problemas sinalizados (por exemplo, comprimento da cópia ou texto denso na tela) editando variantes ou regenerando conforme necessário.

Consulte [Validação da marca](/help/user-guide/guidelines/brand-validation.md).

## Salvar um anúncio de ChatGPT em [!DNL GenStudio for Performance Marketing]

Salvar move sua experiência de anúncio de ChatGPT para [!DNL Content] para que ela possa ser revisada, reutilizada e ativada.

Há dois estados:

* **Experiência de rascunho**: trabalho em andamento e não aprovado.
* **Experiência publicada**: aprovada e disponível em [!DNL Content] para ativação.

### Enviar para revisão

1. No cabeçalho da experiência, clique em **[!UICONTROL Solicitar revisão]**.
1. Selecionar aprovadores (por exemplo, parte interessada de marca, jurídica ou desempenho).
1. Opcional: adicionar uma observação em **[!UICONTROL Configurações]**.
1. Clique em **[!UICONTROL Enviar para revisão]**.

Os aprovadores podem exibir a experiência do ChatGPT, os resultados de verificação da marca e do canal e **[!UICONTROL Aprovar]** ou solicitar alterações.

Consulte [Solicitar revisão e aprovação](/help/user-guide/approvals/request-review.md) e [Revisões e aprovações](/help/user-guide/approvals/overview.md).

### Publicar no conteúdo

Após todas as aprovações necessárias, publique em [!DNL Content]:

1. Clique em **[!UICONTROL Publicar no Conteúdo]**.
1. Confirme os metadados, por exemplo, nome da campanha ou ativação, região, idioma, persona, estágio do funnel e **Canal: ChatGPT**.
1. Clique em **[!UICONTROL Publicar]**.

O anúncio do ChatGPT aparece em [!DNL Content], detectável com filtros como canal ou campanha, e está pronto para seleção em [!DNL Activate].

Consulte [Publicar conteúdo aprovado](/help/user-guide/approvals/publish-content.md) e [[!DNL Content] visão geral](/help/user-guide/content/overview.md).

## Ativar um anúncio de ChatGPT

A ativação do ChatGPT usa o mesmo módulo [[!DNL Activate]](/help/user-guide/activation/overview.md) que outros canais pagos. Consulte [Ativar um anúncio de ChatGPT](/help/user-guide/activation/activate-chatgpt-ad.md) para obter os pré-requisitos e os campos de configuração específicos do ChatGPT.
