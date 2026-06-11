# Hier starten

Willkommen. Dies ist ein funktionierender Studenten-Vault für ein Semester: zwei Kurse, echte Vorlesungsnotizen, Prüfungsvorbereitung und Lektüren bereits vorhanden, plus ein [[Dashboard]], das jede Frist und jede Prüfung automatisch in einer Ansicht zusammenzieht.

## Wie es organisiert ist

- **Nach Semester und Kurs:** `Frühjahr 2026/Biologie 101/` und `Frühjahr 2026/Statistik 201/`. Füge jedes neue Semester einen Ordner pro Kurs hinzu — die Struktur skaliert durch Kopieren.
- **Drei Notiztypen pro Kurs**, jeder aus einer Vorlage: Vorlesungsnotizen, Prüfungsvorbereitung und Lektürenotizen.
- **[[Dashboard]]** liest die Felder `due` und `type` aus dem Frontmatter jeder Notiz und listet, was ansteht. Es wird von Dataview gebaut — ändere eine Frist in einer Notiz und das Dashboard aktualisiert sich selbst.

Die Beispielnotizen sind bewusst mit korrektem, allgemeinem Material gefüllt (Zellbiologie, deskriptive Statistik), damit du die Struktur an echten Inhalten siehst, bevor du sie durch eigene ersetzt.

## Erste Schritte

1. Installiere und aktiviere **Dataview** (erforderlich für das [[Dashboard]]): Einstellungen → Community-Plugins → Durchsuchen → "Dataview".
2. Öffne das [[Dashboard]] und prüfe, dass die Fristen- und Prüfungstabellen rendern.
3. Lege einen Kursordner für einen deiner echten Kurse innerhalb von `Frühjahr 2026/` an (oder einen neuen Semesterordner).
4. Mach deine nächste Vorlesung in einer Kopie von `Vorlagen/Vorlesungsnotiz.md` (Core-Templates-Plugin, bereits konfiguriert). Setz ein `due`-Datum auf alles mit Frist, und es erscheint im Dashboard.
5. Optional: Installiere **Calendar** für eine Monatsansicht neben deinen Tagesnotizen.

## Die Notiztypen

- **Vorlesungsnotiz** — Datum, Thema und ein sauberer Platz für den Stoff des Tages plus Fragen zum späteren Wiederholen.
- **Prüfungsvorbereitung** — `type: exam` und ein `due`-Datum, damit sie im Dashboard auftaucht; eine Checkliste der durchzuarbeitenden Themen.
- **Lektürenotiz** — Quelle, das `due`-Datum der Aufgabe und deine eigene Zusammenfassung des Gelesenen.

## Plugins

- **Erforderlich:** Dataview — das Dashboard braucht es.
- **Optional:** Calendar — Monatsansicht für Tagesnotizen.
- Das Core-Plugin **Templates** ist bereits aktiviert und auf `Vorlagen` gerichtet.

> [!tip] Eine Gewohnheit macht diesen Vault bezahlt
> Setz ein `due`-Datum ins Frontmatter, sobald eine Frist angekündigt wird. Das Dashboard kann nur zeigen, was du ihm sagst — aber wenn du es ihm sagst, verfolgst du Fristen nie wieder aus dem Gedächtnis.
