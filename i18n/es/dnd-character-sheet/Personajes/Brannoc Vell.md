---
type: personaje
player: Sam
class: Guerrero
level: 5
species: Humano
background: Soldado
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
  - Fuerza
  - Constitución
skills:
  - Atletismo
  - Percepción
  - Intimidación
  - Supervivencia
expertise:
  -
---

# Brannoc Vell

Nivel `= this.level` · `= this.species` · `= this.class` · `= this.background`

Antiguo sargento de frontera que sigue contando al grupo como a una patrulla en cada campamento.

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

- Estilo de combate: Duelo (+2 al daño con un arma a una mano)
- Tomar aliento (1d10 + 5 puntos de golpe, una vez por descanso corto)
- Oleada de acción (una acción extra, una vez por descanso corto)
- Arquetipo marcial: Campeón, Crítico mejorado (crítico con 19 o 20)
- Ataque adicional (dos ataques al usar la acción de Atacar)

## Equipo

- Cota de malla y escudo
- Espada larga y cuatro jabalinas
- Paquete de explorador y un cuerno de señales abollado
- 18 piezas de oro

## Trasfondo y vínculos

Dejó la compañía de frontera tras una orden que se negó a transmitir. Le debe la vida a Tamsin, aunque no lo ha dicho. Dejará al grupo si este abandona a alguien que no puede pelear.
