# Project Management Vault — Obsidian Template

A plain-files project management system for Obsidian. Each project is a single note with structured frontmatter, a milestone table, a Mermaid Gantt timeline and linked meeting notes; a Dataview dashboard rolls everything up by status, owner and due date. Ships with two fully worked examples — a website redesign and an office move — including four realistic meeting notes.

## Structure

```
project-management-template/
├── Start Here.md       ← read this first
├── Dashboard.md        ← Dataview rollups: status, owner, due dates, action items
├── Projects/
│   ├── Website Redesign.md
│   └── Office Move.md
├── Meetings/           ← one note per meeting, linked to its project
│   ├── 2026-04-02 Website Redesign Kickoff.md
│   ├── 2026-05-07 Website Redesign Design Review.md
│   ├── 2026-04-21 Office Move Vendor Walkthrough.md
│   └── 2026-05-19 Office Move Logistics Sync.md
└── Templates/
    ├── Project Template.md
    └── Meeting Template.md
```

## Installation

1. Download and unzip the template: **Unzip → Obsidian → Open folder as vault**.
2. When Obsidian asks, enable community plugins for this vault.
3. Install Dataview, then open `Dashboard.md` in reading view.

## Plugins

**Required**

- Dataview — https://obsidian.md/plugins?id=dataview

Gantt timelines use Obsidian's built-in Mermaid rendering; no extra plugin needed.

## License

MIT. Use it, change it, share it — attribution appreciated but not required.

Template by Vaultorial — https://vaultorial.com/project-management-template/
