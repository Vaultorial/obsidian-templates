---
type: company
industry: Gesundheit
website: https://calderdental.example.com
tags: [crm/company]
---
# Calder Dental Clinics

Zwei Zahnarztpraxen mit gemeinsamem Buchungssystem. Entscheidungen laufen über die Praxismanagerin.

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
