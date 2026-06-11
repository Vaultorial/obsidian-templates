# Start Here

Welcome. This vault is a meeting notes system for Obsidian: three ready-made templates (team meeting, 1-on-1, client call), a Dataview dashboard that finds every meeting and every unfinished action item, and four filled-in example meetings from one coherent project so you can see the system working before you adopt it.

## How the vault is organized

- `Templates/` — the product. [[Team Meeting]], [[1-on-1]] and [[Client Call]], each with structured frontmatter (`type`, `date`, `project`, `attendees`) and the same four sections: agenda, notes, decisions, action items.
- `Meetings/` — one note per meeting, named `YYYY-MM-DD Topic`. The examples follow a consultancy project (a client portal build for an insurance client) across a kickoff, a 1-on-1, a client call and a sprint review.
- [[Meetings Dashboard]] — Dataview rollups: recent meetings, meetings by type, by project, and all open action items in one place.

## Conventions that make the dashboard work

- `type` is one of: `team-meeting`, `one-on-one`, `client-call`. Lowercase, hyphenated, exact.
- `project` is a short plain-text label ("Client Portal"). Use identical spelling across meetings — the dashboard groups by it.
- Action items are written in Tasks-plugin format: `- [ ] Owner — what they will do 📅 2026-06-15`. This vault only needs the checkbox part (Dataview reads it), but the date syntax means you can drop these lines into a GTD vault running the Tasks plugin — like our GTD Task Vault — and they will be picked up as scheduled tasks unchanged.
- Decisions get their own section. Six months later, nobody re-reads notes; they search for what was decided.

## Plugins to enable

1. **Dataview** (required) — Settings → Community plugins → Browse → "Dataview". Powers the dashboard.
2. **Templater** (optional) — if you already use Templater, point it at `Templates/` and swap the `{{date}}` and `{{title}}` variables for your preferred dynamic commands. The templates ship in core-Templates syntax so they work out of the box.

The **Templates** core plugin is already enabled and pointed at `Templates/`.

## First steps

1. Enable Dataview and open [[Meetings Dashboard]] in reading view — every section should be populated by the four example meetings.
2. Open [[2026-05-04 Client Portal Kickoff]] to see a filled-in note next to its template.
3. Before your next meeting: create a note in `Meetings/` named with the date and topic, insert the matching template (command palette → "Templates: Insert template"), and fill the frontmatter.
4. During the meeting, write only in notes/decisions/action items. After it, spend one minute assigning owners and dates to the action items.
5. Delete the example meetings once you have a few of your own.
