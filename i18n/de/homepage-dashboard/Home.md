---
type: dashboard
---

# Home

> [!info] Direkt zu
> **Projekte:** [[Balkongarten für den Sommer|Balkongarten]] · [[Relaunch der Portfolio-Website|Portfolio]] · [[Spanisch-Konversationskurs|Spanisch]]
> **Bereiche:** [[Gesundheit & Fitness]] · [[Instandhaltung der Wohnung]]
> **Evergreen:** [[Leseliste]] · [[Wochen-Reset-Checkliste]] · [[Tomatensoße, die funktioniert]]
> Neu hier? Zuerst [[Hier starten]] lesen — oder [[Home (einfach)]] öffnen, die Plugin-freie Version dieser Seite.

## Heute

Offene Aufgaben, die heute fällig oder schon überfällig sind, gesammelt aus jedem Projekt und Bereich.

```dataview
TASK
FROM "Projekte" OR "Bereiche"
WHERE !completed AND due AND due <= date(today)
SORT due ASC
```

## Demnächst (nächste 7 Tage)

```dataview
TASK
FROM "Projekte" OR "Bereiche"
WHERE !completed AND due AND due > date(today) AND due <= date(today) + dur(7 days)
SORT due ASC
```

## Aktive Projekte

```dataview
TABLE WITHOUT ID file.link AS "Projekt", status AS "Status", started AS "Begonnen"
FROM "Projekte"
WHERE status = "aktiv"
SORT started ASC
```

## Zuletzt angefasst

```dataview
TABLE WITHOUT ID file.link AS "Notiz", dateformat(file.mtime, "ccc d MMM, HH:mm") AS "Zuletzt bearbeitet"
FROM "Projekte" OR "Bereiche" OR "Notizen"
SORT file.mtime DESC
LIMIT 7
```

## Der Vault auf einen Blick

```dataview
TABLE WITHOUT ID Ordner AS "Ordner", length(rows) AS "Notizen"
FROM "Projekte" OR "Bereiche" OR "Notizen"
GROUP BY file.folder AS Ordner
SORT Ordner ASC
```

> [!tip] Warum Aufgaben ein `[due:: Datum]` tragen
> Das Inline-Feld ist es, was die Abfragen oben jedes Projekt und jeden Bereich durchkämmen lässt. Aufgabe datieren und vergessen — diese Seite erinnert sich. Die Sonntagsroutine in der [[Wochen-Reset-Checkliste]] hält die Daten ehrlich.
