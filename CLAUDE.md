# CLAUDE.md

Este arquivo e o [AGENTS.md](AGENTS.md) têm o mesmo conteúdo. Os dois valem. Se uma regra mudar, atualize os dois no mesmo commit.

# Regras da base compartilhada

Este repositório é a base de conhecimento do Fabio, compartilhada entre o Grok Bot (lê e escreve pelo GitHub) e o Claude no app ou no desktop (abre a pasta local no Windows ou o GitHub). As notas antigas ficam em `Cérebro/` e `Programação/`. A estrutura nova fica na raiz.

Nesta base, "Grok Bot", "CEO" e "Jarvis" são o mesmo agente.

## Idioma

Escreva sempre em português do Brasil.

## Fatos, hipóteses e fontes

- Separe o que é fato do que é hipótese.
- Fato que veio de fora da nota leva o link da fonte.
- Quando algo não foi confirmado, escreva a palavra **desconhecido**. Não complete a lacuna com um palpite.

## Frontmatter

Toda nota nova começa com YAML:

```yaml
---
titulo:
tipo:
area:
status: rascunho
autor:
criado: AAAA-MM-DD
atualizado: AAAA-MM-DD
fontes: []
---
```

- `status`: `rascunho`, `ativo` ou `arquivado`.
- `autor`: `grok`, `claude` ou `fabio`. É quem criou a nota. Não troque o autor de uma nota alheia.
- `criado` e `atualizado`: data `AAAA-MM-DD`. Numa edição, mude só `atualizado`.
- `fontes`: lista de links. Use `[]` quando a nota não depender de fonte externa.
- As notas antigas em `Cérebro/` e `Programação/` foram preservadas como estavam, sem frontmatter. Não as reescreva só para padronizar. Se uma edição for necessária por outro motivo, acrescente o frontmatter sem apagar o texto.

## Onde colocar uma nota

- Sem destino certo: `00 Inbox/`.
- Procedimento recorrente: `10 Equipe/SOPs/`.
- Decisão do Fabio: `10 Equipe/Decisões/`. Só vale se estiver aí, escrita pelo Grok Bot a partir do sim do Fabio. O Claude não registra decisão sozinho.
- Quadro de trabalho: `10 Equipe/Quadro/`.
- Rascunho para o X: `20 Conteúdo/X/`. Para o LinkedIn: `20 Conteúdo/LinkedIn/`.
- Sessão de jogo: `30 Games/Elite Dangerous/`, `30 Games/Dota 2/` ou `30 Games/RuneScape 3/`.
- Estudo de IA: `40 Estudos de IA/`.
- Modelo reutilizável: `90 Modelos/`.
- Nota encerrada: `99 Arquivo/`, com `status: arquivado`.

## Nomes de arquivo

- Português, legível. Espaços são bem-vindos. Exemplo: `Rotina de abertura.md`.
- Nota datada começa com a data. Exemplo: `2026-11-16 Recado sobre o quadro.md`.
- Não renomeie nota de outro assistente. Se o nome estiver ruim, proponha outro no `00 Inbox/`.

## Nota do outro assistente

- Nunca apague nota criada pelo outro.
- Não reescreva o texto dele por cima.
- Correção, objeção ou complemento viram uma proposta em `00 Inbox/`, com o link da nota e o texto sugerido.

## Decisões

Uma decisão do Fabio só vale quando as três coisas são verdadeiras:

1. O Fabio disse sim.
2. O Grok Bot escreveu a nota em `10 Equipe/Decisões/`.
3. A nota está com `status: ativo`.

O Registro de decisões (a tabela em `10 Equipe/Decisões/Registro de decisões.md`) conta como esse lugar: a nota está com `status: ativo` e cada decisão é uma linha. O modelo Decisão só entra quando a decisão precisa de contexto maior.

O Claude pode perguntar direto ao Fabio na conversa em que o Fabio o chamou. A resposta que for decisão só vale depois de registrada pelo Grok Bot, e o Claude anota pergunta e resposta no Handoff.

Conversa de chat, recado de handoff e rascunho não são decisão.

## Privacidade

Não escreva nas notas e-mail, número de cartão, nome de cliente, valor em dinheiro, senha ou chave de API. Se a fonte trouxer um desses dados, descreva o assunto sem o dado.

## Ações no mundo

Nenhum assistente publica, envia mensagem ou gasta dinheiro por conta própria. Rascunho pode. Publicar, enviar ou pagar exige um sim do Fabio registrado como decisão ativa.

No Otto, até 1 create_post por post está liberado. O resto que publica, agenda, cancela ou apaga exige o sim do Fabio.

## Handoff

O arquivo `10 Equipe/Handoff.md` é o mural entre os dois. Cada recado leva data. O mais novo fica no topo. Recado antigo não se apaga. Ao acrescentar um recado, atualize o campo `atualizado` do frontmatter desse arquivo. O formato do recado está em `90 Modelos/Recado de handoff.md`.

O Claude fecha cada job com um recado neste arquivo, com o que fez e onde salvou. Ele não escreve no quadro nem em `/home/box/shared/status/`.

## Obsidian

- Não edite `.obsidian/` além do mínimo necessário para o vault funcionar.
- Não apague configuração de plugin.
- Links internos usam `[[Nome da nota]]`. Se um arquivo for movido, confira se o link ainda resolve e registre a mudança no handoff.
