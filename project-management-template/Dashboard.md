---
type: dashboard
---

# Dashboard

Open in reading view with Dataview enabled. Every table below is generated from the frontmatter of the notes in `Projects/` and `Meetings/` — nothing on this page is maintained by hand.

## Active projects

```dataview
TABLE owner, area, start, due
FROM "Projects"
WHERE status = "active"
SORT due ASC
```

## All projects by status

```dataview
TABLE rows.file.link AS "Projects", rows.owner AS "Owner"
FROM "Projects"
GROUP BY status
```

## Projects by owner

```dataview
TABLE rows.file.link AS "Projects", rows.due AS "Due"
FROM "Projects"
GROUP BY owner
```

## Due in the next 30 days

```dataview
TABLE owner, status, due
FROM "Projects"
WHERE status != "done" AND due <= date(today) + dur(30 days)
SORT due ASC
```

## Recent meetings

```dataview
TABLE project, date
FROM "Meetings"
SORT date DESC
LIMIT 10
```

## Open action items from meetings

Every unchecked checkbox across all meeting notes. Tick them in the meeting note where they live.

```dataview
TASK
FROM "Meetings"
WHERE !completed
```
