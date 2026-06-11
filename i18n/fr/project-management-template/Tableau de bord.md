---
type: dashboard
---

# Tableau de bord

Ouvrez en mode lecture avec Dataview activé. Chaque tableau ci-dessous est généré à partir du frontmatter des notes dans `Projets/` et `Réunions/` — rien sur cette page n'est maintenu à la main.

## Projets actifs

```dataview
TABLE owner, area, start, due
FROM "Projets"
WHERE status = "actif"
SORT due ASC
```

## Tous les projets par statut

```dataview
TABLE rows.file.link AS "Projets", rows.owner AS "Responsable"
FROM "Projets"
GROUP BY status
```

## Projets par responsable

```dataview
TABLE rows.file.link AS "Projets", rows.due AS "Échéance"
FROM "Projets"
GROUP BY owner
```

## Dus dans les 30 prochains jours

```dataview
TABLE owner, status, due
FROM "Projets"
WHERE status != "terminé" AND due <= date(today) + dur(30 days)
SORT due ASC
```

## Réunions récentes

```dataview
TABLE project, date
FROM "Réunions"
SORT date DESC
LIMIT 10
```

## Actions ouvertes issues des réunions

Chaque case non cochée à travers toutes les notes de réunion. Cochez-les dans la note de réunion où elles vivent.

```dataview
TASK
FROM "Réunions"
WHERE !completed
```
