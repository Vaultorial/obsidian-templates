# Pack de notas de reunión — plantilla de Obsidian

Cinco plantillas de notas de reunión para Obsidian — reunión de equipo, 1-on-1, llamada con cliente, daily standup y retrospectiva — con frontmatter estructurado, una disposición consistente de agenda/notas/decisiones/elementos de acción, y un panel Dataview que aflora cada reunión y cada elemento de acción abierto. Incluye cuatro reuniones de ejemplo rellenadas de un mismo proyecto para que el panel funcione en el primer abrir.

Los elementos de acción usan la sintaxis de fecha del plugin Tasks (`- [ ] Responsable — acción 📅 2026-06-15`), así que pueden trasladarse directamente a un vault GTD con el plugin Tasks.

## Estructura

```
meeting-notes-template/
├── Empieza aquí.md           ← lee esto primero
├── Panel de reuniones.md     ← Dataview: por tipo, por proyecto, elementos de acción abiertos
├── Plantillas/
│   ├── Reunión de equipo.md
│   ├── 1-on-1.md
│   ├── Llamada con cliente.md
│   ├── Daily standup.md
│   └── Retrospectiva.md
└── Reuniones/                ← seis ejemplos rellenados, un mismo proyecto coherente
    ├── 2026-05-04 Arranque del portal de cliente.md
    ├── 2026-05-11 1-on-1 Sarah y Priya.md
    ├── 2026-05-14 Llamada con cliente Brightleaf.md
    ├── 2026-05-19 Daily standup del portal de cliente.md
    ├── 2026-06-01 Revisión de sprint del portal de cliente.md
    └── 2026-06-02 Retrospectiva de sprint del portal de cliente.md
```

## Instalación

1. Descarga y descomprime la plantilla: **Descomprimir → Obsidian → Abrir una carpeta como bóveda**.
2. Cuando Obsidian lo pregunte, activa los plugins de la comunidad para este vault.
3. Instala Dataview y abre `Panel de reuniones.md` en vista de lectura.

## Plugins

**Obligatorios**

- Dataview — https://obsidian.md/plugins?id=dataview

**Opcionales**

- Templater — https://obsidian.md/plugins?id=templater-obsidian (cambia las variables del core Templates por dinámicas si ya lo usas)

## Licencia

MIT. Úsalo, cámbialo, compártelo — la atribución se agradece pero no es obligatoria.

Plantilla de Vaultorial — https://vaultorial.com/es/plantilla-notas-de-reunion/
