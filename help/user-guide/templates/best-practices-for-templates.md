---
title: Práticas recomendadas para modelos
description: Siga as práticas recomendadas ao usar modelos com o Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
TQID: https://experienceleague.adobe.com/fiKHSZ-YFZ2gSD5iZ-aKaZtsC49Mrj1dqHpHqtbXZVM
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: cc72dcf1-72e1-48cc-b434-e7c27d62d67cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 777
ht-degree: 0%

---

# Práticas recomendadas para usar modelos

Os templates reduzem significativamente o tempo e o esforço necessários para gerar novo conteúdo, fornecendo um ponto de partida que inclui layouts e elementos de design pré-configurados.

Siga as seguintes recomendações ao usar modelos com o GenStudio for Performance Marketing:

1. Saber mais sobre [elementos do modelo](#know-about-template-elements)
1. Configure as [diretrizes de canal](#configure-channel-guidelines) para uma personalização eficaz do conteúdo
1. Crie com [padrões de acessibilidade](accessibility-for-templates.md) para obter uma experiência ideal
1. Siga as [diretrizes do modelo específico do canal](#follow-channel-specific-template-guidelines)

>[!TIP]
>
>Saiba mais sobre as noções básicas dos elementos e procedimentos do modelo em [Trabalhar com modelos](use-templates.md). Veja em detalhes o [personalização de um modelo](customize-template.md) para obter instruções específicas sobre como usá-lo na próxima campanha.

## Usar os elementos de modelo corretos

Cada tipo de template usa elementos diferentes para criar uma estrutura para a criação de conteúdo específico do canal. [Familiarize-se com as partes de um modelo](use-templates.md#template-elements) e inclua os melhores elementos para seu conteúdo e tipo de modelo.

Ao personalizar o modelo, use os nomes de campo no lugar desses elementos, onde é necessário que o GenStudio for Performance Marketing gere conteúdo.

Consulte [Elementos do modelo](use-templates.md#template-elements).

## Uso do texto de espaço reservado em modelos

O texto para espaço reservado pode ajudar a definir a sintaxe ou a estrutura do conteúdo a ser preenchido posteriormente em um modelo por um usuário. Por exemplo, {first_name}.{last_name}@email.etc. para definir um endereço de email. No entanto, alguns delimitadores comuns já estão reservados para outros significados no GenStudio for Performance Marketing:

❌ `< >` - Em uso para marcas HTML.
❌ `{{ }}` - Em uso para expressões Handlebar.

Use colchetes simples (sejam retos ou curvos) para indicar o texto do espaço reservado e evitar confusão com as tags existentes.

✅ `{first_name}` - Espaço reservado para nome.

## Configurar diretrizes do canal

Definir diretrizes claras de canal é essencial para garantir que o conteúdo gerado esteja alinhado aos requisitos e objetivos da sua marca. As diretrizes de canal permitem especificar regras para elementos como tom, comprimento e estilo usados no modelo. Por exemplo, é possível definir uma contagem máxima de caracteres para o corpo ou exigir um estilo de call-to-action específico. Ao definir essas diretrizes antecipadamente, você reduz a necessidade de escrever instruções detalhadas em cada prompt de IA, simplificando o processo de geração de conteúdo e garantindo a consistência em seus emails.

Revise e defina as [diretrizes de canal](/help/user-guide/guidelines/brands.md#channel-guidelines) da sua marca para todos os campos principais do seu modelo. Se você não definir diretrizes, as [diretrizes de canal padrão](/help/user-guide/guidelines/brands.md#default-channel-guidelines) serão aplicadas, o que pode não refletir totalmente os requisitos da sua marca.

![Especificações do corpo](/help/assets/channel-email-body.png)

Saiba como as [diretrizes de Marcas, Produtos e Personalidades](/help/user-guide/guidelines/overview.md) influenciam o conteúdo gerado e como adaptá-lo às suas metas de marketing.

## Carregamento de imagens para modelos

As imagens usadas em modelos devem vir do repositório de conteúdo e precisam ser carregadas corretamente para garantir que a imagem seja exibida com precisão.

Quando um modelo apresenta uma imagem de borda a borda (sangria completa), a imagem selecionada é redimensionada automaticamente para se ajustar às dimensões completas do modelo. No entanto, se a imagem não corresponder à taxa de proporção do modelo, ela será cortada para se ajustar às dimensões do modelo e poderá não ser exibida conforme esperado.

Não há nenhuma funcionalidade de &quot;ajuste automático&quot; para imagens incluídas em modelos.

Para resolver o corte da imagem, os usuários devem definir a proporção da imagem a ser usada no modelo quando ele for carregado no repositório de conteúdo. Ao fazer upload de um modelo aprovado:

1. [Continue com o processo de carregamento do modelo](/help/user-guide/templates/use-templates.md#add-a-template) até chegar à página **[!UICONTROL Adicionar detalhes]**.

2. Defina a proporção da imagem a ser usada no modelo em **[!UICONTROL Largura do anúncio (px)]** e **[!UICONTROL Altura do anúncio (px)]**. Isso definirá a janela de imagem para a seção do modelo que exibe a imagem.

3. Na seção **[!UICONTROL Mais detalhes]**, selecione a lista suspensa **[!UICONTROL Tamanho da imagem]** e escolha _Cortar para um tamanho fixo_.
   ![Cortado para um tamanho fixo](images/crop-to-fixed-size.png "Cortado para um tamanho fixo"){width="80%"}

Para determinar o tamanho e a proporção de uma imagem no navegador:

1. Inspecione a imagem.
   - No Windows/Linux:
      - Pressione F12.
   - No macOS:
      - Pressione Command + Option + I.

1. Passe o mouse sobre a imagem.

1. Observe a taxa de proporção. Use essa opção para definir a proporção da imagem no modelo.

Quando esses detalhes não são aplicados durante o upload, presume-se que a imagem seja a proporção inteira do modelo e as imagens que não corresponderem exatamente a essa proporção aparecerão cortadas.

![Imagem cortada em um anúncio de exibição](images/cropped-display.png "Recorte de imagem"){width="60%"}

**❌Imagem cortada em um modelo de anúncio de exibição**

![Imagem exibida em um anúncio de exibição](images/full-fit.png "Imagem exibida em anúncio de exibição"){width="60%"}

**✅Imagem totalmente exibida**

## Seguir as diretrizes do modelo específico do canal

Ao criar modelos, verifique se eles atendem aos requisitos específicos do canal pretendido. Crie modelos que acomodam os requisitos visuais e de layout de cada canal. Há diretrizes gerais que se aplicam a qualquer modelo, como:

- Usar HTML limpo e responsivo e CSS em linha
- Usar fontes do Adobe ou Google
- **não** usar o JavaScript

{{note-css-effects}}

Consulte mais dicas e restrições ao trabalhar com cada tipo de modelo para garantir o desempenho ideal:

- [Emails](/help/user-guide/templates/email-template.md)
- [Anúncios de exibição e banner](/help/user-guide/templates/display-template.md)
- [LinkedIn](/help/user-guide/templates/linkedin-template.md)
- [Anúncios do Meta](/help/user-guide/templates/meta-template.md)
