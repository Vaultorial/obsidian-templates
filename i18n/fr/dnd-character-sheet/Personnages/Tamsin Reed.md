---
type: personnage
player: Jo
class: Roublarde
level: 4
species: Halfeline pied-léger
background: Criminelle
str: 10
dex: 18
con: 12
int: 13
wis: 14
cha: 12
ac: 16
max_hp: 27
hp: 19
hit_dice: 4d8
speed: 25
saves:
  - Dextérité
  - Intelligence
skills:
  - Acrobaties
  - Tromperie
  - Perception
  - Escamotage
  - Discrétion
expertise:
  - Discrétion
  - Escamotage
---

# Tamsin Reed

Niveau `= this.level` · `= this.species` · `= this.class` · `= this.background`

Une voleuse des quais du fleuve qui a rejoint le groupe parce que ce sont les seuls à ne pas l'avoir fouillée.

## Caractéristiques

| Caractéristique | Valeur | Modificateur |
| --- | --- | --- |
| Force | `= this.str` | `= choice(floor((this.str - 10) / 2) >= 0, "+" + floor((this.str - 10) / 2), floor((this.str - 10) / 2))` |
| Dextérité | `= this.dex` | `= choice(floor((this.dex - 10) / 2) >= 0, "+" + floor((this.dex - 10) / 2), floor((this.dex - 10) / 2))` |
| Constitution | `= this.con` | `= choice(floor((this.con - 10) / 2) >= 0, "+" + floor((this.con - 10) / 2), floor((this.con - 10) / 2))` |
| Intelligence | `= this.int` | `= choice(floor((this.int - 10) / 2) >= 0, "+" + floor((this.int - 10) / 2), floor((this.int - 10) / 2))` |
| Sagesse | `= this.wis` | `= choice(floor((this.wis - 10) / 2) >= 0, "+" + floor((this.wis - 10) / 2), floor((this.wis - 10) / 2))` |
| Charisme | `= this.cha` | `= choice(floor((this.cha - 10) / 2) >= 0, "+" + floor((this.cha - 10) / 2), floor((this.cha - 10) / 2))` |

## Combat

- **Classe d'armure:** `= this.ac`
- **Points de vie:** `= this.hp` / `= this.max_hp`
- **Dés de vie:** `= this.hit_dice`
- **Vitesse:** `= this.speed` pieds
- **Bonus de maîtrise:** +`= floor((this.level - 1) / 4) + 2`
- **Initiative:** `= choice(floor((this.dex - 10) / 2) >= 0, "+" + floor((this.dex - 10) / 2), floor((this.dex - 10) / 2))`
- **Perception passive:** `= 10 + floor((this.wis - 10) / 2) + choice(contains(this.skills, "Perception"), floor((this.level - 1) / 4) + 2, 0)`

## Jets de sauvegarde et compétences

Le bloc ci-dessous nécessite d'activer *JavaScript queries* dans les réglages de Dataview. ● indique la maîtrise, ◆ l'expertise.

```dataviewjs
const p = dv.current();
const prof = Math.floor((p.level - 1) / 4) + 2;
const mod = (score) => Math.floor((score - 10) / 2);
const sign = (n) => (n >= 0 ? "+" : "") + n;
const has = (list, name) => (list ?? []).includes(name);
const abilities = [["Force", "str"], ["Dextérité", "dex"], ["Constitution", "con"], ["Intelligence", "int"], ["Sagesse", "wis"], ["Charisme", "cha"]];
const skills = [["Acrobaties", "dex"], ["Dressage", "wis"], ["Arcanes", "int"], ["Athlétisme", "str"], ["Tromperie", "cha"], ["Histoire", "int"], ["Perspicacité", "wis"], ["Intimidation", "cha"], ["Investigation", "int"], ["Médecine", "wis"], ["Nature", "int"], ["Perception", "wis"], ["Représentation", "cha"], ["Persuasion", "cha"], ["Religion", "int"], ["Escamotage", "dex"], ["Discrétion", "dex"], ["Survie", "wis"]];
const short = Object.fromEntries(abilities.map(([name, key]) => [key, name.slice(0, 3)]));
dv.table(["Jet de sauvegarde", "Bonus"], abilities.map(([name, key]) => {
  const proficient = has(p.saves, name);
  return [(proficient ? "● " : "○ ") + name, sign(mod(p[key]) + (proficient ? prof : 0))];
}));
dv.table(["Compétence", "Caractéristique", "Bonus"], skills.map(([name, key]) => {
  const expert = has(p.expertise, name);
  const proficient = expert || has(p.skills, name);
  const bonus = mod(p[key]) + (expert ? 2 * prof : proficient ? prof : 0);
  return [(expert ? "◆ " : proficient ? "● " : "○ ") + name, short[key], sign(bonus)];
}));
```

## Capacités et traits

- Expertise : Discrétion et Escamotage (bonus de maîtrise doublé)
- Attaque sournoise 2d6 (une fois par tour)
- Ruse (Foncer, Se désengager ou Se cacher par une action bonus)
- Archétype de roublard : Voleur, Mains lestes et Monte-en-l'air
- Chanceux et Discrétion naturelle

## Équipement

- Armure de cuir clouté
- Épée courte, deux dagues et un arc court avec 20 flèches
- Outils de voleur enveloppés dans une vieille voile
- 62 pièces d'or qu'elle prétend avoir gagnées aux cartes

## Historique et liens

Doit encore une dette au patron des quais, sans en avoir parlé aux autres. A décidé en silence que Brannoc était de la famille. Ne vole pas le groupe et se fâche si quelqu'un le sous-entend.
