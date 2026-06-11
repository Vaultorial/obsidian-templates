---
type: reunion-equipo
date: 2026-06-01
project: Portal de cliente
attendees:
  - Sarah Chen
  - Priya Nair
  - Marcus Webb
---

# Revisión de sprint del portal de cliente

Revisión interna del sprint 2 (2026-05-18 a 2026-05-29), el lunes posterior al cierre del sprint.

## Agenda

1. Qué se entregó frente a lo que comprometimos
2. El problema de los datos de prueba
3. Preparación de la demo para el viernes
4. Riesgos para la fecha del piloto

## Notas

- Entregado: pantalla de estado de reclamación completa, incluido el texto de la salvedad del lote nocturno, UI del hilo de mensajería funcionando de extremo a extremo en staging, UI de subida construida pero corriendo contra un mock.
- No entregado: subida contra el almacén documental real. Las credenciales llegaron el 2026-05-27, demasiado tarde en el sprint — pasado al sprint 3 con la integración ya planificada.
- Datos de prueba: el extracto anonimizado de reclamaciones de Brightleaf está atascado con su responsable de protección de datos. Sin él demostramos sobre reclamaciones sintéticas que no se parecen en nada a las reales. Marcus propuso generar un conjunto sintético más rico a partir del esquema de eventos de reclamación en vez de esperar; acordado.
- Priya lleva la demo del viernes en solitario, según el plan del último 1-on-1. Ensayo el jueves.
- Revisión de riesgos del piloto: la revisión de seguridad (semana del 2026-06-22) y los nombramientos de asegurados son las dos dependencias externas. Ambas tienen responsables del lado de Brightleaf; Sarah reclama con suavidad a mitad de semana.

## Decisiones

- Dejar de esperar el extracto anonimizado para las demos; invertir media jornada en un generador de datos sintéticos y revisarlo cuando se libere el extracto real.
- La integración de subida es el primer elemento del sprint 3; nada más empieza hasta que esté de extremo a extremo en staging.

## Elementos de acción

- [x] Marcus — generador de reclamaciones sintéticas que produzca datos de demo realistas 📅 2026-06-03 ✅ 2026-06-03
- [x] Priya — ensayo del jueves de la demo en solitario con Sarah de público 📅 2026-06-04 ✅ 2026-06-04
- [ ] Marcus — flujo de subida funcionando contra el almacén documental real en staging 📅 2026-06-12
- [ ] Sarah — aviso de estado a Helen sobre la revisión de seguridad y los nombramientos del piloto 📅 2026-06-11
