# Engenharia agêntica, open claw e o futuro do software

> Rascunho de Palestra para o evento FLISOL 2026 Mossoró
> FLISOL: Festival Latino Americano de Instalação de Software Livre
> Acontece anualmente, em uma determinada semana vários acontecem em toda a américa latina.
> Em Mossoró costuma ter, eu mesmo lembro de ter visitado rapidamente um desses enquanto estava na graduação de ciência da Computação.
> Infelizmente nunca me envolvi muito, estava com outras coisas na cabeça.

## Perfil do palestrante

Arthur Aleksandro Alves Silva.
Eletrotécnico pelo IFRN.
Técnico em TI pelo IMD.
Cientista da Computação pela UFERSA.
Especialista em Testes de Software pela UFPE.
Pau pra toda obra.
Já completei minhas 10000 horas na área.

Talvez me conheçam pelo "UFERSA Vai de Bike" que chegou a ser meu TCC no final da graduação.
Hoje trabalho no SERPRO, o serviço federal de processamento de dados, onde atuo como engenheiro de software e faço parte de uma divisão que atende a receita federal em questão de direito creditório.

Moro em Recife há uns 6 anos, estou saindo mais da caverna recentemente para poder espalhar essa palavra que é a engenharia agêntica, o software agêntico, o open claw e tudo mais que tem a ver com isso.

## Primeiras impressões do título

> Haha que futuro? Estamos rimando com o passado, essa onda de IA só não baixou ainda.
> Existem termos mais abrangentes como o cibernético, gosto da história de como o chile tentou ter seu sistema mas foi sabotado pela golpe militar. Colocar o link do vídeo e possível visão do painel de controle do chile, a sala que parecia nave espacial: <https://www.youtube.com/watch?v=mayoL3XbKwA> (cybersin.png)
> Para depois vermos empresas como a Amazon serem as representantes do estado da arte da coordenação digital de recursos.
> Eles não deixaram a gente evoluir os nossos sistemas, e quem perguntar quem são eles... cara, sinto muito você não esta pronto.
> Pergunto quem são eles, eu já assumo que você não esta pronto ainda e não vai ser nessa palestra que eu vou trazer essa visão pra tu.
> O que eu vim fazer foi repassar o passado e o presente e mostrar o que eu venho fazendo de curadoria de uma possível realidade compartilhada.
> E eu digo isso porque tem gente esquecendo dessa realidade, não deixando ela entrar na sua vida e etc.
> Se não tiver um curso não faz, se não tiver essa palestra aqui não se envolve.
> Mea culpa aqui, porque toda vez que eu me sinto perdido eu tenho que lembrar disso, é sobre ser teimoso ta ligado?
> Você tem que ser tão resiliente quanto seus sistemas, porque frustração vai ter, é caótico.
> Menção ao chaos computing Community na Alemanha com quase 30 anos de web radio e com eventos recentes como o power ranger rosa justiceiro social derrubando site supremacista. Posso colocar uma imagem.

## Segunda seção de brainstorm

Ok ok, estou pronto para despejar o primeiro esboço dessa palestra.

Eu já reconheci que talvez eu já devesse ter vindo para o flisol, foi mal tava doidão, ou com outras prioridades né.
Eu respeito muito quem ta começando por isso, porque equilibrar os ruídos da vida adulta não é fácil.
Na minha experiência aprender com muito ruído não é bom, mas ruído e fricção também é algo que é necessário para te polir então é preciso achar o equilíbrio entre cobrar espaços para aprendizado ao mesmo tempo que tu tenta melhorar ele do jeito que der e confia no processo porque no final da iteração se você não tiver cego você vai ver que tem material para aprender e tentar de novo melhor.

Mas é isso, estou aqui! E estou aqui para dizer, nossa a história rima que é uma beleza né?

> O ditado: a história não se repete (talvez), mas rima que é uma beleza.

Então, não existe nada de muito novo para mim, as mesmas coisas estão em jogo, o caminho é que talvez tenha sido encurtado e agora nós temos praticamente portais para outras dimensões. Você esta a um prompt de um aplicativo monstruoso ai que você jura que vai mudar o mundo porque o chatgepeto disse confia!

Mas essas dimensões avançadas são a da LLM, ela consegue lidar com vários parâmetros, você talvez ainda não.
E olhe que até a LLM tem limites, certo, você não pode carregar qualquer coisa nela e cruzar os dedos que vai dar certo.
Só que esse assunto fica para outra hora, porque é claramente uma grande demonstração de computação do chaos.

Computação do chaos é o que? Quando você jura que fez uma gambiarra mas deu tão certo que que virou framework?

