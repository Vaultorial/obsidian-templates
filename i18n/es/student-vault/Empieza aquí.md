# Empieza aquí

Bienvenido. Este es un vault de estudiante en funcionamiento para un cuatrimestre: dos asignaturas, apuntes de clase reales, preparación de exámenes y lecturas ya colocados, más un [[Panel]] que reúne cada fecha de entrega y cada examen en una sola vista automáticamente.

## Cómo se organiza

- **Por cuatrimestre y asignatura:** `Primavera 2026/Biología 101/` y `Primavera 2026/Estadística 201/`. Añade una carpeta por asignatura cada cuatrimestre nuevo — la estructura escala copiándola.
- **Tres tipos de nota por asignatura**, cada uno desde una plantilla: apuntes de clase, preparación de examen y apuntes de lectura.
- **[[Panel]]** lee los campos `due` y `type` del frontmatter de cada nota y lista lo que viene. Lo construye Dataview — cambia una fecha de entrega en una nota y el panel se actualiza solo.

Las notas de ejemplo están deliberadamente llenas de material correcto y general (biología celular, estadística descriptiva) para que veas la estructura sobre contenido real antes de sustituirlo por el tuyo.

## Primeros pasos

1. Instala y activa **Dataview** (obligatorio para el [[Panel]]): Ajustes → Complementos comunitarios → Buscar → "Dataview".
2. Abre el [[Panel]] y confirma que se renderizan las tablas de entregas y exámenes.
3. Crea una carpeta de asignatura para una de tus asignaturas reales dentro de `Primavera 2026/` (o una carpeta de cuatrimestre nueva).
4. Toma tu próxima clase en una copia de `Plantillas/Apunte de clase.md` (plugin core Templates, ya configurado). Pon una fecha `due` en cualquier cosa con plazo y aparecerá en el panel.
5. Opcional: instala **Calendar** para una vista de mes que acompañe a tus notas diarias.

## Los tipos de nota

- **Apunte de clase** — fecha, tema y un sitio limpio para el material del día más preguntas a repasar luego.
- **Preparación de examen** — `type: exam` y una fecha `due` para que aflore en el panel; una lista de control de temas que machacar.
- **Apunte de lectura** — fuente, la fecha `due` de la tarea y tu propio resumen de lo que leíste.

## Plugins

- **Obligatorios:** Dataview — el panel lo necesita.
- **Opcionales:** Calendar — vista de mes para notas diarias.
- El core **Templates** ya está activado y apuntando a `Plantillas`.

> [!tip] Un hábito hace que este vault valga la pena
> Pon una fecha `due` en el frontmatter en el momento en que se anuncie un plazo. El panel solo puede mostrar lo que le digas — pero si se lo dices, nunca más llevas los plazos de memoria.
