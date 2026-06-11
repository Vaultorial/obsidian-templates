---
type: tableau-de-bord
---

# Accueil

> [!info] Aller à
> **Projets :** [[Potager de balcon pour l'été|Potager de balcon]] · [[Refonte du site portfolio|Portfolio]] · [[Cours de conversation en espagnol|Espagnol]]
> **Domaines :** [[Santé et forme]] · [[Entretien du logement]]
> **Pérennes :** [[Liste de lecture]] · [[Checklist du reset hebdomadaire]] · [[Sauce tomate qui marche]]
> Nouveau ici ? Lisez d'abord [[Commencez ici]] — ou ouvrez [[Accueil (simple)]], la version sans plugin de cette page.

## Aujourd'hui

Les tâches ouvertes dues aujourd'hui ou déjà en retard, tirées de tous les projets et domaines.

```dataview
TASK
FROM "Projets" OR "Domaines"
WHERE !completed AND due AND due <= date(today)
SORT due ASC
```

## À venir (7 prochains jours)

```dataview
TASK
FROM "Projets" OR "Domaines"
WHERE !completed AND due AND due > date(today) AND due <= date(today) + dur(7 days)
SORT due ASC
```

## Projets actifs

```dataview
TABLE WITHOUT ID file.link AS "Projet", status AS "Statut", started AS "Début"
FROM "Projets"
WHERE status = "actif"
SORT started ASC
```

## Touché récemment

```dataview
TABLE WITHOUT ID file.link AS "Note", dateformat(file.mtime, "ccc d MMM, HH:mm") AS "Dernière modification"
FROM "Projets" OR "Domaines" OR "Notes"
SORT file.mtime DESC
LIMIT 7
```

## Le vault en un coup d'œil

```dataview
TABLE WITHOUT ID Dossier AS "Dossier", length(rows) AS "Notes"
FROM "Projets" OR "Domaines" OR "Notes"
GROUP BY file.folder AS Dossier
SORT Dossier ASC
```

> [!tip] Pourquoi les tâches portent `[due:: date]`
> Ce champ inline est ce qui permet aux requêtes ci-dessus de balayer tous les projets et domaines pour vous. Datez une tâche et oubliez-la — cette page s'en souvient. La routine du dimanche de la [[Checklist du reset hebdomadaire]] garde les données honnêtes.