Problemas complexos, soluções complexas, ganha quem deixa o cérebro do usuário o mais liso possível, que nem um peito de frango, certo?

Mas vocês aqui não vão ser esse usuário, eu espero, ou vão criar clusters de agentes que não façam ninguém cair em furada, porque no momento a gente tem gente achando que é jesus cristo e indo pro deserto ter visões.

E eu até pareço jesus e talvez o meu papo pareça que estou falando de despertar da matrix, mas é só coincidência mesmo.

De toda forma psicose agêntica é real, está por ai, se você demorar muito a dominar essas ferramentas você vai ficar no nível de quem é usuário da plataforma dos outros. E se você vai ser esse usuário, que seja de uma que você ajudou a construir e que você auditou ou permitiu ser auditado e etc etc

Esse mesmo papo pode ser usado para nos levar no passado, porque eu acho que agora esta na hora ver por onde andamos com essas ideias.

Eu diria que tudo começa com turing né, a idéia da fita ainda é presente, o que você acha que você esta construindo durante uma sessão de chat com uma IA? Continua sendo uma fita.

E a gente tem o teste de turing que hoje em dia eu acho que virou piada, porque muita gente conversa com bot achando que é humano e ok né, queremos agilidade nas nossas vidas, mas quando não temos controle já era também, se me permite a digressão rápida ao que vivemos atualmente.

A experiência agêntica LISA é também bastante lembrada.
> Posso adicionar mais sobre ela aqui

A questão é que os sistemas experts são tão antigos quanto a própria computação.
A diferença é que a gente generalizou o processamento e conseguimos deixar "pesos" guardados de uma rede neural treinada.
E isso eu to reduzindo bastante, tem todo tipo de arquitetura de modelos treináveis e PLN.

Aqui eu dou um carteirada de leve, enquanto estive no CIn, centro de informática da UFPE, para minha especialização, fui agraciado com cursos de extensão da Unicamp, se não me engano, o primeiro sobre PLN (processamento de linguagem natural) e o outro foi sobre Transformers, modelos de difusão, modelos de atenção no geral e IA na nuvem.

Eu tava atingindo o teto do que eu podia fazer com código dentro do projeto lá, a gente já vinha processando semântica e sintaxe era algo comum para os reports de bug para construção de knowledge base.

Nesse ponto eu preciso olhar para trás e ser gentil comigo mesmo porque eu sinto que eu vacilei em aprender tanto nesses cantos que esqueci de criar a minha arca de noé que sobrevive a esses locais que a gente passa.

Porque eu acho que os sistemas experts eles começam por ai, você tem muito texto processável e quer tirar insights com processamento de linguagem natural.

Aqui a gente entra com a história do utilitário `grep`.
Conta-se que ele foi criado para ajudar no processamento do conjunto de manifestos dos fundadores dos estados unidos.
Eles haviam publicado um manifesto com vários textos mas sem nome de ninguém, apenas uma alcunha genérica.
O grep ajudou a separar que fundador tinha escrito cada um dos textos por ter comparado com escritas assinadas por eles, e que mostram os vícios que eles tinham.

E ai pausa para check de humildade certo? Se até um fundador dos estados unidos pode ser "profiled" assim, quem é você na fila do pão para achar que é muito especial sabe? Você tem vícios, você tem manias e é melhor aceitar isso e usar ao seu favor.

Usar ao seu favor como? Cultive um jardim digital.

Eu tenho todo um repositório no meu GitHub chamado vault-seed que é a semente desse assunto, esta pronto para você criar um repositório a partir dele, com o botão que tem lá e ele já te da um solo básico sobre essas ideias.

É um caderno que você fica para si eterno, uma agenda, mas simples porque funciona em plain text como o utilitário de contabilidade ledger.

Você consegue abrir com a sua IDE, porque ora ora ora, a sua IDE tem que respeitar os que os fontes são para o seu computador: plain text.

O Obsidian é uma apresentação a parte e eu vou deixar só aqui a galera que apoia eles.
> fotos dos apoiadores, só gente grande.

Então, vá por mim, você NÃO QUER sair do mesmo nível que o seu código, porque é texto que poderia ta sendo usado por um agente ou pelo obsidian, ou por você em algum script.

Imagina o gargalo tu ter que lidar com PDF, Excel, Word... esses formatos só atrapalham.

LaTex é um exemplo disso, o seu artigo fica marcação de texto que pode ser projetada, renderizada.
Markdown é isso, HTML é isso só que com tags e ele foi feito para o hyperspace que é a internet.

Porque ele chega em texto no seu computador e são instruções para o navegador não só renderizar, como o que carregar se tiver coisa ainda pra baixar depois e ainda código que pode rodar no navegador do usuário.

