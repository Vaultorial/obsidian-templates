# Start Here

Welcome. This vault is a lightweight project management system for Obsidian: one note per project, one note per meeting, and a Dataview dashboard that reads everything else. Two complete example projects — a website redesign and an office move — come pre-loaded with milestones, Mermaid timelines and linked meeting notes, so every dashboard query has real data behind it.

## How the vault is organized

- `Projects/` — one note per project. The frontmatter carries the fields the dashboard reads (`status`, `owner`, `start`, `due`, `area`); the body holds objectives, a milestone table, a Gantt timeline and links to that project's meetings.
- `Meetings/` — one note per meeting, named `YYYY-MM-DD Project Topic`. Each links back to its project in the frontmatter, so the dashboard can roll up open action items per project.
- [[Dashboard]] — live tables: active projects, projects by status and by owner, upcoming due dates, recent meetings, and every unchecked action item across all meeting notes.
- `Templates/` — [[Project Template]] and [[Meeting Template]], wired to the Templates core plugin.

## Conventions that make the dashboard work

- `status` is one of: `planning`, `active`, `on-hold`, `done`. Lowercase, exact — Dataview matches strings literally.
- `owner` is a name, written the same way everywhere ("Sarah Chen", not "S. Chen" in one file and "sarah" in another).
- Dates are `YYYY-MM-DD`. Dataview parses them as real dates, which is what makes the "due soon" query possible.
- Action items in meeting notes are plain `- [ ]` checkboxes. Tick them where they live; the dashboard reflects it.

## Plugins to enable

1. **Dataview** (required) — Settings → Community plugins → Browse → "Dataview". The dashboard is built on it.

Mermaid timelines render with Obsidian's built-in Mermaid support — no plugin needed. The **Templates** core plugin is already enabled and pointed at `Templates/`.

Current versions of Obsidian ask once per vault before drawing Mermaid diagrams. When a project note shows "Display Mermaid diagrams in this vault?", choose Allow, or switch on "Display Mermaid diagrams in notes" under Settings, Editor.

## First steps

1. Enable Dataview, then open [[Dashboard]] in reading view. Every table should be populated.
2. Open [[Website Redesign]] and skim it top to bottom — frontmatter, milestones, timeline, meetings. That note is the pattern.
3. Create your first real project: new note in `Projects/`, insert [[Project Template]] (command palette → "Templates: Insert template"), fill the frontmatter.
4. After your next meeting, create a note in `Meetings/` from [[Meeting Template]] and link it to the project.
5. Delete the two example projects and their meetings once you have your own.
