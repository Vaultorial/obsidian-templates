---
week: <% tp.file.title %>
start: <% moment(tp.file.title, "GGGG-[W]WW").startOf("isoWeek").format("YYYY-MM-DD") %>
end: <% moment(tp.file.title, "GGGG-[W]WW").endOf("isoWeek").format("YYYY-MM-DD") %>
type: semanal
---

# <% tp.file.title %> — <% moment(tp.file.title, "GGGG-[W]WW").startOf("isoWeek").format("D") %>–<% moment(tp.file.title, "GGGG-[W]WW").endOf("isoWeek").format("D [de] MMMM [de] YYYY") %>

← [[<% tp.date.now("GGGG-[W]WW", -7, tp.file.title, "GGGG-[W]WW") %>]] | [[<% tp.date.now("GGGG-[W]WW", 7, tp.file.title, "GGGG-[W]WW") %>]] →

## Plan de la semana

**Foco:**

- [ ]
- [ ]
- [ ]

## Revisión

### Logros

-

### Números

| Métrica | Objetivo | Real |
| ------- | -------- | ---- |
|         |          |      |

### Queda pendiente

-

### Foco de la semana siguiente

-

> [!note]- Cómo usar esta plantilla
> Variante de Templater. El rango de la semana y los enlaces anterior/siguiente se derivan del nombre del fichero, así que nombra la nota `2026-W24` (semana ISO) y aplica la plantilla con Templater. Configuración: instala Templater y define `Plantillas` como su carpeta de plantillas. Borra este callout de tu copia.
