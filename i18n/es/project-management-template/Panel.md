---
type: dashboard
---

# Panel

Ábrelo en vista de lectura con Dataview activado. Cada tabla de abajo se genera a partir del frontmatter de las notas en `Proyectos/` y `Reuniones/` — nada de esta página se mantiene a mano.

## Proyectos activos

```dataview
TABLE owner, area, start, due
FROM "Proyectos"
WHERE status = "activo"
SORT due ASC
```

## Todos los proyectos por estado

```dataview
TABLE rows.file.link AS "Proyectos", rows.owner AS "Responsable"
FROM "Proyectos"
GROUP BY status
```

## Proyectos por responsable

```dataview
TABLE rows.file.link AS "Proyectos", rows.due AS "Vencimiento"
FROM "Proyectos"
GROUP BY owner
```

## Vencen en los próximos 30 días

```dataview
TABLE owner, status, due
FROM "Proyectos"
WHERE status != "hecho" AND due <= date(today) + dur(30 days)
SORT due ASC
```

## Reuniones recientes

```dataview
TABLE project, date
FROM "Reuniones"
SORT date DESC
LIMIT 10
```

## Elementos de acción abiertos de las reuniones

Cada casilla sin marcar de todas las notas de reunión. Márcalas en la nota de reunión donde viven.

```dataview
TASK
FROM "Reuniones"
WHERE !completed
```
