# Commencez ici

Bienvenue. Ce vault est un système Getting Things Done fonctionnel pour Obsidian, bâti sur le plugin Tasks. Il arrive avec trois projets d'exemple et plus de trente tâches, pour que chaque vue du [[Tableau de bord]] ait quelque chose à montrer. Remplacez les exemples par votre propre travail au fil du temps — la structure est le produit, le contenu n'est qu'une démonstration.

## Comment le vault est organisé

- [[00 Boîte de réception]] — point de capture. Tout atterrit ici d'abord, en vrac.
- [[01 Prochaines actions]] — actions isolées qui ne font partie d'aucun projet, marquées d'un contexte.
- [[02 En attente]] — choses que vous avez déléguées ou sur lesquelles vous êtes bloqué, marquées `#attente`.
- [[03 Un jour ou Peut-être]] — idées sur lesquelles vous ne vous engagez pas encore. Puces simples à dessein : elles ne sont pas actionnables, donc elles restent hors des requêtes de tâches.
- `Projets/` — une note par projet. Les tâches vivent dans la note du projet auquel elles appartiennent.
- [[Tableau de bord]] — le cockpit. Des requêtes en direct tirent les tâches de tout le vault : à échéance aujourd'hui, en retard, par contexte, en attente et éléments de la boîte à traiter.
- `Modèles/` — contient [[Projet]], le modèle pour les nouvelles notes de projet.

## Contextes

Les contextes GTD (les classiques @maison, @ordinateur, @courses) sont ici des tags imbriqués, parce que les tags d'Obsidian ne peuvent pas contenir le caractère `@` :

- `#contexte/maison`
- `#contexte/ordinateur`
- `#contexte/courses`

Ajoutez un tag de contexte à n'importe quelle tâche et elle apparaît dans la section correspondante du Tableau de bord. Ajoutez vos propres contextes (`#contexte/telephone`, `#contexte/bureau`) en marquant des tâches avec eux et en copiant un bloc de requête dans le Tableau de bord.

## Plugins à activer

1. **Tasks** (requis) — Paramètres → Plugins communautaires → Parcourir → "Tasks". Alimente chaque requête du Tableau de bord.
2. **Dataview** (optionnel) — utilisé uniquement pour le tableau récapitulatif des projets en bas du Tableau de bord. Tout le reste fonctionne sans lui.

Le plugin natif **Templates** est déjà activé et pointé sur le dossier `Modèles/`.

## Premiers pas

1. Activez le plugin Tasks, puis ouvrez le [[Tableau de bord]] en mode lecture. Chaque section devrait être remplie par les données d'exemple.
2. Capturez quelques vraies tâches dans [[00 Boîte de réception]] sous forme de cases `- [ ]` simples. La capture est censée être rapide et désordonnée.
3. Traitez la boîte : tout ce qui prend moins de deux minutes, faites-le maintenant. Les actions isolées passent dans [[01 Prochaines actions]] avec un tag de contexte et, si ça compte, une échéance (`📅 2026-06-15`). Les résultats multi-étapes deviennent une note dans `Projets/` — utilisez le modèle [[Projet]].
4. Une fois par semaine, faites une revue : ramenez la boîte à zéro, passez chaque projet en revue pour repérer une prochaine action en panne, et relancez tout ce qui est dans [[02 En attente]].
5. Quand les projets d'exemple ont rempli leur rôle, supprimez-les.

> [!tip] Aide-mémoire de la syntaxe des tâches
> `- [ ] Appeler le plombier #contexte/maison ⏫ 📅 2026-06-15`
> `📅` échéance · `⏫` priorité haute · `🔽` priorité basse · `🔁 every week` récurrence · `✅` date d'achèvement (ajoutée automatiquement quand vous cochez la case).
