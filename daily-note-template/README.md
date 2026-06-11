# Daily Note Starter — Obsidian Template

A clean daily note system for Obsidian: one note per day with **Agenda, Tasks, Log and Gratitude** sections, prev/next day navigation, and a fully worked example week so you can see the system in use before you commit to it.

Two template variants are included: one that runs on core plugins only, and one powered by Templater with automatic date handling.

## Folder structure

```
daily-note-template/
├── Start Here.md                      ← read this first
├── Daily/                             ← one note per day (7 example days, June 2026)
│   ├── 2026-06-01.md … 2026-06-07.md
└── Templates/
    ├── Daily Note (core Templates).md ← no plugins needed
    └── Daily Note (Templater).md      ← adds prev/next links
```

## Installation

1. Unzip the download.
2. Open Obsidian → **Open folder as vault** → select the unzipped folder.
3. Trust the vault when prompted (it ships with plain JSON settings only).
4. Open `Start Here.md`.

To use it inside an existing vault instead, copy the `Daily/` and `Templates/` folders in, and mirror the Daily notes settings (folder `Daily`, format `YYYY-MM-DD`, template `Templates/Daily Note (core Templates)`).

## Plugins

Required: none — the core-only variant works immediately.

Optional:

- **Templater** — dynamic dates and prev/next day links. https://obsidian.md/plugins?id=templater-obsidian

## License

MIT. Use it, modify it, ship it — no attribution required.

Template by Vaultorial — https://vaultorial.com/daily-note-template/
