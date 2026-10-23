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

Qui c'est, comment vous vous êtes rencontrés, ce qui compte pour cette personne.

## Interactions

```dataview
TABLE WITHOUT ID file.link AS "Échange", channel AS "Canal", date AS "Date"
FROM "Interactions" AND [[]]
SORT date DESC
```
