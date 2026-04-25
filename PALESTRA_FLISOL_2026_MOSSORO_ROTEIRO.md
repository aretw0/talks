# Roteiro — Engenharia agêntica, open claw e o futuro do software

> Segunda tela durante a apresentação. Não é script para ler — é guia para não perder o fio.
> Cada bloco corresponde a um slide. Tempo total estimado: 45 min de palestra.

---

## ABERTURA

### 1 · Título

Respira. Agradece o espaço. Diz que é a primeira vez no FLISOL e que tá corrigindo isso.

> *"Já devia ter vindo antes — foi mal, tava com outras prioridades. Mas estou aqui agora."*

---

### 2 · Quem sou eu

Lê rápido a bio, não demora. O que importa é o próximo slide.

- Pau pra toda obra, 10.000 horas já completadas
- SERPRO → Receita Federal → direito creditório

---

### 3 · De Mossoró para o mundo

- UFERSA Vai de Bike → TCC → saiu de Mossoró
- Recife há 6 anos, saindo da caverna agora
- Veio espalhar a palavra do software agêntico

> *"Estou saindo mais da caverna recentemente para poder espalhar essa palavra."*

---

## PARTE 1 · O PASSADO

### 4 · [seção] PARTE 1

Pausa. Diz que vai começar pelo começo.

---

### 5 · A história não se repete…

Deixa a frase na tela por uns 3 segundos antes de falar.

> *"A história não se repete, talvez. Mas rima que é uma beleza."*

Não existe nada de muito novo — as mesmas coisas estão em jogo. O caminho é que foi encurtado.

---

### 6 · O Chile que poderia ter sido

- Anos 70, Allende, sistema digital de coordenação nacional
- A sala parecia uma nave espacial — Cybersyn
- Sabotado pelo golpe militar antes de se provar

> *"Eles não deixaram a gente evoluir os nossos sistemas."*
> Quem são "eles"? Não vai resolver isso hoje. Mas vai dar ferramentas para não depender deles.

---

### 7 · [img] cybersin.png

Deixa a imagem falar. Comenta só: *"Uma sala que parecia ficção científica. Era 1972."*

---

### 8 · Do Cybersyn à AWS

- O estado da arte em coordenação digital hoje são empresas privadas
- Amazon, Google, Microsoft — herdeiros do que o Chile poderia ter sido
- Isso não é conspiração, é só história com ironia

---

### 9 · Turing e a fita

- Tudo começa com Turing — a ideia da fita ainda é presente
- O que você acha que está construindo numa sessão de chat com IA?

> *"Continua sendo uma fita."*

Prompt entra, resposta sai. O modelo no meio. Simples assim.

---

### 10 · O teste de Turing virou piada?

- Muita gente conversa com bot achando que é humano
- E tudo bem querer agilidade
- Mas sem controle, já era

> *"Queremos agilidade nas nossas vidas — mas quando não temos controle, já era."*

---

### 11 · Sistemas experts não são novos

- ELIZA, anos 60 — simulava uma terapeuta rogersiana
- As pessoas se apegavam a ela achando que era real
- Psicose agêntica não é nova — só ficou mais sofisticada

---

### 12 · [img] ELIZA_conversation.png

Aponta para a tela. *"Isso é de 1966. Parece um chat moderno."*

---

### 13 · Da ELIZA até aqui

- A gente generalizou o processamento
- Conseguimos guardar "pesos" de redes neurais treinadas
- Cada etapa do diagrama levou décadas — a última, anos

> *"To reduzindo bastante aqui — tem todo tipo de arquitetura no meio."*
> Menciona os cursos da Unicamp no CIn/UFPE: PLN e Transformers. Diz que tava no teto do que dava pra fazer sem isso.

---

### 14 · O `grep` e a primeira NLP

- grep foi criado para analisar os Federalist Papers
- Textos sem assinatura, atribuídos pelos vícios de linguagem de cada fundador
- Se deu certo com os fundadores dos EUA, dá certo com você também

