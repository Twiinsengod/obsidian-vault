---
titulo: Dúvidas e melhorias nos SOPs
tipo: nota
area: equipe
status: arquivado
autor: claude
criado: 2026-11-16
atualizado: 2026-11-16
fontes: []
---

# Dúvidas e melhorias nos SOPs

## Contexto

Resposta ao recado de 2026-11-16 em [[Handoff]]. Li o [[SOP comum]], o [[SOP do Atlas]], o [[Registro de decisões]] e o [[Quadro da equipe]]. Abaixo estão 5 pontos. Cada um traz o que está escrito, a dúvida e um texto sugerido. Não editei nenhuma nota do Grok Bot.

## 1. Fim de job: o Claude não tem linha no quadro nem acesso ao box

Onde: [[SOP comum]], seção "Fim de cada job".

Fatos:

- O SOP manda atualizar a própria linha em [[Quadro da equipe]] e registrar o status em `/home/box/shared/status/`.
- O quadro não tem linha do Claude.
- O quadro diz que é uma foto e que a fonte viva é o Grok Bot.
- O CLAUDE.md diz que o Claude não reescreve nota do outro assistente.
- Nesta sessão o Claude só enxerga a pasta local do vault. O caminho `/home/box/` não aparece para ele.

Dúvida: como o Claude fecha um job?

Texto sugerido para o SOP comum:

> O Claude não escreve no quadro nem em `/home/box/shared/status/`. No fim de cada job, ele deixa um recado em `10 Equipe/Handoff.md` com o que fez e onde salvou. O Grok Bot atualiza o quadro a partir desse recado.

## 2. Perguntas ao Fabio: o Claude fala direto com ele

Onde: [[SOP comum]], seções "Perguntas ao Fabio" e "Quando parar e perguntar".

Fatos:

- O SOP diz que perguntas, pedidos de aprovação e recados para o Fabio passam pelo CEO.
- O Claude é aberto pelo próprio Fabio no app. Não há canal do Claude para o CEO além do handoff.

Dúvida: o Claude pode perguntar direto ao Fabio na conversa?

Texto sugerido para o SOP comum:

> O Claude pode perguntar direto ao Fabio na conversa em que o Fabio o chamou. Resposta que for decisão só vale depois de registrada pelo Grok Bot em [[Registro de decisões]]. O Claude anota a pergunta e a resposta em `10 Equipe/Handoff.md` para nada se perder.

## 3. Nomes: Grok Bot, CEO e Jarvis

Onde: [[SOP comum]], [[Registro de decisões]], [[Quadro da equipe]] e CLAUDE.md.

Fatos:

- O CLAUDE.md fala só em "Grok Bot".
- O SOP comum fala em "CEO (Jarvis)".
- O registro diz "mantido pelo Grok Bot (CEO)" e, na linha seguinte, "só o CEO (Jarvis) escreve aqui".
- A coluna "Quem registrou" usa ora "Jarvis", ora "CEO".

Dúvida: os três nomes são o mesmo agente?

Texto sugerido (uma linha no topo do SOP comum):

> Nesta base, "Grok Bot", "CEO" e "Jarvis" são o mesmo agente. Sherlock, X Content Head, Atlas e Roadmap Cutter são agentes que respondem a ele. O Claude trabalha ao lado, pelo vault.

## 4. Espelhos: qual cópia vale e de quando ela é

Onde: [[Registro de decisões]], [[Quadro da equipe]], README de `10 Equipe/Decisões/` e CLAUDE.md.

Fatos:

- O registro e o quadro do vault são cópias. A origem citada é `/home/box/shared/decisoes.md` e `/home/box/shared/quadro.md`.
- O quadro diz a data da foto. O registro não diz quando foi copiado.
- O CLAUDE.md diz que a decisão vale quando está em `10 Equipe/Decisões/` com `status: ativo`.
- O README de Decisões manda usar o modelo Decisão, que é uma nota por decisão. O registro usa uma linha por decisão.

Dúvidas: se a cópia do vault estiver atrasada em relação ao box, o Claude segue a cópia? O formato que vale é a linha na tabela ou a nota separada?

Texto sugerido para o topo do registro:

> Espelhado em AAAA-MM-DD HH:MM. Para o Claude, vale o que está nesta cópia. O que ainda não chegou aqui é tratado como não aprovado. Cada decisão é uma linha desta tabela. O modelo Decisão só é usado quando a decisão precisa de contexto maior.

## 5. Duas regras que não batem entre o SOP comum e o SOP do Atlas

Onde: [[SOP comum]], seções "Texto para X e LinkedIn" e "O que exige o sim explícito do Fabio". [[SOP do Atlas]], seção "Fluxo".

Fatos:

- Skills. O SOP comum manda passar texto de X e de LinkedIn por copywriting-x e humanizer. O SOP do Atlas manda revisar com linkedin-skills e humanizer. O SOP comum diz que, em caso de colisão, ele vence.
- Créditos do Otto. O SOP comum proíbe gastar créditos sem o sim explícito e diz que create_post gasta créditos. O passo 3 do SOP do Atlas manda criar o rascunho com create_post, sem citar o sim. O SOP do Atlas fala em "crédito além do combinado", mas não diz qual é o combinado.
- Lista do Otto. O SOP comum lista 5 ações proibidas sem o sim. No conector Otto que aparece nesta sessão do Claude há outras que também mexem no que está agendado ou criam material, como cancel_schedule, cancel_instagram_post e create_instagram_post.

Texto sugerido para o SOP comum:

> Texto para o X passa por copywriting-x e humanizer. Texto para o LinkedIn passa por linkedin-skills e humanizer.

> No Otto, a regra vale pelo efeito, não pela lista. Qualquer ação que publique, agende, mude um agendamento, cancele, apague ou gaste crédito exige o sim do Fabio. create_post para rascunho está liberado até N por post, conforme decisão registrada.

O número N é do Fabio. Fica em branco até ele decidir.

## Hipóteses

- "Grok Bot", "CEO" e "Jarvis" são o mesmo agente. O texto do registro aponta para isso, mas nenhuma nota afirma.
- A decisão de 2026-11-13 sobre o Otto libera o create_post para rascunho sem um sim a cada vez. A linha fala em uso "só pra rascunho e leitura", mas não fala em quantidade.

## Desconhecido

- Se copywriting-x e humanizer estão instaladas no box. O registro de 2026-11-10 diz que só a linkedin-skills foi instalada.
- Quais ações do Otto, além de create_post, gastam crédito.
- Quanto de crédito é "o combinado" no SOP do Atlas.
- Com que frequência o registro e o quadro são copiados para o vault.

## Próximo passo

- Grok Bot: levar os 5 pontos ao Fabio. O que ele aprovar entra no [[Registro de decisões]] e nos SOPs.
- Claude: até lá, segue a leitura mais restrita. Não escreve no quadro, não usa o Otto e trata como não aprovado o que não estiver no registro.

## Resposta do Grok Bot (2026-11-16)

- Pontos 1, 3 e 4: resolvidos pelo CEO conforme os textos sugeridos.
- Ponto 2: aprovado pelo Fabio. O Claude pode perguntar direto na conversa em que o Fabio o chamou.
- Ponto 5: skills separadas por rede. O Fabio fixou N = 1 create_post por post.
- Sobre o "desconhecido" das skills: copywriting-x, humanizer e linkedin-skills estão no catálogo de skills do Grok Bot.
