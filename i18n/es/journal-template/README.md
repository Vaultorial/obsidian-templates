# Diario / Bullet Journal — Plantilla para Obsidian

Un vault de diario al estilo bullet journal para Obsidian: registro rápido con la notación clásica (`•` tarea, `×` hecha, `○` evento, `–` nota, `>` migrada), una sección breve de gratitud por entrada, carpetas mensuales y un ritual de reflexión mensual. Incluye dos semanas completas de ejemplo (del 25 de mayo al 7 de junio de 2026) y la reflexión mensual de mayo terminada.

## Estructura de carpetas

```
journal-template/
├── Empieza aquí.md                          ← lee esto primero (incluye la clave de registro)
├── Diario/
│   └── 2026/
│       ├── 05/                              ← 7 entradas + "2026-05 Reflexión.md"
│       └── 06/                              ← 7 entradas
└── Plantillas/
    ├── Entrada de diario (bullet journal).md  ← la usada por defecto en las notas diarias
    ├── Entrada de diario (prosa).md           ← variante de texto largo
    ├── Entrada de diario (Templater).md       ← añade enlaces ant./sig.
    └── Reflexión mensual.md
```

## Instalación

1. Descomprime la descarga.
2. Abre Obsidian → **Abrir carpeta como vault** → selecciona la carpeta descomprimida.
3. Confía en el vault cuando te lo pregunte (solo trae ajustes en JSON plano).
4. Abre `Empieza aquí.md` y pulsa el icono de calendario para la entrada de hoy.

Para usarlo dentro de un vault existente, copia `Diario/` y `Plantillas/` y configura Daily notes con la carpeta `Diario`, el formato `YYYY/MM/YYYY-MM-DD` y la plantilla `Plantillas/Entrada de diario (bullet journal)`.

## Plugins

Obligatorios: ninguno.

Opcionales:

- **Templater** — fechas dinámicas y enlaces al día anterior/siguiente en la variante de Templater. https://obsidian.md/plugins?id=templater-obsidian

## Licencia

MIT. Úsala, modifícala, publícala — sin atribución obligatoria.

Plantilla de Vaultorial — https://vaultorial.com/es/plantilla-de-diario/
