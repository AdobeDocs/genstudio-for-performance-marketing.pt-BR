---
title: Recursos de texto
description: Saiba mais sobre o recurso de texto das categorias de atributo usadas no GenStudio for Performance Marketing.
feature: Reporting and Insights, Text Attributes, Generative AI
exl-id: 7b81b0ae-0c62-468f-965c-fd8070644fb3
TQID: https://experienceleague.adobe.com/Oec5q249StCtuG-2-n1dYmJoEDRPaqLF2QANpwClQ3A
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: c95c94c1-727b-457a-9184-a4dda4c95ab2id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
subfeature_v2: id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: d095671a-1355-40aa-8b5f-06c33c68080bid: e0eb8757-182f-49f3-94a4-1587d16f5094id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eb30f47f-d87a-400f-8f78-63ce7979ff56id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3id: fc314d1d-7cb9-4a38-8dbd-8f9b6478f40d
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 1298
ht-degree: 1%

---

# Recursos de texto

Os recursos de texto incluem contagens para determinados elementos de texto, como palavras, sentenças, emojis e classificações para semântica, emoção e tom usados para análise com [!DNL Insights]. O texto também pode receber uma pontuação de legibilidade.

O GenStudio for Performance Marketing usa os recursos de IA e aprendizado de máquina do Adobe para estudar texto e aplicar [!UICONTROL atributos de mídia] com base nos tons de texto associados e na narrativa de marketing. O processo valida o texto de entrada para garantir que ele contenha caracteres alfanuméricos, removendo espaços em branco extras e caracteres não imprimíveis e truncando o texto para o máximo permitido de 1500 palavras. Antes de aplicar as tags de atributo detectadas, a IA prevê o tom predominante.

## Tom de voz

Tom representa um caráter geral, atitude ou atmosfera exibida através da linguagem. Uma simples escolha de palavras e pontuação, estrutura de frase e estilo pode alterar o tom da mensagem. Por exemplo, considere as seguintes mensagens urgentes usando os três níveis básicos de tom:

| Tom | Descrição | Exemplo |
| -------------- | ----------------------------------- | --------------------------------------------------------- |
| Formal | Linguagem polida e profissional. | `Take advantage of this distinctive and exceptional opportunity!` |
| Conversação | Linguagem amigável e informal. | `Don't miss out on this great opportunity!` |
| Direto | Direto e direto ao ponto. | `Don't miss the chance!` |

Outros valores secundários para tom fornecem uma distinção mais fina do caractere e da atitude da mensagem. Em conformidade com o exemplo anterior de uma mensagem urgente, a GenAI pode detectar um tom _poético_ neste exemplo caprichoso: `Embrace the moment, without delay, for this occasion won't always stay.`

A tabela a seguir lista os valores de tons reconhecidos pela IA do GenStudio for Performance Marketing.

| Tom | Descrição | Exemplo |
| -------------- | ------------------------------------------------ | --------------------------------------------------------- |
| Assertivo | Confiante e vigoroso na expressão. | `You need to act now to secure this deal!` |
| Direto | Direto e direto ao ponto. | `Don't miss the chance!` |
| Empático | Mostrar compreensão e sensibilidade. | `We understand your needs, and this is perfect for you.` |
| Entusiasta | Mostrando prazer, interesse ou aprovação intensa e ansiosa. | `This is an amazing opportunity you can't miss!` |
| Humorístico/Espirituoso | Leve e inteligente. | `Why wait? Grab this deal before it's gone!` |
| Inspirador | Encorajador e edificante. | `Believe in yourself and seize this opportunity!` |
| Poético | Artístico e expressivo. | `Embrace the dawn of a new opportunity.` |
| Quantitativo | Com base em dados numéricos. | `99% of users loved this offer, and you will too.` |
| Sensorial | Envolver os sentidos. | `Feel the excitement with this incredible offer!` |
| Contar histórias | Narrar uma história para transmitir uma mensagem. | `Once upon a time, there was an offer you couldn't refuse.` |

## Apelo emocional

Os profissionais de marketing usam o poder das emoções humanas para criar uma forte conexão entre o público-alvo e a marca. Ao tocar nos sentidos, como felicidade, medo, excitação ou nostalgia, os profissionais de marketing podem criar mensagens que repercutem em um nível mais profundo, estimulando o engajamento e influenciando o comportamento do consumidor. O apelo emocional ajuda a fornecer conteúdo mais relacionável e memorável, promovendo, em última análise, a fidelidade à marca e incentivando as ações desejadas.

Táticas de persuasão, emoções de marketing e estilos narrativos funcionam juntos para direcionar segmentos de clientes.

