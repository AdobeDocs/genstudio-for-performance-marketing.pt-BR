---
title: Otimizar sua ativação
description: Saiba como otimizar ativações para canais de anúncios pagos de terceiros.
level: Intermediate
feature: Ad Activation
exl-id: 5bc624c2-d064-4190-8761-ed05d0629d1f
source-git-commit: 6ee58b22761be357bb9ff753cf9e5bd5b431c513
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---

# Otimizar ativações

A ativação de uma experiência de anúncio para canais de anúncios pagos envolve duas fases principais:

* Preparando sua experiência para ativação

* Publicar sua experiência para os gerentes de anúncio de canal pago designados

Seguir as práticas recomendadas ao criar e ativar sua experiência de anúncio pode ajudar a minimizar possíveis complicações ou erros durante a entrega aos canais de público-alvo.

## Práticas recomendadas

Estas são algumas práticas recomendadas comuns e os erros que podem ser evitados.

* **Usar URLs de destino válidas e completas**

  URLs inválidos podem acionar erros. Exemplo de erro: _A URL inserida não direciona para um site. Insira um URL válido e tente novamente. (100)_

* **Verifique se o aplicativo lida corretamente com a expiração do token**

  Os aplicativos devem solicitar novos tokens conforme necessário. Conforme necessário, reautentique e obtenha um novo token de acesso fazendo logon novamente ou atualizando a sessão. Erro de exemplo: _Erro ao validar o token de acesso: a sessão foi invalidada porque o usuário alterou a senha ou o Facebook alterou a sessão por motivos de segurança. (190)_

* **Revise seu conjunto de anúncios e certifique-se de que apenas um anúncio esteja ativo a qualquer momento**

  Se precisar ativar vários Meta Ads, crie um Conjunto de anúncios dinâmico do Creative separado para cada um. Exemplo de erro: _O Conjunto de Anúncios Dinâmicos do Creative permite no máximo um anúncio ativo. Os usuários não podem criar mais de um anúncio no mesmo Conjunto de anúncios dinâmico do Creative. (100)_

* **Corresponder o número de regras aplicadas com a quantidade especificada pela plataforma**

  Os canais pagos esperam que o número de regras aplicadas corresponda ao formato especificado.  Se necessário, ajuste o número de regras para corresponder ao valor que a plataforma especifica. Exemplo de erro: _O Ad AssetFeed tem X regra(s) de destino para o formato: nome do formato, mas exatamente X regra de destino para esse formato é esperada. (100)_

* **Escolha uma chamada para ação (CTA) que seja compatível com seu objetivo de conjunto de anúncios**

  Frases de chamariz incompatíveis com o objetivo em Conjuntos de anúncios dinâmicos do Creative acionam um erro. Erro de exemplo: _O objetivo Y do Conjunto de Anúncios do Dynamic Creative não oferece suporte para a chamada para o tipo de ação X. (100)_

* **Verifique se o limite do conjunto de anúncios de destino oferece suporte ao número de experiências de anúncio**

  Confirme se o limite de anúncios do conjunto de anúncios alvo pode acomodar suas experiências de anúncios ativados. Se necessário, remova todos os anúncios desnecessários ou inativos do anúncio definido para ficar dentro desse limite. Como alternativa, crie um novo conjunto de anúncios para ativar anúncios adicionais. Erro de exemplo: _Você atingiu o limite de campanha, anúncios ou anúncios por conta publicitária. Cada conjunto de anúncios pode conter no máximo 50 anúncios. Isso inclui anúncios pausados/inativos/desativados. (100)_

* **Verifique se a plataforma oferece suporte ao tipo de CTA selecionado**

  Confirme se sua experiência inclui um tipo de CTA compatível. Erro de exemplo: _(#100) Chamada inválida para tipo de ação (100)_
