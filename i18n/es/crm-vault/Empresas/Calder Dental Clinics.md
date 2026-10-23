---
type: company
industry: salud
website: https://calderdental.example.com
tags: [crm/company]
---
# Calder Dental Clinics

Dos clínicas dentales con un mismo sistema de citas. Las decisiones pasan por la gerente.

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
