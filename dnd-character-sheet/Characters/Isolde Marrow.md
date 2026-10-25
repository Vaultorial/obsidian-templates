---
type: character
player: Priya
class: Wizard
level: 5
species: High Elf
background: Sage
str: 8
dex: 14
con: 14
int: 18
wis: 12
cha: 10
ac: 12
max_hp: 32
hp: 32
hit_dice: 5d6
speed: 30
saves:
  - Intelligence
  - Wisdom
skills:
  - Arcana
  - History
  - Investigation
  - Insight
expertise:
  -
spellcasting: int
---

# Isolde Marrow

Level `= this.level` · `= this.species` · `= this.class` · `= this.background`

An archivist who left the library to find the books it was missing.

## Ability scores

| Ability | Score | Modifier |
| --- | --- | --- |
| Strength | `= this.str` | `= choice(floor((this.str - 10) / 2) >= 0, "+" + floor((this.str - 10) / 2), floor((this.str - 10) / 2))` |
| Dexterity | `= this.dex` | `= choice(floor((this.dex - 10) / 2) >= 0, "+" + floor((this.dex - 10) / 2), floor((this.dex - 10) / 2))` |
| Constitution | `= this.con` | `= choice(floor((this.con - 10) / 2) >= 0, "+" + floor((this.con - 10) / 2), floor((this.con - 10) / 2))` |
| Intelligence | `= this.int` | `= choice(floor((this.int - 10) / 2) >= 0, "+" + floor((this.int - 10) / 2), floor((this.int - 10) / 2))` |
| Wisdom | `= this.wis` | `= choice(floor((this.wis - 10) / 2) >= 0, "+" + floor((this.wis - 10) / 2), floor((this.wis - 10) / 2))` |
| Charisma | `= this.cha` | `= choice(floor((this.cha - 10) / 2) >= 0, "+" + floor((this.cha - 10) / 2), floor((this.cha - 10) / 2))` |

## Combat

- **Armor Class:** `= this.ac`
- **Hit points:** `= this.hp` / `= this.max_hp`
- **Hit dice:** `= this.hit_dice`
- **Speed:** `= this.speed` ft
- **Proficiency bonus:** +`= floor((this.level - 1) / 4) + 2`
- **Initiative:** `= choice(floor((this.dex - 10) / 2) >= 0, "+" + floor((this.dex - 10) / 2), floor((this.dex - 10) / 2))`
- **Passive Perception:** `= 10 + floor((this.wis - 10) / 2) + choice(contains(this.skills, "Perception"), floor((this.level - 1) / 4) + 2, 0)`

## Saving throws and skills

The block below needs *JavaScript queries* switched on in Dataview's settings. ● marks proficiency, ◆ expertise.

```dataviewjs
const p = dv.current();
const prof = Math.floor((p.level - 1) / 4) + 2;
const mod = (score) => Math.floor((score - 10) / 2);
const sign = (n) => (n >= 0 ? "+" : "") + n;
const has = (list, name) => (list ?? []).includes(name);
const abilities = [["Strength", "str"], ["Dexterity", "dex"], ["Constitution", "con"], ["Intelligence", "int"], ["Wisdom", "wis"], ["Charisma", "cha"]];
const skills = [["Acrobatics", "dex"], ["Animal Handling", "wis"], ["Arcana", "int"], ["Athletics", "str"], ["Deception", "cha"], ["History", "int"], ["Insight", "wis"], ["Intimidation", "cha"], ["Investigation", "int"], ["Medicine", "wis"], ["Nature", "int"], ["Perception", "wis"], ["Performance", "cha"], ["Persuasion", "cha"], ["Religion", "int"], ["Sleight of Hand", "dex"], ["Stealth", "dex"], ["Survival", "wis"]];
const short = Object.fromEntries(abilities.map(([name, key]) => [key, name.slice(0, 3)]));
dv.table(["Saving throw", "Bonus"], abilities.map(([name, key]) => {
  const proficient = has(p.saves, name);
  return [(proficient ? "● " : "○ ") + name, sign(mod(p[key]) + (proficient ? prof : 0))];
}));
dv.table(["Skill", "Ability", "Bonus"], skills.map(([name, key]) => {
  const expert = has(p.expertise, name);
  const proficient = expert || has(p.skills, name);
  const bonus = mod(p[key]) + (expert ? 2 * prof : proficient ? prof : 0);
  return [(expert ? "◆ " : proficient ? "● " : "○ ") + name, short[key], sign(bonus)];
}));
```

## Spellcasting

- **Spell save DC:** `= 8 + floor((this.level - 1) / 4) + 2 + floor((this.int - 10) / 2)`
- **Spell attack bonus:** +`= floor((this.level - 1) / 4) + 2 + floor((this.int - 10) / 2)`
- **Spell slots:** 1st level 4 · 2nd level 3 · 3rd level 2
- **Cantrips:** Fire Bolt, Mage Hand, Prestidigitation, Light
- **Prepared spells:** Mage Armor, Magic Missile, Shield, Detect Magic, Misty Step, Hold Person, Fireball, Counterspell

## Features and traits

- Arcane Recovery (recover spell slots worth 3 levels on a short rest, once per day)
- Arcane Tradition: School of Evocation
- Sculpt Spells (protect allies from her own evocation spells)
- Darkvision 60 ft and Fey Ancestry

## Equipment

- Quarterstaff and component pouch
- Spellbook with a broken clasp
- Scholar's pack, ink and three blank scrolls
- 40 gold pieces

## Background and bonds

Keeps a list of every book the library lost in the fire and crosses off each one she finds. Trusts Brannoc's caution more than her own. Would trade almost anything for the last volume on the list.
