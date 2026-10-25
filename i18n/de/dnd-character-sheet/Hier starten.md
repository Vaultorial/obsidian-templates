# Hier starten

Dieser Vault macht aus einem D&D-5e-Charakterbogen eine Obsidian-Notiz. Die Werte, die sich selten ändern (Attribute, Stufe, Rüstungsklasse, maximale Trefferpunkte), trägst du in die Eigenschaften der Notiz ein, und Dataview berechnet alles, was sich daraus ergibt: Attributsmodifikatoren, Übungsbonus, Initiative, Rettungswürfe, alle achtzehn Fertigkeiten, passive Wahrnehmung und für Zauberwirkende den Zauberrettungswurf-SG und den Zauberangriffsbonus. Für einen Stufenaufstieg änderst du eine Eigenschaft, und der ganze Bogen passt sich an.

## Was drin ist

- `Charaktere/` — drei ausgefüllte Beispielfiguren: Brannoc Vell (Kämpfer, Stufe 5), Isolde Marrow (Magierin, Stufe 5) und Tamsin Reed (Schurkin, Stufe 4, mit Expertise).
- [[Gruppenbogen]] — die ganze Gruppe in einer Tabelle, wer Heilung braucht und wer worin gut ist.
- `Vorlagen/Charakterbogen` — ein leerer Bogen, in dem alle Formeln schon stehen.

## Plugins, die du aktivieren musst

1. **Dataview** (erforderlich). Installiere es über die Community-Plugins.
2. Schalte in den Einstellungen von Dataview **JavaScript queries** ein. Die Tabellen für Rettungswürfe und Fertigkeiten nutzen einen kurzen DataviewJS-Block pro Bogen; alles andere ist normales Dataview.

Das Core-Plugin **Vorlagen** ist bereits aktiviert und zeigt auf `Vorlagen/`.

## So entstehen die Zahlen

- Modifikator = (Wert − 10) ÷ 2, abgerundet. Eine 16 ergibt +3, eine 8 ergibt −1.
- Übungsbonus = +2 auf Stufe 1–4, +3 auf 5–8, +4 auf 9–12, +5 auf 13–16, +6 auf 17–20.
- Eine geübte Fertigkeit oder ein geübter Rettungswurf addiert den Übungsbonus, Expertise addiert ihn doppelt.
- Passive Wahrnehmung = 10 + dein Wahrnehmungsbonus.
- Zauberrettungswurf-SG = 8 + Übungsbonus + Zaubermodifikator; Zauberangriff = Übungsbonus + Zaubermodifikator.

## Erste Schritte

1. Aktiviere Dataview und die JavaScript queries und öffne [[Brannoc Vell]] in der Leseansicht.
2. Ändere seine Eigenschaft `level` von 5 auf 9 und sieh zu, wie sich Übungsbonus, Rettungswürfe und Fertigkeiten ändern.
3. Öffne den [[Gruppenbogen]] und ändere bei jemandem `hp`, um die Heilungstabelle zu aktualisieren.
4. Für deine eigene Figur: neue Notiz in `Charaktere/`, Vorlage Charakterbogen einfügen, Eigenschaften ausfüllen.
