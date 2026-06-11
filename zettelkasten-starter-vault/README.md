# Zettelkasten Starter Vault

An Obsidian starter vault for the Zettelkasten method, pre-populated with a working example: fourteen linked notes on learning and memory that demonstrate the full fleeting → literature → permanent pipeline, timestamp IDs, and an index as the entry point.

## Folder structure

```
zettelkasten-starter-vault/
├── Start Here.md      ← read this first
├── Index.md           ← entry point into the permanent notes
├── Fleeting/          ← quick captures, processed then deleted (3 examples)
├── Literature/        ← one note per source, own words (3 examples)
├── Permanent/         ← one idea per note, timestamp IDs (8 examples)
└── Templates/         ← fleeting / literature / permanent templates
```

Permanent notes are named `YYYYMMDDHHMM Title.md` (for example `202605141030 Write notes in your own words.md`). The ID makes every note uniquely addressable and keeps filenames stable even if titles evolve.

## Installation

1. Unzip the download.
2. Open Obsidian → **Open folder as vault** → select the unzipped folder.
3. Enable the core **Templates** plugin if needed (Settings → Core plugins); it is already pointed at `Templates`.
4. Optional: install Templater (below) and the permanent-note template will generate its timestamp ID automatically.

## Plugins

- **Required:** none — the vault works out of the box with core plugins.
- **Optional:** Templater — https://obsidian.md/plugins?id=templater-obsidian — auto-fills the `YYYYMMDDHHMM` ID and dates in the templates. Without it, type the ID manually.

## License

MIT. Use it, change it, build on it — personally or commercially. No attribution required.

Template by Vaultorial — https://vaultorial.com/zettelkasten-starter-vault/
