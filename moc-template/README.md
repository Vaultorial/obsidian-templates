# MOC Starter Kit

An Obsidian starter vault for organizing notes with Maps of Content (MOCs). It ships fully worked: a home MOC, three topic MOCs (productivity, learning, writing) and fifteen interlinked notes beneath them — open the graph view and the three-level tree is already there.

## Folder structure

```
moc-template/
├── Start Here.md       ← read this first
├── Home MOC.md         ← level 1: the single entry point
├── MOCs/               ← level 2: one map per topic (3 examples)
├── Notes/              ← level 3: one idea per note, flat (15 examples)
└── Templates/          ← MOC template with the linking conventions
```

## Conventions used throughout

- **Home MOC → MOC → note**: the home page links only to MOCs; MOCs link to notes with a line of context each; notes link `Up:` to their MOC and sideways to related notes.
- Notes live flat in `Notes/` — the maps carry the structure, not the folder tree.

## Installation

1. Unzip the download.
2. Open Obsidian → **Open folder as vault** → select the unzipped folder.
3. If Obsidian asks about restricted mode, keep it on — this vault uses no community plugins.
4. Enable the core **Templates** plugin (Settings → Core plugins) to use the MOC template.

## Plugins

- **Required:** none. Works entirely with core plugins.
- **Optional:** none.

## License

MIT. Use it, change it, build on it — personally or commercially. No attribution required.

Template by Vaultorial — https://vaultorial.com/moc-template/