- **Estilos narrativos**, como autenticidade, celebração e comunidade, ajudam a transmitir os valores e a identidade que refletem no público-alvo, criando uma mensagem mais convincente e relacionável.
- **As táticas de persuasão**, como escassez, prova social e reciprocidade, foram projetadas para influenciar o comportamento do consumidor, atraindo suas emoções e preferências.
- **As emoções do marketing** têm como objetivo estimular sentimentos que melhoram o engajamento e a conexão com a marca.

A IA do GenStudio for Performance Marketing detecta e diferencia essas características analisando o texto em busca de dicas emocionais, tom e estilo narrativo. A IA usa processamento de linguagem natural (NLP) e algoritmos de aprendizado de máquina para identificar padrões e classificar o texto com base em atributos emocionais e persuasivos predefinidos.

### Estilo narrativo

Os atributos de narrativa, ou fator de apelo, ajudam a identificar a mídia que comunica os valores, a finalidade ou a identidade que repercute com seu público-alvo. A tabela a seguir lista os estilos narrativos reconhecidos pela IA do GenStudio for Performance Marketing.

| Fator de recurso | Descrição | Exemplo |
| ----------------- | --------------------------------------------------------------------- | ------------------------------------------ |
| Autenticidade | Genuíno e real, destacando muitas vezes a transparência e a honestidade. | `A behind-the-scenes look at how our products are made.` |
| Celebração | Marcando ocasiões ou realizações especiais com alegria e festividade. | `Join us in celebrating our 10th anniversary with special offers!` |
| Comunidade | Promover um sentimento de pertença e união entre um grupo. | `Our brand is built on the strength of our community.` |
| Conveniência | Enfatizando a facilidade de uso e os benefícios que economizam tempo. | `Get what you need with just one click.` |
| Capacitação | Incentivar e permitir que os indivíduos assumam o controle e tomem decisões. | `Empower yourself with our latest tools and resources.` |
| Exploração | Convidar a descoberta e a aventura, muitas vezes associadas a novas experiências. | `Discover new horizons with our travel packages.` |
| Futurista | Destacar a inovação e as ideias prospetivas. | `Experience the future of technology today.` |
| Hipe | Gerar entusiasmo e expectativa em torno de um produto ou evento. | `Don't miss out on the most anticipated event of the year!` |
| Indulgência | Atraindo fantasias, desejos ou prazeres. | `Treat yourself to the finest gourmet chocolates.` |
| Tranquilidade | Dando tranquilidade e segurança. | `Rest easy knowing your data is safe with us.` |
| Personalização | Personalizar experiências ou produtos de acordo com preferências individuais. | `Get a custom-fit solution just for you.` |
| Prestige | Associar com alto status e exclusividade. | `Join the elite with our premium membership.` |
| Timelless | Enfatizando qualidade duradoura e apelo clássico. | `Our designs are timeless and never go out of style.` |
| Versatilidade | Destacando a adaptabilidade e usos múltiplos. | `Our product fits seamlessly into any lifestyle.` |
| Bem-estar | Promover a saúde, a felicidade e o bem-estar geral. | `Enhance your well-being with our holistic approach.` |

### Táticas de persuasão

Técnicas de persuasão são usadas para influenciar o comportamento do consumidor e impulsionar as ações desejadas. Essas estratégias são direcionadas a acionadores psicológicos específicos e segmentos de clientes para melhorar a eficácia das mensagens de marketing. A tabela a seguir lista as táticas de persuasão reconhecidas pela IA do GenStudio for Performance Marketing.

| Tático | Descrição | Exemplo |
| --------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| Antropomorfismo | Atribuição de características humanas a produtos ou marcas. | `Our friendly chatbot is here to help you.` |
| Comparação | Destacar as diferenças entre as opções para influenciar a escolha. | `See how we compare to the competition.` |
| Concretização | Fornecer detalhes específicos para tornar a mensagem mais tangível. | `Save 20% on your next purchase.` |
| Endosso | Apresentando aprovação de fontes ou influenciadores confiáveis. | `Recommended by top industry experts.` |
| Pé na porta | Começando com uma pequena solicitação para aumentar a probabilidade de concordar com uma solicitação maior. | `Try our free trial today.` |
| Superar a reatância | Reduzir a resistência reconhecendo e abordando as objeções. | `We understand your concerns, and here's how we address them.` |
| Reciprocidade | Oferecer algo de valor para incentivar um favor de retorno. | `Get a free gift with your purchase.` |
| Escassez | Criar um senso de urgência destacando a disponibilidade limitada. | `Only a few items left in stock!` |
| Identidade social | Aproveitar o sentimento de pertença do consumidor a um grupo. | `Join our community of innovators.` |
| Impacto social | Sublinhar o impacto positivo na sociedade ou no ambiente. | `Your purchase helps plant a tree.` |
| Prova social | Usar depoimentos ou conteúdo gerado pelo usuário para criar confiança. | `See why thousands of users love our product.` |

### Emoções de marketing

