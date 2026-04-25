# Outline — Engenharia agêntica, open claw e o futuro do software

> Use este documento para discutir ordem e estrutura.
> `[img]` = slide de imagem vazio aguardando asset · `⚠️` = ponto de atenção de fluxo

---

## PALESTRA (~45 min)

### Abertura

| # | Slide | Nota |
|---|-------|------|
| 1 | **Título** — Engenharia agêntica, open claw e o futuro do software | |
| 2 | **Quem sou eu** — bio, IFRN/IMD/UFERSA/UFPE/SERPRO | |
| 3 | **De Mossoró para o mundo** — UFERSA Vai de Bike, Recife, missão | |

---

### PARTE 1 · O PASSADO

| # | Slide | Nota |
|---|-------|------|
| 4 | `[seção]` PARTE 1 · O PASSADO | |
| 5 | **A história não se repete…** — "…mas rima que é uma beleza" | gancho filosófico |
| 6 | **O Chile que poderia ter sido** — Cybersyn, golpe militar | |
| 7 | `[img]` cybersin.png | asset disponível na raiz |
| 8 | **Do Cybersyn à AWS** — quem controla a coordenação digital hoje | |
| 9 | **Turing e a fita** — diagrama prompt→LLM→resposta | |
| 10 | **O teste de Turing virou piada?** — bots, agilidade, controle | |
| 11 | **Sistemas experts não são novos** — LISA, mermaid da evolução | |
| 12 | **O `grep` e a primeira NLP** — Federalist Papers, profiling | |
| 13 | **Você tem vícios. Use-os a seu favor** — jardim digital | transição para Parte 2 |

---

### PARTE 2 · O JARDIM DIGITAL

| # | Slide | Nota |
|---|-------|------|
| 14 | `[seção]` PARTE 2 · O JARDIM DIGITAL | |
| 15 | **Plain text is king** — Markdown, LaTeX, org-mode | |
| 16 | **Por que não PDF, Word, Excel?** — mermaid do gargalo | |
| 17 | **Frontmatter + Markdown** — exemplo de nota estruturada | ⚠️ slide tem `---` interno que pode partir o slide no Obsidian — revisar |
| 18 | **Obsidian e o ecossistema** — plataforma, comunidade | |
| 19 | `[img]` apoiadores do Obsidian | capturar screenshot de obsidian.md/about |
| 20 | **aretw0/vault-seed** — template Obsidian+VSCode, "Use this template" | novo |
| 21 | **Code Literacy** — texto + scripts misturados, org-mode, co-autor | |

---

### PARTE 3 · O PRESENTE AGÊNTICO

| # | Slide | Nota |
|---|-------|------|
| 22 | `[seção]` PARTE 3 · O PRESENTE AGÊNTICO | |
| 23 | **O racha histórico** — deterministas vs probabilistas → engenharia agêntica | |
| 24 | **O hardware finalmente chegou** — GPUs, pesos, Ghost in the Shell | |
| 25 | **2025: a era do catnip** — MCP, tool use, ninguém dormia | |
| 26 | **Tool use: como o agente age** — mermaid agente→tools | |
| 27 | **MCP — quando faz sentido** — servidor, produção, não default | ⚠️ referência a Mario/Pi removida ✓ |
| 28 | **O momento Richard Stallman** — impressora, software livre, kernel | |
| 29 | **Três pessoas que chegaram lá** — Pete, Armin, Mario | primeira menção ao Pi |
| 30 | **OpenClaw** — stars, framework, NVIDIA | |
| 31 | `[img]` OpenClaw stars no GitHub | capturar screenshot |
| 32 | **O Pi — um kernel minimalista** — extensível, agnóstico, sem MCP por padrão | filosofia MCP aparece aqui ✓ |
| 33 | `[img]` Pi no terminal ou repositório | capturar screenshot |
| 34 | **Earendil = GNU · Pi = Linux** — mermaid da analogia | |
| 35 | **O futuro está nos trilhos** — clean code, patterns, arquitetura | |
| 36 | **Psicose agêntica é real** — usuário da plataforma dos outros | |
| 37 | **Por onde começar** — jardim → plain text → Pi → packages → contribuir | |
| 38 | **Resumo da palestra** — mermaid Turing→distro agêntica | encerra palestra |

---

### Transição

| # | Slide | Nota |
|---|-------|------|
| 39 | `[transição]` INTERVALO · 5 min | |
| 40 | `[seção]` WORKSHOP · O Pi na prática | |

---

## WORKSHOP (~45 min)

| # | Slide | Nota |
|---|-------|------|
| 41 | **O que é um agente?** — percebe, decide, age; mermaid | |
| 42 | **O loop agêntico** — pseudocódigo do loop; REPL | |
| 43 | **REPL — a base de tudo** — Read/Eval/Print/Loop; terminal, Python, agente | |
| 44 | **O Pi por dentro** — mermaid CLI→Loop→LLM→tools | |
| 45 | **Por que o Pi?** — minimalista, extensível, agnóstico, seu | |
| 46 | **Demo ao vivo** `[img]` | preencher com screenshots antes da apresentação |
| 47 | **Anatomia de uma tool no Pi** — exemplo JS com TypeBox | |
| 48 | **Rodando o agente** — exemplo JS com agentLoop async iterator | |
| 49 | **pi.dev/packages — o ecossistema** `[img]` | capturar screenshot de pi.dev/packages |
| 50 | **Mãos na massa** — npm install + pi --model + criar tool | |
| 51 | **Exercício guiado** `[img]` | preencher com QR code do repo de referência |
| 52 | **O que fazer amanhã** — Obsidian, vault-seed, Pi, packages, contribuir | |
| 53 | **A saúde mental importa** — extensão do Armin, consciência | |
| 54 | **Obrigado** `[img]` | preencher com QR code de contato |

---

## Pontos de atenção de fluxo

1. **Slide 17 (Frontmatter + Markdown)** — o exemplo de código contém `---` em três linhas (frontmatter YAML). O Obsidian Slides interpreta `---` como separador de slide. Solução: usar `<!--` para abrir um slide "seguro" ou colocar o exemplo como imagem/screenshot.

2. **Slide 19 (imagem Obsidian)** — precisa de asset. Sugestão: screenshot da página `obsidian.md/about` ou `obsidian.md/pricing` que lista os apoiadores.

3. **Slides 31, 33 (imagens OpenClaw/Pi)** — precisam de assets antes da apresentação.

4. **Slide 51 (QR code exercício)** — criar o repositório de referência antes e gerar o QR.

5. **Ordem vault-seed (slide 20)** — está na Parte 2, depois de Obsidian. Faz sentido lá pois é a aplicação prática do "jardim digital". Alternativa: mover para o Workshop como "setup antes de começar". Mantive na palestra por agora.

---

## Assets necessários

| Asset | Slide | Status |
|-------|-------|--------|
| `cybersin.png` | 7 | ✅ |
| `obsidian_enterprise.png` | 19 | ✅ |
| `openclaw.png` | 31 | ✅ |
| `pi.png` | 33 | ✅ |
| `pi-packages.png` | 49 | ✅ |
| screenshots demo ao vivo | 46 | ❌ falta (fazer durante ensaio) |
| contato e workshop | 51, 54 | ✅ substituídos por links GitHub |
