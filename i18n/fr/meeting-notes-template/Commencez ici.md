# Commencez ici

Bienvenue. Ce vault est un système de notes de réunion pour Obsidian : trois modèles prêts à l'emploi (réunion d'équipe, 1-on-1, appel client), un tableau de bord Dataview qui trouve chaque réunion et chaque action inachevée, et quatre réunions d'exemple remplies issues d'un même projet cohérent, pour que vous voyiez le système fonctionner avant de l'adopter.

## Comment le vault est organisé

- `Modèles/` — le produit. [[Réunion d'équipe]], [[1-on-1]] et [[Appel client]], chacun avec un frontmatter structuré (`type`, `date`, `project`, `attendees`) et les mêmes quatre sections : ordre du jour, notes, décisions, actions.
- `Réunions/` — une note par réunion, nommée `YYYY-MM-DD Sujet`. Les exemples suivent un projet de conseil (la construction d'un portail client pour un assureur) à travers un lancement, un 1-on-1, un appel client et une revue de sprint.
- [[Tableau de bord des réunions]] — rollups Dataview : réunions récentes, réunions par type, par projet et toutes les actions ouvertes en un seul endroit.

## Conventions qui font fonctionner le tableau de bord

- `type` vaut l'un de : `reunion-equipe`, `one-on-one`, `appel-client`. En minuscules, avec tiret, exact.
- `project` est une courte étiquette en texte brut (« Portail client »). Utilisez la même orthographe dans toutes les réunions — le tableau de bord regroupe par elle.
- Les actions s'écrivent au format du plugin Tasks : `- [ ] Responsable — ce qu'il fera 📅 2026-06-15`. Ce vault n'a besoin que de la partie case (Dataview la lit), mais la syntaxe de date signifie que vous pouvez déposer ces lignes dans un vault GTD avec le plugin Tasks — comme notre vault de tâches GTD — et elles seront récupérées comme tâches planifiées sans changement.
- Les décisions ont leur propre section. Six mois plus tard, personne ne relit les notes ; on cherche ce qui a été décidé.

## Plugins à activer

1. **Dataview** (requis) — Paramètres → Plugins communautaires → Parcourir → "Dataview". Alimente le tableau de bord.
2. **Templater** (optionnel) — si vous utilisez déjà Templater, pointez-le sur `Modèles/` et remplacez les variables `{{date}}` et `{{title}}` par vos commandes dynamiques préférées. Les modèles arrivent en syntaxe Templates natif pour fonctionner d'emblée.

Le plugin natif **Templates** est déjà activé et pointé sur `Modèles/`.

## Premiers pas

1. Activez Dataview et ouvrez le [[Tableau de bord des réunions]] en mode lecture — chaque section devrait être remplie par les quatre réunions d'exemple.
2. Ouvrez [[2026-05-04 Lancement du portail client]] pour voir une note remplie à côté de son modèle.
3. Avant votre prochaine réunion : créez une note dans `Réunions/` nommée avec la date et le sujet, insérez le modèle correspondant (palette de commandes → "Templates: Insérer un modèle") et remplissez le frontmatter.
4. Pendant la réunion, n'écrivez que dans notes/décisions/actions. Après, passez une minute à attribuer un responsable et une date à chaque action.
5. Supprimez les réunions d'exemple une fois que vous en avez quelques-unes à vous.
