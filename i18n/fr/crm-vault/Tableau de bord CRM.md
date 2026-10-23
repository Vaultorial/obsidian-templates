# Tableau de bord CRM

Vues en direct de tout le CRM. Tout ce qui figure ici est une requête Dataview sur les notes du vault.

## Relances des 7 prochains jours

```dataview
TABLE WITHOUT ID file.link AS "Contact", company AS "Entreprise", next_follow_up AS "Relance"
FROM "Contacts"
WHERE next_follow_up AND next_follow_up <= date(today) + dur(7 days)
SORT next_follow_up ASC
```

## Tâches ouvertes issues des échanges

```dataview
TASK
FROM "Interactions"
WHERE !completed
GROUP BY file.link
```

## Pipeline par étape

```dataview
TABLE WITHOUT ID key AS "Étape", length(rows) AS "Affaires", sum(rows.value) AS "Montant du pipeline (EUR)"
FROM "Affaires"
WHERE stage != "perdu"
GROUP BY stage
```

## Affaires en cours

```dataview
TABLE WITHOUT ID file.link AS "Affaire", company AS "Entreprise", stage AS "Étape", value AS "Montant (EUR)", close_date AS "Clôture"
FROM "Affaires"
WHERE stage != "gagné" AND stage != "perdu"
SORT close_date ASC
```

## Sans contact depuis 60 jours

```dataview
TABLE WITHOUT ID file.link AS "Contact", company AS "Entreprise", last_contact AS "Dernier contact"
FROM "Contacts"
WHERE last_contact AND date(today) - last_contact > dur(60 days)
SORT last_contact ASC
```

## Échanges récents

```dataview
TABLE WITHOUT ID file.link AS "Échange", contact AS "Contact", channel AS "Canal"
FROM "Interactions"
SORT date DESC
LIMIT 8
```
