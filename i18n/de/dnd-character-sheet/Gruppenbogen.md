---
type: index
---

# Gruppenbogen

Eine Seite für den Spieltisch: wer zur Gruppe gehört, wie angeschlagen alle sind und wen man für eine Probe fragt. Jede Zahl kommt aus den Eigenschaften der Charakternotizen.

## Die Gruppe auf einen Blick

```dataview
TABLE WITHOUT ID file.link AS "Charakter", class AS "Klasse", level AS "Stufe", ac AS "RK", hp + " / " + max_hp AS "TP", 10 + floor((wis - 10) / 2) + choice(contains(skills, "Wahrnehmung"), floor((level - 1) / 4) + 2, 0) AS "Passive Wahrnehmung"
FROM "Charaktere"
SORT file.name ASC
```

## Wer Heilung braucht

```dataview
TABLE WITHOUT ID file.link AS "Charakter", hp AS "Aktuelle TP", max_hp - hp AS "Fehlen"
FROM "Charaktere"
WHERE hp < max_hp
SORT (max_hp - hp) DESC
```

## Wer worin gut ist

Geübte Fertigkeiten und Expertise jeder Figur, für den Moment, in dem die Spielleitung fragt, wer es versuchen will.

```dataview
TABLE WITHOUT ID file.link AS "Charakter", skills AS "Geübte Fertigkeiten", expertise AS "Expertise"
FROM "Charaktere"
SORT file.name ASC
```
