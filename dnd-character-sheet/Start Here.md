# Start Here

This vault turns a D&D 5e character sheet into an Obsidian note. You type the numbers that change rarely (ability scores, level, armor class, maximum hit points) into the note's properties, and Dataview works out everything that follows from them: ability modifiers, proficiency bonus, initiative, saving throws, all eighteen skills, Passive Perception and, for spellcasters, spell save DC and spell attack bonus. Level up by changing one property and the whole sheet updates.

## What is inside

- `Characters/` — three filled example characters: Brannoc Vell (fighter, level 5), Isolde Marrow (wizard, level 5) and Tamsin Reed (rogue, level 4, with expertise).
- [[Party Sheet]] — the whole party in one table, who needs healing, and who is good at what.
- `Templates/Character Sheet` — a blank sheet with every formula already in place.

## Plugins to enable

1. **Dataview** (required). Install it from Community plugins.
2. In Dataview's settings, switch on **JavaScript queries**. The saving throw and skill tables use one short DataviewJS block per sheet; everything else is plain Dataview.

The **Templates** core plugin is already enabled and pointed at `Templates/`.

## How the numbers work

- Modifier = (score − 10) ÷ 2, rounded down. A 16 gives +3, an 8 gives −1.
- Proficiency bonus = +2 at levels 1–4, +3 at 5–8, +4 at 9–12, +5 at 13–16, +6 at 17–20.
- A skill or save you are proficient in adds your proficiency bonus; expertise adds it twice.
- Passive Perception = 10 + your Perception bonus.
- Spell save DC = 8 + proficiency bonus + spellcasting modifier; spell attack = proficiency bonus + spellcasting modifier.

## First steps

1. Enable Dataview and JavaScript queries, then open [[Brannoc Vell]] in reading view.
2. Change his `level` property from 5 to 9 and watch the proficiency bonus, saves and skills change.
3. Open [[Party Sheet]] and change someone's `hp` to see the healing table update.
4. For your own character: new note in `Characters/`, insert the Character Sheet template, fill in the properties.
