---
type: company
industry:
website:
tags: [crm/company]
---
# {{title}}

## Personen

```dataview
TABLE WITHOUT ID file.link AS "Kontakt", role AS "Rolle", last_contact AS "Letzter Kontakt"
FROM "Kontakte" AND [[]]
```

## Deals

```dataview
TABLE WITHOUT ID file.link AS "Deal", stage AS "Phase", value AS "Wert (EUR)"
FROM "Deals" AND [[]]
```
