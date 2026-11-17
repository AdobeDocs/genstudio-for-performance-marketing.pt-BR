---
title: Gerar nomes de anúncios
description: Saiba como configurar modelos de nomenclatura, gerar nomes de anúncio consistentes e revisar ou personalizar nomes antes de enviar anúncios às plataformas de ativação compatíveis.
role: User
source-git-commit: 6db986fefd199181e568e5fbc7a3b23554e5e70d
workflow-type: tm+mt
source-wordcount: '1684'
ht-degree: 1%
---

# Gerar nomes de anúncios

A nomenclatura automatizada de anúncios no [!DNL GenStudio for Performance Marketing] ajuda a seguir as convenções de nomenclatura de sua organização ao ativar anúncios. Nomes consistentes são compatíveis com relatórios de desempenho, atribuição e reconciliação de gastos.

Um modelo de nomenclatura define as partes do nome de um anúncio e sua ordem. Exemplos de peças incluem o produto, a campanha e o mercado. Para criar um modelo, faça upload de um arquivo do Excel que descreva a convenção de nomenclatura de sua organização.

Use o template para gerar nomes a partir de informações sobre cada experiência, como produto ou campanha. Analise e corrija os resultados antes de enviar seus anúncios. Os nomes finais são enviados para cada plataforma de destino como nomes de anúncios.

## Antes de começar

