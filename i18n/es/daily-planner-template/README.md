# Planificador diario (bloques de tiempo) — Plantilla para Obsidian

Un planificador diario por bloques de tiempo para Obsidian: tres tareas más importantes, una línea de tiempo hora a hora en sintaxis de Day Planner (`- [ ] 09:00 - 10:30 Trabajo profundo: borrador del informe`) y un ritual de cierre al final del día. Trae tres días de ejemplo realistas y una nota de resumen semanal.

## Estructura de carpetas

```
daily-planner-template/
├── Empieza aquí.md                ← lee esto primero
├── Planificador/                  ← una nota por día + resumen de la semana
│   ├── 2026-06-08.md … 2026-06-10.md
│   └── Semana del 2026-06-08.md
└── Plantillas/
    ├── Planificador diario.md     ← se aplica sola a las notas diarias nuevas
    └── Resumen semanal.md
```

## Instalación

1. Descomprime la descarga.
2. Abre Obsidian → **Abrir una carpeta como bóveda** → selecciona la carpeta descomprimida.
3. Confía en el vault cuando te lo pregunte (solo trae ajustes en JSON plano).
4. Abre `Empieza aquí.md` y crea la nota de hoy desde el icono de calendario de la barra lateral.

Si prefieres usarlo dentro de un vault existente, copia `Planificador/` y `Plantillas/` y apunta Daily notes a la carpeta `Planificador`, formato `YYYY-MM-DD`, plantilla `Plantillas/Planificador diario`.

## Plugins

Obligatorios: ninguno — funciona como listas de tareas normales con plugins core.

Opcional (recomendado):

- **Day Planner** — convierte los bloques de la línea de tiempo en un horario visual con indicador de «ahora» en vivo. https://obsidian.md/plugins?id=obsidian-day-planner

## Licencia

MIT. Úsala, modifícala, publícala — sin atribución obligatoria.

Plantilla de Vaultorial — https://vaultorial.com/es/plantilla-planificador-diario/
