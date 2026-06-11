# Hier starten

Willkommen. Dieser Vault ist ein leichtgewichtiges Projektmanagementsystem für Obsidian: eine Notiz pro Projekt, eine Notiz pro Besprechung und ein Dataview-Dashboard, das alles andere liest. Zwei vollständige Beispielprojekte — ein Website-Redesign und ein Büroumzug — kommen vorgeladen mit Meilensteinen, Mermaid-Zeitleisten und verknüpften Besprechungsnotizen, damit jede Dashboard-Abfrage echte Daten hinter sich hat.

## Wie der Vault aufgebaut ist

- `Projekte/` — eine Notiz pro Projekt. Das Frontmatter trägt die Felder, die das Dashboard liest (`status`, `owner`, `start`, `due`, `area`); der Textkörper enthält Ziele, eine Meilensteintabelle, eine Gantt-Zeitleiste und Links zu den Besprechungen dieses Projekts.
- `Besprechungen/` — eine Notiz pro Besprechung, benannt `YYYY-MM-DD Projekt Thema`. Jede verweist im Frontmatter zurück auf ihr Projekt, damit das Dashboard offene Aktionspunkte pro Projekt zusammenfassen kann.
- [[Dashboard]] — Live-Tabellen: aktive Projekte, Projekte nach Status und nach Verantwortlichem, anstehende Fälligkeiten, jüngste Besprechungen und jeder nicht abgehakte Aktionspunkt über alle Besprechungsnotizen hinweg.
- `Vorlagen/` — [[Projektvorlage]] und [[Besprechungsvorlage]], an das Core-Templates-Plugin angebunden.

## Konventionen, die das Dashboard funktionieren lassen

- `status` ist einer von: `planung`, `aktiv`, `pausiert`, `erledigt`. Kleingeschrieben, exakt — Dataview vergleicht Zeichenketten wörtlich.
- `owner` ist ein Name, überall gleich geschrieben ("Sarah Chen", nicht "S. Chen" in einer Datei und "sarah" in einer anderen).
- Daten sind `YYYY-MM-DD`. Dataview liest sie als echte Daten, was die "bald fällig"-Abfrage erst möglich macht.
- Aktionspunkte in Besprechungsnotizen sind schlichte `- [ ]`-Kästchen. Hak sie dort ab, wo sie leben; das Dashboard spiegelt es.

## Plugins zum Aktivieren

1. **Dataview** (erforderlich) — Einstellungen → Community-Plugins → Durchsuchen → "Dataview". Das Dashboard baut darauf auf.

Mermaid-Zeitleisten werden mit Obsidians eingebauter Mermaid-Unterstützung gerendert — kein Plugin nötig. Das Core-Plugin **Templates** ist bereits aktiviert und auf `Vorlagen/` gerichtet.

## Erste Schritte

1. Aktiviere Dataview und öffne das [[Dashboard]] in der Leseansicht. Jede Tabelle sollte gefüllt sein.
2. Öffne [[Website-Redesign]] und überflieg es von oben bis unten — Frontmatter, Meilensteine, Zeitleiste, Besprechungen. Diese Notiz ist das Muster.
3. Erstelle dein erstes echtes Projekt: neue Notiz in `Projekte/`, füge [[Projektvorlage]] ein (Befehlspalette → "Templates: Vorlage einfügen"), fülle das Frontmatter.
4. Erstelle nach deiner nächsten Besprechung eine Notiz in `Besprechungen/` aus [[Besprechungsvorlage]] und verknüpfe sie mit dem Projekt.
5. Lösche die beiden Beispielprojekte und ihre Besprechungen, sobald du eigene hast.
