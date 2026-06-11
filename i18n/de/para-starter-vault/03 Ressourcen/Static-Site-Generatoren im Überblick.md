---
type: ressource
created: 2026-02-21
tags: [ressource, web]
---

# Static-Site-Generatoren im Überblick

Referenznotiz, entstanden bei der Recherche für [[Launch der eigenen Website]]. Sie liegt in Ressourcen statt im Projektordner, weil sie das Projekt überleben wird — der nächste Website-Umbau will sie auch.

## Was ein Static-Site-Generator ist

Ein Werkzeug, das einfache Textdateien (meist Markdown) plus Templates nimmt und einen Ordner mit fertigem HTML erzeugt. Keine Datenbank, kein Server-Code zur Laufzeit — das Ergebnis lässt sich überall hosten, wo Dateien ausgeliefert werden.

## Was ich verglichen habe, und wie es sich anfühlte

- **Hugo** — eine einzige Binärdatei, sehr schnelle Builds, das Templating braucht Eingewöhnung.
- **Eleventy** — JavaScript-basiert, flexibel, minimale Annahmen über die Struktur.
- **Astro** — Komponentenmodell, mehr bewegliche Teile, als eine Fünf-Seiten-Website braucht.
- **Jekyll** — der Veteran; in Ordnung, aber ich habe sonst nirgendwo Ruby in meinem Leben.

## Entscheidung (21.02.2026)

Eleventy. Begründung: Meine Notizen sind schon Markdown, ich kann die Templates ohne Handbuch lesen, und der Build ist so simpel, dass mein Zukunfts-Ich ihn in zwei Jahren noch versteht. Entscheidung hier festgehalten, damit die Projektnotiz ([[Launch der eigenen Website]]) bei den Schritten bleibt, nicht bei der Recherche.
