# Vault de diagrama de Gantt — Plantilla de Obsidian

Diagramas de Gantt dibujados a partir de tus notas: cada tarea es una nota con fechas de inicio y fin en sus propiedades, y una consulta DataviewJS las convierte en un diagrama de Gantt de Mermaid por proyecto, con una sección por fase. Incluye dos proyectos de ejemplo, un ejemplo estático sin plugins y una plantilla de tarea.

## Estructura

```
gantt-chart-template/
├── Empieza aquí.md                 ← léelo primero
├── Cronograma.md                   ← los diagramas generados
├── Ejemplo de Gantt estático.md    ← diagrama escrito a mano, sin plugins
├── Proyectos/                      ← 2 proyectos de ejemplo, 14 tareas fechadas
└── Plantillas/                     ← nota de tarea en blanco
```

## Instalación

1. Descarga y descomprime la plantilla: **Descomprimir → Obsidian → Abrir carpeta como vault**.
2. Cuando Obsidian lo pregunte, activa los plugins de la comunidad para este vault.
3. Instala Dataview, activa *JavaScript queries* en sus ajustes y abre `Cronograma.md`.

## Plugins

**Obligatorios**

- Dataview — https://obsidian.md/plugins?id=dataview

## Licencia

MIT. Úsala, cámbiala, compártela; se agradece la atribución, pero no es obligatoria.

Plantilla de Vaultorial — https://vaultorial.com/es/plantilla-diagrama-de-gantt/
