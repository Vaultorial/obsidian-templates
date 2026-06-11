# Vault de gestión de proyectos — plantilla de Obsidian

Un sistema de gestión de proyectos en ficheros planos para Obsidian. Cada proyecto es una sola nota con frontmatter estructurado, una tabla de hitos, una línea de tiempo Gantt Mermaid y notas de reunión enlazadas; un panel Dataview lo agrega todo por estado, responsable y fecha de vencimiento. Viene con dos ejemplos completos — un rediseño de web y una mudanza de oficina — incluidas cuatro notas de reunión realistas.

## Estructura

```
project-management-template/
├── Empieza aquí.md     ← lee esto primero
├── Panel.md            ← rollups Dataview: estado, responsable, vencimientos, elementos de acción
├── Proyectos/
│   ├── Rediseño de la web.md
│   └── Mudanza de oficina.md
├── Reuniones/          ← una nota por reunión, enlazada a su proyecto
│   ├── 2026-04-02 Arranque del rediseño de la web.md
│   ├── 2026-05-07 Revisión de diseño del rediseño de la web.md
│   ├── 2026-04-21 Visita de proveedor de la mudanza de oficina.md
│   └── 2026-05-19 Sincronización logística de la mudanza de oficina.md
└── Plantillas/
    ├── Plantilla de proyecto.md
    └── Plantilla de reunión.md
```

## Instalación

1. Descarga y descomprime la plantilla: **Descomprimir → Obsidian → Abrir carpeta como vault**.
2. Cuando Obsidian lo pregunte, activa los plugins de la comunidad para este vault.
3. Instala Dataview y abre `Panel.md` en vista de lectura.

## Plugins

**Obligatorios**

- Dataview — https://obsidian.md/plugins?id=dataview

Las líneas de tiempo Gantt usan el renderizado Mermaid integrado de Obsidian; sin plugin extra.

## Licencia

MIT. Úsalo, cámbialo, compártelo — la atribución se agradece pero no es obligatoria.

Plantilla de Vaultorial — https://vaultorial.com/es/plantilla-gestion-de-proyectos/