As emoções são direcionadas em mensagens de marketing para evocar sentimentos e respostas específicas do público, o que pode melhorar o engajamento e a conexão com a marca. A tabela a seguir lista as emoções reconhecidas pela IA do GenStudio for Performance Marketing.

| Emoção | Descrição | Exemplo |
| ------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| Aspiração | Inspirando um desejo de alcançar ou alcançar algo maior. | `Imagine the possibilities with our premium service.` |
| Desafio | Incentivar o público a superar um obstáculo ou adotar uma nova tarefa. | `Are you ready to take the next step in your career?` |
| Curiosidade | Despertando interesse e desejo de aprender mais. | `Discover the secrets behind our success.` |
| Exclusividade | Criação de uma sensação de fazer parte de um grupo selecionado. | `Join our exclusive club for members-only benefits.` |
| Fascínio | Captivar o público-alvo com conteúdo intrigante ou interessante. | `Be amazed by our latest innovations.` |
| Gratificação | Proporcionando satisfação e prazer ao usar o produto ou serviço. | `Enjoy the ultimate comfort with our luxury bedding.` |
| Reconhecimento | Reconhecer e avaliar as realizações ou o status do público-alvo. | `Get the recognition you deserve with our award-winning service.` |
| Confiança | Aumentar a confiança e a confiabilidade na marca. | `Trust us to deliver quality and excellence every time.` |
| Urgente | Solicitar ação imediata enfatizando oportunidades sensíveis ao tempo. | `Act now before this limited-time offer expires!` |

## Pontuação de legibilidade

A pontuação de legibilidade avalia a facilidade de leitura e compreensão de um texto. Isso ajuda a garantir que seu conteúdo seja apropriado para seu público-alvo. As pontuações são baseadas em vários fatores, incluindo comprimento da frase e complexidade da palavra. A tabela a seguir lista os níveis de legibilidade reconhecidos pela IA do GenStudio for Performance Marketing.

| Nível de legibilidade | Descrição | Exemplo |
| ------------------- | ------------------------------------------------------------------ | --------------------------------------------------------- |
| 5ª série | Linguagem muito simples, adequada para crianças pequenas. | `The cat sat on the mat.` |
| 6ª série | Linguagem simples e clara, adequada para um público em geral. | `You can find great deals on our website.` |
| 7ª série | Fácil de entender, com vocabulário e estrutura simples. | `Our new product is simple to use and very effective.` |
| 8º e 9º ano | Linguagem clara e concisa, adequada para adolescentes. | `This guide will help you understand the basics of our service.` |
| 10º ao 12º ano | Linguagem mais complexa, adequada para adolescentes mais velhos e adultos. | `The comprehensive manual provides detailed instructions for setup.` |
| Faculdade | Linguagem avançada, adequada para um público bem educado. | `The study explores the multifaceted implications of the new policy.` |
| Graduação universitária | Linguagem altamente avançada, adequada para especialistas. | `The dissertation delves into the intricacies of quantum mechanics.` |

## Contagens

Entender e aproveitar atributos de contagem como contagens de hashtag, contagens de palavras, contagens de frases e proporções de palavras de interrupção pode aprimorar significativamente sua estratégia de conteúdo. Essas métricas oferecem insights valiosos sobre a eficácia e o alcance de seus esforços de marketing. A tabela a seguir lista as categorias de contagem reconhecidas pela IA do GenStudio for Performance Marketing.

| Categoria | Descrição | Exemplo |
| --------------------- | --------------------------------------------------------------------------- | --------------------- |
| Contagem de Emojis | O número de emojis presentes no texto. Os emojis podem melhorar o engajamento e transmitir emoções rapidamente. | `😊`, `🚀`, `❤️` |
| Contagem de HashTags | O número de hashtags usadas no texto. As hashtags ajudam a categorizar o conteúdo e aumentar a capacidade de descoberta em redes sociais. | `#Marketing`, `#Sale` |
| Contagem de palavras por frase | O número médio de palavras por frase no texto. Frases mais curtas geralmente são mais fáceis de ler e entender. | `10` |
| Contagem de palavras | O número total de palavras no texto. Uma contagem de palavras mais alta pode fornecer informações mais detalhadas, mas também pode exigir mais esforço para ler. | `1500 words` |
| Taxa de palavras de interrupção | A proporção de palavras de interrupção para palavras significativas no texto. As palavras de interrupção (como &quot;a&quot; &quot;an&quot; &quot;the&quot;) geralmente são ignoradas em consultas e resultados de pesquisa. Uma alta proporção de palavras de interrupção pode tornar o conteúdo menos envolvente e mais difícil de ler. | `0.375` |
| Contagem de frases | O número total de frases no texto. Mais frases podem indicar conteúdo mais detalhado, mas textos muito longos podem perder o interesse do leitor. | `75 sentences` |
