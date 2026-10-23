# Commencez ici

Ce vault est un CRM personnel qui fonctionne. Chaque personne, entreprise et affaire est une note, chaque échange est une note datée dans Interactions, et le [[Tableau de bord CRM]] rassemble le tout. Les données d'exemple appartiennent à une agence de design fictive, pour que chaque requête ait quelque chose à montrer. Supprimez-les quand vos propres contacts seront en place.

## Comment tout s'articule

- `Contacts/` : une note par personne, avec `company`, `role`, `relationship`, `last_contact` et `next_follow_up` dans les propriétés.
- `Entreprises/` : une note par organisation. Chacune liste automatiquement ses personnes et ses affaires.
- `Affaires/` : une note par opportunité, avec `value`, `stage` et `close_date`.
- `Interactions/` : une note par appel, e-mail ou réunion, nommée par sa date. Les tâches de relance y vivent.
- [[Tableau de bord CRM]] : relances de la semaine, tâches ouvertes, pipeline par étape, contacts sans nouvelles depuis 60 jours, échanges récents.
- `Pipeline.base` : les mêmes affaires sous forme de tableau modifiable, avec le plugin principal Bases.

## La routine hebdomadaire

Après chaque échange, créez une note d'interaction à partir du modèle et liez le contact. Mettez à jour `last_contact` et `next_follow_up` du contact, et le `stage` de l'affaire s'il a changé. Une fois par semaine, ouvrez le tableau de bord et traitez les relances du haut.

Étapes d'affaire utilisées ici : `piste`, `qualifié`, `proposition`, `négociation`, `gagné`, `perdu`.

## Plugins

**Dataview** est nécessaire pour le tableau de bord et les listes de chaque note. Le plugin principal **Modèles** est activé et pointe vers `Modèles/`. Le tableau du pipeline utilise le plugin principal **Bases**, inclus dans les versions actuelles d'Obsidian.
