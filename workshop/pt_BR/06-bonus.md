<!-- l10n-sync: source-file="06-bonus.md" -->
# 🎉 Bônus e Extensões

---

Você construiu um app de GitHub Battle totalmente funcional! Agora é hora de ir além com **desafios abertos**. Use o **Agent Mode** para todos eles — descreva o que você quer e deixe o Copilot ajudá-lo a construir.

---

## 🏆 Desafio 1: Banner do Vencedor

Após ambos os gráficos de contribuição carregarem, compare os totais e exiba um anúncio dinâmico do vencedor.

**O que construir:**
- Compare o total de contribuições de ambos os usuários
- Mostre **"🏆 {username} WINS! 🏆"** com um estilo celebratório se houver um vencedor claro
- Mostre **"🤝 IT'S A TIE! 🤝"** se as contribuições forem iguais
- Adicione animação ou confete para um efeito extra

**Sugestão de prompt para o Agent Mode:**
> After both users' contribution data loads, compare total contributions and display a winner banner. Show "🏆 {username} WINS! 🏆" if one user has more contributions, or "🤝 IT'S A TIE! 🤝" if equal. Make it visually exciting with CSS animations.

---

## 🏆 Desafio 2: Contador de Sequência

Calcule e exiba a maior sequência de contribuições consecutivas de cada usuário.

**O que construir:**
- Analise os dados de contribuição dia a dia
- Encontre a maior sequência de dias consecutivos com pelo menos uma contribuição
- Exiba a contagem da sequência de forma destacada para cada usuário
- Destaque quem tem a sequência mais longa

**Sugestão de prompt para o Agent Mode:**
> Add a streak counter feature that analyzes each user's contribution data to find their longest consecutive contribution streak. Display "🔥 Longest Streak: X days" for each user below their contribution graph.

---

## 🏆 Desafio 3: Histórico de Batalhas

Persista os resultados das batalhas para que os usuários possam ver seus confrontos anteriores.

**O que construir:**
- Salve cada resultado de batalha no `localStorage` (nomes de usuário, totais, vencedor, timestamp)
- Adicione uma seção **"Recent Battles"** abaixo da área principal de batalha
- Mostre as últimas 5–10 batalhas com resultados
- Adicione um botão "Clear History"

**Sugestão de prompt para o Agent Mode:**
> Save battle results to localStorage after each comparison. Add a "Recent Battles" section that displays the last 10 battles with usernames, contribution totals, the winner, and when the battle happened. Include a "Clear History" button.

---

## 🏆 Desafio 4: Efeitos Sonoros

Adicione efeitos sonoros retrô estilo arcade usando a Web Audio API — sem necessidade de arquivos externos.

**O que construir:**
- Som de **inserção de moeda** quando o botão "Battle!" for clicado
- Som de **power up** quando os resultados carregarem com sucesso
- Som de **explosão** quando um erro ocorrer (usuário não encontrado, falha na API)
- Um botão de ativar/desativar som (mute/unmute)

**Sugestão de prompt para o Agent Mode:**
> Add retro arcade sound effects using the Web Audio API (no audio files). Play a coin insert sound on battle start, a power-up sound when results load, and an explosion sound on errors. Generate the sounds programmatically with oscillators and gain nodes. Include a mute toggle.

---

## 🏆 Desafio 5: Sequência Animada de Batalha

Crie suspense com uma contagem regressiva dramática antes de revelar os resultados.

**O que construir:**
- Quando "Battle!" for clicado, mostre uma sobreposição em tela cheia
- Anime: **"3..."** → **"2..."** → **"1..."** → **"⚡ FIGHT! ⚡"**
- Em seguida, revele os gráficos de contribuição com uma entrada dramática
- Use animações CSS ou temporização JavaScript

