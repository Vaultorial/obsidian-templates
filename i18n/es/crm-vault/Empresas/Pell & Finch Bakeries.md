---
type: company
industry: alimentación
website: https://pellandfinch.example.com
tags: [crm/company]
---
# Pell & Finch Bakeries

Cadena familiar de panaderías, seis tiendas. Rebranding entregado en septiembre, ahora cliente de referencia.

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
