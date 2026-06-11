---
type: tableau de bord
---

# Écran du MJ

À ouvrir en mode lecture avec Dataview activé. Tout ce qui suit se met à jour tout seul depuis le frontmatter des notes de la campagne.

## Où en est la campagne

- Dernière séance jouée : [[Séance 3 - Du sel sur la plaie]]
- Préparé et prêt : [[Cambriolage du Comptoir]]
- Le groupe : [[Kestrel Thorne]], [[Bram Tuckett]], [[Yneva Marsh]]
- Colonne vertébrale de l'intrigue : [[La Route du Sel]] · [[La Compagnie Carrow]] · [[Les Gardiens de la Saumure]]

## PNJ par lieu

```dataview
TABLE rows.file.link AS "PNJ", rows.role AS "Rôle", rows.status AS "État"
FROM "PNJ"
GROUP BY location
```

## PNJ par faction

```dataview
TABLE rows.file.link AS "PNJ", rows.role AS "Rôle"
FROM "PNJ"
GROUP BY faction
```

## Séances, la plus récente d'abord

```dataview
TABLE date AS "Date", number AS "N°"
FROM "Séances"
SORT date DESC
```

## Rencontres prêtes à jouer

```dataview
TABLE location AS "Lieu", difficulty AS "Difficulté"
FROM "Rencontres"
WHERE status = "prêt"
```

## Rencontres déjà jouées

```dataview
TABLE location AS "Lieu", difficulty AS "Difficulté"
FROM "Rencontres"
WHERE status = "joué"
SORT file.name ASC
```

## Le groupe

```dataview
TABLE player AS "Joueur", class AS "Classe", level AS "Niveau", ancestry AS "Origine"
FROM "PJ"
SORT file.name ASC
```
