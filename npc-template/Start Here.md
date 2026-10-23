# Start Here

A complete NPC kit for game masters: a full NPC template with personality, voice, secrets, hooks and relationships, a quick NPC template for improvising at the table, and a Dataview roster that sorts your cast by location, faction and attitude. It ships with Cinderbrook, an original river town with six detailed NPCs and three quick ones, so every view has data on day one.

## What is in the vault

- `NPCs/` — six full NPCs with `role`, `location`, `faction`, `attitude`, `status`, `first_met` and `revealed` properties.
- `Quick NPCs/` — three quick NPCs: look, want, voice and secret on one screen.
- `Factions/` and `Locations/` — two factions and two places, each listing its people automatically.
- [[NPC Roster]] — the Dataview roster: by location, by attitude, faction members, quick NPCs and unrevealed secrets.
- `Templates/` — NPC and Quick NPC templates.

## Using it at the table

Before a session, check the roster for who the party might meet and which secrets are still hidden. When you improvise a character, fill a quick NPC in under a minute. If the party comes back to them, promote them: create a full NPC from the template and link the quick note. After the session, update `attitude` and set `revealed: true` on any secret that came out.

System neutral. The optional stat block uses 5e-style fields with original numbers; replace or delete it for other systems.

## Plugins

**Dataview** powers the roster and the member lists on faction and location notes. The **Templates** core plugin is enabled and pointed at `Templates/`.
