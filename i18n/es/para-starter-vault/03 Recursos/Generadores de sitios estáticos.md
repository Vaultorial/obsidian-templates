---
type: recurso
created: 2026-02-21
tags: [recurso, web]
---

# Generadores de sitios estáticos

Nota de referencia creada mientras investigaba para [[Lanzamiento de la web personal]]. La guardo en Recursos y no en la carpeta del proyecto porque sobrevivirá al proyecto — la próxima reconstrucción de la web también la querrá.

## Qué es un generador de sitios estáticos

Una herramienta que toma ficheros de texto plano (normalmente Markdown) más unas plantillas y produce una carpeta de HTML terminado. Sin base de datos, sin código de servidor en ejecución — el resultado se puede alojar en cualquier sitio que sirva ficheros.

## Qué comparé, y qué sensación dejó

- **Hugo** — un solo binario, builds rapidísimos, su plantillado requiere acostumbrarse.
- **Eleventy** — basado en JavaScript, flexible, con mínimas suposiciones sobre la estructura.
- **Astro** — modelo de componentes, más piezas móviles de las que necesita una web de cinco páginas.
- **Jekyll** — el veterano; correcto, pero no tengo Ruby en ningún otro rincón de mi vida.

## Decisión (21-02-2026)

Eleventy. Motivo: mis notas ya son Markdown, puedo leer sus plantillas sin manual y el build es tan simple que mi yo del futuro lo seguirá entendiendo dentro de dos años. Decisión registrada aquí para que la nota de proyecto ([[Lanzamiento de la web personal]]) siga siendo de acciones, no de investigación.
