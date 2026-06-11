# Hier starten

Willkommen. Dieser Vault ist eine **Startseite für den eigenen Vault**: eine einzige Notiz, die mit den heutigen Aufgaben, den aktiven Projekten, den letzten Änderungen und Schnellzugriffen begrüßt — statt mit der Datei, die zufällig letzten Dienstag offen war. Es gibt sie in zwei Stärken, beide enthalten und beide bereits mit einem kleinen funktionierenden Beispiel-Vault gefüllt (drei Projekte, zwei Bereiche, drei Evergreen-Notizen).

## Die zwei Dashboards

- [[Home (einfach)]] — Callouts und statische Links, null Plugins. Gleich öffnen; es funktioniert bereits.
- [[Home]] — die lebendige Version. Dataview-Abfragen durchkämmen jedes Projekt und jeden Bereich nach Aufgaben mit Daten im Stil `[due:: 2026-06-12]` und bauen daraus die Abschnitte **Heute** und **Demnächst**. Braucht das Dataview-Plugin.

Die Beispielnotizen drumherum sind echt genug, damit das Dashboard atmet: datierte Aufgaben, Querverlinkungen, ein oder zwei überfällige Punkte. Nach und nach durch das eigene Leben ersetzen.

## Wie der Vault aufgebaut ist

- `Projekte/` — Arbeit mit Endzustand (ein Gartenaufbau, ein Website-Relaunch, ein Kurs).
- `Bereiche/` — laufende Verantwortungen ohne Ziellinie (Gesundheit, Wohnungspflege).
- `Notizen/` — dauerhafte Referenz: Listen, Checklisten, Rezepte.

Die Konvention, die alles trägt: **Jede umsetzbare Aufgabe bekommt ein Inline-Fälligkeitsdatum**, etwa `- [ ] Die Über-mich-Seite neu schreiben [due:: 2026-06-12]`. Diese eine Gewohnheit ist es, wovon [[Home]] lebt.

## Erste Schritte

1. [[Home (einfach)]] öffnen und durch den Beispiel-Vault klicken, um ein Gefühl für die Form zu bekommen.
2. **Dataview** installieren und aktivieren (Links im README), dann [[Home]] öffnen — die Abfragen erwachen über denselben Notizen zum Leben.
3. **Homepage** installieren und in dessen Einstellungen `Home` als Startseite wählen (oder `Home (einfach)`, wenn es ohne Plugins bleiben soll). Genau darum geht es in diesem Vault: Jede Sitzung beginnt am Dashboard.
4. Das Dashboard zu eigen machen: eine Projektnotiz in `Projekte/` mit zwei, drei datierten Aufgaben anlegen und zusehen, wie sie unter **Demnächst** auftaucht.
5. Haben die Beispielnotizen ihren Zweck erfüllt, löschen — den Abfragen ist es egal, sie lesen, was in den Ordnern liegt.

## Plugins

- **Dataview** — erforderlich für [[Home]], nicht für [[Home (einfach)]].
- **Homepage** — öffnet das gewählte Dashboard beim Start. Optional, aber es ist der Unterschied zwischen einer Startseite und einer Notiz namens Home.

> [!tip] Das Dashboard langweilig halten
> Der Versuchung widerstehen, jede entdeckte Abfrage einzubauen. Ein Dashboard, auf das man blickt, schlägt ein Dashboard, durch das man scrollt. Heute, diese Woche, aktive Projekte, zuletzt bearbeitet — wenn ein Abschnitt um 9:00 keine Entscheidung ändert, fliegt er raus.
