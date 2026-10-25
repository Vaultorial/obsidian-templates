---
type: index
---

# Party Sheet

One page for the table: who is in the party, how hurt everyone is and who to ask for a check. Every number comes from the properties of the character notes.

## The party at a glance

```dataview
TABLE WITHOUT ID file.link AS "Character", class AS "Class", level AS "Level", ac AS "AC", hp + " / " + max_hp AS "HP", 10 + floor((wis - 10) / 2) + choice(contains(skills, "Perception"), floor((level - 1) / 4) + 2, 0) AS "Passive Perception"
FROM "Characters"
SORT file.name ASC
```

## Who needs healing

```dataview
TABLE WITHOUT ID file.link AS "Character", hp AS "Current HP", max_hp - hp AS "Missing"
FROM "Characters"
WHERE hp < max_hp
SORT (max_hp - hp) DESC
```

## Who is good at what

Proficient skills and expertise for each character, for when the DM asks who wants to try.

```dataview
TABLE WITHOUT ID file.link AS "Character", skills AS "Proficient skills", expertise AS "Expertise"
FROM "Characters"
SORT file.name ASC
```
