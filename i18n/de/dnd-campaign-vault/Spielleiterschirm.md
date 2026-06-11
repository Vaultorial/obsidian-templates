---
type: dashboard
---

# Spielleiterschirm

In der Leseansicht öffnen, mit aktiviertem Dataview. Alles hier unten aktualisiert sich selbst aus dem Frontmatter der Kampagnennotizen.

## Wo die Kampagne steht

- Zuletzt gespielt: [[Sitzung 3 - Salz in der Wunde]]
- Vorbereitet und bereit: [[Einbruch ins Kontor]]
- Die Gruppe: [[Kestrel Thorne]], [[Bram Tuckett]], [[Yneva Marsh]]
- Rückgrat der Handlung: [[Die Salzstraße]] · [[Die Carrow-Kompanie]] · [[Die Solwächter]]

## NSC nach Ort

```dataview
TABLE rows.file.link AS "NSC", rows.role AS "Rolle", rows.status AS "Status"
FROM "NSC"
GROUP BY location
```

## NSC nach Fraktion

```dataview
TABLE rows.file.link AS "NSC", rows.role AS "Rolle"
FROM "NSC"
GROUP BY faction
```

## Sitzungen, neueste zuerst

```dataview
TABLE date AS "Datum", number AS "Nr."
FROM "Sitzungen"
SORT date DESC
```

## Spielbereite Begegnungen

```dataview
TABLE location AS "Ort", difficulty AS "Schwierigkeit"
FROM "Begegnungen"
WHERE status = "vorbereitet"
```

## Bereits gespielte Begegnungen

```dataview
TABLE location AS "Ort", difficulty AS "Schwierigkeit"
FROM "Begegnungen"
WHERE status = "gespielt"
SORT file.name ASC
```

## Die Gruppe

```dataview
TABLE player AS "Spieler", class AS "Klasse", level AS "Stufe", ancestry AS "Volk"
FROM "SC"
SORT file.name ASC
```
