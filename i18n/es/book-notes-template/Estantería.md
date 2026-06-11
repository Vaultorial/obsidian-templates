---
type: bookshelf
tags: [bookshelf]
---

# Estantería

Montada por Dataview a partir del frontmatter de cada nota en `Libros/`. Nada de esta página se mantiene a mano.

**Mi escala de valoración:** 5 = lo releeré y se lo endoso a los amigos · 4 = cambió algo que hago · 3 = bueno, una idea valió el tiempo · 2 = correcto, olvidable · 1 = abandonado con motivo.

## Leyendo ahora

```dataview
TABLE author AS "Autor", genre AS "Género", row["date-started"] AS "Empezado"
FROM "Libros"
WHERE status = "leyendo"
```

## Leídos — por valoración

```dataview
TABLE author AS "Autor", rating AS "Valoración", row["date-finished"] AS "Terminado"
FROM "Libros"
WHERE status = "leído"
SORT rating DESC
```

## Por leer

```dataview
LIST author
FROM "Libros"
WHERE status = "por leer"
```

## Todo, por autor

```dataview
TABLE author AS "Autor", status AS "Estado", rating AS "Valoración"
FROM "Libros"
SORT author ASC
```

> [!note] Si los estantes están vacíos
> Dataview aún no está activado — mira [[Empieza aquí]] para la configuración de un minuto.
