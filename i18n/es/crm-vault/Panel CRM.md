# Panel CRM

Vistas en vivo de todo el CRM. Todo lo que hay aquí son consultas de Dataview sobre las notas del vault.

## Seguimientos de los próximos 7 días

```dataview
TABLE WITHOUT ID file.link AS "Contacto", company AS "Empresa", next_follow_up AS "Seguimiento"
FROM "Contactos"
WHERE next_follow_up AND next_follow_up <= date(today) + dur(7 days)
SORT next_follow_up ASC
```

## Tareas abiertas de las interacciones

```dataview
TASK
FROM "Interacciones"
WHERE !completed
GROUP BY file.link
```

## Embudo por fase

```dataview
TABLE WITHOUT ID key AS "Fase", length(rows) AS "Oportunidades", sum(rows.value) AS "Importe del embudo (EUR)"
FROM "Oportunidades"
WHERE stage != "perdido"
GROUP BY stage
```

## Oportunidades abiertas

```dataview
TABLE WITHOUT ID file.link AS "Oportunidad", company AS "Empresa", stage AS "Fase", value AS "Importe (EUR)", close_date AS "Cierre"
FROM "Oportunidades"
WHERE stage != "ganado" AND stage != "perdido"
SORT close_date ASC
```

## Sin contacto en 60 días

```dataview
TABLE WITHOUT ID file.link AS "Contacto", company AS "Empresa", last_contact AS "Último contacto"
FROM "Contactos"
WHERE last_contact AND date(today) - last_contact > dur(60 days)
SORT last_contact ASC
```

## Interacciones recientes

```dataview
TABLE WITHOUT ID file.link AS "Interacción", contact AS "Contacto", channel AS "Canal"
FROM "Interacciones"
SORT date DESC
LIMIT 8
```
