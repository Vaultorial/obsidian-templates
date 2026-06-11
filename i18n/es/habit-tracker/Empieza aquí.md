# Empieza aquí

Bienvenido. Este vault registra hábitos de dos maneras — elige la que case con tu paciencia, o lleva las dos como hacen los ejemplos.

- **La manera simple:** una nota por mes con una cuadrícula — días hacia abajo, hábitos en horizontal, `✓` o `·` en cada celda. Sin plugins, perfectamente usable en días de cerebro de papel.
- **La manera avanzada:** una nota minúscula por día con los hábitos como frontmatter de verdadero/falso, y un [[Panel de hábitos]] que calcula rachas, totales mensuales y días perfectos con Dataview.

Se incluyen dos meses completamente registrados (abril y mayo de 2026, cinco hábitos cotidianos: leer 20 min, caminar 30 min, sin azúcar, acostarse antes de las 23:30, diario). Los datos son imperfectos a propósito — una semana de sobrecarga, bajones de fin de semana, la mella de un festivo — porque así es el registro real, y las dos vistas cuentan la misma historia.

## Cómo está organizado el vault

- `Hábitos/2026-04 Hábitos.md`, `Hábitos/2026-05 Hábitos.md` — las cuadrículas mensuales, con totales al pie.
- `Hábitos/Registro diario/` — 61 notas de registro por día que alimentan el panel.
- `Hábitos/Panel de hábitos.md` — rachas, totales mes a mes, últimos 14 días, días perfectos.
- `Plantillas/` — `Cuadrícula mensual de hábitos` (cuadrícula en blanco) y `Entrada de registro diario` (registro diario).

## Primeros pasos

1. Abre [[2026-05 Hábitos]] y lee la cuadrícula como si fuera un gráfico: el patrón de los fines de semana y el bache de mitad de mes se ven sin una sola consulta.
2. Instala **Dataview** (ver README) y abre el [[Panel de hábitos]] para ver los mismos datos convertidos en rachas y totales. Para el bloque de rachas, activa las *consultas JavaScript* en los ajustes de Dataview.
3. Crea `2026-06 Hábitos` en `Hábitos/` e inserta la plantilla `Cuadrícula mensual de hábitos`. Renombra las columnas con **tus** cinco hábitos — cinco como máximo.
4. Esta noche, registra el día uno con la plantilla `Entrada de registro diario`. El ritual completo lleva menos de un minuto.
5. Borra los ejemplos de abril/mayo cuando ya hayas aprendido de ellos (borra las notas mensuales y `Registro diario` — el panel pasará a mostrar solo tus datos).

## Plugins

- **Dataview** — necesario solo para el [[Panel de hábitos]]. Las cuadrículas mensuales funcionan sin ningún plugin.

> [!tip] Registra lo cumplido, no el hueco
> Los días fallados reciben un discreto `·`, no una marca roja, y una racha rota simplemente estrena otra. El trabajo de la cuadrícula es la honestidad, no la culpa — esa diferencia es lo que te mantiene registrando en la tercera semana.
