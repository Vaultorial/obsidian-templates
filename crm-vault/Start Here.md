# Start Here

This vault is a working personal CRM. Every person, company and deal is a note, every conversation is a dated note in Interactions, and the [[CRM Dashboard]] pulls it together. The sample data belongs to an invented design consultancy so that every query has something to show. Delete it once your own contacts are in.

## How it fits together

- `Contacts/` — one note per person, with `company`, `role`, `relationship`, `last_contact` and `next_follow_up` in the properties.
- `Companies/` — one note per organisation. Each lists its people and deals automatically.
- `Deals/` — one note per opportunity, with `value`, `stage` and `close_date`.
- `Interactions/` — one note per call, email or meeting, named by date. Follow-up tasks live here.
- [[CRM Dashboard]] — follow-ups due this week, open tasks, the pipeline by stage, contacts not reached in 60 days, recent interactions.
- `Pipeline.base` — the same deals as an editable table, using Obsidian's core Bases plugin.

## The weekly routine

After each conversation, create an interaction note from the template and link the contact. Update the contact's `last_contact` and `next_follow_up`, and move the deal's `stage` if it changed. Once a week, open the dashboard and work through the follow-ups at the top.

Deal stages used here: `lead`, `qualified`, `proposal`, `negotiation`, `won`, `lost`.

## Plugins

**Dataview** is required for the dashboard and the lists inside each note. The **Templates** core plugin is enabled and pointed at `Templates/`. The pipeline table uses the **Bases** core plugin, included in current versions of Obsidian.
