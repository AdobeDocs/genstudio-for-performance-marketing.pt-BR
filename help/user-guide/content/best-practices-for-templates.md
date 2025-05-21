---
title: Práticas recomendadas para modelos
description: Siga as práticas recomendadas ao usar modelos com o Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: dc958a831e3fa26cfc18f7c1a5febd0662102d43
workflow-type: tm+mt
source-wordcount: '982'
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

Configure as diretrizes do canal para cada marca antes de usar os modelos na GenStudio for Performance Marketing. As diretrizes de canal influenciam diretamente o tipo de conteúdo gerado ao usar o template. Por exemplo, você pode definir limites de caracteres no corpo de um email.

![Especificações do corpo](/help/assets/channel-email-body.png)

Consulte [diretrizes do canal](/help/user-guide/guidelines/brands.md#channel-guidelines).

## Seguir as diretrizes do modelo específico do canal

Ao criar modelos, verifique se eles atendem aos requisitos específicos do canal pretendido. Crie modelos que acomodam os requisitos visuais e de layout de cada canal. Há diretrizes gerais que se aplicam a qualquer modelo, como:

- Usar HTML limpo e responsivo e CSS em linha
- Usar fontes do Adobe ou Google
- **não** usar o JavaScript

{{note-css-effects}}

Considere as seguintes dicas e restrições ao trabalhar com cada tipo de modelo para garantir o desempenho e a compatibilidade ideais:

>[!BEGINTABS]

>[!TAB Email]

Siga estas práticas recomendadas de design ao personalizar modelos de email para funcionar com o GenStudio for Performance Marketing:

- Usar fontes do Adobe ou Google
- Usar HTML limpo e responsivo e CSS em linha
- **não** usar o JavaScript
- **não** usar largura fixa no corpo ou contêiner
- **não** usar a codificação base64 para imagens porque ela pode aumentar significativamente o tamanho do modelo

**Restrições**:

- Os emails de marketing podem ter 0, 2 ou 3 [seções](customize-template.md#sections-or-groups):
   - Um modelo básico (seções zero) pode gerar um único conjunto de elementos de modelo, o que não requer a convenção de nomenclatura de grupo.
   - Um modelo complexo (várias seções) pode gerar até três conjuntos de elementos de modelo, o que requer que você siga a convenção de nomenclatura de grupo: (`groupname_fieldname`)
- O número máximo de campos permitidos em um modelo é 20
- O tamanho máximo do arquivo do HTML é 102 KB

**Nomes de campos reconhecidos**:

Para email, o campo `subject` é incluído automaticamente. Use espaços reservados para o conteúdo para os seguintes campos:

- `pre_header` (rich text não habilitado)
- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (selecionado no JPEG de conteúdo, PNG ou GIF)

Consulte [Espaços reservados para conteúdo](customize-template.md#content-placeholders) para entender mais sobre o uso de nomes de campo em modelos.

>[!TAB Meta-anúncio]

Siga estas práticas recomendadas de design ao personalizar modelos de metadados para funcionar com o GenStudio for Performance Marketing:

- Usar largura de 360 pixels para layouts de coluna
- Use uma resolução mínima de 1080 x 1080 pixels para imagens
- **não** usar tamanho de fonte relativo
- Fazer **não** definir viewport
- **não** usar o JavaScript
- **não** substitua um elemento HTML no CSS
- Usar a marca `<img>` em vez de `background-image`
- Usar o mascaramento para melhorar a legibilidade do texto em imagens de plano de fundo

**Restrições**:

- Uso de [seções](customize-template.md#sections-or-groups):
   - Somente uma seção pode ser usada, gerando um único conjunto de elementos de modelo.
- É necessário exatamente um campo de imagem.

**Taxas de proporção com suporte**:

A taxa de proporção deve ser definida:

- Quadrado 1:1 (1080 x 1080 pixels)
- Retrato 4:5 (1080 x 1350 pixels)
- História 9:16 (1080 x 1920 pixels)
- Paisagem: 1,91:1 (largura de 1080 pixels)
- Tamanho de imagem personalizada: (largura mínima de imagem de 50 x 50 pixels)

**Nomes de campos reconhecidos**:

Para Metadados, os campos `headline`, `body` e `CTA` são gerados automaticamente. Use espaços reservados para o conteúdo para os seguintes campos:

- `image` (selecionado no JPEG de conteúdo, PNG ou GIF)
- `on_image_text`

Consulte [Espaços reservados para conteúdo](customize-template.md#content-placeholders) para entender mais sobre o uso de nomes de campo em modelos.

>[!TAB Banner e anúncio de exibição]

Siga estas práticas recomendadas de design ao personalizar modelos de Banner e Anúncio de exibição para funcionar com o GenStudio for Performance Marketing:

- Usar fontes do Adobe ou Google
- Prepare ativos que sejam bem exibidos em dimensões finas
- **não** usar imagens de fundo inseridas ou codificadas
- Usar imagens de plano de fundo (campo `image`) carregadas no repositório de conteúdo do GenStudio for Performance Marketing
- **não** usar o JavaScript

**Restrições**:

- Uso de [seções](customize-template.md#sections-or-groups):
   - Somente uma seção pode ser usada, gerando um único conjunto de elementos de modelo.
- É necessário exatamente um campo de imagem.

**Dimensões com suporte**:

- A largura x altura (pixels) deve ser definida
- Vertical:
   - 300 x 600
   - 160 x 600&#x200B;
- Horizontal:
   - 300 x 250
   - 728 x 90
   - 336 x 280
   - 320 x 50
   - 970 x 250&#x200B;
- Personalizado: 50 x 50 a 2000 x 2000

**Nomes de campos reconhecidos**:

Para anúncios em banner e Exibição, o campo `CTA` é gerado automaticamente. Use espaços reservados para o conteúdo para os seguintes campos:

- `headline`
- `sub_headline`
- `body`
- `image` (selecionado no JPEG de conteúdo, PNG ou GIF)

Consulte [Espaços reservados para conteúdo](customize-template.md#content-placeholders) para entender mais sobre o uso de nomes de campo em modelos.

>[!TAB Anúncio do LinkedIn]

[!BADGE Beta]{type=Informative tooltip="No momento, esse recurso está no Beta, portanto, algumas funcionalidades podem estar limitadas ou sujeitas a alterações."}

Siga estas práticas recomendadas de design ao personalizar modelos de anúncios do LinkedIn para funcionar com o GenStudio for Performance Marketing:

**Restrições**:

- Uso de [seções](customize-template.md#sections-or-groups):
   - Somente uma seção pode ser usada, gerando um único conjunto de elementos de modelo.
- É necessário exatamente um campo de imagem.
- Tamanho máximo de imagem de 5 MB
- Máximo de 70 caracteres no título
- Texto introdutório com no máximo 150 caracteres

**Taxas de proporção com suporte**:

- Quadrado 1:1
   - desktop ou portátil
   - Mín: 360 x 360 pixels
   - Máx.: 4320 x 4320 pixels
- Horizontal 1.91:1
   - desktop
   - Mín: 640 x 360 pixels
   - Máx.: 7680 x 4320 pixels
- Vertical 1:1.91
   - dispositivo móvel
   - Mín: 360 x 640 pixels
   - Máx.: 2430 x 4320 pixels
- Vertical 2.3
   - dispositivo móvel
   - Mín: 360 x 640 pixels
   - Máx.: 2430 x 4320 pixels
- Vertical 4.5 (recomendado)
   - dispositivo móvel
   - Mín: 360 x 640 pixels
   - Máx.: 2430 x 4320 pixels

**Nomes de campos reconhecidos**:

Para anúncios do LinkedIn, os campos `headline`, `introductory_text` e `CTA` são gerados automaticamente. Use espaços reservados para o conteúdo para os seguintes campos:

- `image` (selecionado no JPEG de conteúdo, PNG ou GIF)
- `on_image_text`

Consulte [Espaços reservados para conteúdo](customize-template.md#content-placeholders) para entender mais sobre o uso de nomes de campo em modelos.

>[!ENDTABS]
