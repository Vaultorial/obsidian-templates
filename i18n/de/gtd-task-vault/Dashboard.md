---
type: dashboard
---

# Dashboard

Öffne diese Notiz in der Leseansicht. Jeder Abschnitt ist eine Live-Query über den ganzen Vault — Aufgaben bleiben in ihren Projektnotizen und Listen und tauchen hier automatisch auf. Die Ansichten spiegeln den Tag wider, an dem du den Vault öffnest.

## Heute fällig

```tasks
not done
due today
tags do not include #warten
```

## Überfällig

```tasks
not done
due before today
tags do not include #warten
sort by due
```

## Demnächst

Die nächsten zehn datierten Aufgaben, die nächste zuerst.

```tasks
not done
due after today
tags do not include #warten
sort by due
limit 10
```

## Nach Kontext

### Zuhause

```tasks
not done
tags include #kontext/zuhause
sort by priority
```

### Computer

```tasks
not done
tags include #kontext/computer
sort by priority
```

### Besorgungen

```tasks
not done
tags include #kontext/besorgungen
sort by priority
```

## Warten auf

```tasks
not done
tags include #warten
sort by due
```

## Inbox zum Verarbeiten

Ziel ist null. Im Wochenrückblick verarbeiten.

```tasks
not done
path includes 00 Inbox
```

## Projektübersicht

> [!note] Erfordert Dataview
> Diese Tabelle braucht das Dataview-Plugin. Alles darüber läuft allein mit Tasks.

```dataview
TABLE status, area, outcome
FROM "Projekte"
SORT status ASC, file.name ASC
```
