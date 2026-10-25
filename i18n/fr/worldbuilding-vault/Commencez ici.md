# Commencez ici

Bienvenue. Ce vault est un système de worldbuilding pour écrivains et meneurs de jeu, démontré avec un décor original complet : **Les Cours des Marées**, un monde de magie rare fait de cités-États d'estuaire gouvernées par la loi des marées. Deux douzaines de notes interconnectées — lieux, personnages, factions et une chronologie liée — montrent la méthode à pleine densité. Ouvrez d'abord la vue graphique : un monde devrait ressembler à une toile, et c'est le cas de celui-ci.

## Comment le vault est organisé

- `Lieux/` — une note par lieu, avec `region` et `ruled-by` dans le frontmatter.
- `Personnages/` — une note par personne, chacune liée à un `home` (un lieu) et à une `faction`.
- `Factions/` — les puissances. Chacune a un `seat` (un lieu) et un `leader` (un personnage).
- `Événements/` — la chronologie. Chaque événement porte `year`, `location` et une liste `participants`, si bien que la frise s'assemble toute seule.
- `Cultures/` — peuples et modes de vie, chacun rattaché à son `homeland` et à ses `beliefs`.
- `Croyances/` — fois et pratiques, avec leurs `followers` et leur `holy-place`.
- `Objets/` — les objets qui comptent pour l'intrigue, avec qui les détient (`held-by`), où ils sont gardés et d'où ils viennent.
- `Cartes/` — vide à dessein ; la note à l'intérieur explique comment ajouter vos cartes.
- [[Index du monde]] — le MOC maître : toutes les entités depuis une seule page, plus des synthèses Dataview.
- [[Chronologie]] — la frise, requêtée et racontée.
- `Modèles/` — un modèle par type d'entité, branché sur le plugin natif Templates.

## La méthode : les relations dans le frontmatter

Chaque note déclare ses relations comme des liens de frontmatter (`home: "[[Basmarche]]"`, `faction: "[[Les Jurés du Flot]]"`). Cette seule habitude vous donne trois choses gratuitement : la vue graphique montre la forme réelle du monde, Dataview peut répondre aux questions (« tous ceux qui ont juré à la Cour du Jusant », « tous les événements sur la Chaussée »), et renommer une note met à jour chaque référence. Les wikilinks en prose tissent le reste.

Les dates suivent le calendrier propre du monde — années du Comput des Marées, écrites `368 CM` — gardé comme simple nombre dans `year` pour que la frise se trie seule. Prenez le calendrier que votre monde exige ; gardez le champ numérique.

## Plugins à activer

1. **Dataview** (requis) — alimente les synthèses de l'[[Index du monde]] et de la [[Chronologie]].
2. **Timelines (Revamped)** (optionnel) — dessine des frises visuelles à partir de plages balisées si vous voulez plus que le tableau requêté. Le vault fonctionne entièrement sans lui.

Le plugin natif **Templates** est déjà activé et pointé sur `Modèles/`.

## Premiers pas

1. Activez Dataview, puis lisez l'[[Index du monde]] — c'est la porte d'entrée vers tout.
2. Ouvrez la vue graphique et assignez des groupes de couleur par dossier (`path:Lieux`, `path:Personnages`, `path:Factions`, `path:Événements`). La structure du monde devient visible immédiatement.
3. Lisez une chaîne de bout en bout pour sentir la méthode de liaison : [[La Pétition de Basmarche]] → [[Bren Callow]] → [[Les Jurés du Flot]] → [[La Noyade de Basmarche]].
4. Ajoutez votre première entité : nouvelle note dans le bon dossier, insertion du modèle correspondant, frontmatter rempli, liens posés en écrivant.
5. Quand vous commencez votre propre monde, supprimez les notes des Cours des Marées et gardez les dossiers, les modèles et l'index.
