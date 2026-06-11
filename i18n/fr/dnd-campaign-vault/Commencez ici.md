# Commencez ici

Bienvenue, MJ. Ce vault est un système de gestion de campagne pour les jeux de rôle sur table compatibles avec le règlement de cinquième édition le plus joué au monde. Il est livré avec une mini-campagne originale complète déjà chargée — **La Conspiration de la Route du Sel** : trois séances jouées, huit PNJ, quatre lieux, trois rencontres, trois personnages joueurs et le contexte qui relie le tout. Menez-la telle quelle, dépiautez-la pour les pièces, ou supprimez-la et gardez la structure.

## Comment le vault est organisé

- `Séances/` — une note par séance : récapitulatif, scènes, indices remis et un bloc « la prochaine fois » qui devient votre liste de préparation.
- `PNJ/` — une note par personnage, avec `role`, `location`, `status` et `faction` dans le frontmatter pour que l'[[Écran du MJ]] puisse les trier.
- `Lieux/` — une note par endroit visitable, chacune liant ses PNJ, ses rencontres et ses rumeurs.
- `Rencontres/` — des rencontres préparées avec blocs de statistiques originaux, notes de terrain et tactiques. `status: prêt` veut dire jouable ce soir ; `status: joué` garde l'archive.
- `PJ/` — une note par personnage joueur : la copie de table des liens, des objectifs et des accroches de campagne qui s'y rattachent.
- `Contexte/` — les pièces mobiles du monde (factions, histoire) sur lesquelles plusieurs notes doivent s'accorder.
- `Modèles/` — un modèle par type d'entité, branché sur le plugin natif Templates.
- [[Écran du MJ]] — le tableau de bord. Des requêtes Dataview rassemblent les PNJ par lieu, les séances récentes, les rencontres prêtes et la liste du groupe.

## Plugins à activer

1. **Dataview** (requis) — alimente chaque tableau de l'[[Écran du MJ]].
2. **Leaflet** (optionnel) — dès que vous ajoutez des images de carte au vault, un bloc de code `leaflet` les transforme en cartes navigables à marqueurs. Rien dans le vault n'en dépend.
3. **Initiative Tracker** (optionnel) — tient l'ordre d'initiative dans la barre latérale ; se marie bien avec les notes de rencontre.

Le plugin natif **Templates** est déjà activé et pointé sur `Modèles/`.

## Premiers pas

1. Activez Dataview et ouvrez l'[[Écran du MJ]] en mode lecture — chaque tableau devrait être peuplé.
2. Lisez [[La Route du Sel]] pour la colonne vertébrale de la campagne, puis [[Séance 3 - Du sel sur la plaie]] pour voir où la table s'est arrêtée. Le [[Cambriolage du Comptoir]] est préparé et prêt pour la prochaine séance.
3. Avant votre propre séance zéro : répétez le flux des modèles — nouvelle note dans le bon dossier, insertion du modèle correspondant, frontmatter rempli.
4. Après chaque séance, écrivez la note de séance à chaud, mettez à jour tout PNJ dont le `status` a changé et passez en `prêt` les notes de rencontre de la séance suivante.

> [!note] Sur le contenu
> Tout ici — la Marche Saumâtre, ses gens, ses monstres — est original à ce modèle. Les lignes de statistiques comme « CA 13, PV 26 » sont des créations maison pour cette campagne, pas des reproductions d'un manuel, si bien que le vault reste compatible sans copier le texte de personne.
