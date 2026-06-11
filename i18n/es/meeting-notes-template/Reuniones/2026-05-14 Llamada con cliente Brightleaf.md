---
type: llamada-cliente
date: 2026-05-14
project: Portal de cliente
attendees:
  - Sarah Chen
  - Marcus Webb
  - Helen Brody (Brightleaf)
  - Tom Aldridge (Brightleaf)
---

# Llamada con cliente Brightleaf

Llamada quincenal programada con Brightleaf Insurance antes de la primera demo de sprint. Helen es la directora de operaciones y patrocinadora del proyecto; Tom dirige el equipo de reclamaciones que pilotará el portal.

## Agenda

1. Progreso del sprint 1, con honestidad
2. Grupo piloto y calendario
3. Restricciones de subida de documentos
4. Programación de la revisión de seguridad

## Notas

- Sarah repasó el sprint 1: la investigación de autenticación tuvo éxito contra el tenant de prueba del proveedor de identidad; la pantalla de estado de reclamación lee datos en vivo del sistema de pólizas de staging. Más lento de lo esperado: los eventos de reclamación llegan en lotes por la noche, así que el estado "en vivo" es realmente "a fecha de anoche" — Tom confirmó que eso coincide con cómo ya trabaja el equipo de reclamaciones, lo que desactiva el problema.
- Piloto: Tom propone su equipo de reclamaciones más un puñado de asegurados de confianza en vez de un lanzamiento suave público. Helen estuvo de acuerdo — más pequeño, más seguro, feedback más rápido.
- Subida de documentos: las reglas de retención de Brightleaf exigen que las subidas aterricen en su almacén documental, no en el nuestro. Marcus confirmó que el almacén tiene una API de ingesta; los límites de tamaño y tipos de archivo permitidos los facilitará el equipo de Tom.
- Revisión de seguridad: el equipo de seguridad interno de Brightleaf necesita tres semanas de aviso y un cuestionario completado. Reservarla ahora para finales de junio mantiene realista la fecha del piloto.

## Decisiones

- El grupo piloto es el equipo de reclamaciones más asegurados invitados; inicio objetivo en la última semana de junio.
- Los documentos subidos van directamente al almacén documental de Brightleaf; el portal solo guarda referencias.
- Revisión de seguridad reservada para la semana del 2026-06-22; cuestionario a cargo de Marcus.

## Elementos de acción

- [x] Tom Aldridge — enviar los tipos de archivo y límites de tamaño permitidos para las subidas 📅 2026-05-20 ✅ 2026-05-19
- [x] Marcus — solicitar las credenciales de la API del almacén documental para staging 📅 2026-05-18 ✅ 2026-05-18
- [ ] Marcus — completar el cuestionario de seguridad 📅 2026-06-15
- [ ] Helen Brody (Brightleaf) — nombrar a los asegurados de confianza para el piloto 📅 2026-06-17
- [ ] Sarah — distribuir los criterios de éxito del piloto para su aprobación 📅 2026-06-19
