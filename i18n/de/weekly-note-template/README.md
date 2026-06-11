# Wochennotiz + Wochenrückblick — Obsidian-Vorlage

Ein Wochenplanungs- und Rückblick-System für Obsidian in einer einzigen Notiz pro Woche: Plan am Montag, Rückblick im GTD-Stil am Wochenende (Erfolge, persönliche Zahlen, Überträge, Fokus der nächsten Woche). Enthält vier aufeinanderfolgende Beispielwochen aus dem Mai 2026, an denen sichtbar wird, wie offene Schleifen von Woche zu Woche wandern.

## Ordnerstruktur

```
weekly-note-template/
├── Hier starten.md                      ← zuerst lesen
├── Wochennotizen/                       ← eine Notiz pro ISO-Woche (4 Beispielwochen)
│   ├── 2026-W19.md … 2026-W22.md
└── Vorlagen/
    ├── Wochennotiz (Core-Templates).md  ← keine Plugins nötig
    └── Wochennotiz (Templater).md       ← ergänzt Datumsbereich + Zurück-/Weiter-Links
```

## Installation

1. Den Download entpacken.
2. Obsidian öffnen → **Ordner als Vault öffnen** → den entpackten Ordner auswählen.
3. Dem Vault beim ersten Öffnen vertrauen (er enthält nur einfache JSON-Einstellungen).
4. `Hier starten.md` öffnen.

Für die Nutzung in einem bestehenden Vault die Ordner `Wochennotizen/` und `Vorlagen/` hineinkopieren und `Vorlagen` als Vorlagenordner setzen (Einstellungen → Templates).

## Plugins

Erforderlich: keine — die Core-Variante funktioniert sofort.

Optional:

- **Periodic Notes** — die Notiz der aktuellen Woche per Befehl öffnen. https://obsidian.md/plugins?id=periodic-notes
- **Templater** — dynamische Wochenbereiche und Zurück-/Weiter-Links. https://obsidian.md/plugins?id=templater-obsidian

## Lizenz

MIT. Nutzen, anpassen, weitergeben — keine Namensnennung erforderlich.

Vorlage von Vaultorial — https://vaultorial.com/de/wochennotiz-vorlage/
