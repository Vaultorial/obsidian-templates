---
type: reunion-equipo
date: 2026-05-04
project: Portal de cliente
attendees:
  - Sarah Chen
  - Priya Nair
  - Marcus Webb
---

# Arranque del portal de cliente

Arranque interno de la fase de construcción del portal de cliente de Brightleaf Insurance. El descubrimiento se cerró a finales de abril; esta reunión convierte los hallazgos en un plan de trabajo.

## Agenda

1. Recapitulación: a qué nos comprometió el descubrimiento
2. Cadencia de sprints y roles
3. Incógnitas técnicas a investigar primero
4. Qué ve el cliente, y cuándo

## Notas

- Alcance del descubrimiento: los asegurados pueden consultar el estado de su reclamación, subir documentos a una reclamación abierta y enviar mensajes al equipo de reclamaciones. Explícitamente fuera: pagos y cambios de póliza — fase dos como muy pronto.
- Roles: Priya lleva el frontend del portal, Marcus lleva la capa de API y la integración con el sistema de pólizas de Brightleaf, Sarah gestiona la relación con el cliente y el backlog.
- Dos incógnitas técnicas que vale la pena investigar antes de comprometer el sprint 1: cómo expone el sistema de pólizas los eventos de reclamación, y si el proveedor de identidad de Brightleaf soporta el flujo de login que esbozamos.
- Acordado demostrar solo software que funciona — nunca demos con diapositivas al cliente. Si un sprint no produce nada demostrable, lo decimos.

## Decisiones

- Sprints de dos semanas a partir del 2026-05-04; demo de cara al cliente cada dos viernes.
- Las revisiones de sprint son internas el lunes posterior a cada sprint; la llamada con el cliente sigue el jueves.
- La investigación de autenticación se lleva los tres primeros días del sprint 1 antes de empezar nada de UI.

## Elementos de acción

- [x] Marcus — investigación de autenticación y eventos de reclamación documentada 📅 2026-05-07 ✅ 2026-05-07
- [x] Sarah — backlog del sprint 1 acordado con Helen en Brightleaf 📅 2026-05-06 ✅ 2026-05-05
- [x] Priya — andamiaje de UI del portal y design tokens en el repo 📅 2026-05-08 ✅ 2026-05-08
- [ ] Sarah — escribir el documento de logística del día de demo para el lado del cliente 📅 2026-06-12
