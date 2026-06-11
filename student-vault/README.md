# Student Vault for Obsidian

An Obsidian vault for managing coursework, organized by term and course, with a Dataview dashboard that surfaces every upcoming deadline and exam from note frontmatter. Ships with two example courses, twelve filled notes across lectures, exam prep and readings, and three templates.

## Folder structure

```
student-vault/
├── Start Here.md          ← read this first
├── Dashboard.md           ← Dataview: deadlines + exams, auto-built
├── 2026 Spring/
│   ├── Biology 101/       ← lectures, exam prep, reading notes
│   └── Statistics 201/    ← lectures, exam prep, reading notes
└── Templates/             ← Lecture Note / Exam Prep / Reading Note
```

## How it works

Notes carry `due` and `type` fields in their frontmatter. `Dashboard.md` queries across the whole vault: a deadlines table (anything with a future `due`), an exams table (`type: exam`), and a per-course breakdown. Edit a date in any note and the dashboard reflects it immediately. Add a course by copying a course folder; add a term with a new `YYYY Season/` folder.

## Installation

1. Unzip the download.
2. Open Obsidian → **Open folder as vault** → select the unzipped folder.
3. Turn off restricted mode when prompted, then install Dataview (link below) and enable it.
4. Open `Dashboard.md` — the tables should populate from the example notes.

## Plugins

- **Required:** Dataview — https://obsidian.md/plugins?id=dataview — powers the dashboard.
- **Optional:** Calendar — https://obsidian.md/plugins?id=calendar — month-view companion for daily notes.

## License

MIT. Use it, change it, build on it — personally or commercially. No attribution required.

Template by Vaultorial — https://vaultorial.com/student-vault/
