# Hier starten

Willkommen. Dieser Vault ist ein System für Besprechungsnotizen für Obsidian: drei fertige Vorlagen (Teammeeting, 1-on-1, Kundengespräch), ein Dataview-Dashboard, das jede Besprechung und jeden unerledigten Aktionspunkt findet, und vier ausgefüllte Beispielbesprechungen aus einem zusammenhängenden Projekt, damit du das System arbeiten siehst, bevor du es übernimmst.

## Wie der Vault aufgebaut ist

- `Vorlagen/` — das Produkt. [[Teammeeting]], [[1-on-1]] und [[Kundengespräch]], jede mit strukturiertem Frontmatter (`type`, `date`, `project`, `attendees`) und denselben vier Abschnitten: Agenda, Notizen, Entscheidungen, Aktionspunkte.
- `Besprechungen/` — eine Notiz pro Besprechung, benannt `YYYY-MM-DD Thema`. Die Beispiele folgen einem Beratungsprojekt (dem Aufbau eines Kundenportals für einen Versicherungskunden) über einen Kickoff, ein 1-on-1, ein Kundengespräch und einen Sprint-Review.
- [[Besprechungs-Dashboard]] — Dataview-Rollups: jüngste Besprechungen, Besprechungen nach Typ, nach Projekt und alle offenen Aktionspunkte an einem Ort.

## Konventionen, die das Dashboard funktionieren lassen

- `type` ist einer von: `teammeeting`, `one-on-one`, `kundengespräch`. Kleingeschrieben, exakt.
- `project` ist ein kurzes Klartext-Label ("Kundenportal"). Überall identisch schreiben — das Dashboard gruppiert danach.
- Aktionspunkte werden im Format des Tasks-Plugins geschrieben: `- [ ] Verantwortlich — was er tut 📅 2026-06-15`. Dieser Vault braucht nur den Kästchen-Teil (Dataview liest ihn), aber die Datumssyntax bedeutet, dass du diese Zeilen in einen GTD-Vault mit dem Tasks-Plugin — wie unseren GTD-Aufgaben-Vault — fallen lassen kannst, und sie werden unverändert als geplante Aufgaben erfasst.
- Entscheidungen bekommen einen eigenen Abschnitt. Sechs Monate später liest niemand die Notizen erneut; man sucht danach, was entschieden wurde.

## Plugins zum Aktivieren

1. **Dataview** (erforderlich) — Einstellungen → Externe Erweiterungen → Durchsuchen → "Dataview". Treibt das Dashboard an.
2. **Templater** (optional) — wenn du Templater bereits nutzt, richte es auf `Vorlagen/` und tausch die Variablen `{{date}}` und `{{title}}` gegen deine bevorzugten dynamischen Befehle. Die Vorlagen kommen in Core-Templates-Syntax, damit sie sofort funktionieren.

Das Core-Plugin **Templates** ist bereits aktiviert und auf `Vorlagen/` gerichtet.

## Erste Schritte

1. Aktiviere Dataview und öffne das [[Besprechungs-Dashboard]] in der Leseansicht — jeder Abschnitt sollte durch die vier Beispielbesprechungen gefüllt sein.
2. Öffne [[2026-05-04 Kickoff Kundenportal]], um eine ausgefüllte Notiz neben ihrer Vorlage zu sehen.
3. Vor deiner nächsten Besprechung: Erstelle eine Notiz in `Besprechungen/`, benannt mit Datum und Thema, füge die passende Vorlage ein (Befehlspalette → "Templates: Vorlage einfügen") und fülle das Frontmatter.
4. Während der Besprechung nur in Notizen/Entscheidungen/Aktionspunkte schreiben. Danach eine Minute investieren, um jedem Aktionspunkt einen Verantwortlichen und ein Datum zu geben.
5. Lösche die Beispielbesprechungen, sobald du ein paar eigene hast.
