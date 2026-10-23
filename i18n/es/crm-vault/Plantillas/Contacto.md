---
type: contact
company:
role:
relationship: prospecto
last_contact: {{date:YYYY-MM-DD}}
next_follow_up:
tags: [crm/contact]
---
# {{title}}

Quién es, cómo os conocisteis, qué le importa.

## Interacciones

```dataview
TABLE WITHOUT ID file.link AS "Interacción", channel AS "Canal", date AS "Fecha"
FROM "Interacciones" AND [[]]
SORT date DESC
```
