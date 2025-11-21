---
title: Editor de código do modelo
description: Saiba como usar o editor de código de modelo no GenStudio for Performance Marketing.
level: Intermediate
role: Developer
feature: Media Templates, Content Generation
exl-id: b46fc7a9-88c1-474a-9d7b-1df7740d8f5a
source-git-commit: 9e51e853542d20f0b90b10071f4f26aaae1d6aad
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# Editor de código de modelo

O editor de código de modelo foi projetado para ajudar você a verificar e refinar seu modelo para uso ideal ao gerar novas experiências com o GenStudio for Performance Marketing. O editor é compatível com a sintaxe Handlebars, que usa espaços reservados dentro do modelo para indicar onde o GenStudio for Performance Marketing deve gerar conteúdo para você.

>[!TIP]
>
>Antes de carregar o código HTML do modelo na exibição [!DNL Content] _Modelos_, prepare o modelo inserindo os espaços reservados para conteúdo definidos na orientação [Personalizar modelos](customize-template.md).

## Verificar campos detectados

O painel _[!UICONTROL Verificar campos detectados]_ mostra uma lista de campos que a GenStudio for Performance Marketing reconhece no modelo. Revise a lista e você pode rolar pelo código HTML para observar a formação do seu template.

![Modo de exibição do editor de código](/help/assets/template-detected-fields.png "Verificar campos detectados"){width="600"}

Se você observar que um campo está ausente na lista, pesquise o código do modelo e localize o local do campo ausente. Insira o espaço reservado correto usando a sintaxe Handlebars e um [nome de campo reconhecido](/help/user-guide/templates/customize-template.md#recognized-field-names). Use o formulário Localizar e substituir, exibido na parte inferior do editor de código, para procurar strings específicas no código. (Windows `CTRL`+`F` ou macOS `CMD`+`F`)

## Ajustar funções para uma variável

Você pode selecionar e alterar funções de campo para funções de campos baseados em texto (por exemplo, `headline`, `sub_headline`, `body`, `cta`, `on_image_text`, `custom`) com uma lista suspensa durante a verificação de estrutura de modelo. As seleções de funções de campo persistem durante as edições de modelo, portanto, as personalizações não são perdidas, melhorando a eficiência do fluxo de trabalho.

>[!NOTE]
>
>As variáveis de imagem não podem ter suas funções ajustadas.

![Seleção de campo de várias funções](/help/assets/multirole-dropdown-field.png "Seleção de campo de várias funções"){width="600"}

Para atribuir uma função a uma variável:

1. Localize a variável no painel _[!UICONTROL Verificar campos detectados]_. Essas variáveis são descobertas automaticamente.
2. Revise as funções atribuídas a cada variável. As funções são atribuídas automaticamente, mas podem ser ajustadas usando a lista suspensa para qualquer variável no modelo.
3. Ajuste uma função selecionando uma nova função na lista suspensa.
4. Clique em **[!UICONTROL Avançar]** para continuar.

## Fazer uma correção

Se houver erros no modelo, você poderá ver uma mensagem `Template is invalid` que inclui uma breve explicação do problema. No exemplo a seguir, a mensagem indica que o campo `_image` não está em conformidade com a convenção de nomenclatura de campos estabelecida no modelo de vários pods. A mensagem informa ainda que é necessário atualizar o nome do campo com o prefixo correto. Localize o campo `_image` no editor de código de modelo e atualize o nome conforme recomendado.

![Corrigir modelo inválido](/help/assets/animation/template-code-editor.gif){width="600"}

O painel _[!UICONTROL Verificar campos detectados]_ atualiza para refletir as alterações feitas. Quando estiver satisfeito com o preenchimento e os campos corretos, clique em **[!UICONTROL Avançar]** para continuar [carregando seu modelo](/help/user-guide/templates/use-templates.md#add-a-template).

## Problemas comuns de modelos e soluções

| **Erro** | **Descrição** | **Solução** |
|-----------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| Falha ao analisar | O conteúdo do modelo não pôde ser analisado como Handlebars válidos. | Verifique se há erros de sintaxe do HTML e Handlebars no modelo e corrija-os para garantir uma formatação válida para os [espaços reservados para o conteúdo](/help/user-guide/templates/customize-template.md#content-placeholders). |
| Grupo não atribuído | Um campo de imagem em um modelo de email de vários grupos não está atribuído a nenhum grupo. | Verifique se os prefixos de seção são usados de maneira consistente. Cada [seção](/help/user-guide/templates/customize-template.md#sections-or-groups) pode usar apenas um de cada tipo de campo (`headline`, `body`, `image` `cta`). Atribua o campo `image` a um grupo válido no modelo. |
| Imagem ausente | Um campo de imagem obrigatório está ausente. | Exatamente um campo `image` é necessário para determinados tipos de modelo, como Meta, exibição ou anúncio de banner. Adicione o campo `image` necessário ao modelo. |
| Grupo único inválido | O template de email contém exatamente um grupo, que é inválido. | Um modelo de email básico contém um único conjunto de elementos de modelo, que não requerem a convenção de nomenclatura de grupo conforme definido em [Seções ou grupos](/help/user-guide/templates/customize-template.md#sections-or-groups). Ajuste seu template para ter zero seções removendo qualquer sintaxe de nomeação de grupo. |
| Nenhum campo | O modelo não contém nenhum campo. | Adicione [nomes de campo reconhecidos](/help/user-guide/templates/customize-template.md#recognized-field-names) usando a sintaxe Handlebars no modelo em que você precisa do GenStudio for Performance Marketing para gerar um determinado tipo de conteúdo. |
| Propriedades obrigatórias ausentes | Algumas propriedades de metadados necessárias estão ausentes. | Cada tipo de modelo tem requisitos e restrições com base nas diretrizes de canal. Por exemplo, o Meta exige uma taxa de proporção e os anúncios de exibição exigem dimensões. [Siga as diretrizes do modelo específico do canal](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines). |
| Nome reservado usado | Um nome de campo proibido ou reservado está sendo usado. | Determinados [nomes de campos](/help/user-guide/templates/customize-template.md#recognized-field-names), como `subject` ou `introductory_text`, estão reservados. Renomeie os campos que usam nomes reservados ou proibidos. |
| Muitos campos | O número de campos excede o limite global de 20. | Remova campos desnecessários para garantir que o total não exceda 20. |
| Muitos grupos | O número de grupos excede o máximo permitido do canal. | Os modelos do Meta, de exibição e do LinkedIn não permitem várias seções. O email exige o nome do grupo ao definir duas ou três seções. Reduza o número de grupos no modelo para atender aos [requisitos do canal](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines). |
| Campo incompatível | O modelo está usando um campo para o qual o canal não oferece suporte. | Substitua ou remova campos sem suporte de acordo com os [nomes de campo reconhecidos](/help/user-guide/templates/customize-template.md#recognized-field-names). |
