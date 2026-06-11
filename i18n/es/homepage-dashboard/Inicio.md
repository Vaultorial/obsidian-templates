---
type: panel
---

# Inicio

> [!info] Ir directo a
> **Proyectos:** [[Huerto de balcón para el verano|Huerto de balcón]] · [[Renovación de la web del portfolio|Portfolio]] · [[Curso de conversación en italiano|Italiano]]
> **Áreas:** [[Salud y forma física]] · [[Mantenimiento del hogar]]
> **Permanentes:** [[Lista de lectura]] · [[Checklist de reinicio semanal]] · [[Salsa de tomate que funciona]]
> ¿Recién llegado? Lee antes [[Empieza aquí]] — o abre [[Inicio (simple)]], la versión sin plugins de esta página.

## Hoy

Tareas abiertas que vencen hoy o ya atrasadas, extraídas de todos los proyectos y áreas.

```dataview
TASK
FROM "Proyectos" OR "Áreas"
WHERE !completed AND due AND due <= date(today)
SORT due ASC
```

## Próximos días (7 días)

```dataview
TASK
FROM "Proyectos" OR "Áreas"
WHERE !completed AND due AND due > date(today) AND due <= date(today) + dur(7 days)
SORT due ASC
```

## Proyectos activos

```dataview
TABLE WITHOUT ID file.link AS "Proyecto", status AS "Estado", started AS "Inicio"
FROM "Proyectos"
WHERE status = "activo"
SORT started ASC
```

## Tocado hace poco

```dataview
TABLE WITHOUT ID file.link AS "Nota", dateformat(file.mtime, "ccc d MMM, HH:mm") AS "Última edición"
FROM "Proyectos" OR "Áreas" OR "Notas"
SORT file.mtime DESC
LIMIT 7
```

## El vault de un vistazo

```dataview
TABLE WITHOUT ID Carpeta AS "Carpeta", length(rows) AS "Notas"
FROM "Proyectos" OR "Áreas" OR "Notas"
GROUP BY file.folder AS Carpeta
SORT Carpeta ASC
```

> [!tip] Por qué las tareas llevan `[due:: fecha]`
> Ese campo inline es lo que permite a las consultas de arriba barrer todos los proyectos y áreas por ti. Ponle fecha a una tarea y olvídala — esta página se acuerda. La rutina del domingo de [[Checklist de reinicio semanal]] mantiene los datos honestos.
