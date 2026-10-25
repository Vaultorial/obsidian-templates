---
type: index
---

# Hoja del grupo

Una página para la mesa: quién forma el grupo, cuánto daño lleva cada uno y a quién pedir una tirada. Cada número sale de las propiedades de las notas de personaje.

## El grupo de un vistazo

```dataview
TABLE WITHOUT ID file.link AS "Personaje", class AS "Clase", level AS "Nivel", ac AS "CA", hp + " / " + max_hp AS "PG", 10 + floor((wis - 10) / 2) + choice(contains(skills, "Percepción"), floor((level - 1) / 4) + 2, 0) AS "Percepción pasiva"
FROM "Personajes"
SORT file.name ASC
```

## Quién necesita curación

```dataview
TABLE WITHOUT ID file.link AS "Personaje", hp AS "PG actuales", max_hp - hp AS "Faltan"
FROM "Personajes"
WHERE hp < max_hp
SORT (max_hp - hp) DESC
```

## Quién es bueno en qué

Habilidades con competencia y pericia de cada personaje, para cuando el DM pregunta quién quiere intentarlo.

```dataview
TABLE WITHOUT ID file.link AS "Personaje", skills AS "Habilidades con competencia", expertise AS "Pericia"
FROM "Personajes"
SORT file.name ASC
```
