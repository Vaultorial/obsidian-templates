# Hier starten

Willkommen. Dieser Vault erfasst Gewohnheiten auf zwei Arten — die wählen, die zur eigenen Geduld passt, oder beide parallel führen wie die Beispiele.

- **Der einfache Weg:** eine Notiz pro Monat mit einem Raster — Tage nach unten, Gewohnheiten quer, `✓` oder `·` in jeder Zelle. Keine Plugins, voll nutzbar auch an Papierhirn-Tagen.
- **Der fortgeschrittene Weg:** eine winzige Notiz pro Tag mit den Gewohnheiten als Wahr/Falsch-Frontmatter und ein [[Habit-Dashboard]], das Streaks, Monatssummen und perfekte Tage mit Dataview berechnet.

Zwei vollständig erfasste Monate liegen bei (April und Mai 2026, fünf Alltagsgewohnheiten: 20 Min lesen, 30 Min spazieren, kein Zucker, Licht aus bis 23:30, Tagebuch). Die Daten sind absichtlich unperfekt — eine Crunch-Woche, Wochenend-Durchhänger, eine Feiertagsdelle —, denn genau so sieht echtes Tracking aus, und beide Ansichten erzählen dieselbe Geschichte.

## Wie der Vault aufgebaut ist

- `Gewohnheiten/2026-04 Gewohnheiten.md`, `Gewohnheiten/2026-05 Gewohnheiten.md` — die Monatsraster, Summen am Ende.
- `Gewohnheiten/Tagesprotokoll/` — 61 Tagesnotizen, die das Dashboard füttern.
- `Gewohnheiten/Habit-Dashboard.md` — Streaks, Summen Monat für Monat, die letzten 14 Tage, perfekte Tage.
- `Vorlagen/` — `Monatsraster Gewohnheiten` (leeres Raster) und `Tagesprotokoll-Eintrag` (Tagesprotokoll).

## Erste Schritte

1. [[2026-05 Gewohnheiten]] öffnen und das Raster wie ein Diagramm lesen: Das Wochenendmuster und die Delle Mitte des Monats sind ohne eine einzige Abfrage erkennbar.
2. **Dataview** installieren (siehe README), dann das [[Habit-Dashboard]] öffnen und zusehen, wie aus denselben Daten Streaks und Summen werden. Für den Streak-Block in den Dataview-Einstellungen *JavaScript queries* aktivieren.
3. `2026-06 Gewohnheiten` in `Gewohnheiten/` anlegen und die Vorlage `Monatsraster Gewohnheiten` einfügen. Die Spalten auf die **eigenen** fünf Gewohnheiten umbenennen — höchstens fünf.
4. Heute Abend Tag eins mit der Vorlage `Tagesprotokoll-Eintrag` erfassen. Das ganze Ritual dauert unter einer Minute.
5. Die April/Mai-Beispiele löschen, sobald sie nichts mehr lehren (beide Monatsnotizen und `Tagesprotokoll` entfernen — das Dashboard zeigt dann nur noch die eigenen Daten).

## Plugins

- **Dataview** — nur für das [[Habit-Dashboard]] nötig. Die Monatsraster funktionieren ganz ohne Plugins.

> [!tip] Das Geschaffte zählen, nicht die Lücke
> Verpasste Tage bekommen ein leises `·`, kein rotes Mal, und eine gerissene Streak beginnt einfach eine neue. Der Job des Rasters ist Ehrlichkeit, nicht Schuldgefühl — dieser Unterschied hält das Eintragen bis in Woche drei am Leben.
