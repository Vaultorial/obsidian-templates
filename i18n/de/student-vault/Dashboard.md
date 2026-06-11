---
type: dashboard
tags: [dashboard]
---

# Dashboard

Von Dataview aus dem Frontmatter jeder Notiz gebaut. Alles mit einem `due`-Datum erscheint unten automatisch — nichts hier wird von Hand gepflegt.

## Anstehende Fristen

```dataview
TABLE course AS "Kurs", type AS "Typ", due AS "Fällig"
FROM "Frühjahr 2026"
WHERE due AND due >= date(today)
SORT due ASC
```

## Prüfungen

```dataview
TABLE course AS "Kurs", topic AS "Thema", due AS "Datum"
FROM "Frühjahr 2026"
WHERE type = "exam"
SORT due ASC
```

## Leseaufgaben

```dataview
TABLE course AS "Kurs", source AS "Quelle", due AS "Fällig"
FROM "Frühjahr 2026"
WHERE type = "reading"
SORT due ASC
```

## Alles nach Kurs

```dataview
TABLE type AS "Typ", topic AS "Thema", due AS "Fällig"
FROM "Frühjahr 2026"
SORT course ASC, due ASC
```

> [!note] Tabellen leer?
> Dataview ist noch nicht aktiviert — siehe [[Hier starten]] für die Einrichtung. Überfällige Einträge fallen von selbst aus der Fristentabelle; die Pro-Kurs-Tabelle unten zeigt weiterhin alles.
