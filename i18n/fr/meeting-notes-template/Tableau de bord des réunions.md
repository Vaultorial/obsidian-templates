---
type: dashboard
---

# Tableau de bord des réunions

Ouvrez en mode lecture avec Dataview activé. Tout ce qui suit est généré à partir du frontmatter et des cases des notes dans `Réunions/`.

## Réunions récentes

```dataview
TABLE type, project, attendees
FROM "Réunions"
SORT date DESC
LIMIT 15
```

## Par type

```dataview
TABLE rows.file.link AS "Réunions", rows.date AS "Date"
FROM "Réunions"
GROUP BY type
```

## Par projet

```dataview
TABLE rows.file.link AS "Réunions", rows.type AS "Type"
FROM "Réunions"
GROUP BY project
```

## Actions ouvertes

Chaque action non cochée à travers toutes les réunions, groupée par la réunion dont elle vient. Cochez-les là où elles vivent.

```dataview
TASK
FROM "Réunions"
WHERE !completed
```

## Journal des décisions

Liste de saut rapide — les décisions vivent sous le titre `## Décisions` de chaque note.

```dataview
LIST
FROM "Réunions"
SORT date ASC
```
