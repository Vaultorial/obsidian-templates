---
type: company
industry: healthcare
website: https://calderdental.example.com
tags: [crm/company]
---
# Calder Dental Clinics

Two dental clinics sharing one booking system. Decisions go through the practice manager.

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
