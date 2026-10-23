---
type: company
industry: commerce
website: https://brightwater.example.com
tags: [crm/company]
---
# Brightwater Outdoor

Magasin de matériel outdoor, en ligne et deux boutiques. Campagnes saisonnières, délais courts.

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
