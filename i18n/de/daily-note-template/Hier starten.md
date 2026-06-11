# Hier starten

Willkommen. Dieser Vault ist ein Tagesnotiz-System mit vier festen Abschnitten — Agenda, Aufgaben, Protokoll und Dankbarkeit —, die sich in unter zwei Minuten ausfüllen oder zu einem vollständigen Journal ausbauen lassen. Mehr gibt es nicht zu konfigurieren.

## Wie der Vault aufgebaut ist

- `Tagesnotizen/` — eine Notiz pro Tag, benannt `YYYY-MM-DD`. Eine komplette Beispielwoche (1.–7. Juni 2026) liegt schon darin, damit sichtbar wird, wie sich die Abschnitte mit echtem Leben darin verhalten.
- `Vorlagen/` — zwei Versionen derselben Tagesvorlage:
	- **Tagesnotiz (Core-Templates)** — funktioniert sofort, ohne Plugins.
	- **Tagesnotiz (Templater)** — dasselbe Layout plus automatische Links zu gestern und morgen. Braucht das Templater-Plugin.

Das Core-Plugin **Daily notes** ist bereits eingerichtet: Neue Tagesnotizen landen in `Tagesnotizen/`, tragen das Datum als Namen und werden aus der Core-Vorlage vorausgefüllt.

## Erste Schritte

1. Auf das **Kalender-Symbol** in der linken Seitenleiste klicken (oder `Tagesnotiz für heute öffnen` über die Befehlspalette ausführen). Die heutige Notiz wird automatisch angelegt.
2. Vor dem Feierabend die wichtigste Aufgabe von morgen unter **Aufgaben** eintragen und eine Zeile ins **Protokoll** schreiben. Diese eine Gewohnheit macht den Vault schon wertvoll.
3. Die Beispielwoche in `Tagesnotizen/` überfliegen und löschen, sobald die Referenz nicht mehr gebraucht wird.
4. Zwei Beispielnotizen nebeneinander öffnen, um zu sehen, wie die Links `← zurück | weiter →` die Tage verbinden.

## Plugins

Ab Werk nutzt dieser Vault nur Core-Plugins (bereits aktiviert). Optionales Upgrade:

- **Templater** — installieren und aktivieren, in den Plugin-Einstellungen `Vorlagen` als Vorlagenordner setzen und Daily notes (Einstellungen → Daily notes → Vorlage) auf `Tagesnotiz (Templater)` zeigen lassen. Ab dann bekommt jede neue Tagesnotiz die Zurück-/Weiter-Navigation automatisch.

> [!tip] Abschnitte behalten, Fragen ändern
> Die vier Überschriften sind absichtlich unspektakulär, damit sie volle Tage überleben. Wer mit Dankbarkeit nichts anfangen kann, benennt den Abschnitt in der Vorlage in "Eine gute Sache" um — ein Schlussabschnitt sollte aber bleiben. Tagesnotizen sterben, wenn sie nur noch eine Aufgabenliste sind.
