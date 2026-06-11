# Start Here

Welcome. This is a working student vault for one term: two courses, real lecture notes, exam prep and readings already in place, plus a [[Dashboard]] that pulls every deadline and exam into one view automatically.

## How it's organized

- **By term and course:** `2026 Spring/Biology 101/` and `2026 Spring/Statistics 201/`. Add a folder per course each new term — the structure scales by copying it.
- **Three note types per course**, each from a template: lecture notes, exam prep, and reading notes.
- **[[Dashboard]]** reads the `due` and `type` fields from every note's frontmatter and lists what is coming up. It is built by Dataview — change a due date in a note and the dashboard updates itself.

The example notes are deliberately filled with correct, general material (cell biology, descriptive statistics) so you can see the structure on real content before replacing it with your own.

## First steps

1. Install and enable **Dataview** (required for the [[Dashboard]]): Settings → Community plugins → Browse → "Dataview".
2. Open [[Dashboard]] and confirm the deadline and exam tables render.
3. Make a course folder for one of your real courses inside `2026 Spring/` (or a new term folder).
4. Take your next lecture in a copy of `Templates/Lecture Note.md` (core Templates plugin, already configured). Set a `due` date on anything with a deadline and it appears on the dashboard.
5. Optional: install **Calendar** for a month view that sits alongside your daily notes.

## The note types

- **Lecture Note** — date, topic, and a clean spot for the day's material plus questions to review later.
- **Exam Prep** — `type: exam` and a `due` date so it surfaces on the dashboard; a checklist of topics to drill.
- **Reading Note** — source, the assignment's `due` date, and your own summary of what you read.

## Plugins

- **Required:** Dataview — the dashboard needs it.
- **Optional:** Calendar — month view for daily notes.
- Core **Templates** is already enabled and pointed at `Templates`.

> [!tip] One habit makes this vault pay off
> Put a `due` date in the frontmatter the moment a deadline is announced. The dashboard can only show what you tell it — but if you tell it, you never track deadlines by memory again.
