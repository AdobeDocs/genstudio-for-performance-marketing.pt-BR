---
title: Plug-in Photoshop para Adobe GenStudio for Performance Marketing
description: Saiba como instalar, configurar e usar o plug-in do Photoshop para GenStudio for Performance Marketing.
feature: Generative AI
role: User
source-git-commit: bb6b8de80bdf6089e70756bea5dbf3e6a7945052
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 1%

---

# Plug-in do Photoshop para GenStudio for Performance Marketing

O plug-in GenStudio for Performance Marketing Photoshop adiciona um painel ao Adobe Photoshop que permite gerar conteúdo na marca.

Esta página descreve como instalar e configurar o plug-in e como usá-lo.

Os recursos deste plug-in incluem:

* Faça logon em uma instância do GenStudio for Performance Marketing com uma Adobe ID
* Mapear campos de geração de conteúdo do GenStudio for Performance Marketing para camadas de texto em um documento do Photoshop
* Especificar uma marca, produto, perfil e prompt de texto para gerar conteúdo
* Opcionalmente, adicione uma imagem para substituir a imagem de modelo
* Visualizar variações de conteúdo geradas na marca
* Aplicar conteúdo gerado a camadas mapeadas no documento atual
* Criar traduções de conteúdo na marca
* Exportação gerada [!DNL Experiences] para o GenStudio for Performance Marketing

