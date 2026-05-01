---
title: Configurar troca de logotipo em modelos
description: Configure espaços reservados para o logotipo da marca em modelos para habilitar a troca de logotipo no  [!DNL GenStudio for Performance Marketing].
feature: Create Canvas
role: User
level: Intermediate
source-git-commit: 98cb7ba338878495e6d7b68f3b8c620abae10127
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 2%

---

# Configurar a troca de logotipos nos modelos

Este guia explica como configurar espaços reservados para o logotipo da marca em seus modelos para habilitar o [recurso de troca de logotipo](/help/user-guide/create/logo-swap.md) no [!DNL GenStudio for Performance Marketing]. Use essas diretrizes para garantir que o espaço reservado seja exibido corretamente em vários tamanhos de imagem e taxas de proporção.

## Configuração rápida

Use o código de modelo básico a seguir para a imagem de logotipo:

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="my-logo"
>
```

Obrigatório:

- `src="{{brand_logo}}"` — Habilita a funcionalidade de troca de logotipo.
- `style="{{defaultLogo}}"` — Aplica o estilo de borda do espaço reservado.

Opcional:

- `class="my-logo"` — Sua classe CSS personalizada para dimensionamento e estilo.

## Entender a borda do espaço reservado

Quando nenhum logotipo é selecionado, `{{brand_logo}}` contém uma imagem transparente de 1×1 pixel. O estilo `{{defaultLogo}}` aplica automaticamente uma estrutura de tópicos para que o espaço reservado fique visível:

```css
outline: clamp(1px, 0.1em, 5px) dashed #FFF;
```

Comportamento da borda:

- Aparece quando o espaço reservado padrão é exibido.
- Desaparece automaticamente após a troca de um logotipo.
- Dimensiona com base no tamanho da fonte principal.

### Dimensionamento de borda

A função `clamp()` adapta a espessura da estrutura de tópicos ao tamanho do modelo:

| Tamanho da fonte principal | Tamanho da estrutura de tópicos |
| --- | --- |
| 10px | 1px (min) |
| 16px | 1.6px |
| 24px | 2.4px |
| 32px | 3.2px |
| 50px+ | 5px (máx.) |

Fórmula: `0.1em` é igual a 10% do tamanho de fonte herdado, apertado entre `1px` e `5px`.

## Personalizar a borda do espaço reservado

Você pode substituir o outline padrão usando classes CSS. O estilo `{{defaultLogo}}` aplica a estrutura de tópicos de base, e sua classe pode personalizar cor, largura e estilo.

HTML de modelo:

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-custom-border"
>
```

Modelo CSS:

```css
.logo-custom-border {
  outline-color: #0066CC !important;
  outline-width: 2px !important;
  outline-style: dotted !important;
}
```

>[!NOTE]
>Os estilos de estrutura de tópicos personalizados afetam apenas o espaço reservado. Depois que um logotipo é trocado, todos os estilos de estrutura de tópicos são removidos automaticamente.

## Definir tamanho de logotipo recomendado

Para garantir que o espaço reservado esteja visível e impeça alterações de layout, defina o dimensionamento explícito na classe CSS:

HTML de modelo:

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-standard"
>
```

Modelo CSS:

```css
.logo-standard {
  width: 120px;
  height: 60px;
}
```

## Posicionamento do logotipo de controle

Use `object-fit` e `object-position` para controlar como o logotipo é dimensionado em seu contêiner.

### Logotipo centralizado (mais comum)

O logotipo é dimensionado para caber dentro de 150×80 pixels, centralizado tanto horizontal quanto verticalmente.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-centered"
>
```

```css
.logo-centered {
  width: 150px;
  height: 80px;
  object-fit: contain;
  object-position: center center;
}
```

### Logotipo alinhado à esquerda

O logotipo é dimensionado para caber, alinhado à borda esquerda, centralizado verticalmente.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-left"
>
```

```css
.logo-left {
  width: 200px;
  height: 60px;
  object-fit: contain;
  object-position: left center;
}
```

### Logotipo no canto superior direito

O logotipo é dimensionado para caber, posicionado no canto superior direito.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-top-right"
>
```

```css
.logo-top-right {
  width: 100px;
  height: 100px;
  object-fit: contain;
  object-position: right top;
}
```

## Exemplos completos

### Configuração mínima

```html
<img src="{{brand_logo}}" style="{{defaultLogo}}">
```

