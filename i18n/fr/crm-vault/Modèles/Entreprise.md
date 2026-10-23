---
type: company
industry:
website:
tags: [crm/company]
---
# {{title}}

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
