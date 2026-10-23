# Liste des PNJ

Toute la distribution d'un coup d'œil. Chaque tableau est une requête Dataview sur les notes de PNJ.

## PNJ par lieu

```dataview
TABLE WITHOUT ID key AS "Lieu", rows.file.link AS "PNJ", rows.role AS "Rôle"
FROM "PNJ"
GROUP BY location
```

## Attitude envers le groupe

```dataview
TABLE WITHOUT ID file.link AS "PNJ", attitude AS "Attitude", status AS "Statut", first_met AS "Première rencontre"
FROM "PNJ"
SORT attitude ASC, first_met ASC
```

## Membres des factions

```dataview
TABLE WITHOUT ID key AS "Faction", length(rows) AS "Nombre", rows.file.link AS "PNJ"
FROM "PNJ"
WHERE faction
GROUP BY faction
```

## PNJ rapides prêts à improviser

```dataview
TABLE WITHOUT ID file.link AS "PNJ", role AS "Rôle", wants AS "Veut"
FROM "PNJ rapides"
```

## Secrets pas encore révélés

```dataview
LIST secret
FROM "PNJ"
WHERE revealed = false
```
