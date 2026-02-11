---
title: Plug-in Figma para Adobe GenStudio for Performance Marketing
description: Saiba como configurar e usar o plug-in do Figma para GenStudio for Performance Marketing.
feature: Generative AI
role: User
exl-id: 232fbbc6-c523-4525-8d26-a8ac8d62c035
source-git-commit: e585c6ff70198fe572b21252ab00b9b1ad368d02
workflow-type: tm+mt
source-wordcount: '1181'
ht-degree: 0%

---

# Plug-in Figma para GenStudio for Performance Marketing

O plug-in Figma do GenStudio for Performance Marketing adiciona um novo painel ao aplicativo Figma que permite gerar conteúdo na marca.

Esta página descreve como configurar e usar o plug-in.

Os recursos deste plug-in incluem:

* Mapeie elementos de texto Figma para campos GenStudio for Performance Marketing, como `headline`, `body`, `on_image_text` e muito mais.
* Gerar novo anúncio de exibição, LinkedIn ou Meta sob marca [!DNL Experiences] com base em marca, persona, produto e prompt de texto.
* Crie [!DNL Experiences] diretamente no documento Figma substituindo o texto em elementos Figma mapeados por valores gerados pelo GenStudio for Performance Marketing.
* reformular, encurtar, aumentar ou traduzir conteúdo existente com base em um prompt.
* Traduzir o [!DNL Experiences] gerado em vários idiomas.
* Exportação gerada [!DNL Experiences] para uma origem local como imagens niveladas.
* Exportação gerada [!DNL Experiences] para o GenStudio for Performance Marketing.
* Use as opções de plug-in que se adaptam aos elementos selecionados na tela do Figma.

