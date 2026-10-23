---
type: company
industry: retail
website: https://brightwater.example.com
tags: [crm/company]
---
# Brightwater Outdoor

Outdoor gear retailer, online and two stores. Seasonal campaigns, short lead times.

## People

```dataview
TABLE WITHOUT ID file.link AS "Contact", role AS "Role", last_contact AS "Last contact"
FROM "Contacts" AND [[]]
```

## Deals

```dataview
TABLE WITHOUT ID file.link AS "Deal", stage AS "Stage", value AS "Value (USD)"
FROM "Deals" AND [[]]
```
