# Start Here

Welcome, DM. This vault is a campaign management system for tabletop games compatible with the world's most popular fifth-edition ruleset. It ships with a complete original mini-campaign — **The Salt Road Conspiracy** — already loaded: three played sessions, eight NPCs, four locations, three encounters, three player characters and the lore that ties them together. Run it as written, strip it for parts, or delete it and keep the structure.

## How the vault is organized

- `Sessions/` — one note per session: recap, scenes, clues handed out, and a "next time" block that becomes your prep list.
- `NPCs/` — one note per character, with `role`, `location`, `status` and `faction` in the frontmatter so the [[DM Screen]] can sort them.
- `Locations/` — one note per place the party can visit, each linking its NPCs, encounters and rumors.
- `Encounters/` — prepped encounters with original stat blocks, terrain notes and tactics. `status: ready` means runnable tonight; `status: run` keeps the record.
- `PCs/` — one note per player character: the table copy of bonds, goals and the campaign hooks attached to them.
- `Lore/` — the moving parts of the world (factions, history) that more than one note needs to agree on.
- `Templates/` — one template per entity type, wired to the Templates core plugin.
- [[DM Screen]] — the dashboard. Dataview queries pull NPCs by location, recent sessions, ready encounters and the party roster.

## Plugins to enable

1. **Dataview** (required) — powers every table on the [[DM Screen]].
2. **Leaflet** (optional) — once you add map images to the vault, a `leaflet` code block turns them into pannable, pinnable maps. Nothing in the vault depends on it.
3. **Initiative Tracker** (optional) — runs turn order in the sidebar; pairs well with the encounter notes.

The **Templates** core plugin is already enabled and pointed at `Templates/`.

## First steps

1. Enable Dataview and open [[DM Screen]] in reading view — every table should be populated.
2. Read [[The Salt Road]] for the campaign's spine, then [[Session 3 - Salt in the Wound]] to see where the table left off. The [[Counting House Break-In]] is prepped and ready for the next session.
3. Before your own session zero: duplicate the templates workflow — new note in the right folder, insert the matching template, fill the frontmatter.
4. After each session, write the session note while it is fresh, update any NPC whose `status` changed, and set next session's encounter notes to `ready`.

> [!note] On the content
> Everything here — the Brinemark, its people, its monsters — is original to this template. Stat lines like "AC 13, HP 26" are houseruled creations for this campaign, not reproductions from any rulebook, so the vault stays compatible without copying anyone's text.
