# Cornell-Notizen-Vorlage für Obsidian

Ein Obsidian-Vault, der die Cornell-Methode der Mitschrift mit schlichten Callouts und einem einzigen CSS-Snippet umsetzt: eine Cue-Spalte links, Notizen rechts, ein Zusammenfassungsband darunter. Keine Community-Plugins. Enthält zwei Vorlagen (allgemeine Cornell-Notiz und eine Mitschrift-Variante mit Kursmetadaten) sowie drei vollständig ausgearbeitete Beispielnotizen.

## Ordnerstruktur

```
cornell-notes-template/
├── Hier starten.md           ← zuerst lesen
├── Notizen/                  ← 3 ausgefüllte Beispiel-Mitschriften
├── Vorlagen/                 ← Cornell-Notiz + Mitschrift (Cornell)
└── .obsidian/snippets/
    └── cornell.css           ← das zweispaltige Layout (vorab aktiviert)
```

## Wie es funktioniert

Jede Notiz nutzt drei Callouts — `[!cue]`, `[!notes]`, `[!summary]` — und das Snippet `cornell.css` ordnet sie als klassische Cornell-Seite an: schwebende Cue-Spalte (32 %), Notizen daneben, Zusammenfassung darunter freigeräumt, auf schmalen Fenstern zu gestapelten Blöcken zusammenklappend. Das Snippet ist über `appearance.json` vorab aktiviert; umschalten lässt es sich unter Einstellungen → Darstellung → CSS-Bausteine.

Die Mitschrift-Variante ergänzt das Frontmatter `course`, `professor` und `date`, damit Mitschriften nach Fach sortier- und durchsuchbar bleiben.

## Installation

1. Den Download entpacken.
2. Obsidian öffnen → **Ordner als Vault öffnen** → den entpackten Ordner wählen.
3. Den eingeschränkten Modus anlassen, wenn gefragt wird — hier gibt es keine Community-Plugins.
4. Eine Notiz in `Notizen/` in der Leseansicht öffnen; es sollten zwei Spalten erscheinen. Falls nicht, das Snippet **cornell** unter Einstellungen → Darstellung → CSS-Bausteine aktivieren.

## Plugins

- **Erforderlich:** keine. Nur das Core-Plugin Templates (auf den Ordner `Vorlagen` vorkonfiguriert).
- **Optional:** keine.

## Lizenz

MIT. Nutzen, ändern, darauf aufbauen — privat oder kommerziell. Keine Namensnennung erforderlich.

Vorlage von Vaultorial — https://vaultorial.com/de/cornell-notizen-vorlage/
