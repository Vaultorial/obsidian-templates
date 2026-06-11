# Página de inicio / Dashboard — Plantilla para Obsidian

Un sistema de página de inicio para Obsidian: una nota-panel con las tareas de hoy, la semana entrante, los proyectos activos, las notas editadas recientemente y los recuentos del vault — en dos variantes. `Inicio (simple)` funciona con callouts y enlaces estáticos sin ningún plugin; `Inicio` es la versión viva, impulsada por consultas de Dataview sobre fechas de tarea `[due:: ]` y pensada para abrirse al arrancar con el plugin Homepage. Incluye un vault de ejemplo pequeño pero del todo interconectado (3 proyectos, 2 áreas, 3 notas permanentes con tareas fechadas realistas), de modo que cada sección del panel muestra datos reales desde el primer momento.

## Estructura de carpetas

```
homepage-dashboard/
├── Empieza aquí.md          ← lee esto primero
├── Inicio.md                ← panel vivo (Dataview)
├── Inicio (simple).md       ← panel sin plugins
├── Proyectos/               ← 3 proyectos de ejemplo con tareas fechadas
├── Áreas/                   ← 2 áreas continuas con tareas fechadas
└── Notas/                   ← 3 notas permanentes (lista, checklist, receta)
```

## Instalación

1. Descomprime la descarga.
2. Abre Obsidian → **Abrir carpeta como vault** → selecciona la carpeta descomprimida.
3. Confía en el vault cuando te lo pregunte (solo trae ajustes en JSON plano).
4. Abre `Empieza aquí.md` y luego `Inicio (simple)` — funciona de inmediato. Instala los plugins de abajo para dar vida a `Inicio`.

Para usarlo dentro de un vault existente, copia `Inicio.md` e `Inicio (simple).md` y ajusta los nombres de carpeta de las consultas (`FROM "Proyectos" OR "Áreas"`) a tu estructura.

## Plugins

Obligatorio para el panel vivo:

- **Dataview** — ejecuta las consultas de `Inicio.md`. https://obsidian.md/plugins?id=dataview

Opcional:

- **Homepage** — abre tu panel automáticamente al arrancar. https://obsidian.md/plugins?id=homepage

`Inicio (simple).md` no necesita ningún plugin.

## Licencia

MIT. Úsala, modifícala, publícala — sin atribución obligatoria.

Plantilla de Vaultorial — https://vaultorial.com/es/dashboard-de-inicio/
