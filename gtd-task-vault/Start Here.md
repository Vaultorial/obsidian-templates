# Start Here

Welcome. This vault is a working Getting Things Done setup for Obsidian, built around the Tasks plugin. It ships with three sample projects and over thirty tasks so every view on the [[Dashboard]] has something to show. Replace the samples with your own work as you go — the structure is the product, the content is just a demonstration.

## How the vault is organized

- [[00 Inbox]] — capture point. Everything lands here first, unsorted.
- [[01 Next Actions]] — single actions that are not part of a project, tagged with a context.
- [[02 Waiting For]] — things you have delegated or are blocked on, tagged `#waiting`.
- [[03 Someday Maybe]] — ideas you are not committing to yet. Plain bullets on purpose: they are not actionable, so they stay out of the task queries.
- `Projects/` — one note per project. Tasks live inside the project note that owns them.
- [[Dashboard]] — the cockpit. Live queries pull tasks from the whole vault: due today, overdue, by context, waiting, and inbox items to process.
- `Templates/` — contains [[Project]], the template for new project notes.

## Contexts

GTD contexts (the classic @home, @computer, @errands) are nested tags here, because Obsidian tags cannot contain the `@` character:

- `#context/home`
- `#context/computer`
- `#context/errands`

Add a context tag to any task and it shows up in the matching Dashboard section. Add your own contexts (`#context/phone`, `#context/office`) by tagging tasks with them and copying a query block on the Dashboard.

## Plugins to enable

1. **Tasks** (required) — Settings → Community plugins → Browse → "Tasks". Powers every query on the Dashboard.
2. **Dataview** (optional) — used only for the projects overview table at the bottom of the Dashboard. Everything else works without it.

The **Templates** core plugin is already enabled and pointed at the `Templates/` folder.

## First steps

1. Enable the Tasks plugin, then open [[Dashboard]] in reading view. Every section should be populated by the sample data.
2. Capture a few real to-dos into [[00 Inbox]] as plain `- [ ]` checkboxes. Capture is meant to be fast and messy.
3. Process the inbox: anything under two minutes, do now. Single actions move to [[01 Next Actions]] with a context tag and, if it matters, a due date (`📅 2026-06-15`). Multi-step outcomes become a note in `Projects/` — use the [[Project]] template.
4. Once a week, do a review: clear the inbox to zero, scan every project for a stalled next action, and chase anything in [[02 Waiting For]].
5. When the sample projects have served their purpose, delete them.

> [!tip] Task syntax cheat sheet
> `- [ ] Call the plumber #context/home ⏫ 📅 2026-06-15`
> `📅` due date · `⏫` high priority · `🔽` low priority · `🔁 every week` recurrence · `✅` completion date (added automatically when you tick the box).
