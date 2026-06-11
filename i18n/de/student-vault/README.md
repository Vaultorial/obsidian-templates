# Studenten-Vault für Obsidian

Ein Obsidian-Vault zur Verwaltung von Studienarbeit, organisiert nach Semester und Kurs, mit einem Dataview-Dashboard, das jede anstehende Frist und Prüfung aus dem Notiz-Frontmatter sichtbar macht. Kommt mit zwei Beispielkursen, zwölf ausgefüllten Notizen über Vorlesungen, Prüfungsvorbereitung und Lektüren, und drei Vorlagen.

## Ordnerstruktur

```
student-vault/
├── Hier starten.md        ← lies das zuerst
├── Dashboard.md           ← Dataview: Fristen + Prüfungen, automatisch gebaut
├── Frühjahr 2026/
│   ├── Biologie 101/      ← Vorlesungen, Prüfungsvorbereitung, Lektürenotizen
│   └── Statistik 201/     ← Vorlesungen, Prüfungsvorbereitung, Lektürenotizen
└── Vorlagen/              ← Vorlesungsnotiz / Prüfungsvorbereitung / Lektürenotiz
```

## Wie es funktioniert

Notizen tragen die Felder `due` und `type` in ihrem Frontmatter. `Dashboard.md` fragt den ganzen Vault ab: eine Fristentabelle (alles mit einem zukünftigen `due`), eine Prüfungstabelle (`type: exam`) und eine Aufschlüsselung pro Kurs. Ändere ein Datum in einer Notiz, und das Dashboard spiegelt es sofort. Füge einen Kurs durch Kopieren eines Kursordners hinzu; füge ein Semester mit einem neuen `Saison JJJJ/`-Ordner hinzu.

## Installation

1. Entpacke den Download.
2. Öffne Obsidian → **Ordner als Vault öffnen** → wähle den entpackten Ordner.
3. Schalte bei Aufforderung den eingeschränkten Modus aus, installiere dann Dataview (Link unten) und aktiviere es.
4. Öffne `Dashboard.md` — die Tabellen sollten sich aus den Beispielnotizen befüllen.

## Plugins

- **Erforderlich:** Dataview — https://obsidian.md/plugins?id=dataview — treibt das Dashboard an.
- **Optional:** Calendar — https://obsidian.md/plugins?id=calendar — Monatsansicht als Begleiter für Tagesnotizen.

## Lizenz

MIT. Nutzen, verändern, darauf aufbauen — privat oder kommerziell. Keine Namensnennung erforderlich.

Vorlage von Vaultorial — https://vaultorial.com/de/studenten-vault/
