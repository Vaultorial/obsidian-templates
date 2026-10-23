---
type: company
industry: logistique
website: https://harrowgate.example.com
tags: [crm/company]
---
# Harrowgate Logistics

Transporteur régional avec trois entrepôts. La plus grosse affaire ouverte du pipeline.

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
