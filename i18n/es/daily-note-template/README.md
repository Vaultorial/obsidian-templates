# Plantilla de nota diaria — Plantilla para Obsidian

Un sistema limpio de notas diarias para Obsidian: una nota por día con secciones de **Agenda, Tareas, Registro y Gratitud**, navegación al día anterior y siguiente, y una semana de ejemplo completamente rellena para que veas el sistema en uso antes de comprometerte con él.

Se incluyen dos variantes de la plantilla: una que funciona solo con plugins core y otra basada en Templater con manejo automático de fechas.

## Estructura de carpetas

```
daily-note-template/
├── Empieza aquí.md                      ← lee esto primero
├── Diario/                              ← una nota por día (7 días de ejemplo, junio 2026)
│   ├── 2026-06-01.md … 2026-06-07.md
└── Plantillas/
    ├── Nota diaria (core Templates).md  ← sin plugins
    └── Nota diaria (Templater).md       ← añade enlaces ant./sig.
```

## Instalación

1. Descomprime la descarga.
2. Abre Obsidian → **Abrir carpeta como vault** → selecciona la carpeta descomprimida.
3. Confía en el vault cuando te lo pregunte (solo trae ajustes en JSON plano).
4. Abre `Empieza aquí.md`.

Si prefieres usarlo dentro de un vault existente, copia las carpetas `Diario/` y `Plantillas/` y replica los ajustes de Daily notes (carpeta `Diario`, formato `YYYY-MM-DD`, plantilla `Plantillas/Nota diaria (core Templates)`).

## Plugins

Obligatorios: ninguno — la variante core funciona desde el primer momento.

Opcionales:

- **Templater** — fechas dinámicas y enlaces al día anterior/siguiente. https://obsidian.md/plugins?id=templater-obsidian

## Licencia

MIT. Úsala, modifícala, publícala — sin atribución obligatoria.

Plantilla de Vaultorial — https://vaultorial.com/es/plantilla-nota-diaria/
