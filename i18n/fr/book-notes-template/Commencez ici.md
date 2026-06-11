# Commencez ici

Bienvenue. Ce vault est un système de lecture en trois parties : une note par livre dans `Livres/`, une [[Bibliothèque]] qui se construit toute seule à partir de ces notes, et un modèle qui garde chaque nouvelle note de livre cohérente.

## Comment ça marche

Chaque note de livre porte ses données dans le frontmatter — `author`, `genre`, `rating`, `status` (`terminé` / `en cours` / `à lire`), `date-started`, `date-finished`. La [[Bibliothèque]] exécute des requêtes Dataview sur ce frontmatter, donc les étagères se mettent à jour dès que vous modifiez une note. Changez le statut d'un livre de `en cours` à `terminé`, ajoutez une note, et il change d'étagère tout seul.

Six livres sont déjà là, dans des états différents, pour que chaque étagère ait quelque chose : commencez par [[Deep Work]] ou [[Un rien peut tout changer]] pour voir une note terminée, [[Le programmeur pragmatique]] pour une en cours de lecture, et [[L'essentialisme]] pour le peu dont une note « à lire » a besoin.

## Philosophie des notes

- Le résumé et les idées clés s'**écrivent dans vos propres mots** — c'est de là que vient la rétention, pas de la collecte de passages.
- Les citations se limitent à une au maximum par livre, courte et attribuée. Une note de livre est votre réflexion sur le livre, pas un fichier d'extraits.

## Premiers pas

1. Installez et activez **Dataview** (requis — la [[Bibliothèque]] est vide sans lui) : Paramètres → Plugins communautaires → Parcourir → "Dataview".
2. Ouvrez la [[Bibliothèque]] et confirmez que les étagères s'affichent.
3. Ajoutez le livre que vous lisez en ce moment : nouvelle note dans `Livres/` nommée d'après le titre, insérez `Modèles/Note de livre.md` (plugin natif Templates, déjà configuré), remplissez le frontmatter, mettez `status: en cours`.
4. Optionnel : installez **Book Search** pour créer des notes de livre avec auteur et métadonnées préremplis depuis une recherche par titre.

> [!tip] Notez sur votre propre échelle
> La note sert à ce que votre futur vous décide quoi relire ou recommander — ce n'est pas une critique publique. Décidez une fois ce qu'un 5 signifie pour vous, écrivez-le en haut de la Bibliothèque, et restez cohérent.
