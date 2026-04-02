<!-- l10n-sync: source-file="06-bonus.md" -->
# 🎉 Bonus y Extensiones

---

¡Has construido una app de GitHub Battle completamente funcional! Ahora es momento de ir más allá con **desafíos abiertos**. Usa **Agent Mode** para todos ellos — describe lo que quieres y deja que Copilot te ayude a construirlo.

---

## 🏆 Desafío 1: Banner de Ganador

Después de que ambos gráficos de contribuciones se carguen, compara los totales y muestra un anuncio dinámico del ganador.

**Qué construir:**
- Comparar las contribuciones totales de ambos usuarios
- Mostrar **"🏆 {username} WINS! 🏆"** con un estilo de celebración si hay un ganador claro
- Mostrar **"🤝 IT'S A TIE! 🤝"** si las contribuciones son iguales
- Agregar animación o confeti para mayor impacto visual

**Sugerencia de prompt para Agent Mode:**
> After both users' contribution data loads, compare total contributions and display a winner banner. Show "🏆 {username} WINS! 🏆" if one user has more contributions, or "🤝 IT'S A TIE! 🤝" if equal. Make it visually exciting with CSS animations.

---

## 🏆 Desafío 2: Contador de Racha

Calcula y muestra la racha de contribuciones consecutivas más larga de cada usuario.

**Qué construir:**
- Analizar los datos de contribuciones día por día
- Encontrar la secuencia más larga de días consecutivos con al menos una contribución
- Mostrar el conteo de la racha de forma prominente para cada usuario
- Resaltar quién tiene la racha más larga

**Sugerencia de prompt para Agent Mode:**
> Add a streak counter feature that analyzes each user's contribution data to find their longest consecutive contribution streak. Display "🔥 Longest Streak: X days" for each user below their contribution graph.

---

## 🏆 Desafío 3: Historial de Batallas

Persiste los resultados de las batallas para que los usuarios puedan ver sus enfrentamientos anteriores.

**Qué construir:**
- Guardar cada resultado de batalla en `localStorage` (nombres de usuario, totales, ganador, marca de tiempo)
- Agregar una sección **"Recent Battles"** debajo del área de batalla principal
- Mostrar las últimas 5–10 batallas con resultados
- Agregar un botón "Clear History"

**Sugerencia de prompt para Agent Mode:**
> Save battle results to localStorage after each comparison. Add a "Recent Battles" section that displays the last 10 battles with usernames, contribution totals, the winner, and when the battle happened. Include a "Clear History" button.

---

## 🏆 Desafío 4: Efectos de Sonido

Agrega efectos de sonido retro arcade usando la Web Audio API — sin necesidad de archivos externos.

**Qué construir:**
- Sonido de **insertar moneda** cuando se hace clic en el botón "Battle!"
- Sonido de **power up** cuando los resultados se cargan exitosamente
- Sonido de **explosión** cuando ocurre un error (usuario no encontrado, fallo de API)
- Un botón de activar/desactivar sonido

**Sugerencia de prompt para Agent Mode:**
> Add retro arcade sound effects using the Web Audio API (no audio files). Play a coin insert sound on battle start, a power-up sound when results load, and an explosion sound on errors. Generate the sounds programmatically with oscillators and gain nodes. Include a mute toggle.

---

## 🏆 Desafío 5: Secuencia de Batalla Animada

Genera suspenso con una cuenta regresiva dramática antes de revelar los resultados.

**Qué construir:**
- Cuando se haga clic en "Battle!", mostrar una superposición a pantalla completa
- Animar: **"3..."** → **"2..."** → **"1..."** → **"⚡ FIGHT! ⚡"**
- Luego revelar los gráficos de contribuciones con una entrada dramática
- Usar animaciones CSS o temporización con JavaScript

**Sugerencia de prompt para Agent Mode:**
> Add an animated battle sequence when the user clicks "Battle!". Show a countdown overlay: "3..." then "2..." then "1..." then "⚡ FIGHT! ⚡" with each step lasting about 1 second. After the countdown, reveal the results with a slide-in animation.

