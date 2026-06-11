# Commencez ici

Bienvenue. Ce vault fait une seule chose : une unique note hebdomadaire qui contient à la fois votre **plan de la semaine** et votre **bilan de celle-ci**. Planifiez le lundi, faites le bilan le vendredi ou le dimanche, dans le même fichier. Quatre semaines d'exemple remplies montrent à quoi cela ressemble quand un mois réel traverse le système.

## Comment le vault est organisé

- `Hebdomadaire/` — une note par semaine ISO, nommée `2026-W19`, `2026-W20`, et ainsi de suite. Les quatre exemples couvrent mai 2026 et se lisent comme une histoire continue : observez comment l'inachevé rampe du **Reporté** d'une semaine vers le plan de la suivante. Cette boucle, c'est toute la méthode.
- `Modèles/` — deux versions du modèle hebdomadaire :
	- **Note hebdomadaire (Templates natif)** — aucun plugin requis.
	- **Note hebdomadaire (Templater)** — ajoute la plage de dates de la semaine et les liens vers la semaine précédente/suivante, calculés depuis le nom du fichier.

## Premiers pas

1. Lisez `2026-W19` à `2026-W22` dans l'ordre. Cinq minutes, et vous saurez exactement comment faire tourner le système.
2. Créez votre semaine en cours : nouvelle note dans `Hebdomadaire/` nommée avec le numéro ISO de cette semaine (par ex. `2026-W24`), puis insérez le modèle avec **Insérer un modèle** depuis la palette de commandes.
3. Le lundi, remplissez l'**Objectif** et 3 à 5 tâches du plan. Pendant la semaine, ne touchez à rien. En fin de semaine, remplissez le bilan d'une traite.
4. Tout ce qui n'est pas terminé va dans **Reporté** — et doit réapparaître dans le plan de la semaine suivante ou être abandonné délibérément. Ce qui se traîne trois semaines d'affilée vous dit quelque chose.

## Plugins

Par défaut, uniquement des plugins natifs. Deux améliorations facultatives :

- **Periodic Notes** — ajoute une commande « ouvrir la note de cette semaine » et une navigation de semaines façon calendrier. Après installation, réglez le format hebdomadaire sur `GGGG-[W]WW` et le dossier sur `Hebdomadaire`.
- **Templater** — nécessaire pour la variante `Note hebdomadaire (Templater)`. Définissez `Modèles` comme son dossier de modèles.

> [!tip] Gardez le bilan honnête
> La section **Chiffres** ne suit que ce que vous comptez vraiment (entraînements, sessions d'étude, pages). Deux ou trois indicateurs suffisent largement — dès que noter ressemble à de la comptabilité, supprimez-en un.
