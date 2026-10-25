# Hier starten

Dieser Vault zeichnet Gantt-Diagramme aus deinen Notizen. Jede Aufgabe ist eine Notiz mit einem `start`- und einem `end`-Datum in den Eigenschaften, und die Notiz [[Zeitplan]] macht aus jeder Aufgabe einen Balken: ein Diagramm pro Projekt, ein Abschnitt pro Phase. Verschiebst du ein Datum, wird das Diagramm neu gezeichnet. Es gibt nichts zu exportieren, und jede Aufgabe bleibt eine normale Markdown-Datei, die du verlinken, taggen und beschreiben kannst.

## Was drin ist

- `Projekte/` — zwei Beispielprojekte mit terminierten Aufgaben: ein Büroumzug und ein Website-Relaunch, mit erledigten, laufenden und kritischen Aufgaben und Meilensteinen.
- [[Zeitplan]] — die erzeugten Diagramme und eine Liste der Aufgaben, die noch kein Datum haben.
- [[Statisches Gantt-Beispiel]] — ein von Hand geschriebenes Mermaid-Gantt-Diagramm ohne Plugin, mit erklärter Syntax.
- `Vorlagen/Aufgabe` — eine leere Aufgabennotiz mit allen Eigenschaften.

## Plugins, die du aktivieren musst

1. **Dataview** (für den [[Zeitplan]] erforderlich). Installiere es über die Community-Plugins.
2. Schalte in den Einstellungen von Dataview **JavaScript queries** ein.
3. Obsidian zeichnet die Diagramme mit dem eingebauten Mermaid. Fragt eine Notiz, ob Mermaid-Diagramme in diesem Vault angezeigt werden sollen, erlaube es.

Das Core-Plugin **Vorlagen** ist bereits aktiviert und zeigt auf `Vorlagen/`.

## Eigenschaften einer Aufgabe

- `project` und `phase` bestimmen, in welchem Diagramm und Abschnitt der Balken landet.
- `start` und `end` sind Daten im Format JJJJ-MM-TT. Eine Aufgabe ohne `start` bleibt außerhalb des Diagramms.
- `status`: `erledigt`, `in Arbeit` oder `offen`.
- `critical: true` zeichnet den Balken rot, `milestone: true` eine Raute am Startdatum.

## Erste Schritte

1. Aktiviere Dataview und die JavaScript queries und öffne den [[Zeitplan]] in der Leseansicht.
2. Öffne eine beliebige Aufgabe in `Projekte/Büroumzug/`, ändere ihr `end`-Datum und geh zurück zum [[Zeitplan]].
3. Für dein eigenes Projekt: Ordner in `Projekte/` anlegen, Aufgabennotizen mit der Vorlage Aufgabe hinzufügen und die Daten eintragen.
