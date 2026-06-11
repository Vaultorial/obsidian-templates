# Kit de inicio MOC

Un vault de inicio para Obsidian para organizar notas con Mapas de Contenido (MOC). Viene del todo resuelto: un MOC de inicio, tres MOC temáticos (productividad, aprendizaje, escritura) y quince notas interconectadas debajo — abre la vista de grafo y el árbol de tres niveles ya está ahí.

## Estructura de carpetas

```
moc-template/
├── Empieza aquí.md     ← lee esto primero
├── MOC de inicio.md    ← nivel 1: el único punto de entrada
├── MOCs/               ← nivel 2: un mapa por tema (3 ejemplos)
├── Notas/              ← nivel 3: una idea por nota, planas (15 ejemplos)
└── Plantillas/         ← plantilla de MOC con las convenciones de enlazado
```

## Convenciones usadas en todo el vault

- **MOC de inicio → MOC → nota**: la página de inicio enlaza solo a MOC; los MOC enlazan a notas con una línea de contexto cada una; las notas enlazan `Up:` a su MOC y de lado a notas relacionadas.
- Las notas viven planas en `Notas/` — los mapas cargan con la estructura, no el árbol de carpetas.

## Instalación

1. Descomprime la descarga.
2. Abre Obsidian → **Abrir carpeta como vault** → selecciona la carpeta descomprimida.
3. Si Obsidian pregunta por el modo restringido, mantenlo — este vault no usa plugins de la comunidad.
4. Activa el plugin core **Templates** (Ajustes → Plugins core) para usar la plantilla de MOC.

## Plugins

- **Obligatorios:** ninguno. Funciona del todo con plugins core.
- **Opcionales:** ninguno.

## Licencia

MIT. Úsala, cámbiala, construye encima — en lo personal o lo comercial. Sin atribución obligatoria.

Plantilla de Vaultorial — https://vaultorial.com/es/plantilla-moc/
