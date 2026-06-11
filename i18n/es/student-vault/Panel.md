---
type: dashboard
tags: [dashboard]
---

# Panel

Construido por Dataview a partir del frontmatter de cada nota. Cualquier cosa con una fecha `due` aparece abajo automáticamente — nada de aquí se mantiene a mano.

## Próximas entregas

```dataview
TABLE course AS "Asignatura", type AS "Tipo", due AS "Entrega"
FROM "Primavera 2026"
WHERE due AND due >= date(today)
SORT due ASC
```

## Exámenes

```dataview
TABLE course AS "Asignatura", topic AS "Tema", due AS "Fecha"
FROM "Primavera 2026"
WHERE type = "exam"
SORT due ASC
```

## Tareas de lectura

```dataview
TABLE course AS "Asignatura", source AS "Fuente", due AS "Entrega"
FROM "Primavera 2026"
WHERE type = "reading"
SORT due ASC
```

## Todo por asignatura

```dataview
TABLE type AS "Tipo", topic AS "Tema", due AS "Entrega"
FROM "Primavera 2026"
SORT course ASC, due ASC
```

> [!note] ¿Tablas vacías?
> Dataview aún no está activado — mira [[Empieza aquí]] para configurarlo. Los elementos ya vencidos desaparecen solos de la tabla de entregas; la tabla por asignatura de abajo sigue mostrándolo todo.
