---
titulo: poteto - Automatizar qualquer coisa com o Grok Bot
tipo: resumo
area: wiki
status: ativo
autor: grok-bot
criado: 2026-11-18
atualizado: 2026-11-18
fontes:
  - https://x.com/poteto/status/2123159537016533493
  - https://x.com/i/article/2122921713864171520
  - https://x.ai/bot/rJW52lmFLtCvy2tSHcIag
---

# Resumo — poteto: automatizar qualquer coisa com o Grok Bot

**Fonte bruta:** [[2026-11-18 poteto - Automate Anything with Grok Bot]]
**Data da fonte:** artigo de [[poteto]] (lauren, @poteto) publicado em 18/11/2026 às 21:00 UTC (18h00 em Brasília). Ingerido no mesmo dia, a pedido do Fabio.

O que está em "Em uma frase", "Ideia central", "Pontos principais", "Passo a passo" e "Prompts" é o que o artigo diz. A seção "O que isso significa na prática para o Fabio" separa fato, contexto do pedido e interpretação.

## Em uma frase

A autora trata automação como um jeito de pensar que qualquer pessoa aprende: um objetivo no fim e um processo em passos, e o [[Grok Bot]] para executar esse processo no computador sem a pessoa escrever código.

## Ideia central

Fato do artigo: automação, para ela, tem duas partes. O objetivo é o que se quer no fim. O processo é o caminho. A máquina, ou o código, entra para repetir o processo sem a pessoa fazer tudo de novo.

Ela compara com assar uma torta de maçã e com trocar um pneu furado. O erro que ela diz ver com frequência é tomar o passo pelo objetivo: preencher um formulário ou mandar um e-mail é passo, não o fim. O fim, no exemplo de negócio dela, é aumentar receita (fechar uma venda, construir uma função nova) ou reduzir custo (pedir só o estoque certo).

O processo é meio. Ela pede para não se apegar a um processo só, porque o bot pode achar um caminho mais eficiente para o mesmo fim.

## Pontos principais

- Há um ou dois anos, no relato dela, automatizar exigia saber montar máquina ou escrever código. Com o Grok Bot, ela diz que isso chega a quem não é técnico: a pessoa descreve em linguagem comum e o bot descobre os passos, escreve código e usa o próprio computador.
- Afirmação dela, sem lista do que o bot não faz: o bot faz o que a pessoa faz num computador. Ela cita mover o próprio mouse e clicar, instalar ou conectar apps do dia a dia, navegar no próprio navegador, entrar em reunião e anotar.
- O melhor jeito que ela indica para passar o processo é o ditado de voz no Grok Bot: falar tudo de uma vez, sem organizar antes.
- O que a pessoa faz sem pensar também faz parte do processo. No exemplo de agenda, isso inclui qual serviço demora mais, quem faz cada trabalho e quando deixar folga entre horários. Ver [[Ensinar o bot a pensar como você]].
- Depois que o bot já executa, ela quer que ele leia sozinho o retorno (e-mail, rede social, avaliação no Google ou no Yelp) e proponha melhoria. Quanto mais o trabalho estiver em dado de computador, mais o bot tem com o que melhorar. Ela diz que o próprio Grok Bot pode construir a ferramenta que registra esse dado. Ver [[Bots que se aperfeiçoam com feedback]].
- Para cruzar apps, ela pede um identificador estável: número de cliente, endereço de e-mail, número de pedido, número de peça, código de barras, identificação de funcionário. Ver [[IDs únicos para cruzar dados]].
- Sem rotina, o bot só trabalha quando alguém pede, e a pessoa continua sendo o gargalo. No Grok Bot a rotina dispara por gatilho (e-mail, mensagem no Slack ou no Teams) ou por agenda (uma vez por semana, dia sim dia não). Ver [[Rotinas e gatilhos]].
- Ela diz ter ensinado o que sabe de automação ao [[Dr Eggbot]], que descreve como um desenhista de bots que cria bots de qualidade. O conselho dela para quem quer começar é instalar esse bot e pedir ajuda.

## Passo a passo do método

