---
type: index
---

# Timeline

Every task note in `Projects/` with a `start` date appears here, one chart per project and one section per phase. Change a date in a task's properties and the bar moves. Mark a task `status: done` or `active` to colour it, `critical: true` to draw it in red, and `milestone: true` to show it as a diamond.

> [!note]
> The charts need Dataview with *JavaScript queries* switched on. Obsidian draws them with Mermaid, and the first time it may ask "Display Mermaid diagrams in this vault?": choose Allow.

## Gantt charts by project

```dataviewjs
const STATUS = { "done": "done", "active": "active" };
const clean = (s) => String(s).replace(/[:#;]/g, " ");
const tasks = dv.pages('"Projects"').where((t) => t.type === "task" && t.start);
for (const project of tasks.groupBy((t) => t.project)) {
  const lines = ["gantt", "  title " + clean(project.key), "  dateFormat YYYY-MM-DD", "  axisFormat %d %b"];
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

## Tasks not on the timeline yet

Tasks without a start date are left out of the charts. They wait here until you schedule them.

```dataview
TABLE WITHOUT ID file.link AS "Task", project AS "Project", phase AS "Phase", status AS "Status"
FROM "Projects"
WHERE type = "task" AND !start
SORT project ASC
```
