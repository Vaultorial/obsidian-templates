# Empieza aquí

Bienvenido. Este vault hace una sola cosa: una única nota semanal que reúne tu **plan de la semana** y tu **revisión de la misma**. Planificas el lunes, revisas el viernes o el domingo, todo en el mismo fichero. Cuatro semanas de ejemplo rellenas muestran qué aspecto tiene cuando un mes real pasa por el sistema.

## Cómo está organizado el vault

- `Semanal/` — una nota por semana ISO, con nombres `2026-W19`, `2026-W20` y así sucesivamente. Los cuatro ejemplos cubren mayo de 2026 y se leen como una historia continua: fíjate en cómo lo no terminado se arrastra desde el **Queda pendiente** de una semana hasta el plan de la siguiente. Ese bucle es todo el método.
- `Plantillas/` — dos versiones de la plantilla semanal:
	- **Nota semanal (core Templates)** — sin plugins.
	- **Nota semanal (Templater)** — añade el rango de fechas de la semana y los enlaces a la anterior/siguiente, calculados a partir del nombre del fichero.

## Primeros pasos

1. Lee `2026-W19` a `2026-W22` en orden. Cinco minutos, y sabrás exactamente cómo llevar el sistema.
2. Crea tu semana en curso: nota nueva en `Semanal/` con el número ISO de esta semana (p. ej. `2026-W24`) e inserta la plantilla con **Insertar plantilla** desde la paleta de comandos.
3. El lunes rellena el **Foco** y de 3 a 5 tareas del plan. Durante la semana, no toques nada. Al acabar la semana, rellena la revisión de una sentada.
4. Todo lo no terminado va a **Queda pendiente** — y debe aparecer en el plan de la semana siguiente o descartarse a conciencia. Lo que se arrastra tres semanas seguidas te está diciendo algo.

## Plugins

De serie, solo plugins core. Dos mejoras opcionales:

- **Periodic Notes** — añade un comando para abrir la nota de la semana en curso y navegación de semanas estilo calendario. Tras instalarlo, define el formato semanal `GGGG-[W]WW` y la carpeta `Semanal`.
- **Templater** — necesario para la variante `Nota semanal (Templater)`. Define `Plantillas` como su carpeta de plantillas.

> [!tip] Mantén la revisión honesta
> La sección **Números** solo registra cosas que de verdad cuentas (entrenamientos, sesiones de estudio, páginas). Con dos o tres métricas sobra — en cuanto apuntar se sienta como contabilidad, elimina una.
