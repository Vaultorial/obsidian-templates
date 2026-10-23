# NPC Roster

Your cast at a glance. Every table is a Dataview query over the NPC notes.

## NPCs by location

```dataview
TABLE WITHOUT ID key AS "Location", rows.file.link AS "NPC", rows.role AS "Role"
FROM "NPCs"
GROUP BY location
```

## Attitude towards the party

```dataview
TABLE WITHOUT ID file.link AS "NPC", attitude AS "Attitude", status AS "Status", first_met AS "First met"
FROM "NPCs"
SORT attitude ASC, first_met ASC
```

## Faction members

```dataview
TABLE WITHOUT ID key AS "Faction", length(rows) AS "Count", rows.file.link AS "NPC"
FROM "NPCs"
WHERE faction
GROUP BY faction
```

## Quick NPCs ready to improvise

```dataview
TABLE WITHOUT ID file.link AS "NPC", role AS "Role", wants AS "Wants"
FROM "Quick NPCs"
```

## Unrevealed secrets

```dataview
LIST secret
FROM "NPCs"
WHERE revealed = false
```
