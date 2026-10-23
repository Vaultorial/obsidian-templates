---
type: contact
company:
role:
relationship: Interessent
last_contact: {{date:YYYY-MM-DD}}
next_follow_up:
tags: [crm/contact]
---
# {{title}}

Wer die Person ist, wie ihr euch kennt, was ihr wichtig ist.

## Interaktionen

```dataview
TABLE WITHOUT ID file.link AS "Interaktion", channel AS "Kanal", date AS "Datum"
FROM "Interaktionen" AND [[]]
SORT date DESC
```
