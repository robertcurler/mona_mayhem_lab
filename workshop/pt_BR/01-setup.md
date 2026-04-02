<!-- l10n-sync: source-file="01-setup.md" -->
# Parte 1: Setup e Context Engineering

---

Nesta parte, você vai configurar seu ambiente de desenvolvimento **e** ensinar o Copilot sobre a base de código — para que cada prompt futuro comece com o contexto correto.

## Seção 1: Setup Inicial

### Passo 1: Crie Seu Repositório

1. Abra [github.com/copilot-dev-days/mona-mayhem](https://github.com/copilot-dev-days/mona-mayhem)
2. Clique em **Use this template** → **Create a new repository**
3. Nomeie como `my-mona-mayhem` e defina a visibilidade como **Public**

### Passo 2: Habilite o GitHub Pages

1. Vá nas **Settings** → **Pages** do seu novo repositório
2. Em **Source**, selecione **GitHub Actions**

### Passo 3: Clone e Abra no VS Code

1. Abra o VS Code e execute **Git: Clone** → **Clone from GitHub**
2. Selecione o seu repositório `my-mona-mayhem`
3. Quando solicitado, instale as **extensões recomendadas**

### Passo 4: Execute o Setup Agent

1. Abra o painel do **Chat** e digite:

   ```
   /setup
   ```

2. O agente vai detectar seu ambiente, instalar dependências e iniciar o servidor de desenvolvimento automaticamente.

> ✅ **O app está rodando no seu navegador!**

## Seção 2: Context Engineering

Context engineering é como você ensina a IA sobre sua base de código. Quanto melhor o contexto, melhor será cada resposta futura.

### Tarefa 1: Gere Instruções do Workspace

1. Abra a Paleta de Comandos e execute:

   ```
   Chat: Generate Workspace Instructions File
   ```

2. Revise o arquivo gerado — provavelmente está muito detalhado.
3. No Copilot Chat, continue com:

   > "Compress down by half and add a mandatory development checklist (lint, build, test) to the top"

4. **Faça commit** do arquivo de instruções.

> **Resultado:** Todos os futuros requests ao Copilot agora terão um mapa básico do seu workspace integrado.

### Tarefa 2: Agentes em Background

**Agente local em background:**

1. No painel do Chat, clique em **+** → **New background agent**
2. Insira o prompt:

   > "Add linting rules for unused vars and improve code style; fix any errors"

3. Quando terminar, clique em **Review and Apply** para aplicar as alterações e depois exclua a sessão.

**Agente na nuvem:**

1. Inicie outro agente em background com:

   > "Make the README more engaging as a landing page"

> **Resultado:** Regras de linting adicionadas, erros corrigidos, README melhorado — tudo sem sair do editor.

### Tarefa 3: Explore o Projeto

Abra o **Copilot Chat** no modo **Ask** e tente estes prompts:

- `"Explain the architecture of this project"`
- `"What does the API route do?"`
- `"How does the contribution graph rendering work?"`

> 💡 Use **@workspace** para dar ao Copilot contexto de todo o projeto e obter respostas mais precisas.

## ✅ Parte 1 Concluída

Você aprendeu a:

- **Configurar** um ambiente de desenvolvimento com o agente `/setup`
- **Gerar instruções do workspace** para que o Copilot entenda seu projeto
- **Usar agentes em background e na nuvem** para automatizar tarefas de manutenção
- **Explorar uma base de código** usando o modo Ask e `@workspace`
