# Lista de PNJ

Todo el reparto de un vistazo. Cada tabla es una consulta de Dataview sobre las notas de PNJ.

## PNJ por lugar

```dataview
TABLE WITHOUT ID key AS "Lugar", rows.file.link AS "PNJ", rows.role AS "Papel"
FROM "PNJ"
GROUP BY location
```

## Actitud hacia el grupo

```dataview
TABLE WITHOUT ID file.link AS "PNJ", attitude AS "Actitud", status AS "Estado", first_met AS "Primer encuentro"
FROM "PNJ"
SORT attitude ASC, first_met ASC
```

## Miembros de cada facción

```dataview
TABLE WITHOUT ID key AS "Facción", length(rows) AS "Número", rows.file.link AS "PNJ"
FROM "PNJ"
WHERE faction
GROUP BY faction
```

## PNJ rápidos listos para improvisar

```dataview
TABLE WITHOUT ID file.link AS "PNJ", role AS "Papel", wants AS "Quiere"
FROM "PNJ rápidos"
```

## Secretos por revelar

```dataview
LIST secret
FROM "PNJ"
WHERE revealed = false
```
