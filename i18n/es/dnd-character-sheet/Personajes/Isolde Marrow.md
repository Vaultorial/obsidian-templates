---
type: personaje
player: Priya
class: Maga
level: 5
species: Alta elfa
background: Sabia
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
  - Inteligencia
  - Sabiduría
skills:
  - Arcanos
  - Historia
  - Investigación
  - Perspicacia
expertise:
  -
spellcasting: int
---

# Isolde Marrow

Nivel `= this.level` · `= this.species` · `= this.class` · `= this.background`

Archivera que salió de la biblioteca para buscar los libros que le faltaban.

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

## Lanzamiento de conjuros

- **CD de salvación de conjuros:** `= 8 + floor((this.level - 1) / 4) + 2 + floor((this.int - 10) / 2)`
- **Bonificador de ataque de conjuros:** +`= floor((this.level - 1) / 4) + 2 + floor((this.int - 10) / 2)`
- **Espacios de conjuro:** nivel 1: 4 · nivel 2: 3 · nivel 3: 2
- **Trucos:** Descarga de fuego, Mano de mago, Prestidigitación, Luz
- **Conjuros preparados:** Armadura de mago, Proyectil mágico, Escudo, Detectar magia, Paso brumoso, Inmovilizar persona, Bola de fuego, Contrahechizo

## Rasgos y atributos

- Recuperación arcana (recupera espacios de conjuro por valor de 3 niveles en un descanso corto, una vez al día)
- Tradición arcana: Escuela de Evocación
- Esculpir conjuros (protege a sus aliados de sus propios conjuros de evocación)
- Visión en la oscuridad 60 pies y Linaje feérico

## Equipo

- Bastón y bolsa de componentes
- Libro de conjuros con el cierre roto
- Paquete de erudito, tinta y tres pergaminos en blanco
- 40 piezas de oro

## Trasfondo y vínculos

Lleva una lista de cada libro que la biblioteca perdió en el incendio y tacha cada uno que encuentra. Confía más en la prudencia de Brannoc que en la suya. Cambiaría casi cualquier cosa por el último volumen de la lista.
