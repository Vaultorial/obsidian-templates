# Tagesplaner (Time-Blocking) — Obsidian-Vorlage

Ein Time-Blocking-Tagesplaner für Obsidian: drei wichtigste Aufgaben, eine Stunde-für-Stunde-Timeline in Day-Planner-Syntax (`- [ ] 09:00 - 10:30 Deep Work: Berichtsentwurf`) und ein Tagesabschluss-Ritual am Ende. Enthält drei realistische Beispieltage und eine Wochenübersichts-Notiz.

## Ordnerstruktur

```
daily-planner-template/
├── Hier starten.md              ← zuerst lesen
├── Planer/                      ← eine Notiz pro Tag + Wochenübersicht
│   ├── 2026-06-08.md … 2026-06-10.md
│   └── Woche vom 2026-06-08.md
└── Vorlagen/
    ├── Tagesplaner.md           ← wird neuen Tagesnotizen automatisch zugewiesen
    └── Wochenübersicht.md
```

## Installation

1. Den Download entpacken.
2. Obsidian öffnen → **Ordner als Vault öffnen** → den entpackten Ordner auswählen.
3. Dem Vault beim ersten Öffnen vertrauen (er enthält nur einfache JSON-Einstellungen).
4. `Hier starten.md` öffnen, dann die heutige Notiz über das Kalender-Symbol anlegen.

Für die Nutzung in einem bestehenden Vault die Ordner `Planer/` und `Vorlagen/` hineinkopieren und Daily notes auf den Ordner `Planer`, Format `YYYY-MM-DD`, Vorlage `Vorlagen/Tagesplaner` zeigen lassen.

## Plugins

Erforderlich: keine — funktioniert als einfache Checklisten mit Core-Plugins.

Optional (empfohlen):

- **Day Planner** — rendert die Timeline-Blöcke als visuellen Zeitplan mit Live-„Jetzt"-Marker. https://obsidian.md/plugins?id=obsidian-day-planner

## Lizenz

MIT. Nutzen, anpassen, weitergeben — keine Namensnennung erforderlich.

Vorlage von Vaultorial — https://vaultorial.com/de/tagesplaner-vorlage/
