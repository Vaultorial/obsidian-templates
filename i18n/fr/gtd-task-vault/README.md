# Vault de tâches GTD — modèle Obsidian

Un système Getting Things Done prêt à l'emploi pour Obsidian, propulsé par le plugin Tasks. Il met en œuvre la boucle GTD complète — capturer, clarifier, organiser, réfléchir, agir — avec un tableau de bord en direct, des tags de contexte et trois projets d'exemple entièrement travaillés, pour que vous voyiez le système tourner avant de lui confier votre propre travail.

## Structure

```
gtd-task-vault/
├── Commencez ici.md            ← lisez ceci en premier
├── Tableau de bord.md          ← requêtes de tâches en direct (échéances, retards, contextes, en attente)
├── 00 Boîte de réception.md    ← capturez tout ici
├── 01 Prochaines actions.md    ← actions autonomes avec tags de contexte
├── 02 En attente.md            ← éléments délégués et bloqués
├── 03 Un jour ou Peut-être.md  ← idées sans engagement
├── Projets/                    ← une note par projet, les tâches vivent ici
│   ├── Rénovation de la cuisine.md
│   ├── Refonte du site portfolio.md
│   └── Camping au bord du lac.md
└── Modèles/
    └── Projet.md               ← modèle pour les nouvelles notes de projet
```

Les contextes GTD sont des tags imbriqués (`#contexte/maison`, `#contexte/ordinateur`, `#contexte/courses`), puisque les tags d'Obsidian ne peuvent pas commencer par `@`.

## Installation

1. Téléchargez et décompressez le modèle : **Décompresser → Obsidian → Ouvrir le dossier comme vault**.
2. Quand Obsidian le demande, activez les plugins communautaires pour ce vault.
3. Installez les plugins listés ci-dessous et ouvrez `Tableau de bord.md` en mode lecture.

## Plugins

**Requis**

- Tasks — https://obsidian.md/plugins?id=obsidian-tasks-plugin

**Optionnels**

- Dataview — https://obsidian.md/plugins?id=dataview (tableau récapitulatif des projets sur le tableau de bord)

## Licence

MIT. Utilisez-le, modifiez-le, partagez-le — attribution appréciée mais non requise.

Modèle par Vaultorial — https://vaultorial.com/fr/vault-taches-gtd/
