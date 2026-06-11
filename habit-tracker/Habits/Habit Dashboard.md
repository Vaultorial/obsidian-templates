---
type: habit-dashboard
---

# Habit Dashboard

Reads the small per-day notes in `Habits/Daily Log` (each one carries the five habits as true/false frontmatter) and summarizes them. Requires the **Dataview** plugin — install and enable it, and these blocks come alive.

## Current streaks

Consecutive days per habit, counting backwards from the most recent logged day. Requires *JavaScript queries* to be enabled in Dataview's settings; if you prefer to keep JS off, just delete this block — everything below it is plain Dataview.

```dataviewjs
const habits = [
	["read", "Read 20 min"],
	["walk", "Walk 30 min"],
	["no_sugar", "No sugar"],
	["sleep_on_time", "Lights out by 23:30"],
	["journal", "Journal"],
];
const logs = dv.pages('"Habits/Daily Log"').values.sort((a, b) => b.date - a.date);
const rows = habits.map(([key, label]) => {
	let streak = 0;
	for (const p of logs) {
		if (p[key] === true) streak++;
		else break;
	}
	return [label, streak + (streak === 1 ? " day" : " days")];
});
dv.table(["Habit", "Streak (ending on last logged day)"], rows);
```

## Days kept, month by month

```dataview
TABLE length(rows) AS "Days logged",
	length(filter(rows.read, (x) => x)) AS "Read",
	length(filter(rows.walk, (x) => x)) AS "Walk",
	length(filter(rows.no_sugar, (x) => x)) AS "No sugar",
	length(filter(rows.sleep_on_time, (x) => x)) AS "Lights out",
	length(filter(rows.journal, (x) => x)) AS "Journal"
FROM "Habits/Daily Log"
GROUP BY dateformat(date, "yyyy-MM") AS Month
SORT Month DESC
```

## Last 14 logged days

```dataview
TABLE WITHOUT ID file.link AS "Day",
	read AS "Read", walk AS "Walk", no_sugar AS "No sugar",
	sleep_on_time AS "Lights out", journal AS "Journal"
FROM "Habits/Daily Log"
SORT date DESC
LIMIT 14
```

## Perfect days

All five habits kept on the same day.

```dataview
LIST
FROM "Habits/Daily Log"
WHERE read AND walk AND no_sugar AND sleep_on_time AND journal
SORT date DESC
```

> [!tip] Renaming habits
> The frontmatter keys (`read`, `walk`, `no_sugar`, `sleep_on_time`, `journal`) are the contract between your daily logs and this dashboard. If you change a habit, change its key in `Templates/Habit Log Entry` **and** in every query here — and start fresh logs rather than rewriting history.
