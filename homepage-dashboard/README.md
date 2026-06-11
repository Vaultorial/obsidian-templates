# Homepage / Dashboard — Obsidian Template

A homepage system for Obsidian: a dashboard note with today's tasks, upcoming week, active projects, recently edited notes and vault counts — in two variants. `Home (simple)` runs on callouts and static links with zero plugins; `Home` is the live version powered by Dataview queries over `[due:: ]` task dates, designed to be opened at launch by the Homepage plugin. Ships with a small but fully cross-linked example vault (3 projects, 2 areas, 3 evergreen notes with realistic dated tasks) so every dashboard section shows real data out of the box.

## Folder structure

```
homepage-dashboard/
├── Start Here.md            ← read this first
├── Home.md                  ← live dashboard (Dataview)
├── Home (simple).md         ← plugin-free dashboard
├── Projects/                ← 3 example projects with dated tasks
├── Areas/                   ← 2 ongoing areas with dated tasks
└── Notes/                   ← 3 evergreen notes (list, checklist, recipe)
```

## Installation

1. Unzip the download.
2. Open Obsidian → **Open folder as vault** → select the unzipped folder.
3. Trust the vault when prompted (it ships with plain JSON settings only).
4. Open `Start Here.md`, then `Home (simple)` — it works immediately. Install the plugins below to bring `Home` alive.

To use it inside an existing vault, copy `Home.md` and `Home (simple).md` in and adjust the folder names inside the queries (`FROM "Projects" OR "Areas"`) to match your structure.

## Plugins

Required for the live dashboard:

- **Dataview** — runs the queries in `Home.md`. https://obsidian.md/plugins?id=dataview

Optional:

- **Homepage** — opens your dashboard automatically on startup. https://obsidian.md/plugins?id=homepage

`Home (simple).md` needs no plugins at all.

## License

MIT. Use it, modify it, ship it — no attribution required.

Template by Vaultorial — https://vaultorial.com/homepage-dashboard/
