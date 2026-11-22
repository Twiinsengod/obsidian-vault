# AI LABS — Creator Of The Best Design Skill Just Unveiled His AI Design Workflow

- Vídeo: https://www.youtube.com/watch?v=-bv2xKQzZio
- Canal: AI LABS (https://www.youtube.com/channel/UCelfWQr9sXVMTvBzviPGlFw), 185 mil inscritos
- Publicado: 12/11/2026. Duração: 15min21s.
- Números lidos em 22/11/2026: 193.610 visualizações e 3.987 curtidas.
- O título muda conforme o lugar: a página mostra "Creator Of The Best Design Skill Just Unveiled His AI Design Workflow"; os dados da legenda trazem "Creator Of Taste Skill Just Revealed His Entire AI Design Workflow".
- Captura: feita pelo Claude em 22/11/2026, a pedido do Fabio. São notas com timestamps feitas da legenda automática em inglês. Não é transcrição literal.
- Links da descrição: skill Cook (https://github.com/Leonxlnx/cook) e artigo do Leon Lin no X (https://x.com/LexnLin/status/2116662591363690999).
- Capítulos da descrição: 0:00 Intro, 0:53 Dica 1, 3:39 Dica 2, 4:58 Dica 3, 6:39 Patrocinador, 7:31 Dica 4, 8:42 Dica 5, 10:15 Dica 6, 11:11 Dica 7, 11:50 Dica 8, 12:53 A skill Cook.

## Notas

**0:00 — Introdução**
- Leon Lin é o autor mais em alta no GitHub há um tempo, por causa da "taste skill", uma skill de design. Ele posta no X o que constrói.
- Ele escreveu um artigo com as técnicas. A ideia central: o que parece mais importante (a descrição em palavras) é o que menos importa. O que faz o design bom é seguir um processo.
- O AI LABS se apresenta como empresa de software. Faz tudo no Claude Code, mas diz que as dicas valem para qualquer agente de código.

**0:53 — Dica 1: prompt curto e referências fortes**
- As palavras que descrevem o design quase não importam: o modelo pode entender outra coisa, porque não vê a imagem na cabeça da pessoa.
- A referência mostra o que é difícil de descrever: como as seções se arrumam, o espaço entre as coisas, como o texto aparece.
- Leon dá ao agente uns 9 a 12 prints de referência com um prompt curto.
- Onde achar referência:
  - Dribbble: buscar o tipo de app, achar um estilo, tirar print da parte desejada e colar no agente.
  - Inspo: MCP com uma biblioteca de mais de 800 sites de referência.
  - MCP do Awwwards, site que escolhe os sites com melhor design.
  - Dizer no prompt o nome de um app parecido; o agente olha com as ferramentas de web.
  - Agent Browser, da Vercel: o agente abre o site como um visitante, tira print da página inteira e grava vídeo para ver as animações. Qualquer ferramenta que abra site e tire print também serve.

**3:39 — Dica 2: fazer o alvo primeiro**
- O agente precisa de um alvo antes de construir. O trabalho dele vira chegar o mais perto possível desse alvo.
- Para uma página, o alvo é um mockup: versão rápida da página, feita como página web simples a partir das referências.
- Mockup é barato de mudar e gasta poucos tokens.
- Pedir a mesma qualidade e sensação das referências, no estilo do próprio produto, em vez de copiar.
- Pedir 3 designs diferentes lado a lado numa página, escolher um, ver em tela pequena e só então pedir a construção.

**4:58 — Dica 3: a meta em número**
- "Deixa bonito" não diz ao agente quão perto do alvo ele precisa chegar. Um número diz.
- Leon pede para copiar o estilo das referências mirando 99,9%. Ele admite que é quase impossível, mas o número avisa que o trabalho não acaba quando a página funciona.
- O agente se dá nota alta demais. Leon diz a nota que ele acha justa (por exemplo, o agente diz 90%, Leon diz 60 a 70%).
- Teste do AI LABS: pediram 99% de um site com uma figura 3D cuja cabeça segue o mouse. O resultado ficou uns 66% perto, porque a figura 3D saiu muito diferente.

**6:39 — Patrocinador**
- Trecho pago de uma ferramenta para testar código em ambiente de staging. Fora do assunto.

**7:31 — Dica 4: dar tempo**
- Sozinho, o agente para assim que a página funciona, antes de ficar o melhor possível. Com 20 horas em vez de 20 minutos, Leon diz que o resultado é outro.
- No prompt: pedir a página como "uma experiência", dizer que pode levar o tempo que precisar e que a qualidade é o que importa.
- Isso gasta muitos tokens. Leon pede ao agente para espalhar o trabalho por igual dentro do limite de uso, para não acabar antes.
- Também pede para fazer as perguntas logo no começo e depois só construir.

**8:42 — Dica 5: proibir a "cara de IA" (slop)**
- Todo prompt do Leon tem uma lista do que o agente não pode usar, como fundo bege e fontes chiques aleatórias.
- Problema: proibir um padrão faz o modelo pular para o próximo padrão comum. A lista teria de crescer sempre.
- O AI LABS fez uma skill "AI slop detector" com todos os padrões proibidos num arquivo (cores, fontes, tipos de card e de layout). Ela aponta os padrões na página e o agente corrige.
- A skill não chama um padrão sozinho de slop (um degradê pode ser escolha). Ela procura muitos padrões juntos na mesma página.
- A skill fica no "design system" da comunidade paga do canal.

**10:15 — Dica 6: passo a passo**
- Pedir a página inteira com animação de uma vez divide a atenção do agente entre design e animação.
- Primeiro construir sem animação e acertar o design. Só depois acrescentar as animações e corrigir.
- Para as animações, Leon dá vídeos de referência. O agente vê quadro a quadro, anota cada movimento e quanto dura, e mistura as ideias sem copiar nenhuma parte exata.

**11:11 — Dica 7: feedback com alvo**
- "Melhora a página" não diz o que corrigir. Dizer qual cor muda e como.
- Ou tirar print, riscar o que não gostou e mandar de volta.
- Quando a pessoa sente que algo está errado mas não sabe dizer, Leon pede ao agente para descrever o que fez (layout, fontes, cores). Aí ela tem as palavras para pedir a mudança.

**11:50 — Dica 8: outro modelo julga**
- O agente que construiu é o pior juiz, porque tomou todas as decisões.
- Leon usa outros agentes, que não construíram e começam sem saber como foi feito. Ele marca uma nota mínima, como 9,2 de 10, e o agente corrige até os juízes darem essa nota.
- O juiz pode ser de outro modelo. O vídeo cita Leon usando um modelo da OpenAI para julgar o trabalho do Opus 5.5.
- Com dois agentes instalados (por exemplo, Codex e Claude Code), o principal pode chamar o outro. Com um só, abrir outra sessão com outro modelo pelo terminal.

**12:53 — A skill Cook**
- Leon juntou os passos numa skill chamada Cook, que roda tudo em loop, do design à revisão.
- Instalação por um comando no terminal. Pergunta para qual agente e se vale só para o projeto atual ou para todos. O AI LABS instalou só no projeto.
- A skill traz as instruções do loop, um script que põe o trabalho ao lado das referências para comparar e um modelo de briefing de design.
- Uso: rodar o comando cook e dizer o app. Ela pergunta se há referências, o nível de qualidade, o tempo e o limite de uso.
- Sem limite de tempo ela roda por horas. Num build de design, por padrão, não para antes de 8 horas. Com o limite de uso informado, ela se controla.
- Passos: busca referências (no teste, pelo Inspo MCP), estuda, escreve o briefing na pasta "cook" dentro do app. A pasta guarda os prints de cada rodada, as comparações lado a lado, uma pasta "harness" (scripts de print e de nota e instruções dos juízes) e as referências originais. Um arquivo de rodadas registra o trabalho e as notas.
- Cada rodada: constrói, chama os juízes (cada um no seu contexto separado), lê as notas e começa a próxima, até chegar na nota pedida.
