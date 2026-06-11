# Journal / Bullet Journal — Obsidian-Vorlage

Ein Journal-Vault im Bullet-Journal-Stil für Obsidian: Rapid Logging mit der klassischen Notation (`•` Aufgabe, `×` erledigt, `○` Ereignis, `–` Notiz, `>` migriert), ein kurzer Dankbarkeitsabschnitt pro Eintrag, Monatsordner und ein monatliches Rückblick-Ritual. Enthält zwei vollständige Beispielwochen (25. Mai – 7. Juni 2026) und einen fertigen Monatsrückblick für Mai.

## Ordnerstruktur

```
journal-template/
├── Hier starten.md                        ← zuerst lesen (enthält den Logging-Schlüssel)
├── Journal/
│   └── 2026/
│       ├── 05/                            ← 7 Einträge + "2026-05 Rückblick.md"
│       └── 06/                            ← 7 Einträge
└── Vorlagen/
    ├── Journaleintrag (Bullet Journal).md ← Standard für neue Tagesnotizen
    ├── Journaleintrag (Fließtext).md      ← Langform-Variante in Prosa
    ├── Journaleintrag (Templater).md      ← ergänzt Links zurück/weiter
    └── Monatsrückblick.md
```

## Installation

1. Den Download entpacken.
2. Obsidian öffnen → **Ordner als Vault öffnen** → den entpackten Ordner wählen.
3. Dem Vault vertrauen, wenn Obsidian fragt (er enthält nur schlichte JSON-Einstellungen).
4. `Hier starten.md` öffnen, dann das Kalender-Symbol für den heutigen Eintrag anklicken.

Für die Nutzung in einem bestehenden Vault `Journal/` und `Vorlagen/` hineinkopieren und Daily notes auf Ordner `Journal`, Format `YYYY/MM/YYYY-MM-DD`, Vorlage `Vorlagen/Journaleintrag (Bullet Journal)` einstellen.

## Plugins

Erforderlich: keine.

Optional:

- **Templater** — dynamische Daten und Links zum Vortag/Folgetag für die Templater-Variante. https://obsidian.md/plugins?id=templater-obsidian

## Lizenz

MIT. Nutzen, anpassen, weitergeben — keine Namensnennung erforderlich.

Vorlage von Vaultorial — https://vaultorial.com/de/journal-vorlage/
