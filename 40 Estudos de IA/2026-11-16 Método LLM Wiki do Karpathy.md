---
titulo: Método LLM Wiki do Karpathy
tipo: estudo
area: estudos-de-ia
status: ativo
autor: claude
criado: 2026-11-16
atualizado: 2026-11-16
fontes:
  - https://x.com/karpathy/status/2039805659525644595
  - https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f
  - https://www.youtube.com/watch?v=UbK5ckxzX98
---

# Estudo — Método LLM Wiki do Karpathy

## Pergunta

O que o método LLM Wiki do Karpathy propõe, e o que dele vale aplicar neste vault?

## Fatos

- O Karpathy publicou um post no X sobre usar IA para montar bases de conhecimento pessoais. Depois publicou um "idea file" no GitHub Gist com o padrão completo. ([gist](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f))
- A ideia central: em vez de a IA reler os documentos brutos a cada pergunta, como faz o RAG, ela monta aos poucos uma wiki em Markdown, com páginas ligadas entre si, e mantém essa wiki em dia. ([gist](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f))
- São três camadas. Fontes brutas, que a IA lê mas não edita. A wiki, que a IA escreve e mantém. E o esquema (CLAUDE.md ou AGENTS.md), com as regras, que a pessoa e a IA ajustam com o tempo. ([gist](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f))
- São três operações. Ingerir: ler a fonte, escrever o resumo, atualizar índice e páginas ligadas, registrar no log. Uma fonte pode mexer em 10 a 15 páginas. Perguntar: ler a wiki e responder com citação; resposta boa volta para a wiki. Revisar: procurar contradição, dado velho, página órfã e lacuna. ([gist](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f))
- Há dois arquivos fixos. O `index.md` é o catálogo das páginas, com link e resumo de uma linha, e a IA lê ele primeiro. O `log.md` é o histórico em ordem de data, só de acréscimo, com um prefixo fixo por linha. ([gist](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f))
- Ferramentas citadas no gist: Obsidian Web Clipper, imagens baixadas para a pasta local, a visão de grafo do Obsidian, Marp para slides, Dataview para consultar o frontmatter e Git para guardar o histórico. ([gist](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f))
- O vídeo do Anwar Hermuche (abril de 2026, 38 min) monta o método com Claude Code e Obsidian. Ele mostra duas ingestões, um artigo pelo Web Clipper e um vídeo do YouTube, e compara o método com o RAG. Li só a página e os capítulos do vídeo, não a transcrição. ([vídeo](https://www.youtube.com/watch?v=UbK5ckxzX98))

## Como ficou neste vault

| Peça do método | Onde ficou |
| --- | --- |
| Fontes brutas | `01 Fontes/`. Os três clips antigos da pasta `Clippings` foram copiados para cá. |
| Wiki | `50 Wiki/`, com `Resumos/`, `Conceitos/`, `Entidades/` e `Respostas/` |
| index.md | [[Índice da wiki]] |
| log.md | [[Log da wiki]] |
| Esquema | Seção "Wiki" do CLAUDE.md e do AGENTS.md |
| Passo a passo | [[SOP da wiki]] |
| Dataview | Não está instalado. Usei o Bases, que já vem no Obsidian: `50 Wiki/Páginas da wiki.base` |
| Marp | O plugin Marp Slides já estava instalado. Resposta em slides vai para `50 Wiki/Respostas/`. |

## Hipóteses

- Como o vault tem dois assistentes, a wiki fica numa pasta própria, e lá os dois podem editar a página do outro. Fora da `50 Wiki/`, a regra antiga continua.
- Com poucas dezenas de páginas, o índice basta e não precisa de busca por embeddings. O gist diz o mesmo para escala moderada.

## Desconhecido

- O texto completo do post no X. O site bloqueou a leitura, e usei o gist e páginas que o citam.
- Os detalhes de cada capítulo do vídeo.
- Se o Grok Bot consegue ler `01 Fontes/` grandes, como o guia de dinheiro de 714 KB, sem cortar o texto.

## Fontes

- [Post do Karpathy no X](https://x.com/karpathy/status/2039805659525644595)
- [Gist "LLM Wiki" do Karpathy](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f)
- [Vídeo do Anwar Hermuche](https://www.youtube.com/watch?v=UbK5ckxzX98)

## Conclusão provisória

O vault já tinha boa parte do método: regras num CLAUDE.md, modelos, frontmatter e Git. Faltavam a camada de fontes brutas, a wiki separada, o índice, o log e as três operações escritas como SOP. Isso foi feito em 16/11/2026.
