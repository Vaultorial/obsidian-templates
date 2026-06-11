# Commencez ici

Bienvenue. Ce vault suit vos habitudes de deux manières — choisissez celle qui correspond à votre patience, ou menez les deux de front comme le font les exemples.

- **La manière simple :** une note par mois avec une grille — les jours vers le bas, les habitudes en travers, `✓` ou `·` dans chaque case. Aucun plugin, parfaitement utilisable les jours de cerveau en compote.
- **La manière avancée :** une minuscule note par jour avec les habitudes en frontmatter vrai/faux, et un [[Tableau de bord des habitudes]] qui calcule séries, totaux mensuels et jours parfaits avec Dataview.

Deux mois entièrement suivis sont inclus (avril et mai 2026, cinq habitudes du quotidien : lire 20 min, marcher 30 min, zéro sucre, coucher avant 23 h 30, journal). Les données sont volontairement imparfaites — une semaine de rush, des creux de week-end, le coup d'un jour férié — parce que c'est à ça que ressemble un vrai suivi, et les deux vues racontent la même histoire.

## Comment le vault est organisé

- `Habitudes/2026-04 Habitudes.md`, `Habitudes/2026-05 Habitudes.md` — les grilles mensuelles, totaux en bas.
- `Habitudes/Journal quotidien/` — 61 notes par jour qui alimentent le tableau de bord.
- `Habitudes/Tableau de bord des habitudes.md` — séries, totaux mois par mois, les 14 derniers jours, jours parfaits.
- `Modèles/` — `Suivi mensuel des habitudes` (grille vierge) et `Entrée de journal quotidien` (journal du soir).

## Premiers pas

1. Ouvrez [[2026-05 Habitudes]] et lisez la grille comme un graphique : le motif des week-ends et le creux de mi-mois se repèrent sans la moindre requête.
2. Installez **Dataview** (voir le README), puis ouvrez le [[Tableau de bord des habitudes]] et regardez les mêmes données devenir séries et totaux. Pour le bloc des séries, activez *JavaScript queries* dans les réglages de Dataview.
3. Créez `2026-06 Habitudes` dans `Habitudes/` et insérez le modèle `Suivi mensuel des habitudes`. Renommez les colonnes avec **vos** cinq habitudes — cinq au maximum.
4. Ce soir, consignez le jour un avec le modèle `Entrée de journal quotidien`. Le rituel complet prend moins d'une minute.
5. Supprimez les exemples d'avril/mai quand vous en avez fini avec eux (supprimez les notes mensuelles et `Journal quotidien` — le tableau de bord n'affichera plus que vos données).

## Plugins

- **Dataview** — requis uniquement pour le [[Tableau de bord des habitudes]]. Les grilles mensuelles fonctionnent sans aucun plugin.

> [!tip] Suivez le tenu, pas le manqué
> Les jours manqués reçoivent un discret `·`, pas une marque rouge, et une série cassée en démarre simplement une nouvelle. Le travail de la grille, c'est l'honnêteté, pas la culpabilité — cette différence est ce qui vous fait encore consigner en troisième semaine.
