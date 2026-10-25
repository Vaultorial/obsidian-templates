---
type: index
---

# Cronograma

Cada nota de tarea de `Proyectos/` que tenga fecha en `start` aparece aquí, con un diagrama por proyecto y una sección por fase. Cambia una fecha en las propiedades de la tarea y la barra se mueve. Pon `status: hecha` o `en curso` para darle color, `critical: true` para pintarla en rojo y `milestone: true` para mostrarla como un rombo.

> [!note]
> Los diagramas necesitan Dataview con *JavaScript queries* activado. Obsidian los dibuja con Mermaid, y la primera vez puede preguntar si quieres mostrar diagramas Mermaid en este vault: elige permitirlo.

## Diagramas de Gantt por proyecto

```dataviewjs
const STATUS = { "hecha": "done", "en curso": "active" };
const clean = (s) => String(s).replace(/[:#;]/g, " ");
const tasks = dv.pages('"Proyectos"').where((t) => t.type === "tarea" && t.start);
for (const project of tasks.groupBy((t) => t.project)) {
  const lines = ["gantt", "  title " + clean(project.key), "  dateFormat YYYY-MM-DD", "  axisFormat %d/%m"];
  for (const phase of dv.array(project.rows).groupBy((t) => t.phase)) {
    lines.push("  section " + clean(phase.key));
    for (const t of phase.rows.sort((t) => t.start)) {
      const tags = [STATUS[t.status], t.critical ? "crit" : null, t.milestone ? "milestone" : null].filter(Boolean);
      const start = t.start.toFormat("yyyy-MM-dd");
      const end = t.milestone || !t.end ? "0d" : t.end.toFormat("yyyy-MM-dd");
      lines.push("    " + clean(t.file.name) + " :" + tags.map((x) => x + ", ").join("") + start + ", " + end);
    }
  }
  dv.paragraph("```mermaid\n" + lines.join("\n") + "\n```");
}
```

## Tareas que aún no están en el cronograma

Las tareas sin fecha de inicio se quedan fuera de los diagramas. Esperan aquí hasta que las programes.

```dataview
TABLE WITHOUT ID file.link AS "Tarea", project AS "Proyecto", phase AS "Fase", status AS "Estado"
FROM "Proyectos"
WHERE type = "tarea" AND !start
SORT project ASC
```
