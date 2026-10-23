---
type: company
industry: Lebensmittelhandel
website: https://pellandfinch.example.com
tags: [crm/company]
---
# Pell & Finch Bakeries

Familienbäckerei mit sechs Filialen. Rebranding im September geliefert, jetzt Referenzkunde.

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
