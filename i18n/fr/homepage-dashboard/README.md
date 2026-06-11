# Page d'accueil / Dashboard — Modèle pour Obsidian

Un système de page d'accueil pour Obsidian : une note-tableau de bord avec les tâches du jour, la semaine à venir, les projets actifs, les notes récemment modifiées et les compteurs du vault — en deux variantes. `Accueil (simple)` tourne avec des callouts et des liens statiques sans aucun plugin ; `Accueil` est la version vivante, alimentée par des requêtes Dataview sur les échéances `[due:: ]` des tâches, pensée pour être ouverte au lancement par le plugin Homepage. Livré avec un petit vault d'exemple entièrement interconnecté (3 projets, 2 domaines, 3 notes pérennes aux tâches datées réalistes), pour que chaque section du tableau de bord affiche des données réelles dès la première ouverture.

## Structure des dossiers

```
homepage-dashboard/
├── Commencez ici.md         ← à lire d'abord
├── Accueil.md               ← tableau de bord vivant (Dataview)
├── Accueil (simple).md      ← tableau de bord sans plugin
├── Projets/                 ← 3 projets d'exemple avec tâches datées
├── Domaines/                ← 2 domaines continus avec tâches datées
└── Notes/                   ← 3 notes pérennes (liste, checklist, recette)
```

## Installation

1. Décompressez le téléchargement.
2. Ouvrez Obsidian → **Ouvrir un dossier comme vault** → sélectionnez le dossier décompressé.
3. Faites confiance au vault quand Obsidian le demande (il ne contient que des réglages JSON bruts).
4. Ouvrez `Commencez ici.md`, puis `Accueil (simple)` — il marche immédiatement. Installez les plugins ci-dessous pour donner vie à `Accueil`.

Pour l'utiliser dans un vault existant, copiez `Accueil.md` et `Accueil (simple).md` et ajustez les noms de dossiers dans les requêtes (`FROM "Projets" OR "Domaines"`) à votre structure.

## Plugins

Requis pour le tableau de bord vivant :

- **Dataview** — exécute les requêtes d'`Accueil.md`. https://obsidian.md/plugins?id=dataview

Facultatif :

- **Homepage** — ouvre votre tableau de bord automatiquement au lancement. https://obsidian.md/plugins?id=homepage

`Accueil (simple).md` n'a besoin d'aucun plugin.

## Licence

MIT. Utilisez-le, modifiez-le, publiez-le — aucune attribution requise.

Modèle par Vaultorial — https://vaultorial.com/fr/tableau-de-bord-accueil/
