# Empieza aquí

Bienvenido. Este vault es un diario construido sobre el **registro rápido del bullet journal**: líneas cortas con un símbolo delante en vez de redacciones, una sección mínima de gratitud por día y una reflexión mensual que cose los días entre sí. Trae dos semanas reales de entradas (del 25 de mayo al 7 de junio de 2026) y la reflexión de mayo terminada, para que notes el ritmo antes de escribir una sola palabra.

## La clave del registro rápido

Una línea por elemento, con el símbolo primero:

•  tarea por hacer
×  tarea hecha
○  evento (ocurrió, no pide acción)
–  nota, observación, idea suelta
\> tarea migrada a otro día

> [!important] La única peculiaridad de Obsidian
> Escribe el símbolo de migración como `\>` (barra invertida + ángulo). Un `>` a secas al inicio de línea se convierte en bloque de cita en Obsidian; la barra lo deja como un `>` normal en la vista de lectura. Apunta cada migración a un día: `\> Arreglar la tapa → [[2026-06-06]]`, y vuelve a anotar la tarea como `•` en ese día. Los ejemplos lo muestran dos veces — sigue el rastro de una fuente de horno por [[2026-05-25]] → [[2026-05-26]].

## Cómo está organizado el vault

- `Diario/2026/05/` y `Diario/2026/06/` — entradas con nombre `YYYY-MM-DD`, una carpeta por mes, más la reflexión mensual (`2026-05 Reflexión`).
- `Plantillas/` — plantillas de entrada en tres sabores (bullet journal, diario en prosa y Templater con enlaces al día anterior/siguiente) y una plantilla de `Reflexión mensual`.

El plugin core **Daily notes** ya está configurado para crear la entrada de hoy en la carpeta del mes que toca (formato `YYYY/MM/YYYY-MM-DD`), rellenada desde la plantilla de bullet journal.

## Primeros pasos

1. Lee en orden las dos semanas de ejemplo, empezando por [[2026-05-25]]. Fíjate en lo cortas que son las líneas — esa brevedad es lo que mantiene vivo un diario en los días de cansancio.
2. Lee [[2026-05 Reflexión]] para ver *para qué* sirven las entradas diarias.
3. Pulsa el icono de calendario de la barra lateral: aparece la entrada de hoy, con la clave incluida. Anota tres líneas y una gratitud. Listo.
4. El último día del mes, crea `2026-06 Reflexión` en `Diario/2026/06/` a partir de la plantilla `Reflexión mensual`.

## Plugins

Ninguno obligatorio. Opcional:

- **Templater** — alimenta la variante `Entrada de diario (Templater)`, con enlaces automáticos a ayer y mañana. Instálalo, define `Plantillas` como su carpeta de plantillas y cambia el ajuste de plantilla de Daily notes a esa variante.

> [!tip] Baja el listón
> Una entrada de dos líneas es un hábito conservado; un día en blanco también vale — eso sí, no rellenes ficción a posteriori. Los ejemplos incluyen líneas mundanas a propósito: la magia está en releer un mes entero de ellas.
