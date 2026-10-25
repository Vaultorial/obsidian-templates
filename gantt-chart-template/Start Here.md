# Start Here

This vault draws Gantt charts from your notes. Each task is a note with a `start` and an `end` date in its properties, and the [[Timeline]] note turns every task into a bar: one chart per project, one section per phase. Move a date and the chart redraws. Nothing to export, and every task stays a plain Markdown file you can link, tag and write in.

## What is inside

- `Projects/` — two example projects with dated tasks: an office move and a website relaunch, with finished, active and critical tasks and milestones.
- [[Timeline]] — the generated charts, plus a list of tasks that have no date yet.
- [[Static Gantt Example]] — a hand-written Mermaid Gantt chart that needs no plugin, with the syntax explained.
- `Templates/Task` — a blank task note with every property in place.

## Plugins to enable

1. **Dataview** (required for [[Timeline]]). Install it from Community plugins.
2. In Dataview's settings, switch on **JavaScript queries**.
3. Obsidian draws the charts with Mermaid, which is built in. If a note shows "Display Mermaid diagrams in this vault?", choose Allow.

The **Templates** core plugin is already enabled and pointed at `Templates/`.

## Task properties

- `project` and `phase` decide which chart and which section the bar goes in.
- `start` and `end` are dates written as YYYY-MM-DD. A task without `start` stays off the chart.
- `status`: `done`, `active` or `todo`.
- `critical: true` draws the bar in red; `milestone: true` draws a diamond on the start date.

## First steps

1. Enable Dataview and JavaScript queries, then open [[Timeline]] in reading view.
2. Open any task in `Projects/Office Move/`, change its `end` date and go back to [[Timeline]].
3. For your own project: create a folder in `Projects/`, add task notes from the Task template and fill in the dates.
