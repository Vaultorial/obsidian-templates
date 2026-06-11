# Start Here

Welcome. This vault is a worldbuilding system for writers and game masters, demonstrated with a complete original setting: **The Tide Courts**, a low-magic world of estuary city-states ruled by tide-law. Around twenty interlinked notes — places, characters, factions and a linked chronology — show the method working at full density. Open the graph view first: a world should look like a web, and this one does.

## How the vault is organized

- `Places/` — one note per location, with `region` and `ruled-by` in the frontmatter.
- `Characters/` — one note per person, each linked to a `home` (a place) and a `faction`.
- `Factions/` — the powers. Each has a `seat` (a place) and a `leader` (a character).
- `Events/` — the chronology. Each event carries a `year`, a `location` and a `participants` list, so the timeline assembles itself.
- `Maps/` — empty on purpose; see the note inside for how to add your maps.
- [[World Index]] — the master MOC: every entity from one page, plus Dataview rollups.
- [[Timeline]] — the chronology, queried and narrated.
- `Templates/` — one template per entity type, wired to the Templates core plugin.

## The method: relationships in frontmatter

Every note declares its relationships as frontmatter links (`home: "[[Lowmark]]"`, `faction: "[[The Floodsworn]]"`). That one habit gives you three things for free: the graph view shows the world's actual shape, Dataview can answer questions ("everyone sworn to the Ebb Court", "every event at the Causeway"), and renaming any note updates every reference. Prose wikilinks do the rest of the weaving.

Dates use the world's own calendar — years of the Tide Reckoning, written `368 TR` — kept as a plain `year` number so the timeline sorts itself. Use whatever calendar your world needs; keep the field numeric.

## Plugins to enable

1. **Dataview** (required) — powers the rollups in [[World Index]] and [[Timeline]].
2. **Timelines** (optional) — renders visual timelines from tagged spans if you want more than the queried table. The vault works fully without it.

The **Templates** core plugin is already enabled and pointed at `Templates/`.

## First steps

1. Enable Dataview, then read [[World Index]] — it is the front door to everything.
2. Open the graph view and assign color groups by folder (`path:Places`, `path:Characters`, `path:Factions`, `path:Events`). The world's structure becomes visible immediately.
3. Read one chain end to end to feel the linking method: [[The Lowmark Petition]] → [[Bren Callow]] → [[The Floodsworn]] → [[The Drowning of Lowmark]].
4. Add your first entity: new note in the right folder, insert the matching template, fill the frontmatter, link as you write.
5. When you start your own world, delete the Tide Courts notes and keep the folders, templates and index.
