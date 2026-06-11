---
type: dashboard
---

# DM Screen

Open in reading view with Dataview enabled. Everything below updates itself from the frontmatter of the campaign notes.

## Where the campaign stands

- Last played: [[Session 3 - Salt in the Wound]]
- Prepped and ready: [[Counting House Break-In]]
- The party: [[Kestrel Thorne]], [[Bram Tuckett]], [[Yneva Marsh]]
- Spine of the plot: [[The Salt Road]] · [[The Carrow Combine]] · [[The Brine Wardens]]

## NPCs by location

```dataview
TABLE rows.file.link AS "NPC", rows.role AS "Role", rows.status AS "Status"
FROM "NPCs"
GROUP BY location
```

## NPCs by faction

```dataview
TABLE rows.file.link AS "NPC", rows.role AS "Role"
FROM "NPCs"
GROUP BY faction
```

## Sessions, most recent first

```dataview
TABLE date, number
FROM "Sessions"
SORT date DESC
```

## Encounters ready to run

```dataview
TABLE location, difficulty
FROM "Encounters"
WHERE status = "ready"
```

## Encounters already run

```dataview
TABLE location, difficulty
FROM "Encounters"
WHERE status = "run"
SORT file.name ASC
```

## The party

```dataview
TABLE player, class, level, ancestry
FROM "PCs"
SORT file.name ASC
```
