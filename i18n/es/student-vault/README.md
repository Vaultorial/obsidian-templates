# Vault de estudiante para Obsidian

Un vault de Obsidian para gestionar el trabajo del curso, organizado por cuatrimestre y asignatura, con un panel Dataview que aflora cada fecha de entrega y cada examen desde el frontmatter de las notas. Viene con dos asignaturas de ejemplo, doce notas rellenas entre clases, preparación de exámenes y lecturas, y tres plantillas.

## Estructura de carpetas

```
student-vault/
├── Empieza aquí.md        ← lee esto primero
├── Panel.md               ← Dataview: entregas + exámenes, autoconstruido
├── Primavera 2026/
│   ├── Biología 101/      ← clases, preparación de examen, apuntes de lectura
│   └── Estadística 201/   ← clases, preparación de examen, apuntes de lectura
└── Plantillas/            ← Apunte de clase / Preparación de examen / Apunte de lectura
```

## Cómo funciona

Las notas llevan los campos `due` y `type` en su frontmatter. `Panel.md` consulta todo el vault: una tabla de entregas (cualquier cosa con un `due` futuro), una tabla de exámenes (`type: exam`) y un desglose por asignatura. Edita una fecha en cualquier nota y el panel lo refleja al instante. Añade una asignatura copiando una carpeta de asignatura; añade un cuatrimestre con una carpeta `Estación AAAA/` nueva.

## Instalación

1. Descomprime la descarga.
2. Abre Obsidian → **Abrir una carpeta como bóveda** → selecciona la carpeta descomprimida.
3. Desactiva el modo restringido cuando se te pregunte, luego instala Dataview (enlace abajo) y actívalo.
4. Abre `Panel.md` — las tablas deberían poblarse con las notas de ejemplo.

## Plugins

- **Obligatorios:** Dataview — https://obsidian.md/plugins?id=dataview — da vida al panel.
- **Opcionales:** Calendar — https://obsidian.md/plugins?id=calendar — vista de mes que acompaña a las notas diarias.

## Licencia

MIT. Úsalo, cámbialo, construye encima — en lo personal o lo comercial. Sin atribución obligatoria.

Plantilla de Vaultorial — https://vaultorial.com/es/vault-para-estudiantes/
