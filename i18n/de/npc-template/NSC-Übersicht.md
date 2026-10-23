# NSC-Übersicht

Alle Figuren auf einen Blick. Jede Tabelle ist eine Dataview-Abfrage über die NSC-Notizen.

## NSC nach Ort

```dataview
TABLE WITHOUT ID key AS "Ort", rows.file.link AS "NSC", rows.role AS "Rolle"
FROM "NSC"
GROUP BY location
```

## Haltung gegenüber der Gruppe

```dataview
TABLE WITHOUT ID file.link AS "NSC", attitude AS "Haltung", status AS "Status", first_met AS "Erstes Treffen"
FROM "NSC"
SORT attitude ASC, first_met ASC
```

## Mitglieder der Fraktionen

```dataview
TABLE WITHOUT ID key AS "Fraktion", length(rows) AS "Anzahl", rows.file.link AS "NSC"
FROM "NSC"
WHERE faction
GROUP BY faction
```

## Schnelle NSC zum Improvisieren

```dataview
TABLE WITHOUT ID file.link AS "NSC", role AS "Rolle", wants AS "Will"
FROM "Schnelle NSC"
```

## Noch nicht enthüllte Geheimnisse

```dataview
LIST secret
FROM "NSC"
WHERE revealed = false
```
