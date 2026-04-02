<!-- l10n-sync: source-file="05-polish.md" -->
# Parte 5: Polimento e Multi-Agent

---

Agora que o app funciona e está bonito, é hora de polir. Em vez de fazer tudo sequencialmente, você vai delegar tarefas de polimento para **agentes em background e na nuvem** que trabalham em paralelo — permitindo que você revise os resultados conforme eles chegam.

## Tarefa 1: Agente em Background para Design Responsivo

1. No painel do Chat, clique em **+** → **New background agent**
2. Insira este prompt:

   ```
   Add responsive CSS media queries: at 1024px switch comparison to single column,
   at 768px reduce font sizes, stack inputs vertically, and make the layout
   mobile-friendly. Also improve keyboard accessibility — ensure tab order works,
   Enter triggers battle, and focus states are visible.
   ```

3. Deixe rodar de forma independente — você não precisa ficar acompanhando
4. Quando terminar, clique em **Review** para revisar as alterações e em **Apply** para aplicá-las

## Tarefa 2: Agente em Background para UX de Erros

1. No painel do Chat, clique em **+** → **New background agent**
2. Insira este prompt:

   ```
   Improve the error experience: add a shake animation for errors, styled error
   messages with red (#ff3366) neon glow effects matching the arcade theme, and
   better input validation feedback. Show clear error messages when usernames are
   empty or invalid.
   ```

3. Clique em **Review** para revisar as alterações quando o agente concluir e em **Apply** para aplicá-las

## Tarefa 3: Agente na Nuvem para Variações (Opcional)

1. No painel do Chat, clique em **+** → **New cloud agent**
2. Insira este prompt:

   ```
   Create an alternative color theme for the battle page — keep the retro arcade
   style but use blue (#00f5ff) and orange (#ff6b35) instead of green and purple.
   Create it as a CSS custom property theme that could be toggled.
   ```

3. Verifique as **sessões de agentes** para monitorar o progresso
4. Revise a variação de design no PR que o agente na nuvem criar

## Tarefa 4: Verifique Tudo

Execute estes cenários de teste para garantir que tudo funciona:

| Teste | Resultado Esperado |
|-------|-------------------|
| Campos vazios, clicar em Battle | Erro estilizado com animação de shake |
| Nomes de usuário válidos | Gráficos de contribuição exibidos |
| Nome de usuário inválido | Erro da API com estilo retrô |
| Tecla Enter no campo de entrada | Dispara a batalha |
| Largura mobile | Layout responsivo em coluna única |
| Hover nos quadrados de contribuição | Tooltip com data e contagem |

Faça o build para produção e confirme que não há erros:

```bash
npm run build && npm run preview
```

Quando tudo estiver funcionando, faça commit do seu código.

---

## ✅ Parte 5 Concluída!

**O que você aprendeu:**

- Usar **agentes em background** para tarefas paralelas isoladas
- Usar **agentes na nuvem** para exploração de design e variações
- Delegar trabalho de polimento para agentes enquanto você revisa e aprova os resultados
