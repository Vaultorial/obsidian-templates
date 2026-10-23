---
type: company
industry:
website:
tags: [crm/company]
---
# {{title}}

## Personas

```dataview
TABLE WITHOUT ID file.link AS "Contacto", role AS "Cargo", last_contact AS "Último contacto"
FROM "Contactos" AND [[]]
```

## Oportunidades

```dataview
TABLE WITHOUT ID file.link AS "Oportunidad", stage AS "Fase", value AS "Importe (EUR)"
FROM "Oportunidades" AND [[]]
```
