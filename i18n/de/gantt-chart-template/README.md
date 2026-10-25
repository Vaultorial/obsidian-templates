# Gantt-Diagramm-Vault — Obsidian-Vorlage

Gantt-Diagramme aus deinen Notizen: Jede Aufgabe ist eine Notiz mit Start- und Enddatum in den Eigenschaften, und eine DataviewJS-Abfrage macht daraus ein Mermaid-Gantt-Diagramm pro Projekt, mit einem Abschnitt pro Phase. Mit zwei Beispielprojekten, einem statischen Beispiel ohne Plugin und einer Aufgabenvorlage.

## Struktur

```
gantt-chart-template/
├── Hier starten.md                 ← zuerst lesen
├── Zeitplan.md                     ← die erzeugten Diagramme
├── Statisches Gantt-Beispiel.md    ← von Hand geschrieben, ohne Plugin
├── Projekte/                       ← 2 Beispielprojekte, 14 terminierte Aufgaben
└── Vorlagen/                       ← leere Aufgabennotiz
```

## Installation

1. Vorlage herunterladen und entpacken: **Entpacken → Obsidian → Ordner als Vault öffnen**.
2. Wenn Obsidian fragt, Community-Plugins für diesen Vault aktivieren.
3. Dataview installieren, in den Einstellungen *JavaScript queries* einschalten und `Zeitplan.md` öffnen.

## Plugins

**Erforderlich**

- Dataview — https://obsidian.md/plugins?id=dataview

## Lizenz

MIT. Nutzen, ändern, teilen — Namensnennung willkommen, aber nicht nötig.

Vorlage von Vaultorial — https://vaultorial.com/de/gantt-diagramm-vorlage/
