# CRM Vault — Obsidian Template

A personal CRM for Obsidian: contacts, companies, deals and a dated log of every interaction, tied together by Dataview. It ships with a small consultancy's pipeline already filled in, so the dashboard shows real follow-ups, open deals and contacts going cold from the moment you open it.

## How it fits together

- `Contacts/` — one note per person, with `company`, `role`, `relationship`, `last_contact` and `next_follow_up` in the properties.
- `Companies/` — one note per organisation. Each lists its people and deals automatically.
- `Deals/` — one note per opportunity, with `value`, `stage` and `close_date`.
- `Interactions/` — one note per call, email or meeting, named by date. Follow-up tasks live here.
- [[CRM Dashboard]] — follow-ups due this week, open tasks, the pipeline by stage, contacts not reached in 60 days, recent interactions.
- `Pipeline.base` — the same deals as an editable table, using Obsidian's core Bases plugin.

Deal stages used here: `lead`, `qualified`, `proposal`, `negotiation`, `won`, `lost`.

## Plugins

**Dataview** is required for the dashboard and the lists inside each note. The **Templates** core plugin is enabled and pointed at `Templates/`. The pipeline table uses the **Bases** core plugin, included in current versions of Obsidian.

- Dataview — https://obsidian.md/plugins?id=dataview

1. Unzip the download, then in Obsidian choose **Open folder as vault**.
2. Enable community plugins for this vault when asked.
3. Install and enable **Dataview**, then open the CRM Dashboard in reading view.

## License

MIT. Use it, change it, share it — attribution appreciated but not required.

Template by Vaultorial — https://vaultorial.com/obsidian-crm/
