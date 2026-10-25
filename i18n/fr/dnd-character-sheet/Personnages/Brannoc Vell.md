---
type: personnage
player: Sam
class: Guerrier
level: 5
species: Humain
background: Soldat
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
  - Force
  - Constitution
skills:
  - Athlétisme
  - Perception
  - Intimidation
  - Survie
expertise:
  -
---

# Brannoc Vell

Niveau `= this.level` · `= this.species` · `= this.class` · `= this.background`

Ancien sergent de la frontière qui compte encore le groupe comme une patrouille à chaque bivouac.

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

- Style de combat : Duel (+2 aux dégâts avec une arme à une main)
- Second souffle (1d10 + 5 points de vie, une fois par repos court)
- Fougue (une action supplémentaire, une fois par repos court)
- Archétype martial : Champion, Critique amélioré (critique sur 19 ou 20)
- Attaque supplémentaire (deux attaques avec l'action Attaquer)

## Équipement

- Cotte de mailles et bouclier
- Épée longue et quatre javelines
- Sac d'explorateur et un cor de signal cabossé
- 18 pièces d'or

## Historique et liens

A quitté la compagnie frontalière après un ordre qu'il a refusé de transmettre. Doit la vie à Tamsin, sans l'avoir jamais dit. Quittera le groupe si celui-ci abandonne quelqu'un qui ne peut pas se battre.
