# Start Here

Welcome. This vault does one thing: a single weekly note that holds both your **plan for the week** and your **review of it**. Plan on Monday, review on Friday or Sunday, same file. Four filled example weeks show what it looks like when a real month passes through it.

## How the vault is organized

- `Weekly/` — one note per ISO week, named `2026-W19`, `2026-W20`, and so on. The four examples cover May 2026 and read as a continuous story: watch how unfinished items crawl from one week's **Carried over** into the next week's plan. That loop is the whole method.
- `Templates/` — two versions of the weekly template:
	- **Weekly Note (core Templates)** — no plugins needed.
	- **Weekly Note (Templater)** — adds the week's date range and prev/next week links, computed from the file name.

## First steps

1. Read `2026-W19` through `2026-W22` in order. Five minutes, and you will know exactly how to run the system.
2. Create your own current week: new note in `Weekly/` named with this week's ISO number (e.g. `2026-W24`), then insert the template with **Insert template** from the command palette.
3. On Monday fill **Focus** and 3–5 plan tasks. During the week, touch nothing. At the end of the week fill the review in one sitting.
4. Anything unfinished goes to **Carried over** — and must show up in next week's plan or be deliberately dropped. Items that drag three weeks running are telling you something.

## Plugins

Core plugins only by default. Two optional upgrades:

- **Periodic Notes** — adds an "open this week's note" command and calendar-style week navigation. After installing, set the weekly format to `GGGG-[W]WW` and folder to `Weekly`.
- **Templater** — needed for the `Weekly Note (Templater)` variant. Set its template folder to `Templates`.

> [!tip] Keep the review honest
> The **Numbers** section tracks only things you actually count (workouts, study sessions, pages). Two or three metrics are plenty — the moment logging feels like accounting, cut one.
