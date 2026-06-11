# Hier starten

Willkommen. Dieser Vault ist ein Worldbuilding-System für Autorinnen, Autoren und Spielleitungen, demonstriert mit einem vollständigen Original-Setting: **Die Gezeitenhöfe**, eine niedermagische Welt aus Mündungsstadtstaaten, die das Gezeitenrecht regiert. Rund zwanzig verknüpfte Notizen — Orte, Charaktere, Fraktionen und eine verlinkte Chronologie — zeigen die Methode bei voller Dichte. Zuerst die Graphenansicht öffnen: Eine Welt sollte wie ein Netz aussehen, und diese tut es.

## Wie der Vault organisiert ist

- `Orte/` — eine Notiz pro Ort, mit `region` und `ruled-by` im Frontmatter.
- `Charaktere/` — eine Notiz pro Person, jede verlinkt mit einem `home` (einem Ort) und einer `faction`.
- `Fraktionen/` — die Mächte. Jede hat einen `seat` (einen Ort) und einen `leader` (einen Charakter).
- `Ereignisse/` — die Chronologie. Jedes Ereignis trägt `year`, `location` und eine `participants`-Liste, sodass die Zeitleiste sich selbst zusammensetzt.
- `Karten/` — absichtlich leer; die Notiz darin erklärt, wie eigene Karten hineinkommen.
- [[Weltindex]] — der Master-MOC: alle Entitäten von einer Seite aus, plus Dataview-Übersichten.
- [[Zeitleiste]] — die Chronologie, abgefragt und erzählt.
- `Vorlagen/` — eine Vorlage pro Entitätstyp, verdrahtet mit dem Core-Plugin Templates.

## Die Methode: Beziehungen im Frontmatter

Jede Notiz erklärt ihre Beziehungen als Frontmatter-Links (`home: "[[Niedermark]]"`, `faction: "[[Die Flutgeschworenen]]"`). Diese eine Gewohnheit liefert drei Dinge gratis: Die Graphenansicht zeigt die tatsächliche Gestalt der Welt, Dataview kann Fragen beantworten („alle, die dem Hof der Ebbe geschworen haben", „jedes Ereignis am Damm"), und das Umbenennen einer Notiz aktualisiert jede Referenz. Prosa-Wikilinks weben den Rest.

Daten folgen dem welteigenen Kalender — Jahre der Gezeitenrechnung, geschrieben `368 GR` — abgelegt als schlichte Zahl in `year`, damit die Zeitleiste sich selbst sortiert. Welcher Kalender auch immer zur eigenen Welt passt: das Feld numerisch halten.

## Zu aktivierende Plugins

1. **Dataview** (erforderlich) — treibt die Übersichten in [[Weltindex]] und [[Zeitleiste]] an.
2. **Timelines (Revamped)** (optional) — rendert visuelle Zeitbänder aus markierten Spannen, falls mehr als die abgefragte Tabelle gewünscht ist. Der Vault funktioniert vollständig ohne.

Das Core-Plugin **Templates** ist bereits aktiviert und zeigt auf `Vorlagen/`.

## Erste Schritte

1. Dataview aktivieren, dann den [[Weltindex]] lesen — er ist die Eingangstür zu allem.
2. Die Graphenansicht öffnen und Farbgruppen nach Ordnern vergeben (`path:Orte`, `path:Charaktere`, `path:Fraktionen`, `path:Ereignisse`). Die Struktur der Welt wird sofort sichtbar.
3. Eine Kette von Ende zu Ende lesen, um die Verlinkungsmethode zu spüren: [[Die Petition von Niedermark]] → [[Bren Callow]] → [[Die Flutgeschworenen]] → [[Die Flutung von Niedermark]].
4. Die erste eigene Entität anlegen: neue Notiz im richtigen Ordner, passende Vorlage einfügen, Frontmatter ausfüllen, beim Schreiben verlinken.
5. Beim Start der eigenen Welt die Gezeitenhöfe-Notizen löschen und Ordner, Vorlagen und Index behalten.
