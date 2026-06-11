# Hier starten

Willkommen, Spielleiterin, willkommen, Spielleiter. Dieser Vault ist ein Kampagnen-Verwaltungssystem für Tischrollenspiele, kompatibel mit dem beliebtesten Regelwerk der fünften Edition. Er kommt mit einer kompletten originalen Mini-Kampagne — **Die Verschwörung der Salzstraße** — bereits geladen: drei gespielte Sitzungen, acht NSC, vier Orte, drei Begegnungen, drei Spielercharaktere und der Hintergrund, der alles zusammenhält. Wie geschrieben leiten, in Einzelteile zerlegen oder löschen und die Struktur behalten.

## Wie der Vault organisiert ist

- `Sitzungen/` — eine Notiz pro Sitzung: Rückblick, Szenen, ausgegebene Hinweise und ein „Nächstes Mal"-Block, der zur Vorbereitungsliste wird.
- `NSC/` — eine Notiz pro Figur, mit `role`, `location`, `status` und `faction` im Frontmatter, damit der [[Spielleiterschirm]] sie sortieren kann.
- `Orte/` — eine Notiz pro besuchbarem Ort, jede mit Links zu ihren NSC, Begegnungen und Gerüchten.
- `Begegnungen/` — vorbereitete Begegnungen mit originalen Werteblöcken, Geländenotizen und Taktik. `status: vorbereitet` heißt heute Abend spielbar; `status: gespielt` bewahrt das Protokoll.
- `SC/` — eine Notiz pro Spielercharakter: die Tischkopie von Bindungen, Zielen und den daran hängenden Kampagnenaufhängern.
- `Hintergrund/` — die beweglichen Teile der Welt (Fraktionen, Geschichte), über die mehr als eine Notiz einig sein muss.
- `Vorlagen/` — eine Vorlage pro Entitätstyp, verdrahtet mit dem Core-Plugin Templates.
- [[Spielleiterschirm]] — das Dashboard. Dataview-Abfragen ziehen NSC nach Ort, jüngste Sitzungen, vorbereitete Begegnungen und die Gruppenliste zusammen.

## Zu aktivierende Plugins

1. **Dataview** (erforderlich) — treibt jede Tabelle auf dem [[Spielleiterschirm]] an.
2. **Leaflet** (optional) — sobald Kartenbilder im Vault liegen, macht ein `leaflet`-Codeblock daraus schwenkbare Karten mit Markern. Nichts im Vault hängt davon ab.
3. **Initiative Tracker** (optional) — führt die Zugreihenfolge in der Seitenleiste; passt gut zu den Begegnungsnotizen.

Das Core-Plugin **Templates** ist bereits aktiviert und zeigt auf `Vorlagen/`.

## Erste Schritte

1. Dataview aktivieren und den [[Spielleiterschirm]] in der Leseansicht öffnen — jede Tabelle sollte befüllt sein.
2. [[Die Salzstraße]] für das Rückgrat der Kampagne lesen, dann [[Sitzung 3 - Salz in der Wunde]], um zu sehen, wo der Tisch aufgehört hat. Der [[Einbruch ins Kontor]] ist vorbereitet und bereit für die nächste Sitzung.
3. Vor der eigenen Session Zero den Vorlagen-Ablauf durchspielen: neue Notiz im richtigen Ordner, passende Vorlage einfügen, Frontmatter ausfüllen.
4. Nach jeder Sitzung die Sitzungsnotiz schreiben, solange alles frisch ist, jeden NSC mit verändertem `status` aktualisieren und die Begegnungsnotizen der nächsten Sitzung auf `vorbereitet` setzen.

> [!note] Zum Inhalt
> Alles hier — die Solmark, ihre Menschen, ihre Monster — ist ein Original dieser Vorlage. Wertezeilen wie „RK 13, TP 26" sind Hausregel-Schöpfungen für diese Kampagne, keine Wiedergaben aus irgendeinem Regelwerk, damit der Vault kompatibel bleibt, ohne fremden Text zu kopieren.
