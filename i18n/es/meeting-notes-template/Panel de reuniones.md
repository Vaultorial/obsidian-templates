---
type: dashboard
---

# Panel de reuniones

Ábrelo en vista de lectura con Dataview activado. Todo lo de abajo se genera a partir del frontmatter y las casillas de las notas en `Reuniones/`.

## Reuniones recientes

```dataview
TABLE type, project, attendees
FROM "Reuniones"
SORT date DESC
LIMIT 15
```

## Por tipo

```dataview
TABLE rows.file.link AS "Reuniones", rows.date AS "Fecha"
FROM "Reuniones"
GROUP BY type
```

## Por proyecto

```dataview
TABLE rows.file.link AS "Reuniones", rows.type AS "Tipo"
FROM "Reuniones"
GROUP BY project
```

## Elementos de acción abiertos

Cada elemento de acción sin marcar de todas las reuniones, agrupado por la reunión de la que salió. Márcalos donde viven.

```dataview
TASK
FROM "Reuniones"
WHERE !completed
```

## Registro de decisiones

Lista de salto rápido — las decisiones viven bajo el encabezado `## Decisiones` de cada nota.

```dataview
LIST
FROM "Reuniones"
SORT date ASC
```
