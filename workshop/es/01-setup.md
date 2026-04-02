<!-- l10n-sync: source-file="01-setup.md" -->
# Parte 1: Configuración e Ingeniería de Contexto

---

En esta parte configurarás tu entorno de desarrollo **y** le enseñarás a Copilot sobre el código — para que cada prompt futuro comience con el contexto adecuado.

## Sección 1: Configuración Inicial

### Paso 1: Crea Tu Repositorio

1. Abre [github.com/copilot-dev-days/mona-mayhem](https://github.com/copilot-dev-days/mona-mayhem)
2. Haz clic en **Use this template** → **Create a new repository**
3. Nómbralo `my-mona-mayhem` y establece la visibilidad en **Public**

### Paso 2: Habilita GitHub Pages

1. Ve a **Settings** → **Pages** de tu nuevo repositorio
2. En **Source**, selecciona **GitHub Actions**

### Paso 3: Clona y Abre en VS Code

1. Abre VS Code y ejecuta **Git: Clone** → **Clone from GitHub**
2. Selecciona tu repositorio `my-mona-mayhem`
3. Cuando se te solicite, instala las **extensiones recomendadas**

### Paso 4: Ejecuta el Agente de Configuración

1. Abre el panel de **Chat** y escribe:

   ```
   /setup
   ```

2. El agente detectará tu entorno, instalará las dependencias e iniciará el servidor de desarrollo automáticamente.

> ✅ **¡La aplicación está corriendo en tu navegador!**

## Sección 2: Ingeniería de Contexto

La ingeniería de contexto es cómo le enseñas a la IA sobre tu código. Cuanto mejor sea el contexto, mejor será cada respuesta futura.

### Tarea 1: Genera las Instrucciones del Workspace

1. Abre la Command Palette y ejecuta:

   ```
   Chat: Generate Workspace Instructions File
   ```

2. Revisa el archivo generado — probablemente sea demasiado detallado.
3. En Copilot Chat, continúa con:

   > "Compress down by half and add a mandatory development checklist (lint, build, test) to the top"

4. **Haz commit** del archivo de instrucciones.

> **Resultado:** Todas las solicitudes futuras de Copilot ahora tienen un mapa básico de tu workspace incorporado.

### Tarea 2: Agentes en Segundo Plano

**Agente local en segundo plano:**

1. En el panel de Chat, haz clic en **+** → **New background agent**
2. Ingresa el prompt:

   > "Add linting rules for unused vars and improve code style; fix any errors"

3. Cuando termine, **revisa y aplica** los cambios, luego elimina la sesión.

**Agente en la nube:**

1. Inicia otro agente en segundo plano con:

   > "Make the README more engaging as a landing page"

> **Resultado:** Reglas de linting agregadas, errores corregidos, README mejorado — todo sin salir de tu editor.

### Tarea 3: Explora el Proyecto

Abre **Copilot Chat** en **Ask mode** y prueba estos prompts:

- `"Explain the architecture of this project"`
- `"What does the API route do?"`
- `"How does the contribution graph rendering work?"`

> 💡 Usa **@workspace** para dar a Copilot contexto de todo el proyecto y obtener respuestas más precisas.

## ✅ Parte 1 Completa

Has aprendido a:

- **Configurar** un entorno de desarrollo con el agente `/setup`
- **Generar instrucciones de workspace** para que Copilot entienda tu proyecto
- **Usar agentes en segundo plano y en la nube** para automatizar tareas de mantenimiento
- **Explorar un código** usando Ask mode y `@workspace`
