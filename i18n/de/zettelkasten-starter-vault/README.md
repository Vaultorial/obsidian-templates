# Zettelkasten-Starter-Vault — Obsidian-Vorlage

Ein Obsidian-Starter-Vault für die Zettelkasten-Methode, vorbefüllt mit einem arbeitenden Beispiel: vierzehn verlinkte Notizen über Lernen und Gedächtnis, die die komplette Pipeline flüchtig → Literatur → permanent zeigen, dazu Zeitstempel-IDs und ein Register als Eingang.

## Ordnerstruktur

```
zettelkasten-starter-vault/
├── Hier starten.md    ← zuerst lesen
├── Register.md        ← Eingang zu den permanenten Notizen
├── Flüchtig/          ← schnelle Erfassungen, verarbeiten und löschen (3 Beispiele)
├── Literatur/         ← eine Notiz pro Quelle, eigene Worte (3 Beispiele)
├── Permanent/         ← eine Idee pro Notiz, Zeitstempel-IDs (8 Beispiele)
└── Vorlagen/          ← Vorlagen für flüchtige, Literatur- und permanente Notizen
```

Permanente Notizen heißen `YYYYMMDDHHMM Titel.md` (zum Beispiel `202605141030 Notizen in eigenen Worten schreiben.md`). Die ID macht jede Notiz eindeutig adressierbar und hält Dateinamen stabil, auch wenn Titel sich weiterentwickeln.

## Installation

1. Den Download entpacken.
2. Obsidian öffnen → **Ordner als Vault öffnen** → den entpackten Ordner wählen.
3. Bei Bedarf das Core-Plugin **Templates** aktivieren (Einstellungen → Obsidian-Erweiterungen); es zeigt bereits auf `Vorlagen`.
4. Optional: Templater installieren (unten), dann erzeugt die Vorlage für permanente Notizen ihre Zeitstempel-ID automatisch.

## Plugins

- **Erforderlich:** keine — der Vault funktioniert ab Werk mit Core-Plugins.
- **Optional:** Templater — https://obsidian.md/plugins?id=templater-obsidian — füllt die `YYYYMMDDHHMM`-ID und die Daten in den Vorlagen selbst aus. Ohne es die ID von Hand tippen.

## Lizenz

MIT. Nutzen, verändern, darauf aufbauen — privat oder kommerziell. Keine Namensnennung erforderlich.

Vorlage von Vaultorial — https://vaultorial.com/de/zettelkasten-starter-vault/
