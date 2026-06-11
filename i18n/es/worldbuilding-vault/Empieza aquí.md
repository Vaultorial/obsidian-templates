# Empieza aquí

Bienvenido. Este vault es un sistema de worldbuilding para escritores y directores de juego, demostrado con una ambientación original completa: **Las Cortes de la Marea**, un mundo de magia escasa hecho de ciudades-estado de estuario gobernadas por la ley de mareas. Una veintena de notas interenlazadas — lugares, personajes, facciones y una cronología enlazada — enseña el método funcionando a plena densidad. Abre primero la vista de grafo: un mundo debería parecer una red, y este lo parece.

## Cómo está organizado el vault

- `Lugares/` — una nota por lugar, con `region` y `ruled-by` en el frontmatter.
- `Personajes/` — una nota por persona, cada una enlazada a un `home` (un lugar) y a una `faction`.
- `Facciones/` — los poderes. Cada uno tiene una `seat` (un lugar) y un `leader` (un personaje).
- `Eventos/` — la cronología. Cada evento lleva `year`, `location` y una lista de `participants`, de modo que la línea temporal se ensambla sola.
- `Mapas/` — vacía a propósito; la nota de dentro explica cómo añadir tus mapas.
- [[Índice del mundo]] — el MOC maestro: todas las entidades desde una página, más resúmenes de Dataview.
- [[Cronología]] — la línea del tiempo, consultada y narrada.
- `Plantillas/` — una plantilla por tipo de entidad, conectadas al plugin core Templates.

## El método: relaciones en el frontmatter

Cada nota declara sus relaciones como enlaces de frontmatter (`home: "[[Bajamarca]]"`, `faction: "[[Los Juramentados de la Creciente]]"`). Ese único hábito te da tres cosas gratis: la vista de grafo enseña la forma real del mundo, Dataview puede responder preguntas ("todos los jurados a la Corte del Reflujo", "todos los eventos de la Calzada") y renombrar cualquier nota actualiza todas sus referencias. Los wikilinks en prosa tejen el resto.

Las fechas usan el calendario propio del mundo — años del Cómputo de las Mareas, escritos `368 CM` — guardado como un simple número en `year` para que la cronología se ordene sola. Usa el calendario que tu mundo necesite; mantén el campo numérico.

## Plugins que activar

1. **Dataview** (obligatorio) — mueve los resúmenes de [[Índice del mundo]] y [[Cronología]].
2. **Timelines (Revamped)** (opcional) — dibuja líneas temporales visuales a partir de tramos etiquetados si quieres algo más que la tabla consultada. El vault funciona entero sin él.

El plugin core **Templates** ya está activado y apuntando a `Plantillas/`.

## Primeros pasos

1. Activa Dataview y lee el [[Índice del mundo]] — es la puerta de entrada a todo.
2. Abre la vista de grafo y asigna grupos de color por carpeta (`path:Lugares`, `path:Personajes`, `path:Facciones`, `path:Eventos`). La estructura del mundo se vuelve visible al instante.
3. Lee una cadena de punta a punta para sentir el método de enlazado: [[La Petición de Bajamarca]] → [[Bren Callow]] → [[Los Juramentados de la Creciente]] → [[El Anegamiento de Bajamarca]].
4. Añade tu primera entidad: nota nueva en la carpeta correcta, inserta la plantilla correspondiente, rellena el frontmatter, enlaza mientras escribes.
5. Cuando empieces tu propio mundo, borra las notas de Las Cortes de la Marea y quédate con las carpetas, las plantillas y el índice.
