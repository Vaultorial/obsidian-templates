---
type: charakter
player: Priya
class: Magierin
level: 5
species: Hochelfin
background: Weise
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
  - Intelligenz
  - Weisheit
skills:
  - Arkane Kunde
  - Geschichte
  - Nachforschungen
  - Motiv erkennen
expertise:
  -
spellcasting: int
---

# Isolde Marrow

Stufe `= this.level` · `= this.species` · `= this.class` · `= this.background`

Eine Archivarin, die die Bibliothek verließ, um die Bücher zu suchen, die ihr fehlten.

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

## Zauberwirken

- **Zauberrettungswurf-SG:** `= 8 + floor((this.level - 1) / 4) + 2 + floor((this.int - 10) / 2)`
- **Zauberangriffsbonus:** +`= floor((this.level - 1) / 4) + 2 + floor((this.int - 10) / 2)`
- **Zauberplätze:** Grad 1: 4 · Grad 2: 3 · Grad 3: 2
- **Zaubertricks:** Feuerpfeil, Magierhand, Taschenspielerei, Licht
- **Vorbereitete Zauber:** Magierrüstung, Magisches Geschoss, Schild, Magie entdecken, Nebelschritt, Person festhalten, Feuerball, Gegenzauber

## Merkmale und Fähigkeiten

- Arkane Erholung (Zauberplätze im Wert von 3 Graden bei einer kurzen Rast zurückgewinnen, einmal pro Tag)
- Arkane Tradition: Schule der Hervorrufung
- Zauber formen (Verbündete vor eigenen Hervorrufungszaubern schützen)
- Dunkelsicht 18 m und Feenblut

## Ausrüstung

- Kampfstab und Komponentenbeutel
- Zauberbuch mit gebrochener Schließe
- Gelehrtenausrüstung, Tinte und drei leere Schriftrollen
- 40 Goldmünzen

## Hintergrund und Bindungen

Führt eine Liste aller Bücher, die die Bibliothek beim Brand verlor, und streicht jedes, das sie findet. Vertraut Brannocs Vorsicht mehr als ihrer eigenen. Würde fast alles für den letzten Band auf der Liste hergeben.
