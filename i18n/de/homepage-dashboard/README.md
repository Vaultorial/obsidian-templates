# Homepage / Dashboard — Obsidian-Vorlage

Ein Startseiten-System für Obsidian: eine Dashboard-Notiz mit den heutigen Aufgaben, der kommenden Woche, aktiven Projekten, zuletzt bearbeiteten Notizen und Vault-Zählern — in zwei Varianten. `Home (einfach)` läuft mit Callouts und statischen Links ganz ohne Plugins; `Home` ist die lebendige Version auf Basis von Dataview-Abfragen über `[due:: ]`-Aufgabendaten, gedacht zum automatischen Öffnen beim Start über das Homepage-Plugin. Enthält einen kleinen, aber vollständig querverlinkten Beispiel-Vault (3 Projekte, 2 Bereiche, 3 Evergreen-Notizen mit realistischen datierten Aufgaben), sodass jeder Dashboard-Abschnitt von Anfang an echte Daten zeigt.

## Ordnerstruktur

```
homepage-dashboard/
├── Hier starten.md          ← zuerst lesen
├── Home.md                  ← lebendiges Dashboard (Dataview)
├── Home (einfach).md        ← Dashboard ohne Plugins
├── Projekte/                ← 3 Beispielprojekte mit datierten Aufgaben
├── Bereiche/                ← 2 laufende Bereiche mit datierten Aufgaben
└── Notizen/                 ← 3 Evergreen-Notizen (Liste, Checkliste, Rezept)
```

## Installation

1. Den Download entpacken.
2. Obsidian öffnen → **Ordner als Vault öffnen** → den entpackten Ordner wählen.
3. Dem Vault vertrauen, wenn Obsidian fragt (er enthält nur schlichte JSON-Einstellungen).
4. `Hier starten.md` öffnen, dann `Home (einfach)` — es funktioniert sofort. Die Plugins unten installieren, um `Home` zum Leben zu erwecken.

Für die Nutzung in einem bestehenden Vault `Home.md` und `Home (einfach).md` hineinkopieren und die Ordnernamen in den Abfragen (`FROM "Projekte" OR "Bereiche"`) an die eigene Struktur anpassen.

## Plugins

Erforderlich für das lebendige Dashboard:

- **Dataview** — führt die Abfragen in `Home.md` aus. https://obsidian.md/plugins?id=dataview

Optional:

- **Homepage** — öffnet das Dashboard automatisch beim Start. https://obsidian.md/plugins?id=homepage

`Home (einfach).md` braucht überhaupt keine Plugins.

## Lizenz

MIT. Nutzen, anpassen, weitergeben — keine Namensnennung erforderlich.

Vorlage von Vaultorial — https://vaultorial.com/de/homepage-dashboard/
