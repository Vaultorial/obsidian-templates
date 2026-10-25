---
type: personnage
player: Priya
class: Magicienne
level: 5
species: Haute-elfe
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
  - Sagesse
skills:
  - Arcanes
  - Histoire
  - Investigation
  - Perspicacité
expertise:
  -
spellcasting: int
---

# Isolde Marrow

Niveau `= this.level` · `= this.species` · `= this.class` · `= this.background`

Une archiviste qui a quitté la bibliothèque pour trouver les livres qui y manquaient.

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

## Incantation

- **DD des sauvegardes contre les sorts:** `= 8 + floor((this.level - 1) / 4) + 2 + floor((this.int - 10) / 2)`
- **Bonus d'attaque des sorts:** +`= floor((this.level - 1) / 4) + 2 + floor((this.int - 10) / 2)`
- **Emplacements de sorts:** niveau 1 : 4 · niveau 2 : 3 · niveau 3 : 2
- **Sorts mineurs:** Trait de feu, Main de mage, Prestidigitation, Lumière
- **Sorts préparés:** Armure de mage, Projectile magique, Bouclier, Détection de la magie, Foulée brumeuse, Immobilisation de personne, Boule de feu, Contresort

## Capacités et traits

- Restauration arcanique (récupère des emplacements pour 3 niveaux lors d'un repos court, une fois par jour)
- Tradition arcanique : École d'évocation
- Sculpter les sorts (protège ses alliés de ses propres sorts d'évocation)
- Vision dans le noir 18 m et Ascendance féerique

## Équipement

- Bâton et sacoche à composantes
- Grimoire au fermoir cassé
- Sac d'érudit, encre et trois parchemins vierges
- 40 pièces d'or

## Historique et liens

Tient la liste de chaque livre perdu par la bibliothèque dans l'incendie et raye chacun de ceux qu'elle retrouve. Se fie davantage à la prudence de Brannoc qu'à la sienne. Échangerait presque n'importe quoi contre le dernier volume de la liste.
