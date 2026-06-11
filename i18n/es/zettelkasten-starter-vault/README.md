# Vault de inicio de Zettelkasten — Plantilla para Obsidian

Un vault de inicio para el método Zettelkasten en Obsidian, ya poblado con un ejemplo en funcionamiento: catorce notas enlazadas sobre aprendizaje y memoria que muestran la tubería completa fugaz → literatura → permanente, los IDs de marca de tiempo y un índice como puerta de entrada.

## Estructura de carpetas

```
zettelkasten-starter-vault/
├── Empieza aquí.md    ← lee esto primero
├── Índice.md          ← puerta de entrada a las notas permanentes
├── Fugaces/           ← capturas rápidas, se procesan y se borran (3 ejemplos)
├── Literatura/        ← una nota por fuente, con tus palabras (3 ejemplos)
├── Permanentes/       ← una idea por nota, IDs de marca de tiempo (8 ejemplos)
└── Plantillas/        ← plantillas de nota fugaz / de literatura / permanente
```

Las notas permanentes se llaman `YYYYMMDDHHMM Título.md` (por ejemplo `202605141030 Escribe las notas con tus propias palabras.md`). El ID hace que cada nota sea direccionable de forma única y mantiene estables los nombres de fichero aunque los títulos evolucionen.

## Instalación

1. Descomprime la descarga.
2. Abre Obsidian → **Abrir carpeta como vault** → selecciona la carpeta descomprimida.
3. Activa el plugin core **Templates** si hace falta (Ajustes → Plugins principales); ya apunta a `Plantillas`.
4. Opcional: instala Templater (abajo) y la plantilla de nota permanente generará su ID de marca de tiempo automáticamente.

## Plugins

- **Obligatorios:** ninguno — el vault funciona de serie con los plugins core.
- **Opcional:** Templater — https://obsidian.md/plugins?id=templater-obsidian — rellena solo el ID `YYYYMMDDHHMM` y las fechas de las plantillas. Sin él, escribe el ID a mano.

## Licencia

MIT. Úsala, modifícala, construye encima — en lo personal o en lo comercial. Sin atribución obligatoria.

Plantilla de Vaultorial — https://vaultorial.com/es/vault-zettelkasten/
