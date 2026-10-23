# CRM Dashboard

Live views of the whole CRM. Everything here is a Dataview query over the notes in this vault.

## Follow-ups due in the next 7 days

```dataview
TABLE WITHOUT ID file.link AS "Contact", company AS "Company", next_follow_up AS "Follow up"
FROM "Contacts"
WHERE next_follow_up AND next_follow_up <= date(today) + dur(7 days)
SORT next_follow_up ASC
```

## Open tasks from interactions

```dataview
TASK
FROM "Interactions"
WHERE !completed
GROUP BY file.link
```

## Pipeline by stage

```dataview
TABLE WITHOUT ID key AS "Stage", length(rows) AS "Deals", sum(rows.value) AS "Pipeline value (USD)"
FROM "Deals"
WHERE stage != "lost"
GROUP BY stage
```

## Open deals

```dataview
TABLE WITHOUT ID file.link AS "Deal", company AS "Company", stage AS "Stage", value AS "Value (USD)", close_date AS "Close date"
FROM "Deals"
WHERE stage != "won" AND stage != "lost"
SORT close_date ASC
```

## Not contacted in 60 days

```dataview
TABLE WITHOUT ID file.link AS "Contact", company AS "Company", last_contact AS "Last contact"
FROM "Contacts"
WHERE last_contact AND date(today) - last_contact > dur(60 days)
SORT last_contact ASC
```

## Recent interactions

```dataview
TABLE WITHOUT ID file.link AS "Interaction", contact AS "Contact", channel AS "Channel"
FROM "Interactions"
SORT date DESC
LIMIT 8
```
