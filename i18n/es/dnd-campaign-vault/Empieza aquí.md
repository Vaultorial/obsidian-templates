# Empieza aquí

Bienvenido, DM. Este vault es un sistema de gestión de campañas para juegos de mesa compatibles con el reglamento de quinta edición más popular del mundo. Viene con una minicampaña original completa ya cargada — **La conspiración de la Ruta de la Sal**: tres sesiones jugadas, ocho PNJ, cuatro lugares, tres encuentros, tres personajes jugadores y el trasfondo que lo ata todo. Dirígela tal cual, despiézala, o bórrala y quédate con la estructura.

## Cómo está organizado el vault

- `Sesiones/` — una nota por sesión: resumen, escenas, pistas entregadas y un bloque de "la próxima vez" que se convierte en tu lista de preparación.
- `PNJ/` — una nota por personaje, con `role`, `location`, `status` y `faction` en el frontmatter para que la [[Pantalla del DM]] pueda ordenarlos.
- `Lugares/` — una nota por sitio visitable, cada una con enlaces a sus PNJ, encuentros y rumores.
- `Encuentros/` — encuentros preparados con bloques de estadísticas originales, notas de terreno y tácticas. `status: preparado` significa jugable esta noche; `status: jugado` conserva el registro.
- `PJ/` — una nota por personaje jugador: la copia de mesa de vínculos, metas y los ganchos de campaña que llevan atados.
- `Trasfondo/` — las piezas móviles del mundo (facciones, historia) en las que más de una nota tiene que estar de acuerdo.
- `Plantillas/` — una plantilla por tipo de entidad, conectadas al plugin core Templates.
- [[Pantalla del DM]] — el panel de mando. Consultas de Dataview que reúnen PNJ por lugar, sesiones recientes, encuentros preparados y la lista del grupo.

## Plugins que activar

1. **Dataview** (obligatorio) — mueve todas las tablas de la [[Pantalla del DM]].
2. **Leaflet** (opcional) — en cuanto añadas imágenes de mapas al vault, un bloque de código `leaflet` las convierte en mapas navegables con marcadores. Nada del vault depende de él.
3. **Initiative Tracker** (opcional) — lleva el orden de turnos en la barra lateral; casa bien con las notas de encuentro.

El plugin core **Templates** ya está activado y apuntando a `Plantillas/`.

## Primeros pasos

1. Activa Dataview y abre la [[Pantalla del DM]] en vista de lectura — todas las tablas deberían salir pobladas.
2. Lee [[La Ruta de la Sal]] para la columna vertebral de la campaña y después [[Sesión 3 - Sal en la herida]] para ver dónde lo dejó la mesa. El [[Asalto a la Contaduría]] está preparado y listo para la próxima sesión.
3. Antes de tu propia sesión cero: ensaya el flujo de plantillas — nota nueva en la carpeta correcta, insertar la plantilla correspondiente, rellenar el frontmatter.
4. Después de cada sesión, escribe la nota de sesión en caliente, actualiza cualquier PNJ cuyo `status` haya cambiado y pon en `preparado` las notas de encuentro de la próxima sesión.

> [!note] Sobre el contenido
> Todo lo de aquí — la Marca Salobre, su gente, sus monstruos — es original de esta plantilla. Las líneas de estadísticas tipo "CA 13, PG 26" son creaciones caseras para esta campaña, no reproducciones de ningún manual, de modo que el vault se mantiene compatible sin copiar el texto de nadie.
