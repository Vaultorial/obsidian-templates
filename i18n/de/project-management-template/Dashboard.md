---
type: dashboard
---

# Dashboard

In der Leseansicht mit aktiviertem Dataview öffnen. Jede Tabelle unten wird aus dem Frontmatter der Notizen in `Projekte/` und `Besprechungen/` generiert — nichts auf dieser Seite wird von Hand gepflegt.

## Aktive Projekte

```dataview
TABLE owner, area, start, due
FROM "Projekte"
WHERE status = "aktiv"
SORT due ASC
```

## Alle Projekte nach Status

```dataview
TABLE rows.file.link AS "Projekte", rows.owner AS "Verantwortlich"
FROM "Projekte"
GROUP BY status
```

## Projekte nach Verantwortlichem

```dataview
TABLE rows.file.link AS "Projekte", rows.due AS "Fällig"
FROM "Projekte"
GROUP BY owner
```

## Fällig in den nächsten 30 Tagen

```dataview
TABLE owner, status, due
FROM "Projekte"
WHERE status != "erledigt" AND due <= date(today) + dur(30 days)
SORT due ASC
```

## Jüngste Besprechungen

```dataview
TABLE project, date
FROM "Besprechungen"
SORT date DESC
LIMIT 10
```

## Offene Aktionspunkte aus Besprechungen

Jedes nicht abgehakte Kästchen über alle Besprechungsnotizen. Hak sie in der Besprechungsnotiz ab, wo sie leben.

```dataview
TASK
FROM "Besprechungen"
WHERE !completed
```
