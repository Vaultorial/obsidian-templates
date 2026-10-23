# Empieza aquí

Un kit completo de PNJ para directores de juego: una plantilla de PNJ completa con personalidad, voz, secretos, ganchos y relaciones, una plantilla rápida para improvisar en la mesa y una lista en Dataview que ordena el reparto por lugar, facción y actitud. Incluye Cinderbrook, un pueblo de río original con seis PNJ detallados y tres rápidos, para que cada vista tenga datos desde el primer día.

## Qué hay en el vault

- `PNJ/`: seis PNJ completos con las propiedades `role`, `location`, `faction`, `attitude`, `status`, `first_met` y `revealed`.
- `PNJ rápidos/`: tres PNJ rápidos, con aspecto, deseo, voz y secreto en una pantalla.
- `Facciones/` y `Lugares/`: dos facciones y dos lugares, cada uno con su gente listada sola.
- [[Lista de PNJ]]: la lista en Dataview por lugar, por actitud, miembros de facción, PNJ rápidos y secretos por revelar.
- `Plantillas/`: plantillas PNJ y PNJ rápido.

## Cómo usarlo en la mesa

Antes de una sesión, revisa la lista para ver a quién puede encontrarse el grupo y qué secretos siguen ocultos. Cuando improvises un personaje, rellena un PNJ rápido en menos de un minuto. Si el grupo vuelve a buscarlo, asciéndelo: crea un PNJ completo con la plantilla y enlaza la nota rápida. Después de la sesión, actualiza `attitude` y pon `revealed: true` en los secretos que hayan salido.

Válido para cualquier sistema. Las estadísticas opcionales usan campos al estilo de 5e con números originales; cámbialas o bórralas para otros sistemas.

## Plugins

**Dataview** mueve la lista y las listas de miembros de las facciones y los lugares. El plugin principal **Plantillas** está activado y apunta a `Plantillas/`.