>[!NOTE]
>Essa configuração funciona, mas o espaço reservado pode ser quase invisível porque a imagem transparente de 1×1 pixel é recolhida para seu tamanho natural. Use uma classe CSS com `width` e `height` para um espaço reservado visível.

### Configuração recomendada

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="brand-logo"
>
```

```css
.brand-logo {
  width: 120px;
  height: 60px;
  object-fit: contain;
  object-position: center center;
}
```

### Configuração avançada com uma borda personalizada

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="sponsor-logo"
>
```

```css
.sponsor-logo {
  width: 180px;
  height: 90px;
  object-fit: contain;
  object-position: left center;
  outline-color: #0066CC !important;
  outline-width: 2px !important;
  outline-style: solid !important;
}
```

### Configuração flexível com limites de tamanho

Use as propriedades `min-*` e `max-*` para modelos responsivos ou tamanhos variados de logotipo.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-flexible"
>
```

```css
.logo-flexible {
  min-width: 20px;
  min-height: 20px;
  max-width: 200px;
  max-height: 100px;
  object-fit: contain;
  object-position: center center;
}
```

Como funciona:

- `min-width` e `min-height` mantêm o espaço reservado visível.
- `max-width` e `max-height` impedem que logotipos grandes quebrem o layout.
- O logotipo é dimensionado proporcionalmente dentro desses limites.

## Referência de propriedades CSS

| Categoria | Propriedade | Valor | Propósito |
| --- | --- | --- | --- |
| Obrigatório (HTML) | `src` | `{{brand_logo}}` | Ativa a funcionalidade de troca de logotipo. |
| Obrigatório (HTML) | `style` | `{{defaultLogo}}` | Aplica o outline do espaço reservado. |
| Recomendado (classe CSS) | `width` | `120px` | Define a largura máxima do logotipo. |
| Recomendado (classe CSS) | `height` | `60px` | Define a altura máxima do logotipo. |
| Recomendado (classe CSS) | `object-fit` | `contain` | Dimensiona o logotipo sem cortar. |
| Recomendado (classe CSS) | `object-position` | `center center` | Controla o alinhamento do logotipo. |
| Opcional (classe CSS) | `outline-color` | `#FF0000` | Altera a cor da estrutura de tópicos. |
| Opcional (classe CSS) | `outline-width` | `3px` | Altera a espessura do contorno. |
| Opcional (classe CSS) | `outline-style` | `solid` | Altera o estilo da estrutura de tópicos. |
| Dimensionamento flexível (classe CSS) | `min-width` | `20px` | Garante a visibilidade do espaço reservado. |
| Dimensionamento flexível (classe CSS) | `min-height` | `20px` | Garante a visibilidade do espaço reservado. |
| Dimensionamento flexível (classe CSS) | `max-width` | `200px` | Evita o excesso de capacidade. |
| Dimensionamento flexível (classe CSS) | `max-height` | `100px` | Controla os limites do layout. |

## Práticas recomendadas

Faça:

- Sempre inclua `{{brand_logo}}` e `{{defaultLogo}}`.
- Defina `width` e `height` para que o espaço reservado fique visível.
- Use as classes CSS para dimensionar e personalizar a estrutura de tópicos.
- Use `object-fit: contain` para preservar as taxas de proporções de logotipo.
- Teste com logotipos de diferentes tamanhos e proporções.

Não:

- Use `border` em vez de `outline` (a borda não será ocultada automaticamente).
- Coloque propriedades de dimensionamento em estilos integrados.
- Omitir restrições de tamanho (o espaço reservado é renderizado em 1×1 pixels).
- Usar `object-fit: cover` (pode cortar logotipos).

## Solução de problemas

Borda não visível:

- Certifique-se de que `style="{{defaultLogo}}"` esteja incluído.
- Confirme se `width` e `height` estão definidos na classe CSS.

O espaço reservado é muito pequeno (1px):

- Adicione `width` e `height` explícitos à sua classe CSS.

A borda não desaparece após a troca:

- Use propriedades de estrutura de tópicos em sua classe CSS, não `border`.

O logotipo é cortado:

- Use `object-fit: contain` em vez de `cover`.

Logotipo muito pequeno ou muito grande:

- Ajuste `width` e `height` na sua classe CSS.

A borda personalizada não mostra:

- Confirmar se `{{defaultLogo}}` está no atributo `style`.
- Coloque as propriedades `outline-*` personalizadas na classe CSS.
