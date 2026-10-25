---
type: personaje
player: Jo
class: Pícara
level: 4
species: Mediana piesligeros
background: Criminal
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
  - Destreza
  - Inteligencia
skills:
  - Acrobacias
  - Engaño
  - Percepción
  - Juego de Manos
  - Sigilo
expertise:
  - Sigilo
  - Juego de Manos
---

# Tamsin Reed

Nivel `= this.level` · `= this.species` · `= this.class` · `= this.background`

Ladrona de los muelles del río que se unió al grupo porque fueron los únicos que no la registraron.

## Características

| Característica | Puntuación | Modificador |
| --- | --- | --- |
| Fuerza | `= this.str` | `= choice(floor((this.str - 10) / 2) >= 0, "+" + floor((this.str - 10) / 2), floor((this.str - 10) / 2))` |
| Destreza | `= this.dex` | `= choice(floor((this.dex - 10) / 2) >= 0, "+" + floor((this.dex - 10) / 2), floor((this.dex - 10) / 2))` |
| Constitución | `= this.con` | `= choice(floor((this.con - 10) / 2) >= 0, "+" + floor((this.con - 10) / 2), floor((this.con - 10) / 2))` |
| Inteligencia | `= this.int` | `= choice(floor((this.int - 10) / 2) >= 0, "+" + floor((this.int - 10) / 2), floor((this.int - 10) / 2))` |
| Sabiduría | `= this.wis` | `= choice(floor((this.wis - 10) / 2) >= 0, "+" + floor((this.wis - 10) / 2), floor((this.wis - 10) / 2))` |
| Carisma | `= this.cha` | `= choice(floor((this.cha - 10) / 2) >= 0, "+" + floor((this.cha - 10) / 2), floor((this.cha - 10) / 2))` |

## Combate

- **Clase de Armadura:** `= this.ac`
- **Puntos de golpe:** `= this.hp` / `= this.max_hp`
- **Dados de golpe:** `= this.hit_dice`
- **Velocidad:** `= this.speed` pies
- **Bonificador por competencia:** +`= floor((this.level - 1) / 4) + 2`
- **Iniciativa:** `= choice(floor((this.dex - 10) / 2) >= 0, "+" + floor((this.dex - 10) / 2), floor((this.dex - 10) / 2))`
- **Percepción pasiva:** `= 10 + floor((this.wis - 10) / 2) + choice(contains(this.skills, "Percepción"), floor((this.level - 1) / 4) + 2, 0)`

## Tiradas de salvación y habilidades

El bloque de abajo necesita activar *JavaScript queries* en los ajustes de Dataview. ● marca competencia y ◆ pericia.

```dataviewjs
const p = dv.current();
const prof = Math.floor((p.level - 1) / 4) + 2;
const mod = (score) => Math.floor((score - 10) / 2);
const sign = (n) => (n >= 0 ? "+" : "") + n;
const has = (list, name) => (list ?? []).includes(name);
const abilities = [["Fuerza", "str"], ["Destreza", "dex"], ["Constitución", "con"], ["Inteligencia", "int"], ["Sabiduría", "wis"], ["Carisma", "cha"]];
const skills = [["Acrobacias", "dex"], ["Trato con Animales", "wis"], ["Arcanos", "int"], ["Atletismo", "str"], ["Engaño", "cha"], ["Historia", "int"], ["Perspicacia", "wis"], ["Intimidación", "cha"], ["Investigación", "int"], ["Medicina", "wis"], ["Naturaleza", "int"], ["Percepción", "wis"], ["Interpretación", "cha"], ["Persuasión", "cha"], ["Religión", "int"], ["Juego de Manos", "dex"], ["Sigilo", "dex"], ["Supervivencia", "wis"]];
const short = Object.fromEntries(abilities.map(([name, key]) => [key, name.slice(0, 3)]));
dv.table(["Tirada de salvación", "Bonificador"], abilities.map(([name, key]) => {
  const proficient = has(p.saves, name);
  return [(proficient ? "● " : "○ ") + name, sign(mod(p[key]) + (proficient ? prof : 0))];
}));
dv.table(["Habilidad", "Característica", "Bonificador"], skills.map(([name, key]) => {
  const expert = has(p.expertise, name);
  const proficient = expert || has(p.skills, name);
  const bonus = mod(p[key]) + (expert ? 2 * prof : proficient ? prof : 0);
  return [(expert ? "◆ " : proficient ? "● " : "○ ") + name, short[key], sign(bonus)];
}));
```

## Rasgos y atributos

- Pericia: Sigilo y Juego de Manos (bonificador por competencia doble)
- Ataque furtivo 2d6 (una vez por turno)
- Acción astuta (Correr, Retirarse u Ocultarse como acción adicional)
- Arquetipo de pícaro: Ladrón, Manos rápidas y Trabajo en las alturas
- Afortunado y Sigilo natural

## Equipo

- Armadura de cuero tachonado
- Espada corta, dos dagas y arco corto con 20 flechas
- Herramientas de ladrón envueltas en una vela vieja
- 62 piezas de oro que dice haber ganado a las cartas

## Trasfondo y vínculos

Aún le debe al jefe de los muelles una deuda de la que no ha hablado a los demás. Ha decidido en silencio que Brannoc es familia. No le roba al grupo y se enfada si alguien insinúa que podría hacerlo.
