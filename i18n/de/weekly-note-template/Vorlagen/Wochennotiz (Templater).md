---
week: <% tp.file.title %>
start: <% moment(tp.file.title, "GGGG-[W]WW").startOf("isoWeek").format("YYYY-MM-DD") %>
end: <% moment(tp.file.title, "GGGG-[W]WW").endOf("isoWeek").format("YYYY-MM-DD") %>
type: wochennotiz
---

# <% tp.file.title %> — <% moment(tp.file.title, "GGGG-[W]WW").startOf("isoWeek").format("D.") %>–<% moment(tp.file.title, "GGGG-[W]WW").endOf("isoWeek").format("D. MMMM YYYY") %>

← [[<% tp.date.now("GGGG-[W]WW", -7, tp.file.title, "GGGG-[W]WW") %>]] | [[<% tp.date.now("GGGG-[W]WW", 7, tp.file.title, "GGGG-[W]WW") %>]] →

## Wochenplan

**Fokus:**

- [ ]
- [ ]
- [ ]

## Rückblick

### Erfolge

-

### Zahlen

| Messwert | Ziel | Ist |
| -------- | ---- | --- |
|          |      |     |

### Überträge

-

### Fokus für nächste Woche

-

> [!note]- Wie diese Vorlage funktioniert
> Templater-Variante. Wochenbereich und Zurück-/Weiter-Links werden aus dem Dateinamen abgeleitet, die Notiz also `2026-W24` (ISO-Woche) nennen und die Vorlage über Templater anwenden. Einrichtung: Templater installieren und `Vorlagen` als Vorlagenordner setzen. Dieses Callout aus der eigenen Kopie löschen.
