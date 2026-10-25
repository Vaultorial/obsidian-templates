---
type: character
player:
class:
level: 1
species:
background:
str: 10
dex: 10
con: 10
int: 10
wis: 10
cha: 10
ac: 10
max_hp: 10
hp: 10
hit_dice: 1d8
speed: 30
saves:
  -
skills:
  -
expertise:
  -
---

# {{title}}

Level `= this.level` · `= this.species` · `= this.class` · `= this.background`

One line: who this character is at the table, in the player's own words.

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

## Features and traits

-

## Equipment

-

## Background and bonds

Where they come from, who they owe, and what would make them walk away from the party.
