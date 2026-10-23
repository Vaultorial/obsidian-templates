# Empieza aquí

Bienvenido. Este vault es un sistema ligero de gestión de proyectos para Obsidian: una nota por proyecto, una nota por reunión y un panel Dataview que lee todo lo demás. Dos proyectos de ejemplo completos — un rediseño de web y una mudanza de oficina — vienen precargados con hitos, líneas de tiempo Mermaid y notas de reunión enlazadas, para que cada query del panel tenga datos reales detrás.

## Cómo se organiza el vault

- `Proyectos/` — una nota por proyecto. El frontmatter lleva los campos que lee el panel (`status`, `owner`, `start`, `due`, `area`); el cuerpo contiene objetivos, una tabla de hitos, una línea de tiempo Gantt y enlaces a las reuniones de ese proyecto.
- `Reuniones/` — una nota por reunión, con el nombre `YYYY-MM-DD Proyecto Tema`. Cada una enlaza de vuelta a su proyecto en el frontmatter, para que el panel pueda agregar los elementos de acción abiertos por proyecto.
- [[Panel]] — tablas en vivo: proyectos activos, proyectos por estado y por responsable, próximos vencimientos, reuniones recientes y todos los elementos de acción sin marcar de todas las notas de reunión.
- `Plantillas/` — [[Plantilla de proyecto]] y [[Plantilla de reunión]], conectadas al plugin core Templates.

## Convenciones que hacen funcionar el panel

- `status` es uno de: `planificación`, `activo`, `en pausa`, `hecho`. En minúsculas, exacto — Dataview compara cadenas literalmente.
- `owner` es un nombre, escrito igual en todas partes ("Sarah Chen", no "S. Chen" en un fichero y "sarah" en otro).
- Las fechas son `YYYY-MM-DD`. Dataview las interpreta como fechas reales, que es lo que hace posible la query de "próximos vencimientos".
- Los elementos de acción en las notas de reunión son casillas `- [ ]` simples. Márcalas donde viven; el panel lo refleja.

## Plugins a activar

1. **Dataview** (obligatorio) — Ajustes → Complementos comunitarios → Buscar → "Dataview". El panel se construye sobre él.

Las líneas de tiempo Mermaid se renderizan con el soporte Mermaid integrado de Obsidian — sin plugin. El plugin core **Templates** ya está activado y apuntando a `Plantillas/`.

## Primeros pasos

1. Activa Dataview y abre el [[Panel]] en vista de lectura. Cada tabla debería poblarse.
2. Abre [[Rediseño de la web]] y léelo de arriba abajo — frontmatter, hitos, línea de tiempo, reuniones. Esa nota es el patrón.
3. Crea tu primer proyecto real: nota nueva en `Proyectos/`, inserta [[Plantilla de proyecto]] (paleta de comandos → "Templates: Insertar plantilla"), rellena el frontmatter.
4. Tras tu próxima reunión, crea una nota en `Reuniones/` desde [[Plantilla de reunión]] y enlázala al proyecto.
5. Borra los dos proyectos de ejemplo y sus reuniones cuando tengas los tuyos.