E tudo isso é texto, porque é scripting, binário a gente deixa para coisas pesadas de verdade que é aonde entraria o WASM (WebAssembly) no caso do navegador mas é verdade que qualquer coisa que você faça em golang ou rust vai ser melhor do que em nodejs pela falta do gargalo que é pro computador ter que interpretar texto.

Você não escrever suas notas em binário ok, então fica no mesmo formato intermediário que a interface entre vocês dois vai facilitar bastante, e se você realmente crescer para precisar de um servidor a disciplina vai ser a mesma!

Então sim, tenha base de dados com markdown e frontmatter para coisas como caderno e agenda!

Cria sua wiki renderizável de markdown para html como o MkDocs para python ou outros gerados de site estático.
É sobre botar seu bloco na rua de algum jeito e ainda cultivar algo que fique contigo.

A galera do org-mode deve esta escutando isso e pensando: eu estava aqui o tempo todo só você não viu.

Querendo ou não o org-mode foi sabotado como muita coisa boa que vem para desbloquear a gente, mas é a partir deles que nasce essa idéia de sistemas experts de conhecimento e muitas vezes agêntico porque seus scripts e seu texto se misturam.

Eu li que se chama code literacy.
> Explicar

De resto o que eu posso dizer para você é que houve sempre esse racha entre os que codavam e os que cultivam um modelo, os deterministas e os probabilistas, só que agora eles chegaram no estado da arte desses dois mundos.

Você tem o rígido que é o córtex pre frontal e a LLM fazendo a parte criativa
> preencher que outra parte do cérebro a LLM representa nessa analogia.

O projeto manhattam é responsável por muita dessas coisas sabe?
A arquitetura de von neuman reflete até hoje pois é como da para tentar controlar o caos probabilístico das reação sub atômicas.
E isso claro, to reduzindo bastante.

o que nos faltava era hardware para termos oficialmente o ghost in the shell quando se trata dos pesos dessas modelos.
E isso é todo um assunto sobre a física da inteligência e como ela se mistura com a regra da natureza do menor esforço.
Nesse ponto é aonde é o vibecode, porque ta todo mundo querendo que os modelos tenha essa malemolência de sempre ter o momento de eureca, o que eles chamam de grokking.

Eles aindam não atingiram a LLM ideal, e muito provavelmente vão se matar pra fazer isso, o que importa é o que da para fazer com as que já tem no momento, se você coordenar direitinho elas, como você coordenaria a carga de um sistema seu, você sai na frente.

Mas agora vamos voltar para algo mais atual.
Começamos a ver os agentes de codificação acontecer de verdade.

Muita gente viciada na minha área, porque é o rush do novo dando certo.

Só que eu digo a você como uma pessoa que experimentou vários e estava entendendo até aonde ia, eu cheguei na mesma conclusão que algumas outras pessoas.

A mesma conclusão que Richard stallman teve quando percebeu que ele ia ficar com uma impressora defeituosa.

A gente precisa de software livre, a gente precisa de um kernel, a gente precisa de um motor.

O OpenClaw seria a distro mais famosa desse motor que saiu.

Não é só um assistente pessoal, é um framework de agentes e é claro que começa por um agente de codificação.
É dele que surge todos os outros.

E acho que agora podemos chegar em 2025, estávamos fervendo de possibilidades.

- MCP tinha saído no começo do ano, o protocolo de comunicação que fez speedrun de adoptabilidade

> Gente quando eu entrei na ufersa ainda tinha material sobre 3 versões de javascript que cada empresa tinha antigamente, os protocolos e padrões demoravam pra pegar, rigidez demais.

- Modelos começaram a ficar bons em gerar chamadas de tools, operando melhor o harness dela e consequentemente melhores resultados.
- Foi a era do catnip, ninguém dormia mais experimentando tudo.

> Eu vou ter um slide só de lições sobre jardinagem digital para cultivo com drones.

E ai tivemos outra situação Richard stalmman das idéias, aparentemente, porque eu so fui descobrir isso tudo quando o open claw chegou para mim e ai fui ler os sites estáticos das pessoas envolvidas:

- Pete, criador do open claw: <https://steipete.me/>
- Armin, criador do flask (python): lucumr.pocoo.org/
- Mario, criado do Pi: <https://mariozechner.at/>

Quando o Presidente da NVIDIA falou que o OpenClaw era o software mais importante já feito nos últimos tempos, ele não estava fazendo hype. Mas eu entendo que para ele qualquer vetor de consumo de tokens ta valendo, não importa, a placa de vídeo é ele que vende e isso é o que importa.

