---
type: index
---

# Feuille du groupe

Une page pour la table : qui compose le groupe, l'état de santé de chacun et à qui demander un test. Chaque chiffre vient des propriétés des notes de personnage.

## Le groupe en un coup d'œil

```dataview
TABLE WITHOUT ID file.link AS "Personnage", class AS "Classe", level AS "Niveau", ac AS "CA", hp + " / " + max_hp AS "PV", 10 + floor((wis - 10) / 2) + choice(contains(skills, "Perception"), floor((level - 1) / 4) + 2, 0) AS "Perception passive"
FROM "Personnages"
SORT file.name ASC
```

## Qui a besoin de soins

```dataview
TABLE WITHOUT ID file.link AS "Personnage", hp AS "PV actuels", max_hp - hp AS "Manquants"
FROM "Personnages"
WHERE hp < max_hp
SORT (max_hp - hp) DESC
```

## Qui est doué pour quoi

Compétences maîtrisées et expertise de chaque personnage, pour le moment où le MJ demande qui veut tenter sa chance.

```dataview
TABLE WITHOUT ID file.link AS "Personnage", skills AS "Compétences maîtrisées", expertise AS "Expertise"
FROM "Personnages"
SORT file.name ASC
```
