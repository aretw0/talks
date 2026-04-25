# Workshop — O Pi na prática

> FLISOL 2026 · Mossoró · github.com/aretw0/talks

---

## Por qual caminho seguir?

```
Tem Node.js 20+ instalado?
├── SIM → Caminho A (mais simples)
└── NÃO → Tem Docker Desktop + VSCode?
           ├── SIM → Caminho B (devcontainer)
           └── NÃO → acompanhe pela tela por enquanto
                      e instale o Node depois em nodejs.org
```

---

## Caminho A — Node.js direto

### Pré-requisito

Confirme que o Node está instalado:

```bash
node --version   # v20 ou maior
npm --version
```

Se não tiver: [nodejs.org](https://nodejs.org) → baixe a versão LTS e instale.

### Instalar o Pi

```bash
npm install -g @mariozechner/pi-coding-agent
```

Verifique:

```bash
pi --version
```

Vá para **[Passo 1 — Autenticar](#passo-1--autenticar)**.

---

## Caminho B — Devcontainer (Docker Desktop + VSCode)

> Ideal para quem não tem Node instalado. O container já vem com Node 20 e Pi prontos.

### Pré-requisitos

- [Docker Desktop](https://www.docker.com/products/docker-desktop/) instalado e rodando
- [VSCode](https://code.visualstudio.com/) com a extensão **Dev Containers** (`ms-vscode-remote.remote-containers`)

Crie uma pasta nova em qualquer lugar, abra no VSCode e crie o arquivo `.devcontainer/devcontainer.json`:

```json
{
  "name": "Pi Workshop",
  "image": "mcr.microsoft.com/devcontainers/javascript-node:20",
  "postCreateCommand": "npm install -g @mariozechner/pi-coding-agent"
}
```

Salve, abra a paleta de comandos (`Ctrl+Shift+P`) e execute:

```
Dev Containers: Reopen in Container
```

Aguarde. Quando o terminal interno abrir, o Pi já está disponível.

---

## Passo 1 — Autenticar

Abra o terminal e rode:

```bash
pi
```

Na primeira vez o Pi pede autenticação. Digite `/login` — aparece uma lista de provedores. Escolha o que você tem conta:

- **GitHub Copilot** — conta gratuita do GitHub
- **Google / Gemini** — conta gratuita do Google
- **Claude / Anthropic** — conta Claude.ai
- Entre outros

O Pi abre o navegador para autorizar. Confirme e volte ao terminal.

> **Sem internet?** Se o Wi-Fi do evento travar, você pode rodar o Pi com um modelo local via [Ollama](https://ollama.com). Instale o Ollama, baixe um modelo (`ollama pull llama3`) e rode `pi --model ollama/llama3`. Sem nuvem, sem chave, sem depender de ninguém.

---

## Passo 2 — Primeira conversa

Com o Pi autenticado, tente:

```
> crie um arquivo chamado ola.md com um parágrafo sobre software livre
```

O Pi usa as tools `write` e `read` automaticamente — sem configuração extra.

Verifique o que ele criou:

```
> o que está no arquivo ola.md?
```

---

## Passo 3 — Pi + suas notas

Crie uma pasta de notas:

```bash
mkdir notas
echo "# Nota de hoje" > notas/hoje.md
echo "Primeira nota do workshop." >> notas/hoje.md
```

Dentro do Pi:

```
> leia tudo em notas/ e me faça um resumo
```

```
> adicione uma seção "Próximos passos" na nota de hoje com 3 itens sobre o que aprendi aqui
```

---

## Passo 4 — Explorar o ecossistema

```bash
# listar extensões instaladas
pi list

# ativar ou desativar uma extensão
pi config

# instalar uma extensão
pi install npm:nome-da-extensao
```

Mais extensões em → **[pi.dev/packages](https://pi.dev/packages)**

---

## O que aconteceu por baixo dos panos

O Pi tem 4 tools por padrão: `read`, `write`, `edit`, `bash`.

Quando você pede "leia a pasta", o modelo:

1. Chama a tool `read` com o caminho
2. Recebe o conteúdo de volta
3. Gera a resposta baseado no que leu

```
você → Pi → modelo decide → tool executa → resultado → modelo responde → você
```

Nenhuma mágica — só um loop bem estruturado.

---

## Extendendo o Pi

O Pi tem quatro camadas de extensibilidade — da mais simples para a mais poderosa:

| Camada | O que é | Exemplo |
|--------|---------|---------|
| **Theme** | Cores e estilos do terminal | `pi-rose-pine` |
| **Skill** | Guia de linguagem natural que orienta o modelo | busca web, resumo de vídeo |
| **Prompt template** | Contexto de sistema reutilizável | modo review, modo arquitetura |
| **Extension** | Módulo TypeScript com acesso total ao TUI e ao loop | tudo abaixo |

### TUI — o terminal como tela

O Pi expõe a TUI inteira para extensões: status bar, header, footer, overlays, canvas interativo.

- **`pi-powerline-footer`** — barra de status estilo Powerline com git, modelo ativo e tokens usados
- **`pi-canvas`** — canvas interativo no terminal: calendário, documento, painel de voo
- **`rhubarb-pi`** — session-emoji, session-color (cada sessão tem identidade visual própria)
- **`pi-sketch`** — abre um sketch pad no **navegador**, você desenha e manda a imagem pro modelo

### Notificações e integrações

- **`pi-notification-extension`** — avisa no **Telegram** quando o agente termina uma task
- **`ferologics/pi-notify`** — notificação nativa de desktop via OSC 777
- **`pi-ssh-remote`** — redireciona as operações para um host remoto via SSH
- **`pi-mobile`** — cliente **Android** com gerenciamento de sessão

### Pi no navegador — `pi-web-ui`

O `@mariozechner/pi-web-ui` é uma biblioteca de web components que permite embedar o Pi em qualquer página:

```js
import { ChatPanel } from "@mariozechner/pi-web-ui";

const panel = new ChatPanel({ agent, storage });
document.body.appendChild(panel);
```

- Streaming, execução de tools e histórico de sessão inclusos
- **Direct Mode** — as chaves de API ficam no `localStorage` do navegador, nunca passam por servidor seu
- Suporta artifacts: HTML, SVG, Markdown renderizado, PDF, DOCX, imagens

> A `pi-mom` usa o mesmo stack para criar um bot no **Slack** que delega mensagens ao Pi.

### Esqueleto de uma extensão

Estender o Pi é criar um arquivo TypeScript que exporta um objeto com os hooks que você quer:

```ts
import type { Extension } from "@mariozechner/pi-agent-core";
import { Type } from "@sinclair/typebox";

export const extension: Extension = {
  name: "minha-extensao",
  tools: [
    {
      name: "oi_mundo",
      description: "Diz oi",
      parameters: Type.Object({ nome: Type.String() }),
      execute: async (id, { nome }) => ({ type: "text", text: `Oi, ${nome}!` }),
    },
  ],
};
```

Coloque em `.pi/extensions/minha-extensao.ts` e o Pi carrega automaticamente.

### Descoberta

- Lista curada da comunidade → `github.com/qualisero/awesome-pi-agent`
- Pacotes publicados → `pi.dev/packages`

---

## Keybindings

### Essenciais

| Ação | Atalho |
|------|--------|
| Cancelar task em andamento | `Esc` |
| Enviar mensagem | `Enter` |
| Nova linha na mensagem | `Shift+Enter` (Linux/Mac) · `Ctrl+Enter` (Windows Terminal) |
| Limpar editor | `Ctrl+C` |
| Sair do Pi | `Ctrl+C` duas vezes · ou `/quit` |

### Navegação e modelos

| Ação | Atalho |
|------|--------|
| Abrir seletor de modelo | `Ctrl+L` |
| Ciclar modelos configurados | `Ctrl+P` / `Shift+Ctrl+P` |
| Ciclar nível de thinking | `Shift+Tab` · ou `/settings` |
| Recolher/expandir output das tools | `Ctrl+O` |
| Recolher/expandir blocos de thinking | `Ctrl+T` |
| Abrir visualização de sessões | `Esc` duas vezes · ou `/tree` |

> **Thinking** — modelos que suportam raciocínio estendido (como Claude e alguns da Google) têm níveis configuráveis: sem thinking, leve, médio, intenso. Níveis mais altos consomem mais tokens mas resolvem problemas mais complexos. `Shift+Tab` cicla entre os níveis disponíveis para o modelo ativo; se o modelo não suportar, o atalho não faz nada.

### Slash commands úteis

| Comando | O que faz |
|---------|-----------|
| `/login` | Autenticar com um provedor |
| `/logout` | Deslogar |
| `/model` | Trocar modelo |
| `/new` | Nova sessão |
| `/resume` | Retomar sessão anterior |
| `/settings` | Ajustar theme, thinking, entrega de mensagens |
| `/compact` | Compactar contexto manualmente |
| `/copy` | Copiar última resposta do agente |
| `/share` | Exportar sessão como gist privado no GitHub |
| `/hotkeys` | Mostrar todos os atalhos dentro do Pi |
| `/quit` | Sair |

> `/hotkeys` dentro do Pi sempre tem a lista mais atualizada — use como referência durante o workshop.

---

## Problemas comuns

| Problema | Solução |
|----------|---------|
| `command not found: pi` | Feche e abra o terminal após o install |
| Login não abre o navegador | Copie a URL do terminal e cole no navegador |
| `EACCES` no npm install | `sudo npm install -g` ou ajuste o prefix do npm |
| Pi fica em loop | `Esc` para cancelar a task |
| Quer trocar de modelo | `Ctrl+L` ou `/model` |
| Container demora a subir | Normal na primeira vez — está baixando a imagem Node 20 |
| "Docker not running" | Abra o Docker Desktop antes de reabrir no container |

---

## Para ir além

- Curadoria de agentes com Pi como engine → `github.com/aretw0/agents-lab`
- Clone o vault-seed → `github.com/aretw0/vault-seed`
- Leia o código do Pi → `github.com/badlogic/pi-mono`
- Extensões → `pi.dev/packages`
- Esta palestra → `github.com/aretw0/talks`

---

<!--
## Para o apresentador

### Enquanto o pessoal configura o ambiente
- Fique no Pi rodando algo visível na tela — peça para ele resumir o README do repositório da palestra, ou criar uma nota sobre o evento. O público vê o loop agêntico acontecendo enquanto instala.
- Se alguém travar na autenticação: o fluxo do GitHub Copilot é o mais confiável, direcione para ele primeiro.
- Quem não conseguir instalar pode abrir o devcontainer — lembre de ter o VSCode + Docker Desktop instalados como plano B no seu próprio notebook para demonstrar.

### Ritmo sugerido
- 5 min: todo mundo instalou o Pi e rodou `pi --version`
- 10 min: autenticação — espere a maioria estar logada antes de avançar
- 15 min: Passos 2 e 3 juntos — mostre na tela, deixe o pessoal repetir
- 10 min: seção "Extendendo o Pi" — apresente, não precisa todo mundo implementar
- 5 min: perguntas e "Para ir além"

### Se o Wi-Fi cair
- Você apresenta do seu notebook com agents-lab, que já tem modelos configurados
- Quem tiver Ollama instalado consegue rodar localmente — mencione na hora
- Quem não tiver nada: o workshop vira demo guiada, não problema
-->
