---
type: character
player: Sam
class: Fighter
level: 5
species: Human
background: Soldier
str: 16
dex: 13
con: 15
int: 10
wis: 12
cha: 8
ac: 18
max_hp: 44
hp: 31
hit_dice: 5d10
speed: 30
saves:
  - Strength
  - Constitution
skills:
  - Athletics
  - Perception
  - Intimidation
  - Survival
expertise:
  -
---

# Brannoc Vell

Level `= this.level` · `= this.species` · `= this.class` · `= this.background`

A former border sergeant who still counts the party like a patrol at every camp.

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

- Fighting Style: Dueling (+2 damage with a one-handed weapon)
- Second Wind (1d10 + 5 hit points, once per short rest)
- Action Surge (one extra action, once per short rest)
- Martial Archetype: Champion, Improved Critical (critical hit on 19 or 20)
- Extra Attack (two attacks when taking the Attack action)

## Equipment

- Chain mail and shield
- Longsword and four javelins
- Explorer's pack, a dented signal horn
- 18 gold pieces

## Background and bonds

Left the border company after an order he refused to pass on. Owes his life to Tamsin, though he has not said so. Will leave the party if it abandons someone who cannot fight.
