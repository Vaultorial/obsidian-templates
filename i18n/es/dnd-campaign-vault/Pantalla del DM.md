---
type: panel
---

# Pantalla del DM

Ábrela en vista de lectura con Dataview activado. Todo lo de abajo se actualiza solo desde el frontmatter de las notas de la campaña.

## Dónde está la campaña

- Última jugada: [[Sesión 3 - Sal en la herida]]
- Preparado y listo: [[Asalto a la Contaduría]]
- El grupo: [[Kestrel Thorne]], [[Bram Tuckett]], [[Yneva Marsh]]
- Columna vertebral de la trama: [[La Ruta de la Sal]] · [[El Consorcio Carrow]] · [[Los Custodios del Salitre]]

## PNJ por lugar

```dataview
TABLE rows.file.link AS "PNJ", rows.role AS "Rol", rows.status AS "Estado"
FROM "PNJ"
GROUP BY location
```

## PNJ por facción

```dataview
TABLE rows.file.link AS "PNJ", rows.role AS "Rol"
FROM "PNJ"
GROUP BY faction
```

## Sesiones, la más reciente primero

```dataview
TABLE date AS "Fecha", number AS "N.º"
FROM "Sesiones"
SORT date DESC
```

## Encuentros listos para jugar

```dataview
TABLE location AS "Lugar", difficulty AS "Dificultad"
FROM "Encuentros"
WHERE status = "preparado"
```

## Encuentros ya jugados

```dataview
TABLE location AS "Lugar", difficulty AS "Dificultad"
FROM "Encuentros"
WHERE status = "jugado"
SORT file.name ASC
```

## El grupo

```dataview
TABLE player AS "Jugador", class AS "Clase", level AS "Nivel", ancestry AS "Linaje"
FROM "PJ"
SORT file.name ASC
```
