# CRM-Vault — Obsidian-Vorlage

Ein persönliches CRM für Obsidian: Kontakte, Unternehmen, Deals und ein datiertes Protokoll jeder Interaktion, verbunden über Dataview. Die Pipeline einer kleinen Agentur ist schon eingetragen, das Dashboard zeigt also vom ersten Öffnen an echte Wiedervorlagen, offene Deals und Kontakte, die einschlafen.

## So hängt alles zusammen

- `Kontakte/` – eine Notiz pro Person, mit `company`, `role`, `relationship`, `last_contact` und `next_follow_up` in den Eigenschaften.
- `Unternehmen/` – eine Notiz pro Organisation. Jede listet ihre Personen und Deals automatisch.
- `Deals/` – eine Notiz pro Verkaufschance, mit `value`, `stage` und `close_date`.
- `Interaktionen/` – eine Notiz pro Anruf, Mail oder Termin, nach Datum benannt. Hier stehen die Folgeaufgaben.
- [[CRM-Dashboard]] – Wiedervorlagen dieser Woche, offene Aufgaben, Pipeline nach Phase, Kontakte ohne Kontakt seit 60 Tagen, letzte Interaktionen.
- `Pipeline.base` – dieselben Deals als bearbeitbare Tabelle, über das Kern-Plugin Bases.

Deal-Phasen in diesem Vault: `Lead`, `qualifiziert`, `Angebot`, `Verhandlung`, `gewonnen`, `verloren`.

## Plugins

**Dataview** ist für das Dashboard und die Listen in den Notizen nötig. Das Kern-Plugin **Vorlagen** ist aktiv und zeigt auf `Vorlagen/`. Die Pipeline-Tabelle nutzt das Kern-Plugin **Bases**, das in aktuellen Obsidian-Versionen enthalten ist.

- Dataview — https://obsidian.md/plugins?id=dataview

1. Download entpacken und in Obsidian **Ordner als Vault öffnen** wählen.
2. Community-Plugins für diesen Vault aktivieren, wenn Obsidian fragt.
3. **Dataview** installieren und aktivieren, dann das CRM-Dashboard in der Leseansicht öffnen.

## License

MIT. Nutzen, ändern, weitergeben – Namensnennung willkommen, aber nicht Pflicht.

Vorlage von Vaultorial — https://vaultorial.com/de/obsidian-crm-vorlage/