---

## 🏆 Desafío 6: Leyenda de Contribuciones

Agrega una leyenda de escala de colores que coincida con la paleta de colores del gráfico de contribuciones.

**Qué construir:**
- Una leyenda horizontal mostrando los niveles de intensidad de contribuciones
- Etiquetas desde **"Less"** hasta **"More"**
- Usar la paleta de colores real de la respuesta de la API de contribuciones de GitHub
- Posicionarla cerca de los gráficos de contribuciones

**Sugerencia de prompt para Agent Mode:**
> Add a contribution legend below the graphs showing the color scale from the API's color palette. Display a row of colored squares ranging from "Less" (lightest) to "More" (darkest), matching the actual contribution level colors returned by the API.

---

## 🏆 Desafío 7: Compartir Resultados

Permite que los usuarios compartan los resultados de su batalla con un solo clic.

**Qué construir:**
- Un botón **"📋 Share Results"** que aparezca después de una batalla
- Copia un resumen formateado al portapapeles
- Incluir nombres de usuario, totales de contribuciones y el ganador
- Mostrar un breve mensaje de confirmación "Copied!"

**Sugerencia de prompt para Agent Mode:**
> Add a "📋 Share Results" button that copies a formatted battle summary to the clipboard. The summary should include both usernames, their contribution totals, and who won. Use the Clipboard API and show a brief "Copied to clipboard!" confirmation.

---

## 🎊 ¡Felicidades!

¡Has completado el taller **Mona Mayhem: GitHub Battle**! Esto es lo que lograste:

### Lo Que Construiste

- ✅ Una **aplicación web multi-página** completa a partir de una especificación de diseño
- ✅ Una **página de inicio** con tematización retro arcade y diseño responsive
- ✅ Una **arena de batalla** que obtiene y compara datos reales de contribuciones de GitHub
- ✅ **Gráficos de contribuciones interactivos** con niveles de actividad codificados por colores
- ✅ **Manejo de errores, estados de carga y mejoras de accesibilidad**
- ✅ **Diseño responsive** que funciona en diferentes dispositivos

### Lo Que Aprendiste

| Habilidad | Lo Que Practicaste |
|-----------|-------------------|
| **Context Engineering** | Proporcionar a Copilot especificaciones de diseño, archivos de referencia y restricciones claras para obtener mejores resultados |
| **Plan Mode** | Usar Copilot para analizar requisitos y generar planes de implementación paso a paso antes de escribir código |
| **Agent Mode** | Delegar tareas de múltiples archivos y múltiples pasos a Copilot e iterar sobre los resultados |
| **Desarrollo orientado al diseño** | Comenzar desde una especificación visual y traducirla en código funcional con asistencia de IA |
| **Flujos de trabajo multi-agente** | Combinar Plan Mode para estrategia con Agent Mode para ejecución en diferentes fases del desarrollo |

### 🚀 Sigue Adelante

- 📺 [Canal de YouTube de VS Code](https://www.youtube.com/@code) — Consejos, tutoriales y novedades
- 📖 [Documentación de GitHub Copilot](https://docs.github.com/en/copilot) — Documentación oficial y guías
- 🌟 [Awesome GitHub Copilot](https://github.com/stefanprodan/awesome-github-copilot) — Recursos y ejemplos de la comunidad
- 🛠️ [Talleres de Copilot Dev Days](https://github.com/github/copilot-dev-days) — Más talleres prácticos como este

---

## 🙏 ¡Gracias!

¡Gracias por participar en este taller! Has experimentado cómo GitHub Copilot puede acelerar cada fase del desarrollo — desde la planificación y el diseño hasta la implementación y el pulido. Las técnicas que practicaste aquí se aplican a cualquier proyecto, cualquier framework y cualquier escala. ¡Ahora ve y construye algo increíble! 🚀
