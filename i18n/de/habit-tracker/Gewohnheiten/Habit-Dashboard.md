---
type: gewohnheiten-dashboard
---

# Habit-Dashboard

Liest die kleinen Tagesnotizen in `Gewohnheiten/Tagesprotokoll` (jede trägt die fünf Gewohnheiten als Wahr/Falsch-Frontmatter) und fasst sie zusammen. Benötigt das **Dataview**-Plugin — installieren und aktivieren, dann erwachen diese Blöcke zum Leben.

## Aktuelle Streaks

Aufeinanderfolgende Tage pro Gewohnheit, rückwärts gezählt ab dem zuletzt erfassten Tag. Benötigt die Einstellung *JavaScript queries* in Dataview; wer JS lieber auslässt, löscht einfach diesen Block — alles darunter ist reines Dataview.

```dataviewjs
const habits = [
	["read", "20 Min lesen"],
	["walk", "30 Min spazieren"],
	["no_sugar", "Kein Zucker"],
	["sleep_on_time", "Licht aus bis 23:30"],
	["journal", "Tagebuch"],
];
const logs = dv.pages('"Gewohnheiten/Tagesprotokoll"').values.sort((a, b) => b.date - a.date);
const rows = habits.map(([key, label]) => {
	let streak = 0;
	for (const p of logs) {
		if (p[key] === true) streak++;
		else break;
	}
	return [label, streak + (streak === 1 ? " Tag" : " Tage")];
});
dv.table(["Gewohnheit", "Streak (endet am letzten erfassten Tag)"], rows);
```

## Geschaffte Tage, Monat für Monat

```dataview
TABLE length(rows) AS "Erfasste Tage",
	length(filter(rows.read, (x) => x)) AS "Lesen",
	length(filter(rows.walk, (x) => x)) AS "Spazieren",
	length(filter(rows.no_sugar, (x) => x)) AS "Kein Zucker",
	length(filter(rows.sleep_on_time, (x) => x)) AS "Licht aus",
	length(filter(rows.journal, (x) => x)) AS "Tagebuch"
FROM "Gewohnheiten/Tagesprotokoll"
GROUP BY dateformat(date, "yyyy-MM") AS Monat
SORT Monat DESC
```

## Die letzten 14 erfassten Tage

```dataview
TABLE WITHOUT ID file.link AS "Tag",
	read AS "Lesen", walk AS "Spazieren", no_sugar AS "Kein Zucker",
	sleep_on_time AS "Licht aus", journal AS "Tagebuch"
FROM "Gewohnheiten/Tagesprotokoll"
SORT date DESC
LIMIT 14
```

## Perfekte Tage

Alle fünf Gewohnheiten am selben Tag geschafft.

```dataview
LIST
FROM "Gewohnheiten/Tagesprotokoll"
WHERE read AND walk AND no_sugar AND sleep_on_time AND journal
SORT date DESC
```

> [!tip] Gewohnheiten umbenennen
> Die Frontmatter-Schlüssel (`read`, `walk`, `no_sugar`, `sleep_on_time`, `journal`) sind der Vertrag zwischen den Tagesprotokollen und diesem Dashboard. Wer eine Gewohnheit ändert, ändert ihren Schlüssel in `Vorlagen/Tagesprotokoll-Eintrag` **und** in jeder Abfrage hier — und beginnt frische Protokolle, statt die Geschichte umzuschreiben.
