---
type: contact
company:
role:
relationship: prospect
last_contact: {{date:YYYY-MM-DD}}
next_follow_up:
tags: [crm/contact]
---
# {{title}}

Who they are, how you met, what they care about.

## Interactions

```dataview
TABLE WITHOUT ID file.link AS "Interaction", channel AS "Channel", date AS "Date"
FROM "Interactions" AND [[]]
SORT date DESC
```
