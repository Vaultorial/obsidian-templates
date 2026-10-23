# Registro de hábitos — Plantilla para Obsidian

Un registro de hábitos para Obsidian con dos niveles: **cuadrículas mensuales** sin plugins (hábitos × días, marcas en una tabla) y un **panel con Dataview** opcional que calcula rachas, totales mensuales y días perfectos a partir de pequeñas notas de registro diarias. Trae dos meses de ejemplo completamente registrados (abril–mayo de 2026, cinco hábitos cotidianos, datos imperfectos de forma realista).

## Estructura de carpetas

```
habit-tracker/
├── Empieza aquí.md                      ← lee esto primero
├── Hábitos/
│   ├── 2026-04 Hábitos.md               ← cuadrícula mensual, rellena
│   ├── 2026-05 Hábitos.md               ← cuadrícula mensual, rellena
│   ├── Panel de hábitos.md              ← Dataview: rachas, totales, días perfectos
│   └── Registro diario/                 ← 61 notas por día (datos en frontmatter)
│       └── 2026-04-01.md … 2026-05-31.md
└── Plantillas/
    ├── Cuadrícula mensual de hábitos.md ← cuadrícula en blanco para un mes nuevo
    └── Entrada de registro diario.md    ← registro diario de un minuto
```

## Instalación

1. Descomprime la descarga.
2. Abre Obsidian → **Abrir una carpeta como bóveda** → selecciona la carpeta descomprimida.
3. Confía en el vault cuando te lo pregunte (solo trae ajustes en JSON plano).
4. Abre `Empieza aquí.md`.

Si prefieres usarlo dentro de un vault existente, copia `Hábitos/` y `Plantillas/` y define `Plantillas` como tu carpeta de plantillas (Ajustes → Plantillas).

## Plugins

Obligatorios: ninguno — las cuadrículas mensuales son tablas Markdown normales.

Opcionales:

- **Dataview** — alimenta el Panel de hábitos (las rachas necesitan su ajuste de *consultas JavaScript* activado). https://obsidian.md/plugins?id=dataview

## Licencia

MIT. Úsala, modifícala, publícala — sin atribución obligatoria.

Plantilla de Vaultorial — https://vaultorial.com/es/registro-de-habitos/
