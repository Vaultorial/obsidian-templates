---
type: bookshelf
tags: [bookshelf]
---

# Bücherregal

Von Dataview aus dem Frontmatter jeder Notiz in `Bücher/` zusammengesetzt. Nichts auf dieser Seite wird von Hand gepflegt.

**Meine Bewertungsskala:** 5 = werde ich wiederlesen und Freunden aufdrängen · 4 = hat etwas verändert, das ich tue · 3 = gut, eine Idee war die Zeit wert · 2 = okay, vergesslich · 1 = mit Grund abgebrochen.

## Lese ich gerade

```dataview
TABLE author AS "Autor", genre AS "Genre", row["date-started"] AS "Begonnen"
FROM "Bücher"
WHERE status = "lese ich"
```

## Gelesen — nach Bewertung

```dataview
TABLE author AS "Autor", rating AS "Bewertung", row["date-finished"] AS "Beendet"
FROM "Bücher"
WHERE status = "gelesen"
SORT rating DESC
```

## Leseliste

```dataview
LIST author
FROM "Bücher"
WHERE status = "Leseliste"
```

## Alles, nach Autor

```dataview
TABLE author AS "Autor", status AS "Status", rating AS "Bewertung"
FROM "Bücher"
SORT author ASC
```

> [!note] Wenn die Regale leer sind
> Dataview ist noch nicht aktiviert — siehe [[Hier starten]] für die Ein-Minuten-Einrichtung.
