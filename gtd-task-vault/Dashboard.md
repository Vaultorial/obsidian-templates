---
type: dashboard
---

# Dashboard

Open this note in reading view. Every section is a live query over the whole vault — tasks stay in their project notes and lists, and surface here automatically. The views reflect the day you open the vault.

## Due today

```tasks
not done
due today
tags do not include #waiting
```

## Overdue

```tasks
not done
due before today
tags do not include #waiting
sort by due
```

## Coming up

The next ten dated tasks, nearest first.

```tasks
not done
due after today
tags do not include #waiting
sort by due
limit 10
```

## By context

### Home

```tasks
not done
tags include #context/home
sort by priority
```

### Computer

```tasks
not done
tags include #context/computer
sort by priority
```

### Errands

```tasks
not done
tags include #context/errands
sort by priority
```

## Waiting for

```tasks
not done
tags include #waiting
sort by due
```

## Inbox to process

Aim for zero. Process during the weekly review.

```tasks
not done
path includes 00 Inbox
```

## Projects overview

> [!note] Requires Dataview
> This table needs the Dataview plugin. Everything above runs on Tasks alone.

```dataview
TABLE status, area, outcome
FROM "Projects"
SORT status ASC, file.name ASC
```
