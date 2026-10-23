# Hier starten

Dieser Vault ist ein funktionierendes persönliches CRM. Jede Person, jedes Unternehmen und jeder Deal ist eine Notiz, jedes Gespräch eine datierte Notiz in Interaktionen, und das [[CRM-Dashboard]] führt alles zusammen. Die Beispieldaten gehören zu einer erfundenen Designagentur, damit jede Abfrage etwas zeigt. Lösch sie, sobald deine eigenen Kontakte drin sind.

## So hängt alles zusammen

- `Kontakte/` – eine Notiz pro Person, mit `company`, `role`, `relationship`, `last_contact` und `next_follow_up` in den Eigenschaften.
- `Unternehmen/` – eine Notiz pro Organisation. Jede listet ihre Personen und Deals automatisch.
- `Deals/` – eine Notiz pro Verkaufschance, mit `value`, `stage` und `close_date`.
- `Interaktionen/` – eine Notiz pro Anruf, Mail oder Termin, nach Datum benannt. Hier stehen die Folgeaufgaben.
- [[CRM-Dashboard]] – Wiedervorlagen dieser Woche, offene Aufgaben, Pipeline nach Phase, Kontakte ohne Kontakt seit 60 Tagen, letzte Interaktionen.
- `Pipeline.base` – dieselben Deals als bearbeitbare Tabelle, über das Kern-Plugin Bases.

## Die Wochenroutine

Nach jedem Gespräch legst du aus der Vorlage eine Interaktionsnotiz an und verlinkst den Kontakt. Aktualisiere `last_contact` und `next_follow_up` beim Kontakt und die `stage` des Deals, falls sie sich geändert hat. Einmal pro Woche öffnest du das Dashboard und arbeitest die Wiedervorlagen oben ab.

Deal-Phasen in diesem Vault: `Lead`, `qualifiziert`, `Angebot`, `Verhandlung`, `gewonnen`, `verloren`.

## Plugins

**Dataview** ist für das Dashboard und die Listen in den Notizen nötig. Das Kern-Plugin **Vorlagen** ist aktiv und zeigt auf `Vorlagen/`. Die Pipeline-Tabelle nutzt das Kern-Plugin **Bases**, das in aktuellen Obsidian-Versionen enthalten ist.
