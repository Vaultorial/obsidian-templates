# Empieza aquí

Este vault dibuja diagramas de Gantt a partir de tus notas. Cada tarea es una nota con una fecha `start` y otra `end` en sus propiedades, y la nota [[Cronograma]] convierte cada tarea en una barra: un diagrama por proyecto y una sección por fase. Mueves una fecha y el diagrama se redibuja. No hay nada que exportar, y cada tarea sigue siendo un archivo Markdown que puedes enlazar, etiquetar y escribir.

## Qué hay dentro

- `Proyectos/` — dos proyectos de ejemplo con tareas fechadas: una mudanza de oficina y el relanzamiento de una web, con tareas terminadas, en curso y críticas, e hitos.
- [[Cronograma]] — los diagramas generados y una lista de las tareas que aún no tienen fecha.
- [[Ejemplo de Gantt estático]] — un diagrama de Gantt de Mermaid escrito a mano que no necesita ningún plugin, con la sintaxis explicada.
- `Plantillas/Tarea` — una nota de tarea en blanco con todas las propiedades.

## Plugins que hay que activar

1. **Dataview** (obligatorio para [[Cronograma]]). Instálalo desde los plugins de la comunidad.
2. En los ajustes de Dataview, activa **JavaScript queries**.
3. Obsidian dibuja los diagramas con Mermaid, que viene integrado. Si una nota pregunta si quieres mostrar diagramas Mermaid en este vault, permítelo.

El plugin nativo **Plantillas** ya está activado y apunta a `Plantillas/`.

## Propiedades de cada tarea

- `project` y `phase` deciden en qué diagrama y en qué sección va la barra.
- `start` y `end` son fechas con el formato AAAA-MM-DD. Una tarea sin `start` se queda fuera del diagrama.
- `status`: `hecha`, `en curso` o `pendiente`.
- `critical: true` pinta la barra en rojo y `milestone: true` dibuja un rombo en la fecha de inicio.

## Primeros pasos

1. Activa Dataview y las JavaScript queries y abre [[Cronograma]] en modo lectura.
2. Abre cualquier tarea de `Proyectos/Mudanza de oficina/`, cambia su fecha `end` y vuelve a [[Cronograma]].
3. Para tu propio proyecto: crea una carpeta en `Proyectos/`, añade notas de tarea con la plantilla Tarea y rellena las fechas.
