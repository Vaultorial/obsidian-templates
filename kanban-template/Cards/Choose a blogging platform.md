---
type: card
board: "[[Project Board]]"
column: Done
---

# Choose a blogging platform

Started as a card on [[Project Board]]; escalated to a note once the comparison needed more than one line. Decision is made — keeping the note as a record of why.

## Requirements

- Own the content: plain files or easy export, no platform lock-in.
- Custom domain on the free or cheap tier.
- Markdown writing flow, ideally straight from this vault.
- Fast pages without fighting a theme.

## Options considered

- **Hosted blogging service** — fastest start, weakest ownership story. Custom domain pushed me into a paid plan, and export quality varies a lot between services.
- **Static site generator + cheap hosting** — full ownership, Markdown-native, free tiers are generous. Costs setup time and a little command-line comfort.
- **Self-hosted CMS** — most powerful, but it is a server to babysit. Overkill for a personal blog.

## Decision

Static site generator, deployed on a free static host. The writing already lives in Markdown, so publishing becomes a copy step rather than a porting step. Accepted trade-off: the first-week setup cost.

## Follow-ups created on the board

- Theme and typography (done)
- [[Design the homepage layout]]
- [[Set up analytics and search console]]
