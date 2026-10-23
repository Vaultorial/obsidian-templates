# Commencez ici

Un kit complet de PNJ pour MJ : un modèle de PNJ détaillé avec personnalité, voix, secrets, accroches et relations, un modèle rapide pour improviser à la table et une liste Dataview qui trie votre distribution par lieu, faction et attitude. Il contient Cinderbrook, une ville fluviale originale avec six PNJ détaillés et trois rapides, pour que chaque vue ait des données dès le premier jour.

## Ce que contient le vault

- `PNJ/` : six PNJ complets avec les propriétés `role`, `location`, `faction`, `attitude`, `status`, `first_met` et `revealed`.
- `PNJ rapides/` : trois PNJ rapides, apparence, envie, voix et secret sur un écran.
- `Factions/` et `Lieux/` : deux factions et deux lieux, qui listent tout seuls leurs personnes.
- [[Liste des PNJ]] : la liste Dataview par lieu, par attitude, membres des factions, PNJ rapides et secrets à révéler.
- `Modèles/` : modèles PNJ et PNJ rapide.

## L'utiliser à la table

Avant une séance, consultez la liste pour savoir qui le groupe peut croiser et quels secrets restent cachés. Quand vous improvisez un personnage, remplissez un PNJ rapide en moins d'une minute. Si le groupe revient le voir, faites-le monter en grade : créez un PNJ complet à partir du modèle et liez la note rapide. Après la séance, mettez à jour `attitude` et passez `revealed: true` pour chaque secret dévoilé.

Compatible avec tous les systèmes. Le profil de jeu facultatif reprend des champs à la manière de 5e avec des valeurs originales ; remplacez-le ou supprimez-le pour un autre système.

## Plugins

**Dataview** fait tourner la liste et les listes de membres des factions et des lieux. Le plugin principal **Modèles** est activé et pointe vers `Modèles/`.
