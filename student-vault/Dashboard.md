---
type: dashboard
tags: [dashboard]
---

# Dashboard

Built by Dataview from the frontmatter of every note. Anything with a `due` date appears below automatically — nothing here is maintained by hand.

## Upcoming deadlines

```dataview
TABLE course AS "Course", type AS "Type", due AS "Due"
FROM "2026 Spring"
WHERE due AND due >= date(today)
SORT due ASC
```

## Exams

```dataview
TABLE course AS "Course", topic AS "Topic", due AS "Date"
FROM "2026 Spring"
WHERE type = "exam"
SORT due ASC
```

## Reading assignments

```dataview
TABLE course AS "Course", source AS "Source", due AS "Due"
FROM "2026 Spring"
WHERE type = "reading"
SORT due ASC
```

## Everything by course

```dataview
TABLE type AS "Type", topic AS "Topic", due AS "Due"
FROM "2026 Spring"
SORT course ASC, due ASC
```

> [!note] Tables empty?
> Dataview is not enabled yet — see [[Start Here]] for setup. Past-due items drop off the deadlines table on their own; the per-course table at the bottom keeps showing everything.
