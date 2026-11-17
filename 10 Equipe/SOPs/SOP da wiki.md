---
titulo: SOP da wiki
tipo: sop
area: equipe
status: ativo
autor: claude
criado: 2026-11-16
atualizado: 2026-11-16
fontes:
  - https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f
---

# SOP — Wiki (ingerir, perguntar, revisar)

Passo a passo do método LLM Wiki neste vault. As regras estão na seção "Wiki" do CLAUDE.md e do AGENTS.md. O estudo está em [[2026-11-16 Método LLM Wiki do Karpathy]].

## Quando usar

- O Fabio salvou algo em `01 Fontes/` e pediu para ingerir.
- O Fabio fez uma pergunta que a wiki pode responder.
- O Fabio pediu uma revisão da wiki. Faça uma revisão também a cada 10 ingestões, mais ou menos.

## Antes de começar

- Leia o [[Índice da wiki]] e as últimas linhas do [[Log da wiki]].
- Fonte bruta não se edita, não se renomeia e não se apaga.

## Ingerir uma fonte

1. Leia a fonte inteira em `01 Fontes/`. Se ela for grande demais, leia por partes e diga no resumo qual parte ficou de fora.
2. Se o Fabio estiver na conversa, diga em poucas linhas o que achou de importante. Pergunte o que ele quer destacar.
3. Crie o resumo em `50 Wiki/Resumos/` com o modelo [Página de resumo](<../../90 Modelos/Página de resumo.md>). Ligue a fonte bruta com `[[nome do arquivo]]` e ponha o link original em `fontes`.
4. Para cada conceito ou entidade importante, abra a página em `50 Wiki/Conceitos/` ou `50 Wiki/Entidades/`. Se não existir, crie com o modelo [Página da wiki](<../../90 Modelos/Página da wiki.md>). Acrescente o que a fonte diz, com link para o resumo.
5. Se a fonte contradiz uma página, escreva a contradição na seção "Contradições" da página, com as duas fontes.
6. Ligue as notas do vault que têm relação, como uma spec em `30 Games/`. Não edite nota de fora da `50 Wiki/` que seja do outro assistente. Ponha o link só na página da wiki.
7. Atualize o [[Índice da wiki]]: uma linha por página nova, com link e resumo de uma linha.
8. Acrescente no topo do [[Log da wiki]] a linha `## AAAA-MM-DD ingestão | Nome da fonte`, com as páginas criadas e as alteradas.

## Perguntar

1. Leia o [[Índice da wiki]] e escolha as páginas.
2. Leia as páginas. Se faltar algo, volte à fonte bruta.
3. Responda citando as páginas com `[[ ]]`. O que a wiki não cobre é **desconhecido**.
4. Se a resposta valer guardar (comparação, tabela, análise), salve em `50 Wiki/Respostas/`, ponha no índice e registre `## AAAA-MM-DD pergunta | Assunto` no log.
5. Slides: escreva em Markdown do Marp (`marp: true` no frontmatter) e salve em `50 Wiki/Respostas/`. O plugin Marp Slides mostra e exporta.

## Revisar

Procure e anote:

- Contradição entre páginas.
- Dado que uma fonte mais nova superou. Preço e lucro por hora de jogo envelhecem rápido.
- Página órfã, sem nenhum link chegando. A visão de grafo do Obsidian ajuda.
- Conceito citado em várias páginas que ainda não tem página própria.
- Afirmação sem fonte.
- Página que não está no índice.

Corrija o que for simples. O resto vira lista em `## AAAA-MM-DD revisão` no log, com sugestão de fonte para buscar.

## Se algo der errado

- A fonte está incompleta ou cortada: diga isso no resumo e no log. Não complete com palpite.
- A pergunta é pessoal ou pede decisão do Fabio: a wiki não decide. Siga o [[SOP comum]].

## Resultado esperado

Cada fonte tem resumo. Cada página aparece no índice. Toda operação deixa uma linha no log. O Claude fecha o job com recado no [[Handoff]].
