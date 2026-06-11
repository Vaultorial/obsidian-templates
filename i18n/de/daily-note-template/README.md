# Tagesnotiz-Starter — Obsidian-Vorlage

Ein aufgeräumtes Tagesnotiz-System für Obsidian: eine Notiz pro Tag mit den Abschnitten **Agenda, Aufgaben, Protokoll und Dankbarkeit**, Navigation zum Vortag und Folgetag sowie einer komplett ausgefüllten Beispielwoche, damit das System im Einsatz erkennbar ist, bevor man sich darauf einlässt.

Zwei Vorlagenvarianten sind enthalten: eine, die nur mit Core-Plugins läuft, und eine auf Templater-Basis mit automatischer Datumsbehandlung.

## Ordnerstruktur

```
daily-note-template/
├── Hier starten.md                      ← zuerst lesen
├── Tagesnotizen/                        ← eine Notiz pro Tag (7 Beispieltage, Juni 2026)
│   ├── 2026-06-01.md … 2026-06-07.md
└── Vorlagen/
    ├── Tagesnotiz (Core-Templates).md   ← keine Plugins nötig
    └── Tagesnotiz (Templater).md        ← ergänzt Zurück-/Weiter-Links
```

## Installation

1. Den Download entpacken.
2. Obsidian öffnen → **Ordner als Vault öffnen** → den entpackten Ordner auswählen.
3. Dem Vault beim Öffnen vertrauen (er enthält nur einfache JSON-Einstellungen).
4. `Hier starten.md` öffnen.

Wer das System stattdessen in einen bestehenden Vault holen will, kopiert die Ordner `Tagesnotizen/` und `Vorlagen/` hinein und übernimmt die Daily-notes-Einstellungen (Ordner `Tagesnotizen`, Format `YYYY-MM-DD`, Vorlage `Vorlagen/Tagesnotiz (Core-Templates)`).

## Plugins

Erforderlich: keine — die Core-Variante funktioniert sofort.

Optional:

- **Templater** — dynamische Daten und Links zum Vortag/Folgetag. https://obsidian.md/plugins?id=templater-obsidian

## Lizenz

MIT. Nutzen, anpassen, weitergeben — keine Namensnennung erforderlich.

Vorlage von Vaultorial — https://vaultorial.com/de/daily-note-vorlage/