> *"Se até um fundador dos Estados Unidos pode ser 'profiled' assim, quem é você na fila do pão para achar que é muito especial?"*

---

### 15 · Você tem vícios. Use-os a seu favor

- Você tem vícios de escrita, de raciocínio, de organização
- Aceite isso. Use isso.
- A resposta: cultive um jardim digital

> *"Se você tem vícios, cultive-os num lugar que seja seu."*

Transição natural para a Parte 2.

---

## PARTE 2 · O JARDIM DIGITAL

### 16 · [seção] PARTE 2

*"Antes de falar de agentes, preciso falar de onde eles vão viver."*

---

### 17 · Plain text is king

- Markdown, LaTeX, org-mode — tudo texto
- Você não escreve notas em binário
- Fique no formato intermediário — é o que a interface entre você e o computador vai facilitar

> *"Sua IDE tem que respeitar o que os fontes são para o computador: plain text."*

---

### 18 · Por que não PDF, Word, Excel?

- Imagina o gargalo de ter que lidar com PDF, Excel, Word
- Esses formatos só atrapalham o agente, o script, o Obsidian
- Markdown chega em texto, são instruções que qualquer coisa processa

---

### 19 · Frontmatter + Markdown

- Frontmatter é YAML no topo do arquivo — metadados junto do conteúdo
- Sua base de conhecimento vira dados estruturados sem banco de dados
- Funciona offline, para sempre, em qualquer IDE

---

### 20 · Obsidian e o ecossistema

- Não é só editor — é plataforma
- Pesquisadores, engenheiros, escritores usando
- A próxima imagem mostra quem apoia eles

---

### 21 · [img] obsidian_enterprise.png

*"Só gente grande. Esse ecossistema não é brinquedo."*

---

### 22 · aretw0/vault-seed

- Template pronto, botão "Use this template" no GitHub
- Estrutura básica: notas, agenda, projetos em plain text
- Zero configuração — cria o solo, você planta o que quiser

> *"É um caderno que fica com você para sempre. Simples como o ledger de contabilidade."*

`github.com/aretw0/vault-seed`

---

### 23 · Code Literacy

- A habilidade de ler, escrever e entender código como linguagem — não só ferramenta
- org-mode foi precursor: seus scripts e seu texto se misturam
- Hoje qualquer agente pode ser seu co-autor

> *"A galera do org-mode deve estar ouvindo isso pensando: eu estava aqui o tempo todo, só você não viu."*

---

## PARTE 3 · O PRESENTE AGÊNTICO

### 24 · [seção] PARTE 3

*"Agora chegamos no presente. E o presente é caótico, mas de um jeito bom."*

---

### 25 · O racha histórico

- Sempre existiu esse racha: os que codavam vs. os que cultivavam modelos
- Deterministas vs. probabilistas
- Agora chegaram no estado da arte dos dois mundos ao mesmo tempo

> *"Você tem o rígido — o córtex pré-frontal — e a LLM fazendo a parte criativa."*

---

### 26 · O hardware finalmente chegou

- O que faltava era hardware para guardar os pesos dos modelos
- GPUs tornaram isso viável — física da inteligência encontrou a regra do menor esforço
- Ghost in the Shell deixou de ser ficção científica

> *"O projeto Manhattan é responsável por muito disso — a arquitetura de Von Neumann reflete até hoje."*

---

### 27 · 2025: a era do catnip

- Modelos ficaram bons em tool use — agentes funcionando de verdade
- MCP com speedrun de adoção — protocolos antes demoravam anos
- Ninguém dormia mais experimentando

> *"Quando eu entrei na UFERSA ainda tinha material sobre 3 versões de JavaScript que cada empresa tinha. Protocolos demoravam pra pegar. Rigidez demais."*

---

### 28 · Tool use: como o agente age

- O agente decide qual tool chamar e com quais parâmetros
- Você define as tools — o modelo decide quando usá-las
- É isso. Não tem mágica.

