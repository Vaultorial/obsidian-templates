---
type: index
---

# Calendrier

Chaque note de tâche de `Projets/` qui a une date `start` apparaît ici, avec un diagramme par projet et une section par phase. Changez une date dans les propriétés de la tâche et la barre se déplace. Indiquez `status: terminée` ou `en cours` pour la colorer, `critical: true` pour la dessiner en rouge et `milestone: true` pour l'afficher en losange.

> [!note]
> Les diagrammes nécessitent Dataview avec *JavaScript queries* activé. Obsidian les dessine avec Mermaid et, la première fois, peut demander s'il faut afficher les diagrammes Mermaid dans ce vault : autorisez-le.

## Diagrammes de Gantt par projet

```dataviewjs
const STATUS = { "terminée": "done", "en cours": "active" };
const clean = (s) => String(s).replace(/[:#;]/g, " ");
const tasks = dv.pages('"Projets"').where((t) => t.type === "tâche" && t.start);
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

## Tâches pas encore planifiées

Les tâches sans date de début restent hors des diagrammes. Elles attendent ici que vous les planifiiez.

```dataview
TABLE WITHOUT ID file.link AS "Tâche", project AS "Projet", phase AS "Phase", status AS "Statut"
FROM "Projets"
WHERE type = "tâche" AND !start
SORT project ASC
```
