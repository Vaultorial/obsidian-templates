# Vault CRM — Plantilla de Obsidian

Un CRM personal para Obsidian: contactos, empresas, oportunidades y un registro fechado de cada interacción, unidos con Dataview. Viene con el embudo de una pequeña consultora ya rellenado, así que el panel muestra seguimientos reales, oportunidades abiertas y contactos que se enfrían desde el primer momento.

## Cómo encaja todo

- `Contactos/`: una nota por persona, con `company`, `role`, `relationship`, `last_contact` y `next_follow_up` en las propiedades.
- `Empresas/`: una nota por organización. Cada una lista su gente y sus oportunidades de forma automática.
- `Oportunidades/`: una nota por oportunidad, con `value`, `stage` y `close_date`.
- `Interacciones/`: una nota por llamada, email o reunión, con la fecha en el nombre. Las tareas de seguimiento viven aquí.
- [[Panel CRM]]: seguimientos de esta semana, tareas abiertas, el embudo por fase, contactos sin hablar en 60 días e interacciones recientes.
- `Embudo.base`: las mismas oportunidades como tabla editable, con el plugin principal Bases de Obsidian.

Fases de oportunidad que usa el vault: `lead`, `cualificado`, `propuesta`, `negociación`, `ganado`, `perdido`.

## Plugins

**Dataview** es necesario para el panel y las listas de cada nota. El plugin principal **Plantillas** está activado y apunta a `Plantillas/`. La tabla del embudo usa el plugin principal **Bases**, incluido en las versiones actuales de Obsidian.

- Dataview — https://obsidian.md/plugins?id=dataview

1. Descomprime la descarga y, en Obsidian, elige **Abrir carpeta como vault**.
2. Activa los plugins de la comunidad para este vault cuando te lo pida.
3. Instala y activa **Dataview** y abre el Panel CRM en vista de lectura.

## License

MIT. Úsala, cámbiala y compártela; se agradece la atribución, pero no es obligatoria.

Plantilla de Vaultorial — https://vaultorial.com/es/plantilla-crm-obsidian/