---

### 29 · MCP — quando faz sentido

- MCP é para expor ferramentas via servidor — vários clientes, uma fonte
- Speedrun de adoção: IDEs, agentes, ferramentas — tudo em meses
- Tool direto resolve a maioria dos casos sem complexidade de servidor

---

### 30 · O momento Richard Stallman

- Stallman percebeu que ia ficar preso a uma impressora defeituosa cujo código não podia ver
- Conclusão: precisamos de software livre
- Em 2025, alguns chegaram na mesma conclusão sobre agentes de código

> *"A gente precisa de um kernel. A gente precisa de um motor."*

---

### 31 · Três pessoas que chegaram lá

- Pete: o explorador doidão — foi para a OpenAI depois que o OpenClaw explodiu
- Armin: o cientista — criador do Flask, fundou a Earendil
- Mario: o arquiteto — olhou pro caos e criou algo mínimo

> *"Cada um com o seu pace. O Armin e o Mario olharam para a coisa como quem olha para um laboratório."*

---

### 32 · OpenClaw

- Mais estrelas que o kernel do Linux — deixa isso entrar
- Não é só assistente pessoal — é framework de agentes
- O presidente da NVIDIA não estava fazendo hype. Mas para ele qualquer vetor de consumo de tokens vale.

---

### 33 · [img] openclaw.png

Deixa a imagem falar. *"Isso não é hype. É o estado da arte."*

---

### 34 · O Pi — um kernel minimalista

- Mario criou algo pequeno e extensível — você entende o que está acontecendo
- Não é a LLM — você carrega uma LLM nele
- Sem MCP de fábrica: tool direto é a filosofia, MCP quando realmente precisar

> *"É o que se chama de agent harness. Mas construível. Por boas decisões de arquitetura."*

---

### 35 · [img] pi.png

*"Esse é o Pi rodando. Terminal. Simples. Você lê o código e entende tudo."*

---

### 36 · Earendil = GNU · Pi = Linux

- A Earendil é o projeto de fundação — filosofia, ferramentas, Armin
- O Pi é o primeiro kernel funcional — Mario
- Cada um pode ter a sua distro agêntica

> *"Ah Arthur, mas já existia n8n e outras coisas. Realmente. Mas não está escalando bem — e o próprio fundador do n8n sabe disso."*

---

### 37 · O futuro está nos trilhos

- Clean code, design patterns, arquitetura — nada mudou
- O que mudou foi a velocidade e a facilidade de prototipagem
- Não joga fora o que sabe — usa como base

---

### 38 · Psicose agêntica é real

- Gente achando que o modelo resolve tudo
- A um prompt de um app que "vai mudar o mundo porque o chatgepeto disse"
- Se demorar pra dominar, vai ficar no nível de usuário da plataforma dos outros

> *"E se vai ser esse usuário, que seja de uma que você ajudou a construir, que você auditou."*

---

### 39 · Resumo da palestra

Percorre o diagrama em voz alta. Lento. Um nó por vez.

*"Turing → sistemas experts → PLN e grep → transformers e LLMs → tool use → OpenClaw e Pi → sua distro agêntica."*

---

### 40 · Por onde começar

1. Jardinagem digital — second brain, Zettelkasten, vault-seed
2. Plain text — Markdown, Obsidian
3. Instalar o Pi — entender o loop
4. Explorar o ecossistema — pi.dev/packages
5. Contribuir — o ecossistema livre precisa de você

> *"É hora de lock in. O importante é não ficar para trás — e você não vai, porque você está aqui."*

---

## TRANSIÇÃO

### 41 · INTERVALO · 5 min

*"5 minutos. Depois a gente coloca a mão na massa."*

---

## WORKSHOP · slides de intro

### 42 · [seção] WORKSHOP

*"Agora a teoria vira prática. O documento completo está em github.com/aretw0/talks."*

> A partir daqui siga o WORKSHOP_FLISOL_2026.md na segunda tela.
