# Projektmanagement-Vault — Obsidian-Vorlage

Ein Projektmanagementsystem aus reinen Dateien für Obsidian. Jedes Projekt ist eine einzelne Notiz mit strukturiertem Frontmatter, einer Meilensteintabelle, einer Mermaid-Gantt-Zeitleiste und verknüpften Besprechungsnotizen; ein Dataview-Dashboard fasst alles nach Status, Verantwortlichem und Fälligkeit zusammen. Kommt mit zwei vollständig ausgearbeiteten Beispielen — einem Website-Redesign und einem Büroumzug — inklusive vier realistischer Besprechungsnotizen.

## Struktur

```
project-management-template/
├── Hier starten.md     ← lies das zuerst
├── Dashboard.md        ← Dataview-Rollups: Status, Verantwortlicher, Fälligkeiten, Aktionspunkte
├── Projekte/
│   ├── Website-Redesign.md
│   └── Büroumzug.md
├── Besprechungen/      ← eine Notiz pro Besprechung, mit ihrem Projekt verknüpft
│   ├── 2026-04-02 Kickoff Website-Redesign.md
│   ├── 2026-05-07 Designreview Website-Redesign.md
│   ├── 2026-04-21 Lieferanten-Begehung Büroumzug.md
│   └── 2026-05-19 Logistik-Sync Büroumzug.md
└── Vorlagen/
    ├── Projektvorlage.md
    └── Besprechungsvorlage.md
```

## Installation

1. Lade die Vorlage herunter und entpacke sie: **Entpacken → Obsidian → Ordner als Vault öffnen**.
2. Wenn Obsidian fragt, aktiviere die Community-Plugins für diesen Vault.
3. Installiere Dataview und öffne `Dashboard.md` in der Leseansicht.

## Plugins

**Erforderlich**

- Dataview — https://obsidian.md/plugins?id=dataview

Gantt-Zeitleisten nutzen Obsidians eingebautes Mermaid-Rendering; kein zusätzliches Plugin nötig.

## Lizenz

MIT. Nutzen, verändern, weitergeben — Namensnennung willkommen, aber nicht erforderlich.

Vorlage von Vaultorial — https://vaultorial.com/de/projektmanagement-vorlage/
