# Empieza aquí

Este vault convierte una hoja de personaje de D&D 5e en una nota de Obsidian. Escribes en las propiedades de la nota los números que cambian poco (características, nivel, clase de armadura, puntos de golpe máximos) y Dataview calcula todo lo que se deriva de ellos: modificadores, bonificador por competencia, iniciativa, tiradas de salvación, las dieciocho habilidades, Percepción pasiva y, para los lanzadores de conjuros, la CD de salvación y el bonificador de ataque de conjuros. Subes de nivel cambiando una propiedad y toda la hoja se actualiza.

## Qué hay dentro

- `Personajes/` — tres personajes de ejemplo rellenos: Brannoc Vell (guerrero, nivel 5), Isolde Marrow (maga, nivel 5) y Tamsin Reed (pícara, nivel 4, con pericia).
- [[Hoja del grupo]] — todo el grupo en una tabla, quién necesita curación y quién es bueno en qué.
- `Plantillas/Hoja de personaje` — una hoja en blanco con todas las fórmulas ya puestas.

## Plugins que hay que activar

1. **Dataview** (obligatorio). Instálalo desde los plugins de la comunidad.
2. En los ajustes de Dataview, activa **JavaScript queries**. Las tablas de tiradas de salvación y habilidades usan un bloque corto de DataviewJS por hoja; todo lo demás es Dataview normal.

El plugin nativo **Plantillas** ya está activado y apunta a `Plantillas/`.

## Cómo se calculan los números

- Modificador = (puntuación − 10) ÷ 2, redondeado hacia abajo. Un 16 da +3 y un 8 da −1.
- Bonificador por competencia = +2 en los niveles 1–4, +3 en 5–8, +4 en 9–12, +5 en 13–16 y +6 en 17–20.
- Una habilidad o tirada de salvación con competencia suma el bonificador por competencia; la pericia lo suma dos veces.
- Percepción pasiva = 10 + tu bonificador de Percepción.
- CD de salvación de conjuros = 8 + bonificador por competencia + modificador de lanzamiento; ataque de conjuros = bonificador por competencia + modificador de lanzamiento.

## Primeros pasos

1. Activa Dataview y las JavaScript queries y abre [[Brannoc Vell]] en modo lectura.
2. Cambia su propiedad `level` de 5 a 9 y mira cómo cambian el bonificador por competencia, las salvaciones y las habilidades.
3. Abre [[Hoja del grupo]] y cambia los `hp` de alguien para ver cómo se actualiza la tabla de curación.
4. Para tu propio personaje: nota nueva en `Personajes/`, inserta la plantilla Hoja de personaje y rellena las propiedades.
