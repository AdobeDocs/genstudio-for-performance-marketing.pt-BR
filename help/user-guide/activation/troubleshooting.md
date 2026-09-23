---
title: Otimizar sua ativação
description: Saiba como otimizar ativações para canais de anúncios pagos de terceiros.
level: Intermediate
feature: Ad Activation
exl-id: 5bc624c2-d064-4190-8761-ed05d0629d1f
TQID: https://experienceleague.adobe.com/-D3DGxTpZ-0J-grE5-jKPrptf4C1Z-OE1t0DCoqhRLQ
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
source-git-commit: db0cebfe795569d9913757d190db853097a00405
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 1%
---
# Otimizar ativações

A ativação de uma experiência de anúncio para canais de anúncios pagos envolve duas fases principais:

* Configuração dos detalhes de anúncio e configuração da plataforma para cada linha na tabela de ativação

* Publicar sua ativação para os gerentes de anúncios dos canais de anúncios pagos designados

Seguir as práticas recomendadas ao configurar e ativar suas experiências de anúncio pode ajudar a minimizar possíveis complicações ou erros durante o delivery para os canais de público-alvo.

## Práticas recomendadas

Estas são algumas práticas recomendadas comuns e os erros que podem ser evitados.

* **Usar uma ID de rastreamento exclusiva para cada linha**

  O [!DNL Activate] sinaliza IDs de rastreamento duplicadas como [!UICONTROL Precisa de Atenção] e não permitirá a publicação até que cada linha no formato afetado e na tabela da plataforma tenha uma ID de rastreamento exclusiva. Cada campo **[!UICONTROL ID de Rastreamento]** é pré-preenchido com o nome da experiência, de modo que as linhas que compartilham uma experiência em formatos de anúncio ou plataformas começam com o mesmo valor. Verifique e resolva essas duplicatas, não apenas as introduzidas por edições em massa. Se você editar uma ID de rastreamento em massa em várias linhas, confirme se deseja aplicar o mesmo valor a cada linha selecionada.

* **Usar URLs de destino válidas e completas**

  URLs inválidos podem acionar erros. Exemplo de erro: _A URL inserida não direciona para um site. Insira um URL válido e tente novamente. (100)_

* **Verifique se o aplicativo lida corretamente com a expiração do token**

  Os aplicativos devem solicitar novos tokens conforme necessário. Reautentique e obtenha um novo token de acesso fazendo logon novamente ou atualizando a sessão. Erro de exemplo: _Erro ao validar o token de acesso: a sessão foi invalidada porque o usuário alterou a senha ou o Facebook alterou a sessão por motivos de segurança. (190)_

* **Revise seu conjunto de anúncios e certifique-se de que apenas um anúncio esteja ativo a qualquer momento**

  Se precisar ativar vários anúncios do Meta, crie um Conjunto de anúncios dinâmico do Creative separado para cada um. Exemplo de erro: _O Conjunto de Anúncios Dinâmicos do Creative permite no máximo um anúncio ativo. Os usuários não podem criar mais de um anúncio no mesmo Conjunto de anúncios dinâmico do Creative. (100)_

* **Corresponder o número de regras aplicadas com a quantidade especificada pela plataforma**

  Os canais pagos esperam que o número de regras aplicadas corresponda ao formato especificado.  Se necessário, ajuste o número de regras para corresponder ao valor que a plataforma especifica. Exemplo de erro: _O Ad AssetFeed tem X regra(s) de destino para o formato: nome do formato, mas exatamente X regra de destino para esse formato é esperada. (100)_

* **Escolha uma call-to-action (CTA) compatível com seu objetivo de conjunto de anúncios**

  Frases de chamariz incompatíveis com o objetivo em Conjuntos de anúncios dinâmicos do Creative acionam um erro. Erro de exemplo: _O tipo de call to action X não é suportado para o objetivo Y no Conjunto de Anúncios do Dynamic Creative. (100)_

* **Verifique se o limite do conjunto de anúncios de destino oferece suporte ao número de experiências de anúncio**

  Confirme se o limite de anúncios do conjunto de anúncios alvo pode acomodar suas experiências de anúncios ativados. Se necessário, remova todos os anúncios desnecessários ou inativos do anúncio definido para ficar dentro desse limite. Como alternativa, crie um novo conjunto de anúncios para ativar anúncios adicionais. Erro de exemplo: _Você atingiu o limite de campanha, anúncios ou anúncios por conta publicitária. Cada conjunto de anúncios pode conter no máximo 50 anúncios. Isso inclui anúncios pausados/inativos/desativados. (100)_

* **Verifique se a plataforma oferece suporte ao tipo de CTA selecionado**

  Confirme se sua experiência inclui um tipo de CTA compatível. Exemplo de erro: _(#100) Tipo de call to action inválido (100)_
