# Plantilla de notas Cornell para Obsidian

Un vault de Obsidian que implementa el método Cornell de toma de apuntes con callouts normales y un único snippet CSS: columna de pistas a la izquierda, apuntes a la derecha, franja de resumen debajo. Sin plugins de la comunidad. Incluye dos plantillas (Cornell genérica y una variante de apuntes de clase con metadatos de asignatura) y tres notas de ejemplo completamente resueltas.

## Estructura de carpetas

```
cornell-notes-template/
├── Empieza aquí.md           ← lee esto primero
├── Apuntes/                  ← 3 notas de clase de ejemplo rellenas
├── Plantillas/               ← Nota Cornell + Apuntes de clase (Cornell)
└── .obsidian/snippets/
    └── cornell.css           ← la disposición a dos columnas (preactivada)
```

## Cómo funciona

Cada nota usa tres callouts — `[!cue]`, `[!notes]`, `[!summary]` — y el snippet `cornell.css` los dispone como la página Cornell clásica: columna de pistas flotada (32 %), apuntes al lado, resumen despejado debajo, plegándose a bloques apilados en ventanas estrechas. El snippet viene preactivado vía `appearance.json`; se puede alternar en Ajustes → Apariencia → Fragmentos de CSS.

La variante de apuntes de clase añade el frontmatter `course`, `professor` y `date` para que los apuntes sigan siendo ordenables y buscables por asignatura.

## Instalación

1. Descomprime la descarga.
2. Abre Obsidian → **Abrir una carpeta como bóveda** → selecciona la carpeta descomprimida.
3. Mantén el modo restringido si te lo pregunta — aquí no hay plugins de la comunidad.
4. Abre una nota de `Apuntes/` en vista de lectura; deberías ver dos columnas. Si no, activa el snippet **cornell** en Ajustes → Apariencia → Fragmentos de CSS.

## Plugins

- **Obligatorios:** ninguno. Solo el core Templates (preconfigurado a la carpeta `Plantillas`).
- **Opcionales:** ninguno.

## Licencia

MIT. Úsala, cámbiala, construye encima — en lo personal o lo comercial. Sin atribución obligatoria.

Plantilla de Vaultorial — https://vaultorial.com/es/plantilla-notas-cornell/
