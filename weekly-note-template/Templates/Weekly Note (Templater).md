---
week: <% tp.file.title %>
start: <% moment(tp.file.title, "GGGG-[W]WW").startOf("isoWeek").format("YYYY-MM-DD") %>
end: <% moment(tp.file.title, "GGGG-[W]WW").endOf("isoWeek").format("YYYY-MM-DD") %>
type: weekly
---

# <% tp.file.title %> — <% moment(tp.file.title, "GGGG-[W]WW").startOf("isoWeek").format("MMM D") %>–<% moment(tp.file.title, "GGGG-[W]WW").endOf("isoWeek").format("D, YYYY") %>

← [[<% tp.date.now("GGGG-[W]WW", -7, tp.file.title, "GGGG-[W]WW") %>]] | [[<% tp.date.now("GGGG-[W]WW", 7, tp.file.title, "GGGG-[W]WW") %>]] →

## Week plan

**Focus:**

- [ ]
- [ ]
- [ ]

## Review

### Wins

-

### Numbers

| Metric | Target | Actual |
| ------ | ------ | ------ |
|        |        |        |

### Carried over

-

### Next week focus

-

> [!note]- How to use this template
> Templater variant. The week range and prev/next links are derived from the file name, so name the note `2026-W24` (ISO week) and apply the template via Templater. Setup: install Templater and set `Templates` as its template folder. Delete this callout from your own copy.
