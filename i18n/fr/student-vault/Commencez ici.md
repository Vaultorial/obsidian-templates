# Commencez ici

Bienvenue. Ceci est un vault étudiant fonctionnel pour un semestre : deux matières, de vraies notes de cours, de la préparation d'examens et des lectures déjà en place, plus un [[Tableau de bord]] qui réunit chaque échéance et chaque examen dans une seule vue, automatiquement.

## Comment c'est organisé

- **Par semestre et par matière :** `Printemps 2026/Biologie 101/` et `Printemps 2026/Statistiques 201/`. Ajoutez un dossier par matière à chaque nouveau semestre — la structure passe à l'échelle en la copiant.
- **Trois types de notes par matière**, chacun depuis un modèle : notes de cours, préparation d'examen et notes de lecture.
- **[[Tableau de bord]]** lit les champs `due` et `type` du frontmatter de chaque note et liste ce qui arrive. Il est construit par Dataview — changez une échéance dans une note et le tableau de bord se met à jour tout seul.

Les notes d'exemple sont délibérément remplies de matière correcte et générale (biologie cellulaire, statistique descriptive) pour que vous voyiez la structure sur du contenu réel avant de la remplacer par le vôtre.

## Premiers pas

1. Installez et activez **Dataview** (requis pour le [[Tableau de bord]]) : Paramètres → Modules complémentaires → Parcourir → "Dataview".
2. Ouvrez le [[Tableau de bord]] et confirmez que les tableaux des échéances et des examens s'affichent.
3. Créez un dossier de matière pour l'une de vos vraies matières dans `Printemps 2026/` (ou un nouveau dossier de semestre).
4. Prenez votre prochain cours dans une copie de `Modèles/Note de cours.md` (plugin natif Templates, déjà configuré). Mettez une date `due` sur tout ce qui a une échéance et cela apparaît sur le tableau de bord.
5. Optionnel : installez **Calendar** pour une vue mensuelle à côté de vos notes quotidiennes.

## Les types de notes

- **Note de cours** — date, sujet et un endroit net pour la matière du jour plus des questions à revoir ensuite.
- **Préparation d'examen** — `type: exam` et une date `due` pour qu'elle remonte sur le tableau de bord ; une liste de contrôle des sujets à travailler.
- **Note de lecture** — source, la date `due` du devoir et votre propre résumé de ce que vous avez lu.

## Plugins

- **Requis :** Dataview — le tableau de bord en a besoin.
- **Optionnel :** Calendar — vue mensuelle pour les notes quotidiennes.
- Le **Templates** natif est déjà activé et pointé sur `Modèles`.

> [!tip] Une habitude rend ce vault rentable
> Mettez une date `due` dans le frontmatter dès qu'une échéance est annoncée. Le tableau de bord ne peut montrer que ce que vous lui dites — mais si vous le lui dites, vous ne suivez plus jamais les échéances de mémoire.
