---
type: tableau-de-bord-habitudes
---

# Tableau de bord des habitudes

Lit les petites notes par jour de `Habitudes/Journal quotidien` (chacune porte les cinq habitudes en frontmatter vrai/faux) et les résume. Nécessite le plugin **Dataview** — installez-le et activez-le, et ces blocs prennent vie.

## Séries en cours

Jours consécutifs par habitude, comptés à rebours depuis le dernier jour consigné. Nécessite *JavaScript queries* activé dans les réglages de Dataview ; si vous préférez laisser le JS désactivé, supprimez simplement ce bloc — tout ce qui suit est du Dataview ordinaire.

```dataviewjs
const habits = [
	["read", "Lire 20 min"],
	["walk", "Marcher 30 min"],
	["no_sugar", "Zéro sucre"],
	["sleep_on_time", "Coucher avant 23 h 30"],
	["journal", "Journal"],
];
const logs = dv.pages('"Habitudes/Journal quotidien"').values.sort((a, b) => b.date - a.date);
const rows = habits.map(([key, label]) => {
	let streak = 0;
	for (const p of logs) {
		if (p[key] === true) streak++;
		else break;
	}
	return [label, streak + (streak === 1 ? " jour" : " jours")];
});
dv.table(["Habitude", "Série (jusqu'au dernier jour consigné)"], rows);
```

## Jours tenus, mois par mois

```dataview
TABLE length(rows) AS "Jours consignés",
	length(filter(rows.read, (x) => x)) AS "Lire",
	length(filter(rows.walk, (x) => x)) AS "Marcher",
	length(filter(rows.no_sugar, (x) => x)) AS "Zéro sucre",
	length(filter(rows.sleep_on_time, (x) => x)) AS "Coucher",
	length(filter(rows.journal, (x) => x)) AS "Journal"
FROM "Habitudes/Journal quotidien"
GROUP BY dateformat(date, "yyyy-MM") AS Mois
SORT Mois DESC
```

## Les 14 derniers jours consignés

```dataview
TABLE WITHOUT ID file.link AS "Jour",
	read AS "Lire", walk AS "Marcher", no_sugar AS "Zéro sucre",
	sleep_on_time AS "Coucher", journal AS "Journal"
FROM "Habitudes/Journal quotidien"
SORT date DESC
LIMIT 14
```

## Jours parfaits

Les cinq habitudes tenues le même jour.

```dataview
LIST
FROM "Habitudes/Journal quotidien"
WHERE read AND walk AND no_sugar AND sleep_on_time AND journal
SORT date DESC
```

> [!tip] Renommer une habitude
> Les clés du frontmatter (`read`, `walk`, `no_sugar`, `sleep_on_time`, `journal`) sont le contrat entre vos journaux quotidiens et ce tableau de bord. Si vous changez une habitude, changez sa clé dans `Modèles/Entrée de journal quotidien` **et** dans chaque requête ici — et repartez sur des journaux neufs plutôt que de réécrire l'histoire.
