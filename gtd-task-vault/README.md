# GTD Task Vault — Obsidian Template

A ready-to-use Getting Things Done system for Obsidian, powered by the Tasks plugin. It implements the full GTD loop — capture, clarify, organize, reflect, engage — with a live dashboard, context tags, and three fully worked sample projects so you can see the system running before you trust it with your own work.

## Structure

```
gtd-task-vault/
├── Start Here.md          ← read this first
├── Dashboard.md           ← live task queries (due, overdue, contexts, waiting)
├── 00 Inbox.md            ← capture everything here
├── 01 Next Actions.md     ← standalone actions with context tags
├── 02 Waiting For.md      ← delegated and blocked items
├── 03 Someday Maybe.md    ← ideas without commitment
├── Projects/              ← one note per project, tasks live here
│   ├── Kitchen Renovation.md
│   ├── Portfolio Website Refresh.md
│   └── Lakeside Camping Trip.md
└── Templates/
    └── Project.md         ← template for new project notes
```

GTD contexts are nested tags (`#context/home`, `#context/computer`, `#context/errands`), since Obsidian tags cannot start with `@`.

## Installation

1. Download and unzip the template: **Unzip → Obsidian → Open folder as vault**.
2. When Obsidian asks, enable community plugins for this vault.
3. Install the plugins listed below, then open `Dashboard.md` in reading view.

## Plugins

**Required**

- Tasks — https://obsidian.md/plugins?id=obsidian-tasks-plugin

**Optional**

- Dataview — https://obsidian.md/plugins?id=dataview (projects overview table on the dashboard)

## License

MIT. Use it, change it, share it — attribution appreciated but not required.

Template by Vaultorial — https://vaultorial.com/gtd-task-vault/
