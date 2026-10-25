---
type: charakter
player: Jo
class: Schurkin
level: 4
species: Leichtfuß-Halbling
background: Kriminelle
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
  - Geschicklichkeit
  - Intelligenz
skills:
  - Akrobatik
  - Täuschen
  - Wahrnehmung
  - Fingerfertigkeit
  - Heimlichkeit
expertise:
  - Heimlichkeit
  - Fingerfertigkeit
---

# Tamsin Reed

Stufe `= this.level` · `= this.species` · `= this.class` · `= this.background`

Eine Diebin von den Flussdocks, die sich der Gruppe anschloss, weil sie die Einzigen waren, die sie nicht durchsuchten.

## Attribute

| Attribut | Wert | Modifikator |
| --- | --- | --- |
| Stärke | `= this.str` | `= choice(floor((this.str - 10) / 2) >= 0, "+" + floor((this.str - 10) / 2), floor((this.str - 10) / 2))` |
| Geschicklichkeit | `= this.dex` | `= choice(floor((this.dex - 10) / 2) >= 0, "+" + floor((this.dex - 10) / 2), floor((this.dex - 10) / 2))` |
| Konstitution | `= this.con` | `= choice(floor((this.con - 10) / 2) >= 0, "+" + floor((this.con - 10) / 2), floor((this.con - 10) / 2))` |
| Intelligenz | `= this.int` | `= choice(floor((this.int - 10) / 2) >= 0, "+" + floor((this.int - 10) / 2), floor((this.int - 10) / 2))` |
| Weisheit | `= this.wis` | `= choice(floor((this.wis - 10) / 2) >= 0, "+" + floor((this.wis - 10) / 2), floor((this.wis - 10) / 2))` |
| Charisma | `= this.cha` | `= choice(floor((this.cha - 10) / 2) >= 0, "+" + floor((this.cha - 10) / 2), floor((this.cha - 10) / 2))` |

## Kampf

- **Rüstungsklasse:** `= this.ac`
- **Trefferpunkte:** `= this.hp` / `= this.max_hp`
- **Trefferwürfel:** `= this.hit_dice`
- **Bewegungsrate:** `= this.speed` Fuß
- **Übungsbonus:** +`= floor((this.level - 1) / 4) + 2`
- **Initiative:** `= choice(floor((this.dex - 10) / 2) >= 0, "+" + floor((this.dex - 10) / 2), floor((this.dex - 10) / 2))`
- **Passive Wahrnehmung:** `= 10 + floor((this.wis - 10) / 2) + choice(contains(this.skills, "Wahrnehmung"), floor((this.level - 1) / 4) + 2, 0)`

## Rettungswürfe und Fertigkeiten

Der Block unten braucht die Option *JavaScript queries* in den Einstellungen von Dataview. ● steht für Übung, ◆ für Expertise.

```dataviewjs
const p = dv.current();
const prof = Math.floor((p.level - 1) / 4) + 2;
const mod = (score) => Math.floor((score - 10) / 2);
const sign = (n) => (n >= 0 ? "+" : "") + n;
const has = (list, name) => (list ?? []).includes(name);
const abilities = [["Stärke", "str"], ["Geschicklichkeit", "dex"], ["Konstitution", "con"], ["Intelligenz", "int"], ["Weisheit", "wis"], ["Charisma", "cha"]];
const skills = [["Akrobatik", "dex"], ["Mit Tieren umgehen", "wis"], ["Arkane Kunde", "int"], ["Athletik", "str"], ["Täuschen", "cha"], ["Geschichte", "int"], ["Motiv erkennen", "wis"], ["Einschüchtern", "cha"], ["Nachforschungen", "int"], ["Heilkunde", "wis"], ["Naturkunde", "int"], ["Wahrnehmung", "wis"], ["Auftreten", "cha"], ["Überzeugen", "cha"], ["Religion", "int"], ["Fingerfertigkeit", "dex"], ["Heimlichkeit", "dex"], ["Überlebenskunst", "wis"]];
const short = Object.fromEntries(abilities.map(([name, key]) => [key, name.slice(0, 3)]));
dv.table(["Rettungswurf", "Bonus"], abilities.map(([name, key]) => {
  const proficient = has(p.saves, name);
  return [(proficient ? "● " : "○ ") + name, sign(mod(p[key]) + (proficient ? prof : 0))];
}));
dv.table(["Fertigkeit", "Attribut", "Bonus"], skills.map(([name, key]) => {
  const expert = has(p.expertise, name);
  const proficient = expert || has(p.skills, name);
  const bonus = mod(p[key]) + (expert ? 2 * prof : proficient ? prof : 0);
  return [(expert ? "◆ " : proficient ? "● " : "○ ") + name, short[key], sign(bonus)];
}));
```

## Merkmale und Fähigkeiten

- Expertise: Heimlichkeit und Fingerfertigkeit (doppelter Übungsbonus)
- Hinterhältiger Angriff 2W6 (einmal pro Zug)
- Raffinierte Aktion (Spurt, Rückzug oder Verstecken als Bonusaktion)
- Schurkenarchetyp: Dieb, Schnelle Hände und Fassadenkletterer
- Glückspilz und Natürliche Heimlichkeit

## Ausrüstung

- Beschlagene Lederrüstung
- Kurzschwert, zwei Dolche und ein Kurzbogen mit 20 Pfeilen
- Diebeswerkzeug, in ein altes Segel gewickelt
- 62 Goldmünzen, angeblich beim Kartenspiel gewonnen

## Hintergrund und Bindungen

Schuldet dem Dockboss noch Geld, wovon die anderen nichts wissen. Hat still entschieden, dass Brannoc Familie ist. Sie bestiehlt die Gruppe nicht und wird wütend, wenn jemand das andeutet.
