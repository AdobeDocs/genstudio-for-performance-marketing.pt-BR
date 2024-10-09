---
title: Criar modelos acessíveis
description: Crie modelos no Adobe GenStudio for Performance Marketing que sejam capazes de alcançar mais do seu público-alvo e fornecer uma experiência ideal.
feature: Templates, Content
exl-id: eaaa5d9f-ad45-4fd0-826d-c250deb6d238
source-git-commit: ce08231cb723bec3d80a732837b72a435d3b552d
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Criar modelos acessíveis

O Adobe tem o compromisso de fornecer uma experiência ideal para todos os públicos-alvo. Consulte [Iniciativas de acessibilidade em Adobe](https://www.adobe.com/trust/accessibility/initiatives.html) para obter mais informações.

No GenStudio for Performance Marketing, você pode fazer upload de ativos e modelos que permitem a criação de conteúdo para uma variedade de experiências. A adesão aos padrões de acessibilidade ajuda seu conteúdo a alcançar o público-alvo máximo desejado.

Use as seguintes recomendações para preparar seus modelos usando os padrões de acessibilidade ideais.

## Texto alternativo

Fornecer alternativas em texto para conteúdo não textual, como imagens.

```html
<img alt="Collage of ideas, books, man holding giant pencil, computer" src="card-create-assets.png">
```

![Colagem de ideias, livros, homem segurando lápis gigante, computador](../../assets/card-create-assets.png){width="400"}

## Taxas de contraste

Forneça um contraste apropriado entre o texto e o plano de fundo. Use as seguintes taxas mínimas de contraste:

- Texto e imagens de texto: taxa de contraste de pelo menos 4.5:1
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
