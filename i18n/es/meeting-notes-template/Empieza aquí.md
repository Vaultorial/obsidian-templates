# Empieza aquí

Bienvenido. Este vault es un sistema de notas de reunión para Obsidian: cinco plantillas listas (reunión de equipo, 1-on-1, llamada con cliente, daily standup, retrospectiva), un panel Dataview que encuentra cada reunión y cada elemento de acción sin terminar, y seis reuniones de ejemplo rellenadas de un mismo proyecto coherente, para que veas el sistema funcionando antes de adoptarlo.

## Cómo se organiza el vault

- `Plantillas/` — el producto. [[Reunión de equipo]], [[1-on-1]], [[Llamada con cliente]], [[Daily standup]] y [[Retrospectiva]], cada una con frontmatter estructurado (`type`, `date`, `project`, `attendees`) y las mismas cuatro secciones: agenda, notas, decisiones, elementos de acción.
- `Reuniones/` — una nota por reunión, con el nombre `YYYY-MM-DD Tema`. Los ejemplos siguen un proyecto de consultoría (la construcción de un portal de cliente para una aseguradora) a través de un arranque, un 1-on-1, una llamada con cliente y una revisión de sprint.
- [[Panel de reuniones]] — rollups Dataview: reuniones recientes, reuniones por tipo, por proyecto y todos los elementos de acción abiertos en un solo sitio.

## Convenciones que hacen funcionar el panel

- `type` es uno de: `reunion-equipo`, `one-on-one`, `llamada-cliente`. En minúsculas, con guion, exacto.
- `project` es una etiqueta breve de texto plano ("Portal de cliente"). Usa la misma ortografía en todas las reuniones — el panel agrupa por ella.
- Los elementos de acción se escriben en formato del plugin Tasks: `- [ ] Responsable — qué hará 📅 2026-06-15`. Este vault solo necesita la parte de la casilla (Dataview la lee), pero la sintaxis de fecha significa que puedes soltar estas líneas en un vault GTD con el plugin Tasks — como nuestro Vault de tareas GTD — y se recogerán como tareas programadas sin cambios.
- Las decisiones tienen su propia sección. Seis meses después, nadie relee las notas; buscan qué se decidió.

## Plugins a activar

1. **Dataview** (obligatorio) — Ajustes → Complementos comunitarios → Buscar → "Dataview". Da vida al panel.
2. **Templater** (opcional) — si ya usas Templater, apúntalo a `Plantillas/` y cambia las variables `{{date}}` y `{{title}}` por tus comandos dinámicos preferidos. Las plantillas vienen en sintaxis del core Templates para que funcionen de inmediato.

El plugin core **Templates** ya está activado y apuntando a `Plantillas/`.

## Primeros pasos

1. Activa Dataview y abre el [[Panel de reuniones]] en vista de lectura — cada sección debería poblarse con las cuatro reuniones de ejemplo.
2. Abre [[2026-05-04 Arranque del portal de cliente]] para ver una nota rellenada junto a su plantilla.
3. Antes de tu próxima reunión: crea una nota en `Reuniones/` con el nombre de la fecha y el tema, inserta la plantilla correspondiente (paleta de comandos → "Templates: Insertar plantilla") y rellena el frontmatter.
4. Durante la reunión, escribe solo en notas/decisiones/elementos de acción. Después, dedica un minuto a asignar responsables y fechas a los elementos de acción.
5. Borra las reuniones de ejemplo cuando tengas algunas propias.
