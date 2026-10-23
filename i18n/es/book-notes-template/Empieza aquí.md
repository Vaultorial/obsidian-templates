# Empieza aquí

Bienvenido. Este vault es un sistema de lectura en tres partes: una nota por libro en `Libros/`, una [[Estantería]] que se monta sola a partir de esas notas, y una plantilla que mantiene consistente cada nueva nota de libro.

## Cómo funciona

Cada nota de libro lleva sus datos en el frontmatter — `author`, `genre`, `rating`, `status` (`leído` / `leyendo` / `por leer`), `date-started`, `date-finished`. La [[Estantería]] ejecuta queries Dataview sobre ese frontmatter, así que los estantes se actualizan en el momento en que editas una nota. Cambia el estado de un libro de `leyendo` a `leído`, añade una valoración, y cambia de estante solo.

Ya hay seis libros, en distintos estados, para que cada estante tenga algo: empieza con [[Céntrate (Deep Work)]] o [[Hábitos atómicos]] para ver una nota terminada, [[El programador pragmático]] para una a media lectura, y [[Esencialismo]] para lo poco que necesita una nota de "por leer".

## Filosofía de las notas

- El resumen y las ideas clave se **escriben con tus propias palabras** — ahí está la retención, no en coleccionar pasajes.
- Las citas se limitan a una por libro como mucho, breve y atribuida. Una nota de libro es tu pensamiento sobre el libro, no un fichero de extractos.

## Primeros pasos

1. Instala y activa **Dataview** (obligatorio — la [[Estantería]] está en blanco sin él): Ajustes → Complementos comunitarios → Buscar → "Dataview".
2. Abre la [[Estantería]] y confirma que los estantes se renderizan.
3. Añade el libro que estás leyendo ahora: nota nueva en `Libros/` con el nombre del título, inserta `Plantillas/Nota de libro.md` (plugin core Templates, ya configurado), rellena el frontmatter, pon `status: leyendo`.
4. Opcional: instala **Book Search** para crear notas de libro con autor y metadatos rellenados desde una búsqueda por título.

> [!tip] Valora en tu propia escala
> La valoración es para que tu yo futuro decida qué releer o recomendar — no es una reseña pública. Decide qué significa un 5 para ti una vez, escríbelo arriba en la Estantería, y mantén la coherencia.
