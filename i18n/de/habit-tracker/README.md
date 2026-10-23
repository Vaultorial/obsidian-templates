# Habit Tracker — Obsidian-Vorlage

Ein Habit Tracker für Obsidian mit zwei Ebenen: plugin-freie **Monatsraster** (Gewohnheiten × Tage, Häkchen in einer Tabelle) und ein optionales **Dataview-Dashboard**, das Streaks, Monatssummen und perfekte Tage aus winzigen Tagesnotizen berechnet. Enthält zwei vollständig erfasste Beispielmonate (April–Mai 2026, fünf Alltagsgewohnheiten, realistisch unperfekte Daten).

## Ordnerstruktur

```
habit-tracker/
├── Hier starten.md                  ← zuerst lesen
├── Gewohnheiten/
│   ├── 2026-04 Gewohnheiten.md      ← Monatsraster, ausgefüllt
│   ├── 2026-05 Gewohnheiten.md      ← Monatsraster, ausgefüllt
│   ├── Habit-Dashboard.md           ← Dataview: Streaks, Summen, perfekte Tage
│   └── Tagesprotokoll/              ← 61 Tagesnotizen (Frontmatter-Daten)
│       └── 2026-04-01.md … 2026-05-31.md
└── Vorlagen/
    ├── Monatsraster Gewohnheiten.md ← leeres Raster für einen neuen Monat
    └── Tagesprotokoll-Eintrag.md    ← Ein-Minuten-Protokoll am Abend
```

## Installation

1. Den Download entpacken.
2. Obsidian öffnen → **Ordner als Vault öffnen** → den entpackten Ordner auswählen.
3. Dem Vault beim ersten Öffnen vertrauen (er enthält nur einfache JSON-Einstellungen).
4. `Hier starten.md` öffnen.

Für die Nutzung in einem bestehenden Vault die Ordner `Gewohnheiten/` und `Vorlagen/` hineinkopieren und `Vorlagen` als Vorlagenordner setzen (Einstellungen → Vorlagen).

## Plugins

Erforderlich: keine — die Monatsraster sind reine Markdown-Tabellen.

Optional:

- **Dataview** — treibt das Habit-Dashboard an (für die Streaks muss die Einstellung *JavaScript queries* aktiviert sein). https://obsidian.md/plugins?id=dataview

## Lizenz

MIT. Nutzen, anpassen, weitergeben — keine Namensnennung erforderlich.

Vorlage von Vaultorial — https://vaultorial.com/de/habit-tracker/
