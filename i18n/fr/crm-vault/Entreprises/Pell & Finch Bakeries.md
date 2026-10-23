---
type: company
industry: alimentaire
website: https://pellandfinch.example.com
tags: [crm/company]
---
# Pell & Finch Bakeries

Chaîne familiale de six boulangeries. Refonte de marque livrée en septembre, client de référence.

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
