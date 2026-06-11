---
type: dashboard
---

# Besprechungs-Dashboard

In der Leseansicht mit aktiviertem Dataview öffnen. Alles unten wird aus dem Frontmatter und den Kästchen der Notizen in `Besprechungen/` generiert.

## Jüngste Besprechungen

```dataview
TABLE type, project, attendees
FROM "Besprechungen"
SORT date DESC
LIMIT 15
```

## Nach Typ

```dataview
TABLE rows.file.link AS "Besprechungen", rows.date AS "Datum"
FROM "Besprechungen"
GROUP BY type
```

## Nach Projekt

```dataview
TABLE rows.file.link AS "Besprechungen", rows.type AS "Typ"
FROM "Besprechungen"
GROUP BY project
```

## Offene Aktionspunkte

Jeder nicht abgehakte Aktionspunkt über alle Besprechungen, gruppiert nach der Besprechung, aus der er stammt. Hak sie dort ab, wo sie leben.

```dataview
TASK
FROM "Besprechungen"
WHERE !completed
```

## Entscheidungsprotokoll

Schnellsprungliste — Entscheidungen leben unter der Überschrift `## Entscheidungen` jeder Notiz.

```dataview
LIST
FROM "Besprechungen"
SORT date ASC
```
