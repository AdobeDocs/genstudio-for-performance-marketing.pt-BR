---
title: Fluxo de trabalho de ativação
description: Saiba mais sobre o fluxo de trabalho de ativação para experiências de anúncio.
feature: Ad Activation
exl-id: 17e1bade-d52a-4953-a85c-c10d093e73d6
TQID: https://experienceleague.adobe.com/HSwFeL1qCzgFao2Ii64Hx-kaADRnd3dxaswFMzJ7nfA
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: dd48f9df-f2e2-49fe-a918-332a8e240ffe
    internal-label: Channels
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: 0844f7407c4b3a3f8eafe248f498ef7fcd51555d
workflow-type: tm+mt
source-wordcount: '1238'
ht-degree: 1%
---
# Fluxo de trabalho de ativação

[!DNL Activate] ativa experiências publicadas nos canais de anúncios pagos. Uma experiência do GenStudio for Performance Marketing é um componente de campanha de marketing, como um anúncio, preparado para um público específico em um canal de anúncio pago. As experiências para ativação contêm três componentes principais:

* **Ativos de mídia**: imagens ou vídeos incluídos na sua experiência com anúncios. Os tipos de arquivos suportados e as taxas de proporção variam de acordo com o canal e o formato.

* **Texto**: todas as formas de cópia incluídas no anúncio, incluindo títulos, corpo de texto e elementos call-to-action.

* **Metadados**: atributos definidos pelo usuário que aprimoram a análise, a filtragem e o rastreamento de desempenho. Normalmente, os metadados não são visíveis para o público-alvo do anúncio final.

Você prepara e aprova esses componentes no [!DNL Content] antes da ativação. [!DNL Activate] não cria ou edita ativos, títulos ou cópia do corpo aprovados. Ela aplica apenas a configuração de que cada canal precisa e publica a experiência.

Uma única tabela de ativação pode incluir experiências para vários canais de anúncios pagos e formatos de anúncios ao mesmo tempo.

