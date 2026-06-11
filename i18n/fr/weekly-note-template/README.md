# Note hebdomadaire + bilan de semaine — Modèle Obsidian

Un système de planification et de bilan hebdomadaires pour Obsidian, en une seule note par semaine : plan du lundi, bilan de fin de semaine façon GTD (réussites, chiffres personnels, tâches reportées, objectif de la semaine suivante). Quatre semaines d'exemple consécutives de mai 2026 sont incluses, pour voir comment les sujets ouverts circulent d'une semaine à l'autre.

## Structure des dossiers

```
weekly-note-template/
├── Commencez ici.md                            ← à lire en premier
├── Hebdomadaire/                               ← une note par semaine ISO (4 semaines d'exemple)
│   ├── 2026-W19.md … 2026-W22.md
└── Modèles/
    ├── Note hebdomadaire (Templates natif).md  ← aucun plugin requis
    └── Note hebdomadaire (Templater).md        ← ajoute plage de dates + liens préc./suiv.
```

## Installation

1. Décompressez le téléchargement.
2. Ouvrez Obsidian → **Ouvrir le dossier comme vault** → sélectionnez le dossier décompressé.
3. Faites confiance au vault quand il vous le demande (il ne contient que des réglages JSON simples).
4. Ouvrez `Commencez ici.md`.

Pour l'utiliser dans un vault existant, copiez-y `Hebdomadaire/` et `Modèles/`, puis définissez `Modèles` comme dossier de modèles (Réglages → Templates).

## Plugins

Requis : aucun — la variante native fonctionne immédiatement.

Facultatifs :

- **Periodic Notes** — ouvrir la note de la semaine en cours en une commande. https://obsidian.md/plugins?id=periodic-notes
- **Templater** — plages de semaine dynamiques et liens précédent/suivant. https://obsidian.md/plugins?id=templater-obsidian

## Licence

MIT. Utilisez-le, modifiez-le, publiez-le — aucune attribution requise.

Modèle par Vaultorial — https://vaultorial.com/fr/modele-note-hebdomadaire/
