<!-- l10n-sync: source-file="05-polish.md" -->
# Parte 5: Pulir y Multi-Agente

---

Ahora que la app funciona y se ve genial, es hora de pulir. En lugar de hacer todo secuencialmente, delegarás tareas de pulido a **agentes en segundo plano y en la nube** que trabajan en paralelo — permitiéndote revisar los resultados a medida que llegan.

## Tarea 1: Agente en Segundo Plano para Diseño Responsive

1. En el panel de Chat, haz clic en **+** → **New background agent**
2. Ingresa este prompt:

   ```
   Add responsive CSS media queries: at 1024px switch comparison to single column,
   at 768px reduce font sizes, stack inputs vertically, and make the layout
   mobile-friendly. Also improve keyboard accessibility — ensure tab order works,
   Enter triggers battle, and focus states are visible.
   ```

3. Déjalo ejecutar de forma independiente — no necesitas observarlo
4. Cuando termine, **revisa** los cambios y haz clic en **Apply** para integrarlos

## Tarea 2: Agente en Segundo Plano para UX de Errores

1. En el panel de Chat, haz clic en **+** → **New background agent**
2. Ingresa este prompt:

   ```
   Improve the error experience: add a shake animation for errors, styled error
   messages with red (#ff3366) neon glow effects matching the arcade theme, and
   better input validation feedback. Show clear error messages when usernames are
   empty or invalid.
   ```

3. **Revisa** los cambios cuando el agente termine y haz clic en **Apply**

## Tarea 3: Agente en la Nube para Variaciones (Opcional)

1. En el panel de Chat, haz clic en **+** → **New cloud agent**
2. Ingresa este prompt:

   ```
   Create an alternative color theme for the battle page — keep the retro arcade
   style but use blue (#00f5ff) and orange (#ff6b35) instead of green and purple.
   Create it as a CSS custom property theme that could be toggled.
   ```

3. Revisa las **sesiones de agentes** para monitorear el progreso
4. Revisa la variación de diseño en el PR que crea el agente en la nube

## Tarea 4: Verifica Todo

Ejecuta estos escenarios de prueba para asegurarte de que todo funciona:

| Prueba | Resultado Esperado |
|--------|-------------------|
| Campos vacíos, clic en Battle | Error estilizado con animación de sacudida |
| Nombres de usuario válidos | Gráficos de contribuciones mostrados |
| Nombre de usuario inválido | Error de la API con estilo retro |
| Tecla Enter en el campo de entrada | Activa la batalla |
| Ancho móvil | Diseño responsive en una sola columna |
| Hover en cuadros de contribución | Tooltip con fecha y cantidad |

Compila para producción y confirma que no hay errores:

```bash
npm run build && npm run preview
```

Una vez que todo se vea bien, haz commit de tu código funcional.

---

## ✅ ¡Parte 5 Completa!

**Lo que aprendiste:**

- Usar **agentes en segundo plano** para tareas aisladas en paralelo
- Usar **agentes en la nube** para exploración y variaciones de diseño
- Delegar trabajo de pulido a los agentes mientras revisas y apruebas los resultados
