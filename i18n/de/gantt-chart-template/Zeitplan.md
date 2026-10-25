---
type: index
---

# Zeitplan

Jede Aufgabennotiz in `Projekte/` mit einem Datum in `start` erscheint hier, ein Diagramm pro Projekt und ein Abschnitt pro Phase. Ändere ein Datum in den Eigenschaften der Aufgabe, und der Balken verschiebt sich. Mit `status: erledigt` oder `in Arbeit` wird er eingefärbt, mit `critical: true` rot gezeichnet und mit `milestone: true` als Raute dargestellt.

> [!note]
> Die Diagramme brauchen Dataview mit eingeschalteten *JavaScript queries*. Obsidian zeichnet sie mit Mermaid und fragt beim ersten Mal eventuell, ob Mermaid-Diagramme in diesem Vault angezeigt werden sollen: erlaube es.

## Gantt-Diagramme nach Projekt

```dataviewjs
const STATUS = { "erledigt": "done", "in Arbeit": "active" };
const clean = (s) => String(s).replace(/[:#;]/g, " ");
const tasks = dv.pages('"Projekte"').where((t) => t.type === "aufgabe" && t.start);
for (const project of tasks.groupBy((t) => t.project)) {
  const lines = ["gantt", "  title " + clean(project.key), "  dateFormat YYYY-MM-DD", "  axisFormat %d.%m."];
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

## Aufgaben, die noch nicht im Zeitplan stehen

Aufgaben ohne Startdatum bleiben aus den Diagrammen draußen. Sie warten hier, bis du sie einplanst.

```dataview
TABLE WITHOUT ID file.link AS "Aufgabe", project AS "Projekt", phase AS "Phase", status AS "Status"
FROM "Projekte"
WHERE type = "aufgabe" AND !start
SORT project ASC
```
