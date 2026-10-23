# Hier starten

Willkommen. Dieser Vault ist ein Lesesystem in drei Teilen: eine Notiz pro Buch in `Bücher/`, ein [[Bücherregal]], das sich aus diesen Notizen selbst zusammensetzt, und eine Vorlage, die jede neue Buchnotiz konsistent hält.

## Wie es funktioniert

Jede Buchnotiz trägt ihre Daten im Frontmatter — `author`, `genre`, `rating`, `status` (`gelesen` / `lese ich` / `Leseliste`), `date-started`, `date-finished`. Das [[Bücherregal]] führt Dataview-Abfragen über dieses Frontmatter aus, sodass sich die Regale in dem Moment aktualisieren, in dem du eine Notiz bearbeitest. Ändere den Status eines Buchs von `lese ich` auf `gelesen`, füge eine Bewertung hinzu, und es wechselt von selbst das Regal.

Sechs Bücher sind bereits da, in verschiedenen Zuständen, damit jedes Regal etwas hat: Beginn mit [[Konzentriert arbeiten]] oder [[Die 1%-Methode]] für eine fertige Notiz, [[Der pragmatische Programmierer]] für eine mitten im Lesen, und [[Essentialismus]] für das, was eine Leselisten-Notiz an Wenigem braucht.

## Notiz-Philosophie

- Zusammenfassung und Kernideen werden **in eigenen Worten geschrieben** — daher kommt die Behaltensleistung, nicht vom Sammeln von Passagen.
- Zitate auf höchstens eines pro Buch beschränkt, kurz und mit Quelle. Eine Buchnotiz ist dein Denken über das Buch, keine Auszugsdatei.

## Erste Schritte

1. Installiere und aktiviere **Dataview** (erforderlich — das [[Bücherregal]] ist ohne es leer): Einstellungen → Externe Erweiterungen → Durchsuchen → "Dataview".
2. Öffne das [[Bücherregal]] und prüfe, dass die Regale rendern.
3. Füge das Buch hinzu, das du gerade liest: neue Notiz in `Bücher/`, benannt nach dem Titel, füge `Vorlagen/Buchnotiz.md` ein (Core-Templates-Plugin, bereits konfiguriert), fülle das Frontmatter, setz `status: lese ich`.
4. Optional: Installiere **Book Search**, um Buchnotizen mit Autor und Metadaten aus einer Titelsuche vorgefüllt zu erstellen.

> [!tip] Bewerte auf deiner eigenen Skala
> Die Bewertung ist dafür, dass dein zukünftiges Ich entscheidet, was es wiederliest oder empfiehlt — keine öffentliche Rezension. Entscheide einmal, was eine 5 für dich bedeutet, schreib es oben ins Bücherregal, und bleib konsistent.
