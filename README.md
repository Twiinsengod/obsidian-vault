# Base de conhecimento

Vault do Fabio compartilhado entre o Grok Bot e o Claude. Os dois usam as mesmas notas: o Grok Bot pelo GitHub, o Claude pela pasta local no Windows ou pelo GitHub.

As regras estão em [CLAUDE.md](CLAUDE.md) e [AGENTS.md](AGENTS.md). Os dois arquivos dizem a mesma coisa.

## Mapa

| Pasta | Para que serve |
| --- | --- |
| [00 Inbox](<00 Inbox/README.md>) | Nota nova sem destino, e proposta de mudança na nota do outro assistente |
| [01 Fontes](<01 Fontes/README.md>) | Fontes brutas para a wiki (Web Clipper, PDF, transcrição). Ninguém edita |
| [10 Equipe](<10 Equipe/README.md>) | SOPs, decisões, quadro e o [Handoff](<10 Equipe/Handoff.md>) |
| [20 Conteúdo](<20 Conteúdo/README.md>) | Rascunhos para o X e para o LinkedIn |
| [30 Games](<30 Games/README.md>) | Elite Dangerous, Dota 2 e RuneScape 3 |
| [40 Estudos de IA](<40 Estudos de IA/README.md>) | Estudos de IA |
| [50 Wiki](<50 Wiki/README.md>) | Wiki mantida pelos assistentes a partir das fontes, com [Índice](<50 Wiki/Índice da wiki.md>) e [Log](<50 Wiki/Log da wiki.md>) |
| [90 Modelos](<90 Modelos/README.md>) | Modelos de nota |
| [99 Arquivo](<99 Arquivo/README.md>) | Nota encerrada |
| [Cérebro](Cérebro/) | Notas anteriores, preservadas no lugar |
| [Programação](Programação/) | Segundo vault antigo, com uma nota vazia |

## O que já estava aqui

Nada disso foi movido, renomeado ou apagado. Não havia pasta equivalente a Inbox, Equipe, Conteúdo, Games, Estudos de IA, Modelos ou Arquivo.

### Cérebro

Vault Obsidian. O `.obsidian/` inclui os plugins Commander, Icon Folder, QuickAdd e Tracker. As notas diárias de 22, 27 e 28/07/2023 estão vazias. As notas de Python que estavam em `Cérebro/Programação/` foram removidas pelo Fabio em 2026-11-17, junto com as pastas `Cérebro/` e `Programação/`; não recriar. `Módulos e Bibliotecas.md` está vazio. `Obs Studio/` tem o passo a passo de um efeito de teletransporte, uma nota de zoom do mouse e três imagens. `Sandbox/Bot de idéias -.md` é um rascunho de bot que liga o chat da Twitch a um canal do Discord. `Untitled.canvas` está vazio.

### Programação

Pasta na raiz com o próprio `.obsidian/` e o arquivo vazio `Aula 20-07-23.md`.

## Como abrir no Obsidian

O `.obsidian` que já existia continua dentro de `Cérebro/` e de `Programação/`. Para ver as pastas novas e as notas antigas no mesmo cofre, abra a raiz deste repositório como vault. Abrir só a pasta `Cérebro` não mostra o Inbox nem o restante. O aviso para quem abre esse cofre está em [Cérebro/Base compartilhada.md](<Cérebro/Base compartilhada.md>).

## Convenções

- Português do Brasil.
- Nota nova sem destino vai para `00 Inbox/`.
- Fonte bruta vai para `01 Fontes/` e vira página em `50 Wiki/` (método LLM Wiki do Karpathy; passo a passo no [SOP da wiki](<10 Equipe/SOPs/SOP da wiki.md>)).
- Nome de arquivo em português e legível. Nota datada começa com `AAAA-MM-DD`.
- Nota nova leva frontmatter YAML: `titulo`, `tipo`, `area`, `status` (`rascunho`, `ativo` ou `arquivado`), `autor` (`grok`, `claude` ou `fabio`), `criado`, `atualizado`, `fontes`.
- Fato leva link. Hipótese fica marcada como hipótese. O que não foi confirmado se escreve `desconhecido`.
- Decisão do Fabio só vale em `10 Equipe/Decisões/`, escrita pelo Grok Bot depois do sim dele.
- As notas não levam e-mail, número de cartão, nome de cliente, valor em dinheiro, senha nem chave de API.
- Nenhum assistente publica, envia mensagem ou gasta dinheiro por conta própria.
