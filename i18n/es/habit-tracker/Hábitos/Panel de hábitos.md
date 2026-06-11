---
type: panel-de-hábitos
---

# Panel de hábitos

Lee las pequeñas notas por día de `Hábitos/Registro diario` (cada una lleva los cinco hábitos como frontmatter de verdadero/falso) y las resume. Requiere el plugin **Dataview** — instálalo y actívalo, y estos bloques cobran vida.

## Rachas actuales

Días consecutivos por hábito, contando hacia atrás desde el último día registrado. Requiere las *consultas JavaScript* activadas en los ajustes de Dataview; si prefieres no activar JS, borra este bloque sin más — todo lo de abajo es Dataview normal.

```dataviewjs
const habits = [
	["read", "Leer 20 min"],
	["walk", "Caminar 30 min"],
	["no_sugar", "Sin azúcar"],
	["sleep_on_time", "Acostarse antes de las 23:30"],
	["journal", "Diario"],
];
const logs = dv.pages('"Hábitos/Registro diario"').values.sort((a, b) => b.date - a.date);
const rows = habits.map(([key, label]) => {
	let streak = 0;
	for (const p of logs) {
		if (p[key] === true) streak++;
		else break;
	}
	return [label, streak + (streak === 1 ? " día" : " días")];
});
dv.table(["Hábito", "Racha (hasta el último día registrado)"], rows);
```

## Días cumplidos, mes a mes

```dataview
TABLE length(rows) AS "Días registrados",
	length(filter(rows.read, (x) => x)) AS "Leer",
	length(filter(rows.walk, (x) => x)) AS "Caminar",
	length(filter(rows.no_sugar, (x) => x)) AS "Sin azúcar",
	length(filter(rows.sleep_on_time, (x) => x)) AS "Acostarse",
	length(filter(rows.journal, (x) => x)) AS "Diario"
FROM "Hábitos/Registro diario"
GROUP BY dateformat(date, "yyyy-MM") AS Mes
SORT Mes DESC
```

## Últimos 14 días registrados

```dataview
TABLE WITHOUT ID file.link AS "Día",
	read AS "Leer", walk AS "Caminar", no_sugar AS "Sin azúcar",
	sleep_on_time AS "Acostarse", journal AS "Diario"
FROM "Hábitos/Registro diario"
SORT date DESC
LIMIT 14
```

## Días perfectos

Los cinco hábitos cumplidos el mismo día.

```dataview
LIST
FROM "Hábitos/Registro diario"
WHERE read AND walk AND no_sugar AND sleep_on_time AND journal
SORT date DESC
```

> [!tip] Renombrar hábitos
> Las claves del frontmatter (`read`, `walk`, `no_sugar`, `sleep_on_time`, `journal`) son el contrato entre tus registros diarios y este panel. Si cambias un hábito, cambia su clave en `Plantillas/Entrada de registro diario` **y** en todas las consultas de aquí — y estrena registros nuevos en vez de reescribir la historia.
