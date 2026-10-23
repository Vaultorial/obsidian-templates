# Modèle de note quotidienne — Modèle Obsidian

Un système de notes quotidiennes épuré pour Obsidian : une note par jour avec les sections **Agenda, Tâches, Journal et Gratitude**, une navigation vers le jour précédent et le suivant, et une semaine d'exemple entièrement remplie pour voir le système à l'œuvre avant de vous y engager.

Deux variantes du modèle sont incluses : une qui fonctionne uniquement avec les plugins natifs, et une propulsée par Templater avec gestion automatique des dates.

## Structure des dossiers

```
daily-note-template/
├── Commencez ici.md                          ← à lire en premier
├── Quotidien/                                ← une note par jour (7 jours d'exemple, juin 2026)
│   ├── 2026-06-01.md … 2026-06-07.md
└── Modèles/
    ├── Note quotidienne (Templates natif).md ← aucun plugin requis
    └── Note quotidienne (Templater).md       ← ajoute les liens préc./suiv.
```

## Installation

1. Décompressez le téléchargement.
2. Ouvrez Obsidian → **Ouvrir un dossier comme coffre** → sélectionnez le dossier décompressé.
3. Faites confiance au vault quand Obsidian le demande (il ne contient que des réglages JSON ordinaires).
4. Ouvrez `Commencez ici.md`.

Pour l'utiliser dans un vault existant, copiez-y les dossiers `Quotidien/` et `Modèles/` et reprenez les réglages Daily notes (dossier `Quotidien`, format `YYYY-MM-DD`, modèle `Modèles/Note quotidienne (Templates natif)`).

## Plugins

Requis : aucun — la variante native fonctionne immédiatement.

Facultatif :

- **Templater** — dates dynamiques et liens vers le jour précédent/suivant. https://obsidian.md/plugins?id=templater-obsidian

## Licence

MIT. Utilisez-le, modifiez-le, publiez-le — aucune attribution requise.

Modèle par Vaultorial — https://vaultorial.com/fr/modele-note-quotidienne/
