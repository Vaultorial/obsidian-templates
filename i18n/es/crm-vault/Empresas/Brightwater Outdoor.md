---
type: company
industry: comercio
website: https://brightwater.example.com
tags: [crm/company]
---
# Brightwater Outdoor

Tienda de material de montaña, online y dos locales. Campañas de temporada con plazos cortos.

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