>[!VIDEO](https://video.tv.adobe.com/v/3478814?captions=por_br&learn=on)

## Criar um modelo

O plug-in requer os dois primeiros níveis do seu documento do Figma para seguir esta convenção:

* **Seção** - Representa o projeto pai, que pode conter vários modelos.
* **Quadro** - Representa um modelo dentro de um projeto. O modelo pode ser preenchido com texto, imagens, componentes e outros elementos.

### Modelos do Meta

Estes tamanhos de modelo são compatíveis:

Para publicações no Instagram ou no Facebook:

* Largura: 1080 px (fixa)
* Altura: 1080 px ou 1350 px

Para histórias do Instagram ou do Facebook:

* Largura: 1080 px (fixa)
* Altura: 1920 px

O plug-in decide o cromo da experiência gerada com base na altura do template.

### Modelos de exibição

Não há requisito de tamanho fixo. Os modelos de exibição são compatíveis com qualquer tamanho.

### Modelos do LinkedIn

* Largura: 1200 px (fixa)
* Altura: 1200 px, 628 px, 2292 px, 1800 px ou 1500 px

### Mapeamento de funções do campo

O plug-in precisa entender os diferentes elementos do seu modelo, como título, corpo de texto ou imagem.

Para atribuir funções de elemento:

1. Selecione um elemento no modelo (texto, imagem etc.).
1. Use o menu suspenso para atribuir uma função.

O plug-in lembra desses mapeamentos para usar no conteúdo gerado. Uma função de campo\ pode ser mapeada para vários elementos de modelo.

![Mapeamento de função de campo](./field-role-mapping.png){width="600"}

### Exceções de mapeamento de campo

{{$include /help/_includes/field-mapping-exceptions.md}}

## Gerar novo conteúdo

Use a IA do GenStudio for Performance Marketing para gerar ou fazer variações em elementos nos modelos do Figma.

1. Se você usa o GenStudio Plugin Playground ou modelos já preparados, selecione o nó da seção que contém seus modelos de anúncios. Você pode fazer isso no painel **Camadas** ou clicando diretamente na seção na tela.
   ![Seleção ou variações de seção](./plugin-playground.png){width="500" zoomable="yes"}
1. Na janela de plug-in, insira um nome de projeto para as variações, escolha uma plataforma para o conteúdo e preencha as outras informações necessárias. Em seguida, clique no botão **[!UICONTROL Concluir Instalação]**.
   ![Janela do projeto de instalação](./setup-project.png){width="300" zoomable="yes"}
1. Selecione os [!DNL Brand], [!DNL Persona] e [!DNL Product] a serem usados para a geração de conteúdo.
1. Selecione o número de variações a serem produzidas (até oito).
1. Use o botão em **[!UICONTROL Selecionar conteúdo]** para procurar e escolher imagens dos seus ativos. Os 40 ativos adicionados mais recentemente aparecem primeiro e você pode pesquisar outros ativos. As imagens selecionadas são redimensionadas automaticamente para se ajustarem aos seus modelos.
1. Digite um prompt de texto. Cada campo na lista **[!UICONTROL Campos]** tem a opção **[!UICONTROL Ação]** definida como **[!UICONTROL Gerar]** para novo conteúdo.
1. Mapeie todas as funções de campo. Consulte [Mapeamento de função de campo](#field-role-mapping).
1. Clique no botão **[!UICONTROL Gerar]**.

## Traduzir ou gerar variações de cópia de anúncio a partir de conteúdo existente

Use a IA do GenStudio for Performance Marketing para gerar variações de cópia de anúncios ou traduzir modelos do Figma.

1. Selecione o nó da seção que contém seus modelos de anúncios. Você pode fazer isso no painel **Camadas** ou clicando diretamente na seção na tela.
   ![Seleção ou variações de seção](./plugin-playground.png){width="500" zoomable="yes"}
1. Na janela de plug-in, insira um nome de projeto para as variações e escolha uma plataforma para o conteúdo.
1. Em **[!UICONTROL Qual é a meta?]**, selecione **[!UICONTROL Gerar Variações]** ou **[!UICONTROL Traduzir]** e clique no botão **[!UICONTROL Concluir Instalação]**.
   ![Janela do projeto de instalação](./setup-project.png){width="300" zoomable="yes"}
1. Selecione os [!DNL Brand], [!DNL Persona] e [!DNL Product] a serem usados para a geração de conteúdo.
1. Selecione o número de variações a serem produzidas.
1. Use o botão em **[!UICONTROL Selecionar conteúdo]** para procurar e escolher imagens dos seus ativos. Os 40 ativos adicionados mais recentemente aparecem primeiro e você pode pesquisar outros ativos. As imagens selecionadas são redimensionadas automaticamente para se ajustarem aos seus modelos.
1. Digite um prompt de texto. Cada campo na lista **[!UICONTROL Campos]** tem a opção **[!UICONTROL Ação]** definida como **[!UICONTROL Gerar]** para novo conteúdo.
1. Mapeie todas as funções de campo. Consulte [Mapeamento de função de campo](#field-role-mapping).
1. Selecione cada tipo de campo para gerar variações ou traduzir no painel no lado esquerdo do plug-in e cole o conteúdo inicial em cada caixa de **[!UICONTROL Conteúdo inicial]**.
   ![Texto de exemplo na caixa Conteúdo Inicial](./initial-content-box.png){width="60%" zoomable="yes"}
1. Clique no botão **[!UICONTROL Gerar]**.

## Traduzir conteúdo após geração

1. Selecione uma geração que deseja traduzir.
   ![Selecionar geração](./select-generation.png){width="200" zoomable="yes"}
1. Escolha **[!UICONTROL Tradução]** e clique em **[!UICONTROL Traduzir]**.
1. Selecione o idioma ou idiomas de destino.
1. Clique em **[!UICONTROL Selecionar]**.

Os resultados da tradução incluem:

* Uma nova página é exibida com conteúdo traduzido.
* Cada tradução mostra o idioma ou localidade de destino.
* O conteúdo original permanece inalterado na página original.

![Resultados da tradução](./translation-results.png){width="60%" zoomable="yes"}

## Outras ações em campos de conteúdo após a geração

Quando você está editando o conteúdo existente em um campo, opções úteis aparecem no painel de plug-in.

![Opções de Ações do Plug-in](./figma-other-actions.png){width="300" zoomable="yes"}

As opções incluem:

* Altere o **[!UICONTROL Valor]** para alterar o texto diretamente. A alteração desse conteúdo se aplica automaticamente a todas as variações selecionadas.
* A IA pode executar várias opções de **[!UICONTROL Ação]**, incluindo:

| Ação | Descrição |
| --- | --- |
| **[!UICONTROL Gerar]** | Gerar uma nova variação do texto. |
| **[!UICONTROL Refrase]** | Gerar uma nova variação do texto. |
| **[!UICONTROL Encurtar]** | Gere uma variação mais curta do texto. |
| **[!UICONTROL Ampliar]** | Gere uma variação mais longa do texto. |

Depois de selecionar uma opção **[!UICONTROL Ação]**, gere novamente o conteúdo com o botão **[!UICONTROL Gerar novamente]**.

## Exportar experiências

As variações podem ser exportadas do Figma as GenStudio for Performance Marketing [!DNL Experiences].

1. Selecione o conteúdo a ser exportado na tela do Figma seguindo um destes procedimentos:
   * Selecione a seção de geração na tela e clique em **[!UICONTROL Marcar tudo para exportação]** no painel de plug-in.
     ![Seleção da seção de geração](./select-generation-section.png){width="200" zoomable="yes"}
   * Selecione uma geração individual na tela e clique em **[!UICONTROL Marcar para exportação]** no painel de plug-in.
     ![Seleção de geração individual](./select-generation.png){width="200" zoomable="yes"}
1. Selecione o item Exportar no menu da barra lateral.
   ![Botão Marcar para exportar exibido para um anúncio do Meta](./mark-for-export.png){width="60%" zoomable="yes"}
1. Selecione um destino.
1. Clique em **[!UICONTROL Exportar]** para exportar o conteúdo.

Um arquivo ZIP foi criado no painel de plug-in ou um link para **[!UICONTROL Abrir no GenStudio]** é exibido. Use o link do ZIP para escolher onde salvar o arquivo ou selecione **[!UICONTROL Abrir no GenStudio]**.

## Histórico de geração

O plug-in mantém um histórico de alterações para cada campo. Na página do modelo, escolha **[!UICONTROL Histórico de geração]** na barra lateral do plug-in.

![Opção de histórico de geração exibida para um anúncio de Meta](./generation-history.png){width="80%" zoomable="yes"}

## Solução de problemas

Considere essas práticas recomendadas e dicas se o texto ou as imagens não estiverem sendo substituídos em variações geradas.

### Campos mapeados

Se o texto ou as imagens não estiverem sendo substituídos, verifique se os campos foram mapeados para funções de campo do GenStudio na interface do usuário do plug-in. Consulte [Mapeamento de função de campo](#field-role-mapping).

### Confirmar se as fontes estão disponíveis

A fonte de um campo de texto deve estar disponível no computador para que a substituição ocorra durante a geração. Confirme se todas as fontes usadas no arquivo estão disponíveis no computador, especialmente se o arquivo foi criado no computador de outra pessoa.

### Considere o suporte à função no campo

Alguns canais só oferecem suporte à substituição em campos específicos. Esteja ciente das exceções para [mapeamento de função de campo](#field-role-mapping).
