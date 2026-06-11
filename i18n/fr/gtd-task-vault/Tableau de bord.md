---
type: dashboard
---

# Tableau de bord

Ouvrez cette note en mode lecture. Chaque section est une requête en direct sur tout le vault — les tâches restent dans leurs notes de projet et leurs listes, et surgissent ici automatiquement. Les vues reflètent le jour où vous ouvrez le vault.

## À échéance aujourd'hui

```tasks
not done
due today
tags do not include #attente
```

## En retard

```tasks
not done
due before today
tags do not include #attente
sort by due
```

## À venir

Les dix prochaines tâches datées, la plus proche d'abord.

```tasks
not done
due after today
tags do not include #attente
sort by due
limit 10
```

## Par contexte

### Maison

```tasks
not done
tags include #contexte/maison
sort by priority
```

### Ordinateur

```tasks
not done
tags include #contexte/ordinateur
sort by priority
```

### Courses

```tasks
not done
tags include #contexte/courses
sort by priority
```

## En attente

```tasks
not done
tags include #attente
sort by due
```

## Boîte à traiter

Visez zéro. Traitez-la pendant la revue hebdomadaire.

```tasks
not done
path includes 00 Boîte de réception
```

## Vue d'ensemble des projets

> [!note] Nécessite Dataview
> Ce tableau a besoin du plugin Dataview. Tout ce qui précède tourne avec Tasks seul.

```dataview
TABLE status, area, outcome
FROM "Projets"
SORT status ASC, file.name ASC
```
