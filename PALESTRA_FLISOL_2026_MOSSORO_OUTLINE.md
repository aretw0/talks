# Outline — Engenharia agêntica, open claw e o futuro do software

> Use este documento para discutir ordem e estrutura.
> `[img]` = slide de imagem · `[seção]` = slide divisor de parte

---

## PALESTRA (~45 min · 40 slides)

### Abertura

| # | Slide | Nota |
|---|-------|------|
| 1 | **Título** — Engenharia agêntica, open claw e o futuro do software | |
| 2 | **Quem sou eu** — bio IFRN/IMD/UFERSA/UFPE/SERPRO | |
| 3 | **De Mossoró para o mundo** — UFERSA Vai de Bike, Recife, missão | |

### PARTE 1 · O PASSADO

| # | Slide | Nota |
|---|-------|------|
| 4 | `[seção]` PARTE 1 · O PASSADO | |
| 5 | **A história não se repete…** — "…mas rima que é uma beleza" | gancho filosófico |
| 6 | **O Chile que poderia ter sido** — Cybersyn, golpe militar | |
| 7 | `[img]` cybersin.png | ✅ |
| 8 | **Do Cybersyn à AWS** — quem controla a coordenação digital hoje | |
| 9 | **Turing e a fita** — diagrama prompt→LLM→resposta | |
| 10 | **O teste de Turing virou piada?** — bots, agilidade, controle | |
| 11 | **Sistemas experts não são novos** — ELIZA, generalização do processamento | |
| 12 | `[img]` ELIZA_conversation.png | ✅ |
| 13 | **Da ELIZA até aqui** — mermaid Regras manuais→LLMs | |
| 14 | **O `grep` e a primeira NLP** — Federalist Papers, profiling por vícios | |
| 15 | **Você tem vícios. Use-os a seu favor** — jardim digital | transição para Parte 2 |

### PARTE 2 · O JARDIM DIGITAL

| # | Slide | Nota |
|---|-------|------|
| 16 | `[seção]` PARTE 2 · O JARDIM DIGITAL | |
| 17 | **Plain text is king** — Markdown, LaTeX, org-mode | |
| 18 | **Por que não PDF, Word, Excel?** — mermaid do gargalo | |
| 19 | **Frontmatter + Markdown** — exemplo de nota estruturada | |
| 20 | **Obsidian e o ecossistema** — plataforma, comunidade | |
| 21 | `[img]` obsidian_enterprise.png | ✅ |
| 22 | **aretw0/vault-seed** — template Obsidian+VSCode, "Use this template" | |
| 23 | **Code Literacy** — texto + scripts misturados, org-mode, co-autor | |

### PARTE 3 · O PRESENTE AGÊNTICO

| # | Slide | Nota |
|---|-------|------|
| 24 | `[seção]` PARTE 3 · O PRESENTE AGÊNTICO | |
| 25 | **O racha histórico** — deterministas vs probabilistas → engenharia agêntica | |
| 26 | **O hardware finalmente chegou** — GPUs, pesos, Ghost in the Shell | |
| 27 | **2025: a era do catnip** — tool use em primeiro, MCP, ninguém dormia | |
| 28 | **Tool use: como o agente age** — mermaid agente→tools | |
| 29 | **MCP — quando faz sentido** — servidor, produção, não default | |
| 30 | **O momento Richard Stallman** — impressora, software livre, kernel | |
| 31 | **Três pessoas que chegaram lá** — Pete, Armin, Mario | primeira menção ao Pi |
| 32 | **OpenClaw** — stars, framework, NVIDIA | |
| 33 | `[img]` openclaw.png | ✅ |
| 34 | **O Pi — um kernel minimalista** — extensível, agnóstico, sem MCP por padrão | |
| 35 | `[img]` pi.png | ✅ |
| 36 | **Earendil = GNU · Pi = Linux** — mermaid da analogia | |
| 37 | **O futuro está nos trilhos** — clean code, patterns, arquitetura | |
| 38 | **Psicose agêntica é real** — usuário da plataforma dos outros | |
| 39 | **Resumo da palestra** — mermaid Turing→distro agêntica | fecha o conteúdo |
| 40 | **Por onde começar** — jardim → plain text → Pi → packages → contribuir | call to action |

### Transição

| # | Slide | Nota |
|---|-------|------|
| 41 | `[transição]` INTERVALO · 5 min | |
| 42 | `[seção]` WORKSHOP · O Pi na prática | |

---

## WORKSHOP (~45 min · 15 slides + 1 img)

| # | Slide | Nota |
|---|-------|------|
| 43 | **O que é um agente?** — percebe, decide, age; mermaid | |
| 44 | **O loop agêntico** — pseudocódigo; REPL | |
| 45 | **REPL — a base de tudo** — Read/Eval/Print/Loop | |
| 46 | **O Pi por dentro** — mermaid CLI→Loop→LLM→tools (graph LR) | |
| 47 | **Por que o Pi?** — minimalista, extensível, agnóstico, seu | |
| 48 | **Demo ao vivo** | ❌ preencher com screenshots antes da apresentação |
| 49 | **Anatomia de uma tool no Pi** — JS com TypeBox | |
| 50 | **Rodando o agente** — JS com agentLoop async iterator | |
| 51 | **pi.dev/packages — o ecossistema** — texto + install command | |
| 52 | `[img]` pi-packages.png | ✅ |
| 53 | **Mãos na massa** — install + /login + link para workshop | |
| 54 | **Exercício guiado** — link para WORKSHOP_FLISOL_2026.md | |
| 55 | **O que fazer amanhã** — Obsidian, vault-seed, Pi, packages | |
| 56 | **A saúde mental importa** — extensão do Armin, consciência | |
| 57 | **Obrigado** — github.com/aretw0 · github.com/aretw0/talks | |

---

## Assets

| Asset | Slide | Status |
|-------|-------|--------|
| `cybersin.png` | 7 | ✅ |
| `ELIZA_conversation.png` | 12 | ✅ |
| `obsidian_enterprise.png` | 21 | ✅ |
| `openclaw.png` | 33 | ✅ |
| `pi.png` | 35 | ✅ |
| `pi-packages.png` | 52 | ✅ |
| screenshots demo ao vivo | 48 | ❌ fazer durante ensaio |

---

## Arquivos do projeto

| Arquivo | Descrição |
|---------|-----------|
| `PALESTRA_FLISOL_2026_MOSSORO.md` | Rascunho original com as ideias brutas |
| `PALESTRA_FLISOL_2026_MOSSORO_SLIDES.md` | Slides em formato Obsidian Reveal.js |
| `PALESTRA_FLISOL_2026_MOSSORO_ROTEIRO.md` | Roteiro slide a slide para segunda tela |
| `PALESTRA_FLISOL_2026_MOSSORO_OUTLINE.md` | Este arquivo — visão geral e status |
| `WORKSHOP_FLISOL_2026.md` | Guia completo do workshop para os participantes |
