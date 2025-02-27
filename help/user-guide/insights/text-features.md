---
title: Recursos de texto
description: Saiba mais sobre o recurso de texto das categorias de atributo usadas no GenStudio for Performance Marketing.
feature: Insights, Attributes, Generative AI
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 5cff6d1dd097b18e4fa3d286afddc1db553a415d
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 1%

---

# Recursos de texto

Os recursos de texto incluem contagens para determinados elementos de texto, como palavras, sentenças, emojis e classificações para semântica, emoção e tom usados para análise com [!DNL Insights]. O texto também pode receber uma pontuação de legibilidade.

O GenStudio for Performance Marketing usa os recursos de IA e aprendizado de máquina do Adobe para estudar texto e aplicar [!UICONTROL atributos de ativos] com base nos tons de texto associados e na narrativa de marketing. O processo valida o texto de entrada para garantir que ele contenha caracteres alfanuméricos, removendo espaços em branco extras e caracteres não imprimíveis e truncando o texto para o máximo permitido de 1500 palavras. Antes de aplicar as tags de atributo detectadas, a IA prevê o tom predominante.

## Tom de voz

Tom representa um caráter geral, atitude ou atmosfera exibida através da linguagem. Uma simples escolha de palavras e pontuação, estrutura de frase e estilo pode alterar o tom da mensagem. Por exemplo, considere as seguintes mensagens urgentes usando os três níveis básicos de tom:

- `Formal`

  ```
  Take advantage of this distinctive and exceptional opportunity!
  ```

- `Conversational`

  ```
  Don't miss out on this great opportunity!
  ```

- `Direct`

  ```
  Don't miss the chance!
  ```

A IA detecta ainda mais um tom mais sutil. Usando a mesma declaração urgente do exemplo anterior, a versão a seguir usa um tom `poetic` fantástico:

- `Poetic`

  ```
  Embrace the moment, without delay, for this occasion won't always stay.
  ```

Outros valores secundários para tom incluem: `Enthusiastic`, `Assertive`, `Humorous/Witty`, `Inspirational`, `Empathetic`, `Sensory`, `Storytelling`, `Poetic`, `Quantitative`, `Personal`

## Narrativa

Os atributos narrativos ajudam a identificar ativos que comunicam os valores, a finalidade ou a identidade que repercutem com seu público-alvo.

| Narrativa | Descrição | Exemplo |
| ----------------- | ----------- | ------- |
| `Authenticity` |             |         |
| `Celebration` |             |         |
| `Community` |             |         |
| `Convenience` |             |         |
| `Empowerment` |             |         |
| `Exploration` |             |         |
| `Futuristic` |             |         |
| `Hype` |             |         |
| `Indulgence` |             |         |
| `Peace of mind` |             |         |
| `Personalization` |             |         |
| `Prestige` |             |         |
| `Timelessness` |             |         |
| `Versatility` |             |         |
| `Well-being` |             |         |

## Pontuação de legibilidade

A pontuação de legibilidade avalia a facilidade de leitura e compreensão de um texto. Isso ajuda a garantir que seu conteúdo seja apropriado para seu público-alvo. As pontuações são baseadas em vários fatores, incluindo comprimento da frase e complexidade da palavra.

| Pontuação | Nível escolar | Notas |
| ----------- | ------------------ | ------------------------------------------------------------------------- |
| 100,00-90,00 | 5ª série | Muito fácil de ler. Facilmente compreendido por um aluno médio de 11 anos. |
| 90.0-80.0 | 6ª série | Fácil de ler. Conversação em inglês para consumidores. |
| 80.0-70.0 | 7ª série | Bastante fácil de ler. |
| 70.0-60.0 | 8º e 9º ano | Inglês simples. Facilmente compreendido por estudantes de 13 a 15 anos. |
| 60.0-50.0 | 10º ao 12º ano | Bem difícil de ler. |
| 50.0-30.0 | Faculdade | Difícil de ler. |
| 30.0-0.0 | Graduação universitária | Muito difícil de ler. Mais bem compreendido pelos graduados da universidade. |

## Contagens de palavras

A ser definido

A tabela a seguir lista as categorias de recursos de imagem reconhecidas pela IA do GenStudio for Performance Marketing.

| Categoria | Descrição | Exemplo |
| -------------------- | ------------- | --------------------- |
| Contagem de Emojis |             |        |
| Contagem de HashTags |             |        |
| Palavras-chave |             |        |
| Emoções de marketing | As emoções são direcionadas em mensagens de marketing para evocar sentimentos e respostas específicas do público, o que pode melhorar o engajamento e a conexão com a marca. | `Aspiration`, `Challenge`, `Curiosity`, `Exclusivity`, `Fascination`, `Gratification`, `Recognition`, `Trust`, `Urgency` |
| Estratégias de persuasão | Técnicas usadas para influenciar o comportamento do consumidor e impulsionar as ações desejadas. Essas estratégias são direcionadas a acionadores psicológicos específicos e segmentos de clientes para melhorar a eficácia das mensagens de marketing. | `Social identity`, `Social proof`, `Endorsement`, `Concreteness`, `Foot in the door`, `Overcoming reactance`, `Reciprocity`, `Comparison`, `Social impact`, `Scarcity`, `Anthropomorphism` |
| Tom de voz | O caractere geral, a atitude ou a atmosfera transmitida em uma mensagem de marketing por meio de escolha de palavra, pontuação, estrutura de frase e estilo. | `Enthusiastic`, `Assertive`, `Humorous/Witty`, `Inspirational`, `Empathetic`, `Sensory`, `Storytelling`, `Poetic`, `Quantitative`, `Personal` |
