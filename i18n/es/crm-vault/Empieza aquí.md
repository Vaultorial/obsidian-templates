# Empieza aquí

Este vault es un CRM personal que funciona. Cada persona, empresa y oportunidad es una nota, cada conversación es una nota fechada en Interacciones y el [[Panel CRM]] lo reúne todo. Los datos de ejemplo son de una consultora de diseño inventada para que cada consulta tenga algo que mostrar. Bórralos cuando hayas metido tus contactos.

## Cómo encaja todo

- `Contactos/`: una nota por persona, con `company`, `role`, `relationship`, `last_contact` y `next_follow_up` en las propiedades.
- `Empresas/`: una nota por organización. Cada una lista su gente y sus oportunidades de forma automática.
- `Oportunidades/`: una nota por oportunidad, con `value`, `stage` y `close_date`.
- `Interacciones/`: una nota por llamada, email o reunión, con la fecha en el nombre. Las tareas de seguimiento viven aquí.
- [[Panel CRM]]: seguimientos de esta semana, tareas abiertas, el embudo por fase, contactos sin hablar en 60 días e interacciones recientes.
- `Embudo.base`: las mismas oportunidades como tabla editable, con el plugin principal Bases de Obsidian.

## La rutina semanal

Después de cada conversación, crea una nota de interacción con la plantilla y enlaza el contacto. Actualiza `last_contact` y `next_follow_up` del contacto, y cambia el `stage` de la oportunidad si se ha movido. Una vez por semana, abre el panel y resuelve los seguimientos de arriba.

Fases de oportunidad que usa el vault: `lead`, `cualificado`, `propuesta`, `negociación`, `ganado`, `perdido`.

## Plugins

**Dataview** es necesario para el panel y las listas de cada nota. El plugin principal **Plantillas** está activado y apunta a `Plantillas/`. La tabla del embudo usa el plugin principal **Bases**, incluido en las versiones actuales de Obsidian.
