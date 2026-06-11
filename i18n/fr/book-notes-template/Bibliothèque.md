---
type: bookshelf
tags: [bookshelf]
---

# Bibliothèque

Assemblée par Dataview à partir du frontmatter de chaque note dans `Livres/`. Rien sur cette page n'est maintenu à la main.

**Mon échelle de notation :** 5 = je relirai et imposerai aux amis · 4 = a changé quelque chose que je fais · 3 = bon, une idée valait le temps · 2 = correct, oubliable · 1 = abandonné à raison.

## En cours de lecture

```dataview
TABLE author AS "Auteur", genre AS "Genre", row["date-started"] AS "Commencé"
FROM "Livres"
WHERE status = "en cours"
```

## Lus — par note

```dataview
TABLE author AS "Auteur", rating AS "Note", row["date-finished"] AS "Terminé"
FROM "Livres"
WHERE status = "terminé"
SORT rating DESC
```

## À lire

```dataview
LIST author
FROM "Livres"
WHERE status = "à lire"
```

## Tout, par auteur

```dataview
TABLE author AS "Auteur", status AS "Statut", rating AS "Note"
FROM "Livres"
SORT author ASC
```

> [!note] Si les étagères sont vides
> Dataview n'est pas encore activé — voir [[Commencez ici]] pour la configuration d'une minute.
