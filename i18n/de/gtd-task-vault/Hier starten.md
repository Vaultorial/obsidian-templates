# Hier starten

Willkommen. Dieser Vault ist ein funktionierendes Getting-Things-Done-Setup für Obsidian, aufgebaut auf dem Tasks-Plugin. Er kommt mit drei Beispielprojekten und über dreißig Aufgaben, damit jede Ansicht im [[Dashboard]] etwas zu zeigen hat. Ersetze die Beispiele nach und nach durch deine eigene Arbeit — die Struktur ist das Produkt, der Inhalt nur eine Demonstration.

## Wie der Vault aufgebaut ist

- [[00 Inbox]] — der Erfassungspunkt. Alles landet zuerst hier, unsortiert.
- [[01 Nächste Schritte]] — einzelne Aktionen, die nicht zu einem Projekt gehören, mit einem Kontext getaggt.
- [[02 Warten auf]] — Dinge, die du delegiert hast oder bei denen du blockiert bist, getaggt mit `#warten`.
- [[03 Irgendwann oder Vielleicht]] — Ideen, auf die du dich noch nicht festlegst. Absichtlich schlichte Aufzählungspunkte: Sie sind nicht handlungsreif und bleiben deshalb aus den Aufgaben-Queries heraus.
- `Projekte/` — eine Notiz pro Projekt. Aufgaben leben in der Projektnotiz, zu der sie gehören.
- [[Dashboard]] — das Cockpit. Live-Queries ziehen Aufgaben aus dem ganzen Vault: heute fällig, überfällig, nach Kontext, wartend und Inbox-Einträge zum Verarbeiten.
- `Vorlagen/` — enthält [[Projekt]], die Vorlage für neue Projektnotizen.

## Kontexte

Die GTD-Kontexte (die klassischen @zuhause, @computer, @besorgungen) sind hier verschachtelte Tags, weil Obsidian-Tags kein `@`-Zeichen enthalten dürfen:

- `#kontext/zuhause`
- `#kontext/computer`
- `#kontext/besorgungen`

Häng einer beliebigen Aufgabe einen Kontext-Tag an, und sie taucht im passenden Abschnitt des Dashboards auf. Füge eigene Kontexte hinzu (`#kontext/telefon`, `#kontext/büro`), indem du Aufgaben damit taggst und einen Query-Block im Dashboard kopierst.

## Plugins zum Aktivieren

1. **Tasks** (erforderlich) — Einstellungen → Community-Plugins → Durchsuchen → "Tasks". Treibt jede Query im Dashboard an.
2. **Dataview** (optional) — nur für die Projektübersichtstabelle am Ende des Dashboards verwendet. Alles andere funktioniert ohne.

Das Core-Plugin **Templates** ist bereits aktiviert und auf den Ordner `Vorlagen/` gerichtet.

## Erste Schritte

1. Aktiviere das Tasks-Plugin und öffne das [[Dashboard]] in der Leseansicht. Jeder Abschnitt sollte durch die Beispieldaten gefüllt sein.
2. Erfasse ein paar echte To-dos in [[00 Inbox]] als einfache `- [ ]`-Kästchen. Erfassen soll schnell und unordentlich sein.
3. Verarbeite die Inbox: Alles unter zwei Minuten sofort erledigen. Einzelne Aktionen wandern nach [[01 Nächste Schritte]] mit einem Kontext-Tag und, falls es zählt, einem Fälligkeitsdatum (`📅 2026-06-15`). Mehrschrittige Ergebnisse werden zu einer Notiz in `Projekte/` — nutze die Vorlage [[Projekt]].
4. Mach einmal pro Woche einen Rückblick: Inbox auf null bringen, jedes Projekt auf einen stockenden nächsten Schritt prüfen und allem in [[02 Warten auf]] nachgehen.
5. Wenn die Beispielprojekte ihren Zweck erfüllt haben, lösche sie.

> [!tip] Spickzettel zur Aufgaben-Syntax
> `- [ ] Klempner anrufen #kontext/zuhause ⏫ 📅 2026-06-15`
> `📅` Fälligkeitsdatum · `⏫` hohe Priorität · `🔽` niedrige Priorität · `🔁 every week` Wiederholung · `✅` Abschlussdatum (wird beim Abhaken automatisch hinzugefügt).