>[!VIDEO](https://video.tv.adobe.com/v/3478808?learn=on)

## Instalar o plug-in

Siga estas instruções para instalar o plug-in.

### Pré-requisitos

* aplicativo de desktop do Creative Cloud
* Photoshop, versão mínima 25.6.0

### Etapas de instalação

1. Baixe e atualize o plug-in do Creative Cloud Marketplace no Adobe Exchange.
1. Pesquise por **Plug-in do GenStudio para o Photoshop** no Adobe Exchange.
1. Siga as instruções para instalar o plug-in.

### Desinstalar o plug-in

1. Inicie o aplicativo de desktop do Creative Cloud.
1. Clique na opção **[!UICONTROL Plug-ins]**.
1. Clique nas reticências **[!UICONTROL (...)]** no cartão do GenStudio for Creative Cloud para ver as opções.
1. Escolha **Desinstalar**.

## Criar um modelo

Para gerar conteúdo, você precisa de um modelo do GenStudio for Performance Marketing criado a partir do documento do Photoshop.

Para criar um modelo pronto para GenStudio:

1. Abra um documento no Photoshop.
1. Identificar uma camada de texto para o conteúdo gerado.
1. Renomeie a camada com o formato de convenção de nome de campo: `{<name_of_generated_field>}`. Por exemplo, `{body}`, `{headline}`, `{cta}`.
1. Renomeie as camadas para todos os [campos exigidos pelo canal destinado ao tipo de modelo](../../user-guide/templates/customize-template.md#recognized-field-names).

| Canal | Campos obrigatórios para geração | Campos opcionais para geração |
| --- | --- | --- |
| LinkedIn | `{on_image_text}`, `{image}` | `{headline}`, `{introductory_text}`, `{cta}`, `{website_url}` |
| Meta | `{on_image_text}`, `{image}` | `{body}`, `{headline}`, `{cta}`, `{website_url}`, `{display_link}` |
| Exibir | `{body}`, `{image}` | `{headline}`, `{cta}`, `{website_url}` |

Observe que várias camadas podem compartilhar a mesma designação de campo, mas cada camada só pode especificar um campo. Por exemplo, se houver várias pranchetas no documento:

* Você pode especificar uma camada `{headline}` em cada prancheta.
* É possível especificar várias `{headline}` camadas em uma única prancheta.
* Você não pode especificar que uma única camada receba os nomes de campo `{headline}` e `{cta}`.

### Requisitos de tamanho do modelo

#### Modelos do Meta

Para publicações do Instagram e do Facebook:

* Largura: 1080 px (fixa)
* Altura: 1080 px ou 1350 px

Para histórias do Instagram e do Facebook:

* Largura: 1080 px (fixa)
* Altura: 1920 px

O plug-in decide o cromo da experiência gerada com base na altura do template.

#### Modelos de exibição

Não há requisito de tamanho fixo. Os modelos de exibição são compatíveis com qualquer tamanho.

#### Modelos do LinkedIn

* Largura: 1200 px (fixa)
* Altura: 1200 px, 628 px, 2292 px, 1800 px ou 1500 px

O documento está pronto para ser usado com o plug-in.

## Gerar novo conteúdo

1. Abra o Photoshop.
1. Abra um documento de modelo pronto para GenStudio que você tenha criado (veja as instruções acima) ou use o modelo inicial do GenStudio for Performance Marketing: `branding-template-acrobat-handlebars.psd`.
1. Abra o painel Plug-in em **[!UICONTROL Plug-ins]** > **[!UICONTROL GenStudio]**.
1. Clique no botão **[!UICONTROL Logon]**. Se for solicitada permissão para abrir uma URL, marque **Lembrar minha escolha** e clique em **[!UICONTROL Permitir]**.
1. Use o navegador da Web para fazer logon com um perfil que tenha acesso ao GenStudio for Performance Marketing.
1. Selecione o canal (Meta, LinkedIn ou Display) que se aplica ao modelo aberto.
   ![Seleção de canal](./ps-select-channel.png){width="300" zoomable="yes"}
1. Selecione o contexto [!DNL Brand], [!DNL Persona] e [!DNL Product] para a geração de conteúdo.
   ![Seleção de marca, persona e produto](./ps-select-box.png){width="300" zoomable="yes"}
1. Selecione o número de variações a serem produzidas.
1. Use o botão em **[!UICONTROL Selecionar conteúdo]** para procurar e escolher imagens dos seus ativos. Os 40 ativos adicionados mais recentemente aparecem primeiro e você pode pesquisar outros ativos. As imagens selecionadas são redimensionadas automaticamente para se ajustarem aos seus modelos.
1. Forneça um prompt de texto para o conteúdo na caixa **[!UICONTROL Prompt de Texto]**.
1. Clique no botão **[!UICONTROL Gerar]**. As variações aparecem em cartões no painel de plug-in.

Novos documentos são adicionados ao espaço de trabalho do Photoshop com conteúdo gerado aplicado aos campos de modelo. Esses documentos são nomeados com um sufixo de variação numerada.

## Traduzir conteúdo

Os usuários podem traduzir o conteúdo para idiomas compatíveis após a geração de cópia.

1. Clique em **[!UICONTROL Traduzir]** após gerar uma cópia de anúncio com o plug-in.
1. Selecione um ou mais idiomas para a tradução.
1. Clique no botão **[!UICONTROL Converter]**.

Novos documentos são adicionados ao espaço de trabalho do Photoshop com conteúdo gerado aplicado aos campos de modelo. Esses documentos são nomeados com um sufixo de variação numerada.

## Exportar experiências para o GenStudio

Os usuários podem selecionar a exportação após a geração ou tradução do conteúdo. Experiências exportadas são preenchidas na seção de conteúdo do GenStudio for Performance Marketing.

![Ativos exportados mostrados na seção Conteúdo](./content-assets.png){width="90%"}

## Solução de problemas

Considere essas práticas recomendadas e dicas se o texto ou as imagens não estiverem sendo substituídos em variações geradas.

### Campos mapeados

Se o texto ou as imagens não estiverem sendo substituídos, confirme se os campos estão mapeados corretamente com chaves `{}` (e não parênteses `()`).

### Confirmar se as fontes estão disponíveis

A fonte de um campo de texto deve estar disponível no computador para que a substituição ocorra durante a geração. Confirme se todas as fontes usadas no arquivo estão disponíveis no computador, especialmente se o arquivo foi criado no computador de outra pessoa.

### Exceções de mapeamento de campo

{{$include /help/_includes/field-mapping-exceptions.md}}
