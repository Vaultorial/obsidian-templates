# Cornell Notes Template for Obsidian

An Obsidian vault implementing the Cornell note-taking method with plain callouts and a single CSS snippet: a cue column on the left, notes on the right, summary band below. No community plugins. Ships with two templates (generic Cornell and a Class Notes variant with course metadata) and three fully worked example notes.

## Folder structure

```
cornell-notes-template/
├── Start Here.md             ← read this first
├── Notes/                    ← 3 filled example class notes
├── Templates/                ← Cornell Note + Class Notes (Cornell)
└── .obsidian/snippets/
    └── cornell.css           ← the two-column layout (pre-enabled)
```

## How it works

Each note uses three callouts — `[!cue]`, `[!notes]`, `[!summary]` — and the `cornell.css` snippet lays them out as the classic Cornell page: floated cue column (32%), notes beside it, summary cleared underneath, collapsing to stacked blocks on narrow windows. The snippet ships pre-enabled via `appearance.json`; it can be toggled in Settings → Appearance → CSS snippets.

The Class Notes variant adds `course`, `professor` and `date` frontmatter so class notes stay sortable and searchable by subject.

## Installation

1. Unzip the download.
2. Open Obsidian → **Open folder as vault** → select the unzipped folder.
3. Keep restricted mode on if asked — there are no community plugins here.
4. Open a note in `Notes/` in reading view; you should see two columns. If not, enable the **cornell** snippet under Settings → Appearance → CSS snippets.

## Plugins

- **Required:** none. Core Templates only (preconfigured to the `Templates` folder).
- **Optional:** none.

## License

MIT. Use it, change it, build on it — personally or commercially. No attribution required.

Template by Vaultorial — https://vaultorial.com/cornell-notes-template/