Esse pessoal esticou muito a corda, experimentou bastante, chegou nos limites de cada assistente de código agêntico.
Cada um com o seu pace, o Pete é mais doidão, não a toa depois que o open claw explodiu ele foi para a open ai a convite!

O Armim e o Mario olharam para a coisa como quem olha para um laboratório, e o Mario criou esse minimal kernel ótimo para se controlar o caos das opções que se tem de agentes.

Só que melhor, é extensível de um jeito que você não fica preso a ele, até porque ele não é a LLM, você carrega uma LLM nele e o usa.

Ele é o que se chama de agente harness, só que uma que pode se construir, por boas decisões de arquitetura.

E arquitetura é algo que se você se ligar tu replica em uma linguagem melhor e ta sossegado.
Se você prefere python, que seja.
Vai cada um fazer bootstrap de alguma coisa parecida, e ai tu tem o teu próprio agente de codificação, o teu próprio framework de agentes, o teu próprio sistema operacional de agentes, o teu próprio kernel de agentes, o teu próprio software livre de agentes.

Eu comecei a fazer algumas coisas em golang, os blocos, mas o pi já entregou a receita e agora eu já to portando para rust em outro projeto.

Todas as linguagens tem como tu fazer algum tipo de REPL.
> Explicar REPL rapidamente para não entrar em assuntos do workshop.

Então não importa a jornada, o software agora pode se modificar no caminho para o que você precisar e essas modificações serem com o tempo fortalecidas ao ponto de serem determinísticas e não precisar de nenhum classificador de llm no meio do processo e se precisar que seja um llm que esteja rodando na sua casa ou algo do tipo.

Ah Arthur mas já existia n8n e outras coisas.
Realmente existia, mas não ta escalando bem e o próprio fundado do n8n sabe disso porque olha só a galera que ta apoiando a nova empreitada do Armin (Flask)
> Colocar imagem do <https://earendil.com/> empresa do Armin e o texto dos apoiadores deles.
> Nesse ponto talvez eu já tenha falado de como o Pi foi para a <https://earendil.com/>.

Então temos a earendil como o projeto GNU e o Pi como o seu primeiro kernel como o Linux.

## Extras

> OpenClaw se tornou tão popular quando outros projeto de software, hoje com mais estrelas que o kernel do linux.
> O Pi ainda esta sendo popularizado massivamente, muita gente ainda não percebeu a blueprint que ele é.
> Cada um pode fazer sua curadoria de extensões Pi e ter a sua distro agêntica.
> As regras do processo de desenvolvimento de software ainda estão em vigor, o que mudou foi a velocidade e a facilidade de prototipagem.
> Clean code, design patterns, arquitetura de software, tudo isso ainda é necessário, só que agora a gente tem um monte de ferramentas para ajudar a gente a seguir essas regras e não ter que ficar inventando a roda toda hora.
> O futuro do software é o software agêntico, o software que se modifica e se adapta para o que a gente precisa, e isso é algo que a gente já tem hoje, só que ainda ta engatinhando, mas a tendência é que isso se torne cada vez mais comum e acessível para todo mundo. Ainda mais se depender de mim haha.
> Eu não comentei aqui nada sobre saúde mental, geopolítica, economia, etc, mas é claro que tudo isso vai ser impactado por essas mudanças tecnológicas, e a gente precisa estar preparado para lidar com isso de forma consciente e responsável.
> O Armin inclusive fez uma extensão do pi que fica te avisando se você tiver de prompt em prompt de madrugada, para cuidar da saúde mental dos usuários, e isso é algo que a gente precisa pensar cada vez mais, porque a tecnologia tem um impacto enorme na nossa vida, e a gente precisa usar ela de forma consciente e responsável.
> De toda forma, é hora de lock in, porque o futuro do software é o software agêntico, e a gente tem que estar preparado para isso, seja aprendendo a usar essas ferramentas, seja contribuindo para o desenvolvimento delas, seja criando as nossas próprias soluções agênticas, o importante é não ficar para trás nessa revolução tecnológica que ta acontecendo.
> Por onde começar: entender jardinagem digital, second brain, zettelkasten, etc, para criar a sua própria arca de noé digital, para começar a experimentar com essas ferramentas e ver o que você consegue criar com elas. E claro, sempre estar aberto para aprender e se adaptar, porque o futuro do software é algo que a gente ainda não sabe exatamente como vai ser, mas que com certeza vai ser muito diferente do que a gente tem hoje e ter um ambiente seu onde você possa experimentar e aprender é algo que vai ser fundamental para se adaptar a essas mudanças. Sempre foi, agora é mais do que nunca.
