# Commencez ici

Bienvenue. Ce vault est un système léger de gestion de projet pour Obsidian : une note par projet, une note par réunion et un tableau de bord Dataview qui lit tout le reste. Deux projets d'exemple complets — une refonte de site web et un déménagement de bureau — arrivent préchargés avec des jalons, des chronologies Mermaid et des notes de réunion liées, pour que chaque requête du tableau de bord ait de vraies données derrière elle.

## Comment le vault est organisé

- `Projets/` — une note par projet. Le frontmatter porte les champs que lit le tableau de bord (`status`, `owner`, `start`, `due`, `area`) ; le corps contient les objectifs, un tableau de jalons, une chronologie Gantt et des liens vers les réunions de ce projet.
- `Réunions/` — une note par réunion, nommée `YYYY-MM-DD Projet Sujet`. Chacune renvoie à son projet dans le frontmatter, pour que le tableau de bord puisse regrouper les actions ouvertes par projet.
- [[Tableau de bord]] — des tableaux en direct : projets actifs, projets par statut et par responsable, échéances à venir, réunions récentes et chaque action non cochée à travers toutes les notes de réunion.
- `Modèles/` — [[Modèle de projet]] et [[Modèle de réunion]], reliés au plugin natif Templates.

## Conventions qui font fonctionner le tableau de bord

- `status` vaut l'un de : `planification`, `actif`, `en pause`, `terminé`. En minuscules, exact — Dataview compare les chaînes littéralement.
- `owner` est un nom, écrit de la même façon partout (« Sarah Chen », pas « S. Chen » dans un fichier et « sarah » dans un autre).
- Les dates sont `YYYY-MM-DD`. Dataview les lit comme de vraies dates, ce qui rend la requête « bientôt dû » possible.
- Les actions dans les notes de réunion sont de simples cases `- [ ]`. Cochez-les là où elles vivent ; le tableau de bord le reflète.

## Plugins à activer

1. **Dataview** (requis) — Paramètres → Modules complémentaires → Parcourir → "Dataview". Le tableau de bord est bâti dessus.

Les chronologies Mermaid s'affichent grâce au support Mermaid intégré d'Obsidian — aucun plugin nécessaire. Le plugin natif **Templates** est déjà activé et pointé sur `Modèles/`.

## Premiers pas

1. Activez Dataview et ouvrez le [[Tableau de bord]] en mode lecture. Chaque tableau devrait être rempli.
2. Ouvrez [[Refonte du site web]] et parcourez-le de haut en bas — frontmatter, jalons, chronologie, réunions. Cette note est le modèle.
3. Créez votre premier vrai projet : nouvelle note dans `Projets/`, insérez [[Modèle de projet]] (palette de commandes → "Templates: Insérer un modèle"), remplissez le frontmatter.
4. Après votre prochaine réunion, créez une note dans `Réunions/` depuis [[Modèle de réunion]] et liez-la au projet.
5. Supprimez les deux projets d'exemple et leurs réunions une fois que vous avez les vôtres.
