# Empieza aquí

Bienvenido. Este vault es un montaje de Getting Things Done en funcionamiento para Obsidian, construido sobre el plugin Tasks. Viene con tres proyectos de ejemplo y más de treinta tareas para que cada vista del [[Panel]] tenga algo que mostrar. Ve sustituyendo los ejemplos por tu propio trabajo — la estructura es el producto, el contenido es solo una demostración.

## Cómo se organiza el vault

- [[00 Bandeja de entrada]] — punto de captura. Todo aterriza aquí primero, sin ordenar.
- [[01 Próximas acciones]] — acciones sueltas que no forman parte de un proyecto, etiquetadas con un contexto.
- [[02 En espera]] — cosas que has delegado o que te tienen bloqueado, etiquetadas con `#espera`.
- [[03 Algún día o Quizá]] — ideas con las que aún no te comprometes. Viñetas simples a propósito: no son accionables, así que se quedan fuera de las queries de tareas.
- `Proyectos/` — una nota por proyecto. Las tareas viven dentro de la nota del proyecto al que pertenecen.
- [[Panel]] — la cabina de mando. Las queries en vivo recogen tareas de todo el vault: vencen hoy, vencidas, por contexto, en espera y elementos de la bandeja por procesar.
- `Plantillas/` — contiene [[Proyecto]], la plantilla para nuevas notas de proyecto.

## Contextos

Los contextos de GTD (los clásicos @casa, @ordenador, @recados) son etiquetas anidadas aquí, porque las etiquetas de Obsidian no pueden contener el carácter `@`:

- `#contexto/casa`
- `#contexto/ordenador`
- `#contexto/recados`

Añade una etiqueta de contexto a cualquier tarea y aparecerá en la sección correspondiente del Panel. Añade tus propios contextos (`#contexto/telefono`, `#contexto/oficina`) etiquetando tareas con ellos y copiando un bloque de query en el Panel.

## Plugins a activar

1. **Tasks** (obligatorio) — Ajustes → Plugins de la comunidad → Explorar → "Tasks". Da vida a cada query del Panel.
2. **Dataview** (opcional) — se usa solo para la tabla resumen de proyectos al final del Panel. Todo lo demás funciona sin él.

El plugin core **Templates** ya está activado y apuntando a la carpeta `Plantillas/`.

## Primeros pasos

1. Activa el plugin Tasks y abre el [[Panel]] en vista de lectura. Cada sección debería poblarse con los datos de ejemplo.
2. Captura unas cuantas tareas reales en [[00 Bandeja de entrada]] como casillas `- [ ]` simples. La captura está pensada para ser rápida y desordenada.
3. Procesa la bandeja: cualquier cosa de menos de dos minutos, hazla ya. Las acciones sueltas pasan a [[01 Próximas acciones]] con una etiqueta de contexto y, si importa, una fecha de vencimiento (`📅 2026-06-15`). Los resultados de varios pasos se convierten en una nota en `Proyectos/` — usa la plantilla [[Proyecto]].
4. Una vez por semana, haz una revisión: deja la bandeja a cero, repasa cada proyecto en busca de una próxima acción atascada y persigue cualquier cosa en [[02 En espera]].
5. Cuando los proyectos de ejemplo hayan cumplido su función, bórralos.

> [!tip] Chuleta de sintaxis de tareas
> `- [ ] Llamar al fontanero #contexto/casa ⏫ 📅 2026-06-15`
> `📅` fecha de vencimiento · `⏫` prioridad alta · `🔽` prioridad baja · `🔁 every week` recurrencia · `✅` fecha de finalización (se añade automáticamente al marcar la casilla).