**Sugestão de prompt para o Agent Mode:**
> Add an animated battle sequence when the user clicks "Battle!". Show a countdown overlay: "3..." then "2..." then "1..." then "⚡ FIGHT! ⚡" with each step lasting about 1 second. After the countdown, reveal the results with a slide-in animation.

---

## 🏆 Desafio 6: Legenda de Contribuições

Adicione uma legenda de escala de cores que corresponda à paleta de cores do gráfico de contribuições.

**O que construir:**
- Uma legenda horizontal mostrando os níveis de intensidade de contribuição
- Rótulos de **"Less"** a **"More"**
- Use a paleta de cores real da resposta da API de contribuições do GitHub
- Posicione próximo aos gráficos de contribuição

**Sugestão de prompt para o Agent Mode:**
> Add a contribution legend below the graphs showing the color scale from the API's color palette. Display a row of colored squares ranging from "Less" (lightest) to "More" (darkest), matching the actual contribution level colors returned by the API.

---

## 🏆 Desafio 7: Compartilhar Resultados

Permita que os usuários compartilhem os resultados da batalha com um único clique.

**O que construir:**
- Um botão **"📋 Share Results"** que aparece após uma batalha
- Copia um resumo formatado em texto para a área de transferência
- Inclua nomes de usuário, totais de contribuições e o vencedor
- Mostre uma breve mensagem de confirmação "Copied!"

**Sugestão de prompt para o Agent Mode:**
> Add a "📋 Share Results" button that copies a formatted battle summary to the clipboard. The summary should include both usernames, their contribution totals, and who won. Use the Clipboard API and show a brief "Copied to clipboard!" confirmation.

---

## 🎊 Parabéns!

Você concluiu o workshop **Mona Mayhem: GitHub Battle**! Aqui está o que você realizou:

### O Que Você Construiu

- ✅ Uma **aplicação web multi-página** completa a partir de uma especificação de design
- ✅ Uma **página inicial** com tema retrô arcade e layout responsivo
- ✅ Uma **arena de batalha** que busca e compara dados reais de contribuição do GitHub
- ✅ **Gráficos de contribuição interativos** com níveis de atividade codificados por cores
- ✅ **Tratamento de erros, estados de carregamento e acessibilidade** aprimorados
- ✅ **Design responsivo** que funciona em diferentes dispositivos

### O Que Você Aprendeu

| Habilidade | O Que Você Praticou |
|---|---|
| **Context Engineering** | Fornecer ao Copilot especificações de design, arquivos de referência e restrições claras para obter melhores resultados |
| **Plan Mode** | Usar o Copilot para analisar requisitos e gerar planos de implementação passo a passo antes de escrever código |
| **Agent Mode** | Delegar tarefas de múltiplos arquivos e múltiplas etapas ao Copilot e iterar nos resultados |
| **Desenvolvimento Orientado a Design** | Partir de uma especificação visual e transformá-la em código funcional com assistência de IA |
| **Fluxos Multi-Agent** | Combinar Plan Mode para estratégia com Agent Mode para execução em diferentes fases do desenvolvimento |

### 🚀 Continue Aprendendo

- 📺 [Canal do VS Code no YouTube](https://www.youtube.com/@code) — Dicas, tutoriais e novidades
- 📖 [Documentação do GitHub Copilot](https://docs.github.com/en/copilot) — Documentação oficial e guias
- 🌟 [Awesome GitHub Copilot](https://github.com/stefanprodan/awesome-github-copilot) — Recursos e exemplos da comunidade
- 🛠️ [Copilot Dev Days Workshops](https://github.com/github/copilot-dev-days) — Mais workshops práticos como este

---

## 🙏 Obrigado!

Obrigado por participar deste workshop! Você experimentou como o GitHub Copilot pode acelerar cada fase do desenvolvimento — do planejamento e design à implementação e polimento. As técnicas que você praticou aqui se aplicam a qualquer projeto, qualquer framework e qualquer escala. Agora vá construir algo incrível! 🚀