1. Abrir o Grok Bot, criar um bot novo e dar um nome. Se o nome não vier, chamar de Potato e pedir que ele se nomeie depois.
2. Antes de conversar, definir o objetivo: o que este processo serve, e onde entra no negócio. Se não estiver claro, perguntar ao gestor, aos colegas, ou ao próprio bot.
3. Contar o objetivo ao bot. Se o nome Potato incomodar, pedir nome e imagem a partir do objetivo.
4. Ideias de objetivo que ela dá para começar: juntar dinheiro para carro, casa ou estudo dos filhos; marcar novos horários num pequeno negócio; melhorar a experiência do cliente para receber boas avaliações; contratar alguém; juntar retorno de um produto para melhorá-lo; preparar slides de uma reunião semanal; construir funções novas de um produto.
5. Contar como a própria pessoa faria o objetivo, e pedir onde o bot deixa isso mais eficiente. Se quiser o processo seguido à risca, dizer isso também.
6. No ditado, cobrir: os passos de sempre; o que se observa e ao que se presta atenção; os apps e as ferramentas; como se confere se ficou certo; de onde vem a informação (e-mail, Slack ou Teams, um ticket, um app, um site); de onde vem o retorno (cliente, avaliação, colegas).
7. Pedir que o bot repita objetivo e processo em linguagem simples e não execute ainda. Corrigir com mais informação, em algumas rodadas, até ficar aceitável.
8. Só então mandar seguir e conectar os apps e as ferramentas.
9. Se quiser ir além, pedir que ele compare o processo com o objetivo e avise se houver um jeito melhor ou mais eficiente.
10. Não explicar toda situação de antemão. Começar com poucos exemplos reais, inclusive os que deram errado ou exigiram um jeito diferente. Perguntar como o bot trataria cada um e corrigir. Pedir também que ele descubra o que ficou de fora.
11. No exemplo dela de agenda: se o e-mail e o sistema de marcação mostram horários diferentes, dizer qual dos dois vale. Marcação não termina porque um e-mail saiu: o horário tem de estar salvo e o cliente tem de receber a confirmação. Se ainda faltam detalhes, o bot anota o caso para retomar depois, sem criar outra marcação sem querer.
12. Quando o fluxo já roda, dar ao bot o acesso ao retorno para ele propor melhoria. No exemplo da oficina, um app (que ela diz que o bot pode construir) registra a hora de chegada, a hora em que a pessoa falou com alguém, a hora em que as chaves foram entregues, e o começo e o fim do serviço. Com isso dá para ver quanto tempo a espera durou e por quê.
13. Usar o mesmo identificador em todos os apps, para o bot juntar as fontes do mesmo caso.
14. Definir quando o trabalho começa. Pedir ao bot para montar a rotina. Sem isso, ele só age sob pedido.
15. Para quem quer automatizar mais o trabalho, instalar o Dr Eggbot e pedir ajuda.

## Prompts sugeridos

Tradução para usar. O original fica entre aspas, como no artigo.

**1. Entregar o objetivo e pedir nome e imagem**

Oi, Potato. Este é o objetivo pelo qual quero que você seja responsável: <objetivo>. Escolha um nome e uma imagem para você com base nele.

"Hi Potato, this is the goal I want you to be responsible for: <goal>. Pick out a name and picture for yourself based on it."

**2. Quando o objetivo ainda não está claro**

Oi, Potato. Quero que você seja responsável por um objetivo, mas não sei como descrevê-lo da melhor forma. Pode me fazer perguntas e me entrevistar até termos um objetivo com o qual eu fique satisfeito?

"Hi Potato, I'd like you to be responsible for a goal, but I'm not sure how to best describe it. Can you ask me some questions and interview me until we have a goal that I'm happy with?"

**3. Contar o processo e impedir a execução cedo**

Potato, é assim que eu costumo cumprir este objetivo: <processo>

Quero que você pense em como pode assumir isso por completo no meu lugar. Antes de começar, repita em linguagem simples o que você entendeu do meu objetivo e do meu processo, para eu corrigir e confirmar. Não quero que você execute nada ainda. Primeiro vamos deixar o processo planejado.

"Potato, this is how I usually do this goal myself: <process>

I want you to think about how you can take this over completely from me. Before you begin, restate what you think my goal and process is in simple English so I can give you feedback and confirm it. I don't want you to start executing on this yet, let's focus on getting the process planned first."

