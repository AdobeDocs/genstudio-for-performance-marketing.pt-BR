---
title: Criar experiência de anúncio do Meta - Anúncios do carrossel
description: Saiba como criar experiências de anúncio de carrossel do Meta com vários cartões, gerenciar cartões e gerar conceitos sobre a marca no [!DNL GenStudio for Performance Marketing].
role: User
source-git-commit: 1b407c1c66a2426b21cbbf423774ebdff16a7dec
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 1%
---

# Crie uma experiência de anúncio no carrossel do Meta

Um anúncio de carrossel do Meta é um formato de anúncio pago que mostra de dois a dez cartões deslizantes, cada um com sua própria imagem ou vídeo, título e link.

Esta página aborda as etapas específicas dos anúncios no carrossel. Para as etapas compartilhadas que esta página não repete, como escolher um modelo, adicionar parâmetros, revisar variantes e publicar, consulte [Criar uma experiência de anúncio do Meta](/help/user-guide/create/create-meta-ad.md).

## Pré-requisitos

Antes de criar um anúncio no carrossel, verifique se você tem um modelo cujas páginas compartilham uma taxa de proporção, 1:1 ou 4:5. Cada página de modelo se torna um cartão. Para obter mais informações, consulte [diretrizes de modelos de anúncio do Meta](/help/user-guide/templates/meta-template.md).

## Escolha o formato do carrossel

Depois de selecionar um modelo e abrir a Tela de Pintura, escolha o formato do carrossel na gaveta do prompt.

1. No painel _[!DNL Create your ads]_, expanda_[!UICONTROL  Parâmetros ]_.
1. No menu suspenso **[!UICONTROL Formatar]**, selecione **[!UICONTROL Anúncio do carrossel]**.

   ![O painel Criar seus anúncios com a lista suspensa Formatar definida como Anúncio do carrossel e uma lista de cartões](./carousel-format-cards.png){width="70%" zoomable="yes"}

Se você começar com um modelo de página única, o [!DNL GenStudio for Performance Marketing] duplica a página para atingir o mínimo de dois cartões. Se nem todas as páginas de modelo compartilharem uma taxa de proporção, a opção de formato será bloqueada até que você use um modelo com uma taxa de proporção consistente.

## Gerenciar cartões

Crie o conjunto de cartões na gaveta do prompt antes de gerar. Para adicionar mais cartões, duplique um cartão existente.

* **Para duplicar um cartão**, selecione **[!UICONTROL Duplicar]** nas opções de cartão.
* **Para reordenar cartões**, arraste um cartão pela alça para uma nova posição.
* **Para excluir um cartão**, selecione **[!UICONTROL Excluir]** nas opções de cartão. Não é possível excluir os dois últimos cartões, pois um carrossel requer pelo menos dois cartões.

Para cada cartão, selecione uma imagem e, se necessário, defina um produto por cartão que substitua o produto principal. Selecione uma imagem por cartão individualmente. As URLs de destino por cartão são definidas posteriormente em [!DNL Activate]. Para obter mais informações, consulte [Ativar um anúncio Meta](/help/user-guide/activation/activate-meta-ad.md).

## Gravar um prompt do carrossel

Seu prompt sinaliza a intenção do carrossel, portanto, descreva como os cartões se relacionam entre si. A cópia do carrossel pode seguir uma das duas abordagens:

* **Modular:** cada cartão é um anúncio independente e nenhuma cópia flui entre cartões. Use essa abordagem para um conjunto de mensagens relacionadas, mas independentes, como vários produtos.
* **Sequencial:** a cópia se conecta entre cartões para contar uma história, uma sequência passo a passo ou uma instrução. Use essa abordagem quando as placas forem criadas uma na outra.

Você também pode descrever se o carrossel apresenta um único produto ou vários produtos, além de qualquer detalhe por cartão.

Por exemplo, este prompt descreve um carrossel modular com vários produtos:

```properties
Create a multi-product carousel for our end-of-summer skincare sale. For each card, lead with the product's core benefit and emphasize the sale value.
```

Este prompt descreve um carrossel sequencial que conta uma história em cinco cartões:

```properties
Create a narrative carousel for our compliance alert-management platform. Start with shared intro text about the cost of alert fatigue. Across five cards, build the story: rising review costs, too many low-value alerts, false positives as the hidden cost driver, a solution that cuts false positives by more than 50%, and a closing learn-more call to action.
```

Para fundamentos de prompt, consulte [Gravar prompts efetivos](/help/user-guide/effective-prompts.md).

## Gerar e revisar conceitos

Depois de configurar os cartões e o prompt, gere o carrossel e revise os resultados.

1. Selecione **[!UICONTROL Gerar]**.

   [!DNL GenStudio for Performance Marketing] gera quatro conceitos de carrossel. Cada conceito é um carrossel completo com várias placas e sua própria pontuação de marca.

   ![Quatro conceitos de carrossel gerados, cada um com uma pontuação de marca e um botão Editar](./carousel-concepts.png){width="80%" zoomable="yes"}

1. Selecione um conceito e, em seguida, **[!UICONTROL Editar]** para abri-lo para edição.
1. Use as setas para se mover entre cartões e edite o texto ou selecione **[!UICONTROL Trocar]** para alterar a imagem de um cartão. Para obter mais informações sobre edição, consulte [Gerenciar variantes](/help/user-guide/create/manage-variants.md).

Se você reordenar os cartões antes de gerar, a Tela será atualizada imediatamente. Se você reordenar cartões na gaveta de prompt depois de gerar, a alteração será aplicada somente depois de gerar novamente e um aviso de regeneração será exibido.

## Entender campos compartilhados e por cartão

Alguns campos do carrossel se aplicam a cada cartão individualmente, e outros se aplicam a todo o anúncio. A tabela a seguir descreve como cada campo se comporta para os anúncios do carrossel do Meta.

| Campo | Escopo |
|---|---|
| Título | Por cartão |
| Descrição | Por cartão, opcional, definido em [!DNL Activate] |
| Call to action | Compartilhado no anúncio |
| Texto primário | Compartilhado no anúncio |
| Mídia | Por placa (imagem, vídeo ou mista) |
| Texto na imagem | Por cartão |
| URL de destino | Por cartão, definido em [!DNL Activate] |

## Publicar, exportar e ativar

Quando o carrossel estiver pronto, publique-o e exporte-o da mesma forma que faz para outros anúncios do Meta. Um carrossel é armazenado como uma única experiência que corresponde a um conceito. A exportação fornece um arquivo CSV e a mídia de cartão. Consulte [[!DNL Content]](/help/user-guide/content/overview.md) para saber como as experiências publicadas são armazenadas. Para ativar o carrossel no Meta, consulte [Ativar um anúncio do Meta](/help/user-guide/activation/activate-meta-ad.md).
