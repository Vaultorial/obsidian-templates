# Empieza aquí

Bienvenido. Este vault es un sistema de notas diarias con cuatro secciones fijas — Agenda, Tareas, Registro y Gratitud — que puedes rellenar en menos de dos minutos o expandir hasta un diario completo. No hay nada más que configurar.

## Cómo está organizado el vault

- `Diario/` — una nota por día, con nombre `YYYY-MM-DD`. Dentro hay una semana de ejemplo completa (del 1 al 7 de junio de 2026) para que veas cómo se comportan las secciones con vida real dentro.
- `Plantillas/` — dos versiones de la misma plantilla diaria:
	- **Nota diaria (core Templates)** — funciona tal cual, sin plugins.
	- **Nota diaria (Templater)** — el mismo diseño más enlaces automáticos a ayer y mañana. Necesita el plugin Templater.

El plugin core **Daily notes** ya viene configurado: las notas diarias nuevas se crean en `Diario/`, con la fecha como nombre y rellenadas desde la plantilla core.

## Primeros pasos

1. Pulsa el **icono de calendario** en la barra lateral izquierda (o ejecuta `Abrir la nota diaria de hoy` desde la paleta de comandos). La nota de hoy se crea sola.
2. Antes de cerrar el día, escribe la tarea principal de mañana en **Tareas** y una línea en **Registro**. Ese hábito, por sí solo, ya justifica el vault.
3. Hojea la semana de ejemplo en `Diario/` y bórrala cuando ya no necesites la referencia.
4. Abre dos notas de ejemplo en paralelo para ver cómo los enlaces `← ant. | sig. →` conectan los días.

## Plugins

De serie, este vault solo usa plugins core (ya activados). Mejora opcional:

- **Templater** — instálalo y actívalo, define `Plantillas` como su carpeta de plantillas en los ajustes del plugin, y apunta Daily notes (Ajustes → Notas diarias → Plantilla) a `Nota diaria (Templater)`. A partir de ahí, cada nota diaria nueva trae la navegación anterior/siguiente funcionando sola.

> [!tip] Conserva las secciones, cambia las preguntas
> Los cuatro encabezados son deliberadamente sosos para que sobrevivan a los días con prisa. Si lo de Gratitud no va contigo, renómbralo a "Una cosa buena" en la plantilla — pero mantén una sección de cierre. Las notas diarias mueren cuando se quedan en una simple lista de tareas.