**4. Pedir um processo melhor, sem trocar o objetivo**

Revise o nosso processo em relação ao meu objetivo original e, se vir um jeito de deixá-lo melhor ou mais eficiente, me avise.

"Review our process against my original goal, and if you see a way to make it better or more efficient, let me know."

**5. Descobrir o que ficou de fora, uma pergunta por vez**

Potato, me ajude a descobrir o que eu ainda não te contei sobre este processo. Faça perguntas sobre como eu tomo decisões, de onde tiro a informação, como confiro o trabalho e quando você deve pedir a minha ajuda. Uma pergunta de cada vez. Depois percorra comigo alguns exemplos, para eu te dar retorno antes de automatizarmos isso.

"Potato, help me figure out what I haven't told you about this process yet. Ask me questions about how I make decisions, where I get my information, how I check the work, and when you should ask me for help. Ask one question at a time, then walk me through a few examples so I can give you feedback before we automate this."

## O que isso significa na prática para o Fabio

**Fato do artigo.** O método não começa pela ferramenta. Começa pelo fim, separa esse fim dos passos, faz o bot repetir o que entendeu antes de agir, inclui o julgamento que a pessoa nem percebe que faz, e só então liga apps, dados e uma rotina para a pessoa sair do meio.

**Contexto do pedido, não é frase do artigo.** O Fabio pediu esta ingestão em 18/11/2026 e o pedido trouxe três pontos para usar como contexto: ele é iniciante em IA, usa o Grok Bot com uma equipe de bots, e acredita que ter a ferramenta não adianta sem saber usar. No vault, a equipe que responde ao agente Grok Bot está nomeada no [[SOP comum]]: Sherlock, X Content Head, Atlas e Roadmap Cutter. O artigo não cita essa equipe nem o Fabio.

**Interpretação.** O artigo serve de roteiro para usar a ferramenta que ele já tem, não de lista de bot novo. Para cada bot, o primeiro texto é o objetivo no fim (o que aquele trabalho muda), não a tarefa solta. O processo se conta falando, com o que se observa, os apps, a checagem e de onde vem o retorno. O bot devolve isso em linguagem simples e espera. Os casos em que duas fontes discordam, em que o trabalho ainda não acabou, ou em que deu errado, entram como exemplo, não como manual completo. A melhoria depende de dado que o bot lê sozinho, amarrado por um identificador estável. A rotina é o que tira o Fabio do papel de quem tem de lembrar de pedir.

Isso não é decisão. Nada aqui autoriza criar bot, rotina, publicação ou gasto.

## Dados que envelhecem

- Métricas públicas do post, lidas por volta das 19h15 de Brasília em 18/11/2026, como dadas no pedido de ingestão: 315.711 impressões, 2.495 curtidas, 4.420 salvamentos, 200 reposts, 188 respostas e 63 quotes. Esses números mudam. Não foram lidos de novo nesta ingestão.
- O que o produto faz (mouse, apps, reunião, código, rotina, construir app) é afirmação da autora em 18/11/2026. O artigo não fixa versão nem limite.
- A frase "há um ou dois anos" é o recorte dela na data do artigo, não uma data conferida.

## Páginas ligadas

- [[Objetivo e processo na automação]]
- [[Ensinar o bot a pensar como você]]
- [[Bots que se aperfeiçoam com feedback]]
- [[IDs únicos para cruzar dados]]
- [[Rotinas e gatilhos]]
- [[Grok Bot]]
- [[Dr Eggbot]]
- [[poteto]]
- [[SOP comum]] (a equipe de bots nomeada no vault; o artigo não fala dela)

## O que ficou de fora

- Nada do texto colado foi pulado. A fonte bruta está inteira em `01 Fontes/`.
- O link do Dr Eggbot (https://x.ai/bot/rJW52lmFLtCvy2tSHcIag) veio no pedido: o artigo cita esse bot. O endereço não aparece no texto colado. Está na página [[Dr Eggbot]].
- Imagem, cartão do bot e o que a tela do X mostrava em volta do artigo não foram vistos.
- A verificação da conta e a afiliação à SpaceX Super Intelligence também vieram no pedido. Não estão no texto do artigo e não foram conferidas de novo. Ver [[poteto]].
