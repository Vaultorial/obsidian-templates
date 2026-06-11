# Suivi des habitudes — Modèle Obsidian

Un suivi des habitudes pour Obsidian à deux niveaux : des **grilles mensuelles** sans plugin (habitudes × jours, des coches dans un tableau) et un **tableau de bord Dataview** facultatif qui calcule séries, totaux mensuels et jours parfaits à partir de minuscules notes quotidiennes. Livré avec deux mois d'exemple entièrement suivis (avril–mai 2026, cinq habitudes du quotidien, données imparfaites de façon réaliste).

## Structure des dossiers

```
habit-tracker/
├── Commencez ici.md                     ← à lire en premier
├── Habitudes/
│   ├── 2026-04 Habitudes.md             ← grille mensuelle, remplie
│   ├── 2026-05 Habitudes.md             ← grille mensuelle, remplie
│   ├── Tableau de bord des habitudes.md ← Dataview : séries, totaux, jours parfaits
│   └── Journal quotidien/               ← 61 notes par jour (données en frontmatter)
│       └── 2026-04-01.md … 2026-05-31.md
└── Modèles/
    ├── Suivi mensuel des habitudes.md   ← grille vierge pour un nouveau mois
    └── Entrée de journal quotidien.md   ← journal du soir en une minute
```

## Installation

1. Décompressez le téléchargement.
2. Ouvrez Obsidian → **Ouvrir le dossier comme vault** → sélectionnez le dossier décompressé.
3. Faites confiance au vault quand il vous le demande (il ne contient que des réglages JSON simples).
4. Ouvrez `Commencez ici.md`.

Pour l'utiliser dans un vault existant, copiez-y `Habitudes/` et `Modèles/`, puis définissez `Modèles` comme dossier de modèles (Réglages → Templates).

## Plugins

Requis : aucun — les grilles mensuelles sont de simples tableaux Markdown.

Facultatifs :

- **Dataview** — alimente le tableau de bord (les séries demandent son réglage *JavaScript queries* activé). https://obsidian.md/plugins?id=dataview

## Licence

MIT. Utilisez-le, modifiez-le, publiez-le — aucune attribution requise.

Modèle par Vaultorial — https://vaultorial.com/fr/suivi-des-habitudes/
