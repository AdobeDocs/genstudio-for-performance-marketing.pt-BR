---
title: Criar Modelos Acessíveis
description: Crie modelos no Adobe GenStudio for Performance Marketing que sejam capazes de alcançar mais do seu público-alvo e fornecer uma experiência ideal.
feature: Media Templates
exl-id: eaaa5d9f-ad45-4fd0-826d-c250deb6d238
TQID: https://experienceleague.adobe.com/b56YHJsOAunGenV-F3u7Y2mo56f6CnnX4qPXyzczPJY
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 369
ht-degree: 0%

---

# Criar modelos acessíveis

A Adobe tem o compromisso de fornecer uma experiência ideal para todos os públicos-alvo. Consulte [Iniciativas de acessibilidade no Adobe](https://www.adobe.com/trust/accessibility/initiatives.html) para obter mais informações.

No GenStudio for Performance Marketing, você pode fazer upload de ativos e modelos que permitem a criação de conteúdo para uma variedade de experiências. A adesão aos padrões de acessibilidade ajuda seu conteúdo a alcançar o público-alvo máximo desejado.

Use as seguintes recomendações para preparar seus modelos usando os padrões de acessibilidade ideais.

## Texto alternativo

Fornecer alternativas em texto para conteúdo não textual, como imagens.

```html
<img alt="Collage of ideas, books, man holding giant pencil, computer" src="card-create-assets.png">
```

![Colagem de ideias, livros, homem segurando lápis gigante, computador](/help/assets/card-create-assets.png){width="400"}

Ao personalizar seu modelo, use espaços reservados para o conteúdo para os atributos `alt` e `aria-label`:

- [Texto alternativo](/help/user-guide/templates/customize-template.md#alternative-text)
- [Rótulo de acessibilidade](/help/user-guide/templates/customize-template.md#accessibility-label)

## Fontes

Use fontes fáceis de ler. Por exemplo, as fontes Sans Serif têm uma aparência limpa, semelhante a blocos, o que contribui para uma maior legibilidade.

Forneça um contraste apropriado entre o texto e o plano de fundo. Evite usar cores de fonte que produzem texto escuro em um plano de fundo escuro e texto claro em um plano de fundo claro. Considere as diretrizes de contraste para obter uma proporção ideal:

- Texto e imagens de texto: taxa de contraste de pelo menos 4,5:1
- Texto e imagens grandes de texto em grande escala: taxa de contraste de pelo menos 3:1

## Finalidade do link (somente link)

Crie um texto de link claro que descreva a finalidade e o local do link.

Por exemplo, usar o texto do link como &quot;Clique aqui&quot; ou &quot;Leia mais&quot; não descreve claramente a finalidade do link:

```html
<a href="product-site.html">Click here</a>
```

Como prática recomendada, você deve usar um texto que descreva claramente para onde o link vai. Um exemplo melhor pode usar o título da fonte do link e a finalidade:

```html
<a href="product-site.html">Explore Product Site</a>
```

## Idioma

Muitos produtos e serviços usam a linguagem de forma criativa ou única. Evite jargões, frases longas e frases complexas. Use um idioma claro, conciso e fácil de ler, compatível com seu público-alvo.

- Use descrições claras, definições em linha ou exemplos relacionáveis quando possível. Pode ser difícil traduzir um vernáculo único.

- Soletre ou vincule a uma definição para as primeiras instâncias de um acrônimo ou abreviação. Pode ser difícil traduzir abreviações.

- Use elementos visuais para complementar texto ou ideias complexas quando possível.
