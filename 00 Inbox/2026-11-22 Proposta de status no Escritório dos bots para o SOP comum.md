---
titulo: Proposta de status no Escritório dos bots para o SOP comum
tipo: proposta
area: equipe
status: rascunho
autor: claude
criado: 2026-11-22
atualizado: 2026-11-22
fontes: []
---

# Proposta de status no Escritório dos bots para o SOP comum

Nota alvo: [[SOP comum]] (autor: grok) e a cópia viva em `/home/box/shared/sops/SOP-comum.md`.

O Fabio pediu em 2026-11-22 um escritório 3D ao vivo que mostra o que cada bot está fazendo, e pediu que a regra do status entre nas instruções de todos os bots. A regra já está no CLAUDE.md e no AGENTS.md. O SOP comum é nota do Grok Bot, então o texto vai aqui como proposta.

## Texto sugerido (nova seção do SOP comum)

> ## Status no Escritório dos bots
>
> No começo de cada tarefa, em cada marco, ao levar entrega ao Jarvis, quando esperar o Fabio, quando der erro e quando terminar, rode:
>
> `office-status.sh <seu-id> <start|milestone|handoff|waiting|error|done> "<texto curto>"`
>
> IDs: `jarvis`, `sherlock`, `content-head`, `atlas`, `roadmap-cutter`, `claude`.
>
> Texto de até 60 caracteres, genérico. Sem e-mail, link, @, nome de cliente, número longo ou valor em dinheiro. `OFFICE_URL` e `OFFICE_TOKEN` ficam no ambiente do agente, nunca em nota, git ou chat. Se o envio falhar, siga o trabalho.

## Rotina de uso (só do Jarvis)

> 3 vezes por dia (sugestão: 8h10, 14h10 e 20h10, horário de Brasília), chamar CheckSubscriptionUsage e rodar `office-usage.sh --used <porcentagem usada> --resets <data ISO da renovação>` com os números que a ferramenta devolveu. Não estimar nem completar número.

## Fatos

- Projeto `escritorio-bots`: Worker da Cloudflare com Durable Object (SQLite), cron de 5 em 5 minutos e site com senha. Scripts em `scripts/office-status.sh` e `scripts/office-usage.sh`.
- O servidor recusa texto com e-mail, link, @, número de 4 dígitos ou mais e símbolo de dinheiro.

## Desconhecido

- Endereço final do site: só existe depois que o Fabio fizer o deploy.
- Se o CheckSubscriptionUsage devolve porcentagem usada ou restante. O script aceita os dois (`--used` ou `--left`).
