# Start Here

Welcome. This vault turns Obsidian into a Cornell note-taking system using three callouts and one CSS snippet — no plugins at all.

## How the layout works

Every Cornell note is built from three callouts:

- `> [!cue]` — the narrow left column: questions and keywords, written *after* the class.
- `> [!notes]` — the wide right column: what you capture live.
- `> [!summary]` — the full-width band at the bottom: the whole page in two or three of your own sentences.

The included CSS snippet (`cornell`, already enabled in this vault's appearance settings) floats the cue callout left, sets the notes callout beside it, and clears the summary underneath — the classic Cornell page. On narrow windows it gracefully collapses to stacked blocks. If the columns ever look stacked on a wide window, check Settings → Appearance → CSS snippets and make sure **cornell** is on.

## See it filled in

Three completed class notes live in `Notes/`:

- [[Statistics - Describing Data]]
- [[History - The Printing Press]]
- [[Biology - Photosynthesis Overview]]

Open one in reading view first to see the layout doing its job.

## The workflow the layout is for

1. **During class:** write only in the notes zone. Short lines, abbreviations, gaps are fine.
2. **Same day, ten minutes:** fill the cue column — turn each chunk of notes into a question or keyword in the margin.
3. **Then the summary:** two or three sentences, your own words, no peeking at the notes zone.
4. **To review:** cover the notes column and answer the cue questions out loud. The cues make self-testing possible; the summary tells you tomorrow what this page was about.

## First steps

1. Read one example note, then its raw Markdown (toggle to editing view) to see how little syntax there is.
2. Create a note from `Templates/Class Notes (Cornell).md` — the core Templates plugin is preconfigured — and take your next set of notes in it.
3. Use `Templates/Cornell Note.md` for non-class material: meetings, reading, talks.

## Plugins

None required, none suggested. Core **Templates** only, already pointed at the `Templates` folder.
