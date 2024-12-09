---
title: Gravar prompts efetivos
description: Saiba como escrever prompts efetivos para o Adobe GenStudio for Performance Marketing.
feature: Prompt, Generative AI, Brands Service, Personas Service, Products Service, Guidelines
exl-id: 0cd4db4f-d031-4c1f-a4e7-adc220f947fc
source-git-commit: 79430c3279529c4871141489e409240852e1f4fc
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Gravar prompts efetivos

A comunicação com a IA gerativa é essencial para trabalhar com eficiência no Adobe GenStudio for Performance Marketing.

O GenStudio for Performance Marketing fornece um prompt de IA generativo sempre que há uma oportunidade de modificar um ativo. Os componentes de um prompt efetivo devem incluir linguagem descritiva, exemplos e informações não fornecidas através das diretrizes configuradas.

Como prática recomendada, forneça à GenStudio for Performance Marketing as informações da sua marca usando as [diretrizes](/help/user-guide/guidelines/overview.md) e, em seguida, você poderá aproveitar totalmente a IA gerativa para produzir experiências de conteúdo alinhadas à marca.

## Linguagem descritiva

Você pode usar a linguagem natural para articular suas ideias e criar experiências. Seu prompt orienta a IA a gerar conteúdo de canal personalizado e imagens que complementam sua visão. Quanto mais detalhes você fornecer, maior a chance de produzir uma imagem ou experiência que atenda às suas necessidades. Use uma linguagem clara e descritiva para fornecer o máximo de detalhes possível:

- Para **imagens**, use palavras que descrevam ambiente, humor, cor, composição e estilo.
- Para **copiar**, use palavras que descrevam o público-alvo, a finalidade, as descrições dos novos recursos, exemplos e ações.

Veja a seguir um exemplo de prompt que articula informações sobre sua intenção, público-alvo e estilo.

```bash
Write an email to motivate infrequent users of Photoshop to follow an in-app tutorial that teaches them to combine elements of two photos into a beautiful work of art. Highlight the generative AI capabilities of Photoshop and use references to natural imagery.
```

+++Ver resultados de exemplo

![três emails gerados](/help/assets/sample-email.png)

+++

## Critérios de solicitação

No GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md), você pode usar **[!UICONTROL Critérios de solicitação]** ([_Parâmetros_](/help/user-guide/create/overview.md#parameters) e um prompt) na gaveta do prompt para adicionar detalhes por meio da seleção para melhorar a interpretação da IA.

Para [emails](/help/user-guide/create/email-experiences.md), os critérios de prompt podem incluir a adição de [diretrizes](/help/user-guide/guidelines/overview.md) em _Parâmetros_, o carregamento de um ativo para usar nas variantes de email e um prompt descritivo. Para um [Meta ad](/help/user-guide/create/create-meta-ad.md), os critérios de prompt podem incluir uma diretriz de marca em _Parâmetros_, a seleção ou o upload de um ativo existente, configurações relacionadas a imagens ou ativos, como proporção, e um prompt. A verdadeira potência começa com [diretrizes de configuração](/help/user-guide/guidelines/add-guidelines.md).

>[!NOTE]
>
>Se as diretrizes forem adicionadas em _Parâmetros_ na gaveta do prompt, não será necessário incluir uma referência a elas no prompt. O GenStudio for Performance Marketing aproveita esses [!DNL Brands], [!DNL Products] e [!DNL Personas] na geração de conteúdo.

### Diretrizes

As diretrizes do GenStudio for Performance Marketing ajudam a IA gerativa a personalizar a composição do ativo. Quando apresentado com os critérios de prompt, você pode escolher um [[!DNL Brand]](/help/user-guide/guidelines/brands.md), um [[!DNL Persona]](/help/user-guide/guidelines/personas.md) e um [[!DNL Product]](/help/user-guide/guidelines/products.md) a partir das diretrizes configuradas.

>[!TIP]
>
>Você controla como e quando a GenStudio for Performance Marketing usa suas diretrizes do [!DNL Brand]. Consulte [Diretrizes](/help/user-guide/guidelines/overview.md) para saber como configurar e gerenciar as diretrizes da sua marca.

### Prompts estruturados

Para emails de várias seções, você pode estruturar prompts para fornecer instruções específicas da seção para gerar conteúdo variável para cada seção em um email. Os prompts estruturados devem fazer referência direta aos [nomes de seção no modelo de email](/help/user-guide/content/customize-template.md#sections-or-groups), para que o conteúdo gerado possa ser inserido nos espaços reservados de conteúdo correspondentes.

Por exemplo, você pode instruir o GenStudio for Performance Marketing a gerar conteúdo para um email que promove um novo produto na primeira seção e detalha os benefícios de economia na segunda seção.

O prompt estruturado deve:

- Use uma das seguintes referências ao nome da seção no template de email:
   - Pod
   - Grupo
   - Seção
   - Módulo

  Por exemplo, se o modelo usa `moduleA` ou `Group-3` como um nome de seção, você pode fazer referência a esses nomes de seção no prompt.

- Siga as regras/estruturas recomendadas. Se a estrutura de prompts não aderir ao formato fornecido, o prompt se aplica a *todas* as seções de email e ainda facilita a geração de conteúdo.
- Use nomes de seção conforme definidos no modelo de email. As referências de prompt devem corresponder aos nomes de seção codificados em seu modelo de email.
- Não diferencie maiúsculas de minúsculas. Por exemplo, você pode usar `Pod` ou `pod` no modelo de email e no prompt estruturado.
- Consulte o prompt de usuário genérico primeiro e, em seguida, as diretivas específicas da seção.
- Use dois pontos, hífen, vírgula ou outra demarcação (`,:;#$!~|@=-%&*^_`) como uma separação entre a referência de nome de seção e a diretiva. Por exemplo, você pode usar o seguinte como uma diretiva de prompt específica de seção: `Pod1; Describe how to easily edit text and swap images.`

Este é um exemplo de prompt que articula a estrutura de prompt recomendada e aproveita um modelo de email que usa o termo de identificação `Pod` como em `Pod1`, `Pod2` e `Pod3`.

```properties
Create an exciting multi-pod email focusing on Creative Cloud and its powerful generative AI capabilities.

Encourage customers to convert to Photoshop or use a free Photoshop trial. We want to better educate them about app features.

Pod1: Focus on Adobe Photoshop and its new generative AI tools that enable creators to bring images to life in minutes.

Pod2: Focus on Adobe Illustrator and its new generative AI tools, such as Generative Shape Fill, which allows you to quickly fill your vector outline and explore a variety of options that match the look and feel of your own artwork.

Pod3: Focus on Adobe Acrobat Pro. Make users aware that with Acrobat Pro they can edit images and text inside a PDF.
```

Consulte [práticas recomendadas para usar modelos](/help/user-guide/content/best-practices-for-templates.md).

## Tente novamente

A solicitação é um processo iterativo. Se os resultados não atenderem às suas expectativas, revise seu prompt e faça algumas alterações ou adicione mais detalhes. Ou você pode colar seções de um resumo da campanha. Você pode até solicitar que o GenStudio for Performance Marketing evite determinadas palavras, elementos ou temas.

## Práticas recomendadas

Algumas práticas recomendadas simples para criar prompts eficazes:

- Seja específico e forneça detalhes sobre o que fazer ou não fazer.
- Fornecer contexto usando referências externas.
- Aproveite as diretrizes do GenStudio for Performance Marketing.
- Revise e ajuste as diretrizes regularmente.
- Iterar e refinar.
- Aprenda por meio da experimentação.

{{in-academy}}
