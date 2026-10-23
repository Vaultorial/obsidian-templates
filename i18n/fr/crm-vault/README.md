# Vault CRM — Modèle Obsidian

Un CRM personnel pour Obsidian : contacts, entreprises, affaires et un journal daté de chaque échange, reliés par Dataview. Le pipeline d'une petite agence est déjà rempli, le tableau de bord affiche donc dès l'ouverture de vraies relances, des affaires en cours et les contacts qui refroidissent.

## Comment tout s'articule

- `Contacts/` : une note par personne, avec `company`, `role`, `relationship`, `last_contact` et `next_follow_up` dans les propriétés.
- `Entreprises/` : une note par organisation. Chacune liste automatiquement ses personnes et ses affaires.
- `Affaires/` : une note par opportunité, avec `value`, `stage` et `close_date`.
- `Interactions/` : une note par appel, e-mail ou réunion, nommée par sa date. Les tâches de relance y vivent.
- [[Tableau de bord CRM]] : relances de la semaine, tâches ouvertes, pipeline par étape, contacts sans nouvelles depuis 60 jours, échanges récents.
- `Pipeline.base` : les mêmes affaires sous forme de tableau modifiable, avec le plugin principal Bases.

Étapes d'affaire utilisées ici : `piste`, `qualifié`, `proposition`, `négociation`, `gagné`, `perdu`.

## Plugins

**Dataview** est nécessaire pour le tableau de bord et les listes de chaque note. Le plugin principal **Modèles** est activé et pointe vers `Modèles/`. Le tableau du pipeline utilise le plugin principal **Bases**, inclus dans les versions actuelles d'Obsidian.

- Dataview — https://obsidian.md/plugins?id=dataview

1. Décompressez le téléchargement puis, dans Obsidian, choisissez **Ouvrir un dossier comme vault**.
2. Activez les plugins communautaires pour ce vault quand Obsidian le demande.
3. Installez et activez **Dataview**, puis ouvrez le Tableau de bord CRM en mode lecture.

## License

MIT. Utilisez-le, modifiez-le, partagez-le ; la mention de la source est appréciée mais pas obligatoire.

Modèle par Vaultorial — https://vaultorial.com/fr/modele-crm-obsidian/
