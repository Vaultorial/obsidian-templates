---
type: company
industry: santé
website: https://calderdental.example.com
tags: [crm/company]
---
# Calder Dental Clinics

Deux cabinets dentaires qui partagent un système de rendez-vous. Les décisions passent par la gérante.

## Personnes

```dataview
TABLE WITHOUT ID file.link AS "Contact", role AS "Fonction", last_contact AS "Dernier contact"
FROM "Contacts" AND [[]]
```

## Affaires

```dataview
TABLE WITHOUT ID file.link AS "Affaire", stage AS "Étape", value AS "Montant (EUR)"
FROM "Affaires" AND [[]]
```
