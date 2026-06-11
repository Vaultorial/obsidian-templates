# Habit Tracker — Obsidian Template

A habit tracker for Obsidian with two levels: plugin-free **monthly grids** (habits × days, check marks in a table) and an optional **Dataview dashboard** that computes streaks, monthly totals and perfect days from tiny per-day log notes. Ships with two fully tracked example months (April–May 2026, five everyday habits, realistically imperfect data).

## Folder structure

```
habit-tracker/
├── Start Here.md                    ← read this first
├── Habits/
│   ├── 2026-04 Habits.md            ← monthly grid, filled
│   ├── 2026-05 Habits.md            ← monthly grid, filled
│   ├── Habit Dashboard.md           ← Dataview: streaks, totals, perfect days
│   └── Daily Log/                   ← 61 per-day notes (frontmatter data)
│       └── 2026-04-01.md … 2026-05-31.md
└── Templates/
    ├── Monthly Habit Tracker.md     ← blank grid for a new month
    └── Habit Log Entry.md           ← one-minute daily log
```

## Installation

1. Unzip the download.
2. Open Obsidian → **Open folder as vault** → select the unzipped folder.
3. Trust the vault when prompted (it ships with plain JSON settings only).
4. Open `Start Here.md`.

To use it inside an existing vault, copy `Habits/` and `Templates/` in and set your template folder to `Templates` (Settings → Templates).

## Plugins

Required: none — the monthly grids are plain Markdown tables.

Optional:

- **Dataview** — powers the Habit Dashboard (streaks need its *JavaScript queries* setting enabled). https://obsidian.md/plugins?id=dataview

## License

MIT. Use it, modify it, ship it — no attribution required.

Template by Vaultorial — https://vaultorial.com/habit-tracker/
