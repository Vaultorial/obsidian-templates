# Vault de gestion de projet — modèle Obsidian

Un système de gestion de projet en fichiers simples pour Obsidian. Chaque projet est une seule note avec un frontmatter structuré, un tableau de jalons, une chronologie Gantt Mermaid et des notes de réunion liées ; un tableau de bord Dataview regroupe tout par statut, responsable et échéance. Livré avec deux exemples entièrement travaillés — une refonte de site web et un déménagement de bureau — y compris quatre notes de réunion réalistes.

## Structure

```
project-management-template/
├── Commencez ici.md    ← lisez ceci en premier
├── Tableau de bord.md  ← rollups Dataview : statut, responsable, échéances, actions
├── Projets/
│   ├── Refonte du site web.md
│   └── Déménagement de bureau.md
├── Réunions/           ← une note par réunion, liée à son projet
│   ├── 2026-04-02 Lancement de la refonte du site web.md
│   ├── 2026-05-07 Revue de design de la refonte du site web.md
│   ├── 2026-04-21 Visite fournisseur du déménagement de bureau.md
│   └── 2026-05-19 Synchro logistique du déménagement de bureau.md
└── Modèles/
    ├── Modèle de projet.md
    └── Modèle de réunion.md
```

## Installation

1. Téléchargez et décompressez le modèle : **Décompresser → Obsidian → Ouvrir un dossier comme coffre**.
2. Quand Obsidian le demande, activez les plugins communautaires pour ce vault.
3. Installez Dataview et ouvrez `Tableau de bord.md` en mode lecture.

## Plugins

**Requis**

- Dataview — https://obsidian.md/plugins?id=dataview

Les chronologies Gantt utilisent le rendu Mermaid intégré d'Obsidian ; aucun plugin supplémentaire nécessaire.

## Licence

MIT. Utilisez-le, modifiez-le, partagez-le — attribution appréciée mais non requise.

Modèle par Vaultorial — https://vaultorial.com/fr/modele-gestion-de-projet/
