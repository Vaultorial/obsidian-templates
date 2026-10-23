---
type: company
industry: logística
website: https://harrowgate.example.com
tags: [crm/company]
---
# Harrowgate Logistics

Operador regional de transporte con tres almacenes. La mayor oportunidad abierta del embudo.

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
