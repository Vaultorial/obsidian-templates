---
type: company
industry: Logistik
website: https://harrowgate.example.com
tags: [crm/company]
---
# Harrowgate Logistics

Regionaler Logistiker mit drei Lagern. Die größte offene Chance in der Pipeline.

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