>[!VIDEO](https://video.tv.adobe.com/v/3503538?learn=on)

## Conectar suas contas de canal

Um gerente de sistema ou editor do GenStudio deve conectar as contas de anúncio de cada canal de anúncio pago antes de você poder ativar uma experiência para esse canal. Para ver as etapas deste processo, consulte [Conectar contas de mídia paga](/help/user-guide/connectors/connect-channel.md).

## Iniciar uma ativação

Inicie uma ativação de um de dois pontos de entrada:

* **De[!DNL Content]**: filtre por Experiências, selecione uma ou mais experiências publicadas e clique em **[!UICONTROL Ativar]** na barra de ações superior.
* **De[!DNL Activate]**: na página de aterrissagem [!DNL Activate], clique em **[!UICONTROL + Nova ativação]**. Isso abre a galeria Experiência, onde você seleciona experiências para ativação.

![Selecionando experiências publicadas em Conteúdo e clicando em Ativar para iniciar uma ativação](./images/content-select-activate.png)

Em ambos os casos, pesquise por nome de experiência ou filtre por vários canais para encontrar as experiências desejadas.

Se sua seleção incluir experiências de formato de exibição, especifique qual plataforma de exibição usar: Google Campaign Manager 360, Innovid, Amazon Ads ou The Trade Desk. Em seguida, clique em **[!UICONTROL Iniciar ativação]**. Para outros formatos, como Meta, LinkedIn, TikTok, YouTube e ChatGPT, o [!DNL Activate] infere a plataforma do canal da experiência e ignora esta etapa.

[!DNL Activate] gera uma tabela de ativação listando todas as experiências selecionadas. A tabela é organizada em subtabelas por formato de anúncio e canal, por exemplo, imagem única do Meta ou imagem única do LinkedIn. Cada linha representa um anúncio. Para a maioria dos canais, como LinkedIn, TikTok e canais de exibição, uma experiência com várias taxas de proporção gera uma linha por taxa de proporção; exclua todas as linhas desnecessárias. O Meta é a exceção. Um anúncio do Meta pode incluir várias taxas de proporção em um único anúncio, de modo que uma experiência de Meta com várias taxas de proporção ainda gera apenas uma linha.

A tabela de ativação é salva como rascunho automaticamente ao ser aberta. Você pode sair e retomar o rascunho a qualquer momento antes de publicar.

Para adicionar mais experiências a uma tabela de ativação já aberta, clique em **[!UICONTROL Adicionar mais experiências]** na parte superior direita da tabela. Isso reabre a Galeria de experiências para que você possa selecionar experiências adicionais, que [!DNL Activate] adiciona à tabela existente.

**[!UICONTROL Adicionar mais experiências]** também permite ativar para mais de uma plataforma de exibição na mesma tabela. As experiências de formato de exibição exigem que você escolha primeiro uma única plataforma de exibição, mas você pode clicar em **[!UICONTROL Adicionar mais experiências]**, selecionar mais experiências de formato de exibição e escolher uma plataforma de exibição diferente da que já está na tabela. Por exemplo, é possível adicionar anúncios da Trade Desk a uma tabela que já contém anúncios inóvios.

## Definir detalhes de configuração do anúncio e da plataforma

Os ativos, títulos e cópia do corpo aprovados estão bloqueados e não podem ser editados na tabela de ativação, pois já passaram por revisão e aprovação em [!DNL Content]. Os campos restantes podem ser editados e variam de acordo com o canal:

>[!NOTE]
>
>[!DNL Content] chama um destino como Meta ou LinkedIn de um **canal**. [!DNL Activate] chama o mesmo destino de **plataforma** (por exemplo, em **[!UICONTROL Configuração de plataforma]** e na coluna **Campos de configuração de plataforma editáveis** abaixo). Os dois termos se referem à mesma coisa.

Você não precisa pesquisar os campos do seu canal antecipadamente. [!DNL Activate] mostra apenas as colunas relevantes aos canais e formatos selecionados. Use a tabela abaixo como referência para o que é editável por canal.

**Campos editáveis por canal**

| Canal | Formatos compatíveis | Cópia bloqueada | Campos de texto editáveis | Campos editáveis de configuração da plataforma |
|---|---|---|---|---|
| Meta | Imagem, Vídeo, Carrossel | Título, corpo | Descrição, Call-to-action, URL de destino, Parâmetros de URL, ID de rastreamento | Conta de anúncio, página do Facebook, perfil do Instagram, campanha do Meta, conjunto de anúncios do Meta |
| LinkedIn | Imagem única, Vídeo único | Título, texto introdutório | Descrição, Call-to-action, URL de destino, Parâmetros de URL, ID de rastreamento | Conta do anúncio, Campanha, Conjunto de anúncios |
| Google Campaign Manager 360 | Tela estática, Tela de vídeo, Tela com CEP HTML5 | n/a | ID de rastreamento | Anunciante |
| Anúncios do Amazon | Exibição estática | n/a | ID de rastreamento | Conta |
| Innovid | Exibição estática, exibição de zip HTML5 | n/a | ID de rastreamento | Conta, Biblioteca da Creative, Nome do conceito |
| TikTok | Anúncios de vídeo no feed | Texto primário | Call-to-action, URL de destino, ID de rastreamento | Conta de anúncio, Campanha, Grupo de publicidade |
| YouTube | Shorts em campanhas da geração de demanda do Google Ads | Descrição | Call-to-action, Nome da empresa, URL de destino, Parâmetros de URL, ID de rastreamento | Conta, Campanha, Grupo de publicidade, Logotipo |
| ChatGPT | Cartões de chat | Título, corpo | URL de direcionamento, ID de rastreamento | Conta de anúncio OpenAI, Campanha OpenAI, grupo de anúncios OpenAI |
| A Trade Desk | Exibição estática | n/a | ID de rastreamento | Conta, Campanha |

Uma **ID de rastreamento** é um rótulo exclusivo que você atribui a uma linha de anúncio. Ele é transmitido para a plataforma de destino como o anúncio ou nome criativo, portanto, use-o para identificar esse anúncio para relatórios e solução de problemas.

Edite campos em linha por linha ou selecione várias linhas na mesma tabela de formato e clique em **[!UICONTROL Editar detalhes]** na barra de ferramentas que aparece para editar esses campos em massa de uma só vez. Para configurar campos de configuração de plataforma para um grupo de formatos de anúncio, clique em **[!UICONTROL Gerenciar configurações da plataforma]** e edite os campos na caixa de diálogo resultante.

![Selecionar vários anúncios em uma tabela de ativação para editar detalhes ou configurações da plataforma em massa](./images/bulk-edit-action-bar.png)

![A caixa de diálogo Gerenciar configurações da plataforma para escolher uma conta de anúncio, campanha e conjunto de anúncios da Meta](./images/manage-platform-settings.png)

Para mover entre campos de **[!UICONTROL ID de rastreamento]** mais rapidamente, use estes atalhos de teclado:

* Pressione **Enter** para abrir o campo de edição para a **[!UICONTROL ID de Acompanhamento]** selecionada.
* Pressione a tecla de seta **Para cima** ou **Para baixo** para mover para o campo **[!UICONTROL ID de rastreamento]** anterior ou seguinte nessa coluna.
* Pressione **Enter** novamente para salvar sua edição.

![Editando um campo de ID de Acompanhamento em linha na tabela de ativação](./images/tracking-id-edit.png)

## Revise e publique suas experiências nos canais de publicidade deles

Confirme se cada linha mostra [!UICONTROL Pronto para Ativar]. [!DNL Activate] sinalizadores sem campos ou com campos inválidos, chamadas de ação incompatíveis e IDs de rastreamento duplicadas, pois [!UICONTROL Requer Atenção]. Quando cada linha estiver pronta, clique em **[!UICONTROL Enviar para a Platform]** e confirme na caixa de diálogo de publicação.

![Uma tabela de ativação onde cada linha mostra Pronto para ativar, habilitando Enviar para plataformas](./images/ready-to-activate.png)

[!DNL Activate] relata o status de cada anúncio em tempo quase real: Pending, Published ou Failed. Se um anúncio falhar, passe o mouse sobre o status para ver o erro da plataforma. Você pode repetir cada anúncio com falha na tabela de uma só vez clicando em **[!UICONTROL Tentar novamente]**, em vez de repetir cada um individualmente. As linhas publicadas são bloqueadas para reenvio e incluem um deep link para o anúncio no gerenciador de anúncios nativo da plataforma de destino. A revisão final de pré-publicação e a inicialização de anúncios ocorrem no próprio gerenciador de anúncios do canal de destino: o [!DNL Activate] sempre fornece anúncios em um estado inativo.

![Uma tabela de ativação que mostra uma combinação dos status Pendente e Enviado para plataformas após a publicação](./images/activation-status-pending.png)

Suas tabelas de ativação aparecem na página de aterrissagem [!DNL Activate].

## Canais compatíveis

Cada canal de anúncio pago tem campos de configuração e pré-requisitos específicos do canal. Selecione o canal de anúncios pagos para obter as diretrizes de ativação:

* [Meta](activate-meta-ad.md)
* [LinkedIn](activate-linkedin-ad.md)
* [Google Campaign Manager 360](activate-cm360-ad.md)
* [Anúncios do Amazon](activate-amazon-ad.md)
* [Innovid](activate-innovid-ad.md)
* [TikTok](activate-tiktok-ad.md)
* [YouTube](activate-youtube-ad.md)
* [GPTchat](activate-chatgpt-ad.md)
* [Trade Desk](activate-trade-desk-ad.md)
