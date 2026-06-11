---
type: dashboard
---

# Home

> [!info] Jump to
> **Projects:** [[Balcony Garden Summer Setup|Balcony Garden]] · [[Portfolio Website Refresh|Portfolio]] · [[Conversational Spanish Course|Spanish]]
> **Areas:** [[Health & Fitness]] · [[Home Maintenance]]
> **Evergreen:** [[Reading List]] · [[Weekly Reset Checklist]] · [[Tomato Sauce That Works]]
> New here? Read [[Start Here]] first — or open [[Home (simple)]] for the plugin-free version of this page.

## Today

Open tasks due today or already overdue, pulled from every project and area.

```dataview
TASK
FROM "Projects" OR "Areas"
WHERE !completed AND due AND due <= date(today)
SORT due ASC
```

## Coming up (next 7 days)

```dataview
TASK
FROM "Projects" OR "Areas"
WHERE !completed AND due AND due > date(today) AND due <= date(today) + dur(7 days)
SORT due ASC
```

## Active projects

```dataview
TABLE WITHOUT ID file.link AS "Project", status AS "Status", started AS "Started"
FROM "Projects"
WHERE status = "active"
SORT started ASC
```

## Recently touched

```dataview
TABLE WITHOUT ID file.link AS "Note", dateformat(file.mtime, "ccc d MMM, HH:mm") AS "Last edited"
FROM "Projects" OR "Areas" OR "Notes"
SORT file.mtime DESC
LIMIT 7
```

## Vault at a glance

```dataview
TABLE WITHOUT ID Folder AS "Folder", length(rows) AS "Notes"
FROM "Projects" OR "Areas" OR "Notes"
GROUP BY file.folder AS Folder
SORT Folder ASC
```

> [!tip] Why tasks carry `[due:: date]`
> The inline field is what lets the queries above sweep every project and area for you. Date a task and forget it — this page remembers. The Sunday routine in [[Weekly Reset Checklist]] keeps the data honest.
