# Hier starten

Willkommen. Dieser Vault macht genau eine Sache: eine einzige Wochennotiz, die sowohl den **Plan für die Woche** als auch den **Rückblick darauf** enthält. Montags planen, freitags oder sonntags zurückblicken, dieselbe Datei. Vier ausgefüllte Beispielwochen zeigen, wie es aussieht, wenn ein echter Monat durch das System läuft.

## Wie der Vault aufgebaut ist

- `Wochennotizen/` — eine Notiz pro ISO-Woche, benannt `2026-W19`, `2026-W20` und so weiter. Die vier Beispiele decken den Mai 2026 ab und lesen sich als durchgehende Geschichte: Es lohnt sich zu beobachten, wie Unerledigtes aus den **Überträgen** einer Woche in den Plan der nächsten kriecht. Diese Schleife ist die ganze Methode.
- `Vorlagen/` — zwei Versionen der Wochenvorlage:
	- **Wochennotiz (Core-Templates)** — keine Plugins nötig.
	- **Wochennotiz (Templater)** — ergänzt den Datumsbereich der Woche und die Links zur Vor- und Folgewoche, berechnet aus dem Dateinamen.

## Erste Schritte

1. `2026-W19` bis `2026-W22` der Reihe nach lesen. Fünf Minuten, und das System ist klar.
2. Die eigene aktuelle Woche anlegen: neue Notiz in `Wochennotizen/`, benannt nach der ISO-Nummer dieser Woche (z. B. `2026-W24`), dann die Vorlage über **Vorlage einfügen** aus der Befehlspalette einsetzen.
3. Am Montag den **Fokus** und 3–5 Plan-Aufgaben eintragen. Unter der Woche nichts anfassen. Am Wochenende den Rückblick in einem Rutsch ausfüllen.
4. Alles Unerledigte wandert in die **Überträge** — und muss im Plan der nächsten Woche auftauchen oder bewusst gestrichen werden. Was sich drei Wochen am Stück durchschleppt, will etwas sagen.

## Plugins

Ab Werk nur Core-Plugins. Zwei optionale Upgrades:

- **Periodic Notes** — ergänzt einen Befehl zum Öffnen der aktuellen Wochennotiz und eine kalenderartige Wochennavigation. Nach der Installation das Wochenformat auf `GGGG-[W]WW` und den Ordner auf `Wochennotizen` setzen.
- **Templater** — nötig für die Variante `Wochennotiz (Templater)`. Als Vorlagenordner `Vorlagen` eintragen.

> [!tip] Den Rückblick ehrlich halten
> Der Abschnitt **Zahlen** erfasst nur Dinge, die tatsächlich gezählt werden (Workouts, Lerneinheiten, Seiten). Zwei oder drei Messwerte genügen völlig — sobald sich das Eintragen nach Buchhaltung anfühlt, einen streichen.
