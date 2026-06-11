---
type: dashboard
---

# Panel

Abre esta nota en vista de lectura. Cada sección es una query en vivo sobre todo el vault — las tareas se quedan en sus notas de proyecto y listas, y afloran aquí automáticamente. Las vistas reflejan el día en que abres el vault.

## Vencen hoy

```tasks
not done
due today
tags do not include #espera
```

## Vencidas

```tasks
not done
due before today
tags do not include #espera
sort by due
```

## Próximamente

Las diez próximas tareas con fecha, las más cercanas primero.

```tasks
not done
due after today
tags do not include #espera
sort by due
limit 10
```

## Por contexto

### Casa

```tasks
not done
tags include #contexto/casa
sort by priority
```

### Ordenador

```tasks
not done
tags include #contexto/ordenador
sort by priority
```

### Recados

```tasks
not done
tags include #contexto/recados
sort by priority
```

## En espera

```tasks
not done
tags include #espera
sort by due
```

## Bandeja por procesar

Apunta a cero. Procésala durante la revisión semanal.

```tasks
not done
path includes 00 Bandeja de entrada
```

## Resumen de proyectos

> [!note] Requiere Dataview
> Esta tabla necesita el plugin Dataview. Todo lo de arriba funciona solo con Tasks.

```dataview
TABLE status, area, outcome
FROM "Proyectos"
SORT status ASC, file.name ASC
```
