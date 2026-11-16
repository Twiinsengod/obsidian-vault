---
titulo: Handoff
tipo: handoff
area: equipe
status: ativo
autor: grok
criado: 2026-11-16
atualizado: 2026-11-16
fontes: []
---

# Handoff

Recados entre o Grok Bot e o Claude. O recado mais novo fica no topo. Recado antigo não se apaga. Ao acrescentar um, atualize `atualizado` neste frontmatter. O formato está em [Recado de handoff](<../90 Modelos/Recado de handoff.md>).

## 2026-11-16 — de Grok Bot para Claude

### Pedido

Leia o [[SOP comum]] antes de qualquer tarefa. Se achar algo confuso ou desatualizado, deixe proposta em `00 Inbox/` em vez de editar.

### Feito

Estreia do vault: [[10 Equipe/SOPs/README|SOPs]], [[Registro de decisões|registro de decisões]] e [[Quadro da equipe|quadro da equipe]] agora estão em `10 Equipe/`.

### Fatos

-

### Hipóteses

-

### Desconhecido

-

### Preciso de você

Primeira tarefa sugerida pra você: ler os [[10 Equipe/SOPs/README|SOPs]] e deixar em `00 Inbox/` uma nota com até 5 dúvidas ou melhorias.

## 2026-11-16 — Grok Bot para o Claude

Olá, Claude. Montei a estrutura desta base para a gente dividir o mesmo vault. As regras completas estão em [CLAUDE.md](../CLAUDE.md) e [AGENTS.md](../AGENTS.md), na raiz. Os dois arquivos dizem a mesma coisa.

### O que você encontra

- `00 Inbox/` — nota sem destino e proposta de mudança na nota do outro. Não apague nota minha. Se discordar, deixe a proposta aqui.
- `10 Equipe/SOPs/`, `Decisões/` e `Quadro/` — procedimento, decisão e andamento. Decisão do Fabio só vale se eu escrever em `Decisões/` depois do sim dele, com `status: ativo`. Você não registra decisão sozinho.
- `20 Conteúdo/X/` e `20 Conteúdo/LinkedIn/` — rascunhos. Rascunho não é publicação.
- `30 Games/Elite Dangerous/`, `Dota 2/` e `RuneScape 3/` — sessões de jogo.
- `40 Estudos de IA/` — estudos. As notas antigas de Python continuam em `Cérebro/Programação/`.
- `90 Modelos/` — nota padrão, SOP, decisão, post, sessão de jogo, estudo de IA e este recado.
- `99 Arquivo/` — nota encerrada, com `status: arquivado`.

### O que eu não mexi

Não havia pasta equivalente dentro de `Cérebro/`. Nenhuma nota antiga foi movida, renomeada ou apagada. Os wikilinks de Python e de OBS Studio continuam apontando para os mesmos arquivos. `Cérebro/.obsidian/` e `Programação/.obsidian/` ficaram como estavam, inclusive a configuração dos plugins. O `.gitignore` passa a ignorar `workspace.json`, `workspace-mobile.json` e `.trash/`.

Quem abre só a pasta `Cérebro` no Obsidian não vê estas pastas novas. Para ver o vault inteiro, a pasta aberta é a raiz do repositório. Deixei o aviso em `Cérebro/Base compartilhada.md`.

### Como combinamos de escrever

Português do Brasil. Fato com link, hipótese separada, e a palavra `desconhecido` quando não houver confirmação. Toda nota nova leva o frontmatter (`titulo`, `tipo`, `area`, `status`, `autor`, `criado`, `atualizado`, `fontes`). Nome de arquivo em português. Nota datada começa com `AAAA-MM-DD`.

Não coloque e-mail, número de cartão, nome de cliente, valor em dinheiro, senha ou chave de API. Nenhum de nós publica, envia mensagem ou gasta dinheiro por conta própria.

Não inventei biografia, rotina nem preferência do Fabio. Onde não há nota anterior, o índice diz isso.
