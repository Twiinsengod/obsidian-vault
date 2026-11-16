---
titulo: Status da nota de dúvidas dos SOPs
tipo: proposta
area: equipe
status: arquivado
autor: claude
criado: 2026-11-16
atualizado: 2026-11-16
fontes: []
---

# Status da nota de dúvidas dos SOPs

## Contexto

Proposta sobre a nota [[2026-11-16 Dúvidas e melhorias nos SOPs]], que fica em `00 Inbox/`. O Fabio pediu esta proposta na conversa de 2026-11-16 com o Claude. Não editei a nota nem o CLAUDE.md.

## Fatos

- A nota está com `status: resolvido` no frontmatter.
- O CLAUDE.md, na seção "Frontmatter", diz: `status`: `rascunho`, `ativo` ou `arquivado`. A palavra `resolvido` não está na lista.
- O CLAUDE.md, na seção "Onde colocar uma nota", diz: nota encerrada vai para `99 Arquivo/`, com `status: arquivado`.
- O README de `99 Arquivo/` pede três coisas ao mover: mudar o `status`, conferir os wikilinks e avisar no Handoff.
- A nota continua em `00 Inbox/`.
- O Handoff cita a nota por wikilink em dois recados.

## Proposta

Há dois caminhos. O Fabio ou o Grok Bot escolhe um.

### Caminho A: seguir a regra atual

Texto sugerido para o frontmatter da nota:

> status: arquivado

E mover o arquivo para `99 Arquivo/`, com o mesmo nome. Depois, conferir os dois wikilinks do Handoff e avisar lá.

### Caminho B: aceitar `resolvido` como status

Texto sugerido para a seção "Frontmatter" do CLAUDE.md e do AGENTS.md, no mesmo commit:

> - `status`: `rascunho`, `ativo`, `resolvido` ou `arquivado`. `resolvido` é para proposta do `00 Inbox/` que já foi respondida e ainda não foi movida para `99 Arquivo/`.

## Hipóteses

- O wikilink `[[2026-11-16 Dúvidas e melhorias nos SOPs]]` continua resolvendo depois da mudança de pasta, porque o Obsidian acha a nota pelo nome. Falta conferir abrindo o vault.
- O caminho A é o mais simples, porque não muda nenhuma regra.

## Desconhecido

- Se o Grok Bot usou `resolvido` de propósito ou por engano.
- Se existe outra nota com `status` fora da lista. Só olhei esta.

## Próximo passo

- Grok Bot: escolher o caminho A ou o B, com o Fabio se precisar, e responder no [[Handoff]].
- Claude: se for o caminho A, faz a troca do status e a mudança de pasta quando o Fabio pedir.

Decisão do Grok Bot em 2026-11-16: caminho A aplicado.
