# CRM-Dashboard

Live-Ansichten des gesamten CRM. Alles hier sind Dataview-Abfragen über die Notizen dieses Vaults.

## Wiedervorlagen der nächsten 7 Tage

```dataview
TABLE WITHOUT ID file.link AS "Kontakt", company AS "Unternehmen", next_follow_up AS "Wiedervorlage"
FROM "Kontakte"
WHERE next_follow_up AND next_follow_up <= date(today) + dur(7 days)
SORT next_follow_up ASC
```

## Offene Aufgaben aus Interaktionen

```dataview
TASK
FROM "Interaktionen"
WHERE !completed
GROUP BY file.link
```

## Pipeline nach Phase

```dataview
TABLE WITHOUT ID key AS "Phase", length(rows) AS "Deals", sum(rows.value) AS "Pipeline-Wert (EUR)"
FROM "Deals"
WHERE stage != "verloren"
GROUP BY stage
```

## Offene Deals

```dataview
TABLE WITHOUT ID file.link AS "Deal", company AS "Unternehmen", stage AS "Phase", value AS "Wert (EUR)", close_date AS "Abschluss"
FROM "Deals"
WHERE stage != "gewonnen" AND stage != "verloren"
SORT close_date ASC
```

## Seit 60 Tagen kein Kontakt

```dataview
TABLE WITHOUT ID file.link AS "Kontakt", company AS "Unternehmen", last_contact AS "Letzter Kontakt"
FROM "Kontakte"
WHERE last_contact AND date(today) - last_contact > dur(60 days)
SORT last_contact ASC
```

## Letzte Interaktionen

```dataview
TABLE WITHOUT ID file.link AS "Interaktion", contact AS "Kontakt", channel AS "Kanal"
FROM "Interaktionen"
SORT date DESC
LIMIT 8
```
