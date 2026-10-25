# Commencez ici

Ce vault transforme une feuille de personnage D&D 5e en note Obsidian. Vous saisissez dans les propriétés de la note les valeurs qui changent rarement (caractéristiques, niveau, classe d'armure, points de vie maximum) et Dataview calcule tout ce qui en découle : modificateurs, bonus de maîtrise, initiative, jets de sauvegarde, les dix-huit compétences, Perception passive et, pour les lanceurs de sorts, le DD des sauvegardes et le bonus d'attaque des sorts. Pour monter de niveau, vous changez une propriété et toute la feuille se met à jour.

## Ce que contient le vault

- `Personnages/` — trois personnages d'exemple remplis : Brannoc Vell (guerrier, niveau 5), Isolde Marrow (magicienne, niveau 5) et Tamsin Reed (roublarde, niveau 4, avec expertise).
- [[Feuille du groupe]] — tout le groupe dans un tableau, qui a besoin de soins et qui est doué pour quoi.
- `Modèles/Feuille de personnage` — une feuille vierge avec toutes les formules déjà en place.

## Plugins à activer

1. **Dataview** (obligatoire). Installez-le depuis les plugins communautaires.
2. Dans les réglages de Dataview, activez **JavaScript queries**. Les tableaux des jets de sauvegarde et des compétences utilisent un court bloc DataviewJS par feuille ; tout le reste est du Dataview classique.

Le plugin natif **Modèles** est déjà activé et pointe vers `Modèles/`.

## Comment sont calculés les chiffres

- Modificateur = (valeur − 10) ÷ 2, arrondi à l'inférieur. Un 16 donne +3, un 8 donne −1.
- Bonus de maîtrise = +2 aux niveaux 1 à 4, +3 de 5 à 8, +4 de 9 à 12, +5 de 13 à 16, +6 de 17 à 20.
- Une compétence ou un jet de sauvegarde maîtrisé ajoute le bonus de maîtrise ; l'expertise l'ajoute deux fois.
- Perception passive = 10 + votre bonus de Perception.
- DD des sauvegardes contre les sorts = 8 + bonus de maîtrise + modificateur d'incantation ; attaque des sorts = bonus de maîtrise + modificateur d'incantation.

## Premiers pas

1. Activez Dataview et les JavaScript queries, puis ouvrez [[Brannoc Vell]] en mode lecture.
2. Passez sa propriété `level` de 5 à 9 et regardez changer le bonus de maîtrise, les sauvegardes et les compétences.
3. Ouvrez la [[Feuille du groupe]] et modifiez les `hp` de quelqu'un pour voir le tableau des soins se mettre à jour.
4. Pour votre propre personnage : nouvelle note dans `Personnages/`, insérez le modèle Feuille de personnage et remplissez les propriétés.
