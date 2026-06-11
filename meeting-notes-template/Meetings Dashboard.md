---
type: dashboard
---

# Meetings Dashboard

Open in reading view with Dataview enabled. Everything below is generated from the frontmatter and checkboxes of the notes in `Meetings/`.

## Recent meetings

```dataview
TABLE type, project, attendees
FROM "Meetings"
SORT date DESC
LIMIT 15
```

## By type

```dataview
TABLE rows.file.link AS "Meetings", rows.date AS "Date"
FROM "Meetings"
GROUP BY type
```

## By project

```dataview
TABLE rows.file.link AS "Meetings", rows.type AS "Type"
FROM "Meetings"
GROUP BY project
```

## Open action items

Every unchecked action item across all meetings, grouped by the meeting it came from. Tick them where they live.

```dataview
TASK
FROM "Meetings"
WHERE !completed
```

## Decisions log

Quick jump list — decisions live under the `## Decisions` heading of each note.

```dataview
LIST
FROM "Meetings"
SORT date ASC
```
