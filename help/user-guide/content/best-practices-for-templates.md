---
title: Práticas recomendadas para modelos
description: Siga as práticas recomendadas ao usar modelos com o Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: e2b2e3b541c4d07530b9e725fceebabccbf6c84d
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Práticas recomendadas para usar modelos

Os templates reduzem significativamente o tempo e o esforço necessários para gerar novo conteúdo, fornecendo um ponto de partida que inclui layouts e elementos de design pré-configurados.

Use as seguintes recomendações ao usar modelos com o GenStudio for Performance Marketing:

1. Saber mais sobre [elementos do modelo](#know-about-template-elements)
1. Configure as [diretrizes de canal](#configure-channel-guidelines) para uma personalização eficaz do conteúdo
1. Crie com [padrões de acessibilidade](accessibility-for-templates.md) para obter uma experiência ideal
1. Siga as [diretrizes do modelo específico do canal](#follow-channel-specific-template-guidelines)

>[!TIP]
>
>Saiba mais sobre elementos e procedimentos básicos do modelo em [Trabalhar com modelos](use-templates.md). Veja em detalhes como [personalizar um modelo](customize-template.md) para usar na próxima campanha.

## Saber mais sobre elementos do modelo

Como prática recomendada, familiarize-se com as partes de um modelo. Cada tipo de template usa elementos diferentes para criar uma estrutura para a criação de conteúdo específico do canal. Para personalizar o modelo, use os nomes de campo no lugar desses elementos, onde é necessário que o GenStudio for Performance Marketing gere conteúdo.

Consulte [Elementos do modelo](use-templates.md#template-elements).

## Configurar diretrizes do canal

Definir diretrizes claras de canal é essencial para garantir que o conteúdo gerado esteja alinhado aos requisitos e objetivos da sua marca. As diretrizes de canal permitem especificar regras para elementos como tom, comprimento e estilo usados no modelo. Por exemplo, é possível definir uma contagem máxima de caracteres para o corpo ou exigir um estilo de call-to-action específico. Ao definir essas diretrizes antecipadamente, você reduz a necessidade de escrever instruções detalhadas em cada prompt de IA, simplificando o processo de geração de conteúdo e garantindo a consistência em seus emails.

Revise e defina as [diretrizes de canal](/help/user-guide/guidelines/brands.md#channel-guidelines) da sua marca para todos os campos principais do seu modelo. Se você não definir diretrizes, as [diretrizes de canal padrão](/help/user-guide/guidelines/brands.md#default-channel-guidelines) serão aplicadas, o que pode não refletir totalmente os requisitos da sua marca.

![Especificações do corpo](/help/assets/channel-email-body.png)

Saiba como as [diretrizes de Marcas, Produtos e Personalidades](/help/user-guide/guidelines/overview.md) influenciam o conteúdo gerado e como adaptá-lo às suas metas de marketing.

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
- [Meta ads](/help/user-guide/templates/meta-template.md)