Você só precisa configurar um template uma vez. Se sua plataforma já tiver um modelo atribuído no Projeto atual, vá diretamente para [Gerar nomes para uma ativação](#generate-names-for-an-activation).

Caso contrário, crie um modelo e peça a um gerente de sistema para [atribuí-lo às suas plataformas](#assign-a-template-to-platforms). Cada projeto pode ter um modelo padrão diferente para a mesma plataforma.

Para configurar o modelo, prepare um arquivo do Excel de no máximo 3 MB, com apenas uma folha. Arquivos CSV não são compatíveis. Descreva a convenção de nomenclatura para anúncios individuais, não campanhas ou grupos de anúncios.

Liste os campos na ordem exigida. Para cada campo, inclua os valores permitidos, os códigos correspondentes e instruções para escolher um valor. Por exemplo, a opção `Image` para o campo `format` usa o código `IMG` no nome.

Para obter uma estrutura de exemplo, baixe o [exemplo de convenção de nomenclatura do WKND Meta (Excel)](assets/wknd-meta-naming-convention.xlsx). O arquivo define campos e valores de exemplo para o produto, campanha, mercado e outras partes do nome de um anúncio.

Substitua os valores e as regras de exemplo pela convenção de sua organização antes de usar o arquivo para suas próprias ativações. Os valores de plataforma do exemplo ilustram as opções de nomenclatura, não uma lista de destinos de ativação compatíveis.

## Criar um modelo de nomenclatura

Crie um modelo a partir do arquivo de convenção de nomenclatura existente e, em seguida, revise a estrutura extraída antes de usá-la.

1. Abra o Projeto onde deseja usar o modelo.
1. Vá para **[!UICONTROL Mais]** > **[!UICONTROL Configurações]**.
1. Selecione **[!UICONTROL Configurar]** ao lado de **[!UICONTROL Modelo de nome do anúncio]**.

   Se os modelos já existirem, abra **[!UICONTROL Modelo de nome do anúncio]** e selecione **[!UICONTROL Criar modelo]**.

1. Selecione **[!UICONTROL Selecionar arquivo]** na caixa de diálogo **[!UICONTROL Carregar arquivo]**.
1. Escolha seu arquivo do Excel.

   Como alternativa, arraste o arquivo para a área de upload. Enquanto **[!UICONTROL Analisando sua planilha...]** é exibido, os campos e valores são mapeados para seu modelo. Aguarde alguns minutos para a conclusão da análise.

1. Revise os campos, os valores permitidos e a **[!UICONTROL Visualização do nome do anúncio]**.

   A visualização usa valores de amostra, não os detalhes de um anúncio específico.

1. Selecione **[!UICONTROL Salvar]**.

Os arquivos maiores que 3 MB, os tipos de arquivos não suportados e os arquivos vazios mostram um erro sem alterar os modelos ou atribuições de plataforma existentes.

## Personalizar um modelo

Edite um modelo salvo para ajustar seu nome, campos, separador ou regras.

1. Vá para **[!UICONTROL Mais]** > **[!UICONTROL Configurações]** > **[!UICONTROL Modelo de nome do anúncio]**.
1. Abra o menu de três pontos ao lado do modelo.
1. Selecione **[!UICONTROL Editar]**.
1. Para renomear o modelo, selecione o ícone de lápis ao lado do título.
1. Defina o **[!UICONTROL Separador de campo]** para o caractere que separa as partes do nome, como um sublinhado (`_`).
1. Arraste os campos para a ordem necessária.

   Use **[!UICONTROL Adicionar campo]** ou um ícone de lixeira de campo se precisar alterar quais campos são incluídos.

1. Para abrir as configurações de um campo, selecione o ícone de lápis.
1. Revise **[!UICONTROL Type]** e **[!UICONTROL Name]** na caixa de diálogo **[!UICONTROL Editar um campo]**.

   Use a **[!UICONTROL Lista suspensa]** para um campo com opções predefinidas ou o **[!UICONTROL Texto livre]** para um valor inserido.

1. Para um campo suspenso, examine as **[!UICONTROL Opções]** e o **[!UICONTROL Código]**.

   **[!UICONTROL Opções]** contém as opções legíveis. **[!UICONTROL Código]** contém os valores correspondentes usados no nome do anúncio. Por exemplo, a opção `Image` usa o código `IMG`.

   Para adicionar uma opção, selecione **[!UICONTROL Adicionar opção]**. Para remover uma opção, selecione seu ícone de subtração. Valores duplicados em um campo não são permitidos.

1. Insira quaisquer **[!UICONTROL Regras de campo]** necessárias para escolher ou formatar o valor desse campo.

   Para o campo de texto livre `creativeVersion`, insira esta regra de exemplo: `Use the experience name as a starting value, with spaces removed.`

1. Selecione **[!UICONTROL Salvar]** na caixa de diálogo do campo.

   Repita a revisão de campo para quaisquer outros campos que precisem de alterações.

1. Digite quaisquer **[!UICONTROL Regras de modelo]** que se apliquem ao nome.

   Por exemplo, digite `Remove spaces from Product and Campaign values.`

1. Selecione **[!UICONTROL Salvar]** na parte superior da página.

A visualização reflete a ordem e o separador de campos atualizados. Para verificar as alterações salvas, abra o template novamente.

O editor de campo mostra como as opções legíveis são mapeadas para os códigos incluídos nos nomes gerados:

![Edite uma caixa de diálogo de campo com as opções de formato Imagem, Vídeo, Carrossel e HTML5 e seus códigos correspondentes.](images/ad-name-field-options-codes.png)

## Atribuir um modelo às plataformas

Os gerentes de sistema definem o modelo padrão para cada plataforma dentro de um Projeto. Se você não for um gerenciador de sistemas, peça a um deles para concluir este procedimento.

1. Abra o Projeto cujos padrões de plataforma você deseja definir.
1. Vá para **[!UICONTROL Mais]** > **[!UICONTROL Configurações]** > **[!UICONTROL Modelo de nome do anúncio]**.
1. Abra o menu de três pontos ao lado do modelo.
1. Selecione **[!UICONTROL Editar]**.
1. Selecione uma ou mais plataformas em **[!UICONTROL Plataformas preferenciais]**, na parte inferior do editor.
1. Selecione **[!UICONTROL Salvar]**.

Cada plataforma tem um modelo padrão por projeto. Você pode atribuir o mesmo modelo a várias plataformas.

Os modelos estão disponíveis para visualização e edição entre projetos. No entanto, você pode alterar as atribuições da plataforma somente no Projeto atual.

Substituir o padrão de uma plataforma não exclui o modelo anterior nem altera as atribuições de outros projetos.

O exemplo abaixo mostra a visualização do modelo, a ordem dos campos, as regras e as **[!UICONTROL Plataformas preferenciais]** com Meta Ads selecionados:

![Editor de modelo do WKND com um separador de sublinhado, 12 campos de nome de anúncio, regras de modelo e Meta Ads selecionados nas Plataformas preferenciais.](images/ad-name-template-editor.png)

## Gerar nomes para uma ativação

Prepare a ativação antes de gerar nomes. Os metadados de cada experiência contêm informações como campanha, produto ou persona. Verifique se os metadados fornecem os valores de que seu modelo precisa. Consulte [Fluxo de trabalho de ativação](create-activation.md) para obter ajuda sobre como preparar uma ativação.

1. Abra **[!UICONTROL Ativar]** no projeto pretendido.
1. Adicione suas experiências a uma ativação.
1. Complete a configuração da plataforma e todas as informações necessárias, incluindo cópia, call-to-action (CTA) e URL do site.
1. Verifique se as experiências têm os metadados necessários para sua convenção de nomenclatura.
1. Selecione **[!UICONTROL Gerar nome do anúncio]** acima da tabela de ativação.

   Aguarde a conclusão de **[!UICONTROL Geração de nomes de anúncio]** antes de examinar os resultados.

1. Revise a coluna **[!UICONTROL Nome do anúncio]**.

A geração se aplica a todos os anúncios nas plataformas com um modelo atribuído, exceto anúncios com [substituições de nome personalizado](#use-a-custom-ad-name). Os nomes não são gerados automaticamente ao abrir a tabela.

Inicialmente, cada anúncio usa o nome da experiência. Se uma plataforma não tiver um template atribuído, a geração deixará os nomes inalterados. Edite esses nomes manualmente conforme necessário.

Se nenhuma plataforma tiver templates atribuídos, nenhum nome será gerado.

## Corrigir um nome de anúncio individual

Analise os nomes gerados antes de enviar seus anúncios. Os valores ausentes aparecem como espaços reservados para o campo destacado, como `[market]`, e os anúncios afetados mostram **[!UICONTROL Precisa de atenção]**.

Para localizar nomes que precisam de correções, procure os espaços reservados destacados e os status **[!UICONTROL Precisa de atenção]** na tabela de ativação:

![Tabela de ativação com um aviso de valores ausentes, marcados marcadores de posição de mercado na coluna Nome do anúncio e status Precisa de atenção.](images/ad-names-missing-values.png)

1. Selecione a linha do anúncio na tabela de ativação.
1. Selecione **[!UICONTROL Editar nome do anúncio]**.
1. Atualize os menus suspensos ou campos de texto relevantes.
1. Selecione **[!UICONTROL Salvar]**.

Por exemplo, se `market` não tiver valor, insira ou selecione o mercado apropriado para substituir `[market]` no nome.

Verifique o nome atualizado em relação à sua convenção.

## Resolver possíveis nomes duplicados

Nomes de anúncios idênticos na mesma plataforma são sinalizados como duplicatas potenciais.

1. Selecione um dos anúncios afetados.
1. Selecione **[!UICONTROL Editar nome do anúncio]**.
1. Altere o nome para que os dois nomes sejam diferentes.
1. Selecione **[!UICONTROL Salvar]**.

O aviso de possível duplicação é apagado depois que os nomes se tornam diferentes.

## Editar vários nomes de anúncios {#edit-several-ad-names-at-once}

Use a edição em massa para aplicar uma correção compartilhada, preservando valores diferentes entre os anúncios.

1. Marque os anúncios usando as caixas de seleção de linha.
1. Selecione **[!UICONTROL Editar nome do anúncio]** na barra de ferramentas de seleção.
1. Altere somente os campos que precisam do mesmo valor nos anúncios selecionados.

   **[!UICONTROL Valores mistos]** significa que os anúncios selecionados atualmente têm valores diferentes para um campo. Deixe esse campo intacto para preservar o valor de cada anúncio.

1. Selecione **[!UICONTROL Salvar]**.
1. Revise os nomes atualizados quanto à precisão e possíveis duplicatas.

Somente os anúncios selecionados são atualizados. Os anúncios não selecionados permanecem inalterados.

O editor de itens em massa exibe **[!UICONTROL Valores mistos]** para campos que diferem entre os anúncios selecionados:

![Detalhe da caixa de diálogo Editar nomes de anúncios 4 mostrando Valores mistos para produto, campanha, creativeVersion e persona.](images/ad-names-bulk-edit.png)

Por exemplo, alterar apenas a persona de `OutdoorBeginners` para `Adventurers` preserva os produtos diferentes. Esses nomes encurtados ilustram a alteração:

| Antes | Depois |
| --- | --- |
| `WKND_TrailBag_OutdoorBeginners` | `WKND_TrailBag_Adventurers` |
| `WKND_RiosShirt_OutdoorBeginners` | `WKND_RiosShirt_Adventurers` |

## Usar um nome de anúncio personalizado

Use uma substituição para substituir todo o nome gerado por um nome personalizado, em vez de editar campos de modelo individuais.

1. Selecione a linha do anúncio.
1. Selecione **[!UICONTROL Editar nome do anúncio]**.
1. Ative **[!UICONTROL Substituir nomes de anúncios]**.
1. Insira o nome personalizado.
1. Selecione **[!UICONTROL Salvar]**.

O nome personalizado permanece inalterado quando você gera nomes novamente.

Com a substituição ativada, edite o nome completo em vez de seus campos de modelo individuais:

![Caixa de diálogo Editar nome do anúncio com a opção Substituir nomes de anúncio habilitada e o nome completo do anúncio WKND disponível para edição.](images/ad-name-override.png)

Para retornar à nomeação baseada em modelo, siga estas etapas:

1. Abra **[!UICONTROL Editar nome do anúncio]** para o anúncio.
1. Desative **[!UICONTROL Substituir nomes de anúncios]**.
1. Selecione **[!UICONTROL Salvar]**.
1. Selecione **[!UICONTROL Gerar nome do anúncio]** acima da tabela de ativação.

Essa ação também gera novamente nomes para outros anúncios na tabela que têm um modelo atribuído e nenhuma substituição de nome personalizado.

## Responder às alterações do modelo

Ao editar uma tabela de ativação, um aviso será exibido se um modelo que ele usa tiver sido alterado ou excluído.

Se o modelo tiver sido alterado, revise o modelo atualizado antes de gerar os nomes novamente. Selecione **[!UICONTROL Gerar nome do anúncio]** para aplicá-lo.

Se o modelo tiver sido excluído ou você precisar de uma substituição, siga estas etapas:

1. Peça a um gerente de sistema para atribuir um modelo de substituição à plataforma afetada no mesmo Projeto.
1. Retorne à tabela de ativação.
1. Selecione **[!UICONTROL Gerar nome do anúncio]**.
1. Revise os nomes atualizados.

Os nomes com substituições ativadas permanecem inalterados durante a regeneração.

## Enviar anúncios para plataformas

Revise seus nomes finais e endereços de campos não resolvidos, duplicatas potenciais e outros problemas **[!UICONTROL Precisa de atenção]** antes de enviar anúncios.

Quando a ativação estiver pronta, selecione **[!UICONTROL Enviar para plataformas]**.

[!DNL GenStudio for Performance Marketing] envia o nome final de cada anúncio para a plataforma de destino como seu nome de anúncio. O nome enviado inclui edições nos campos do modelo ou substituições do nome personalizado. Os nomes dos anúncios na plataforma correspondem exatamente aos nomes finais revisados.

Para destinos de exibição como Innovid, os nomes são exibidos como nomes criativos.
