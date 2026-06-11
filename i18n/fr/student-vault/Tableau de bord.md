---
type: dashboard
tags: [dashboard]
---

# Tableau de bord

Construit par Dataview à partir du frontmatter de chaque note. Tout ce qui a une date `due` apparaît ci-dessous automatiquement — rien ici n'est maintenu à la main.

## Échéances à venir

```dataview
TABLE course AS "Matière", type AS "Type", due AS "Échéance"
FROM "Printemps 2026"
WHERE due AND due >= date(today)
SORT due ASC
```

## Examens

```dataview
TABLE course AS "Matière", topic AS "Sujet", due AS "Date"
FROM "Printemps 2026"
WHERE type = "exam"
SORT due ASC
```

## Lectures à faire

```dataview
TABLE course AS "Matière", source AS "Source", due AS "Échéance"
FROM "Printemps 2026"
WHERE type = "reading"
SORT due ASC
```

## Tout par matière

```dataview
TABLE type AS "Type", topic AS "Sujet", due AS "Échéance"
FROM "Printemps 2026"
SORT course ASC, due ASC
```

> [!note] Tableaux vides ?
> Dataview n'est pas encore activé — voir [[Commencez ici]] pour la configuration. Les éléments en retard disparaissent d'eux-mêmes du tableau des échéances ; le tableau par matière en bas continue de tout montrer.
