# Journal / Bullet journal — Modèle pour Obsidian

Un vault de journal façon bullet journal pour Obsidian : rapid logging avec la notation classique (`•` tâche, `×` faite, `○` événement, `–` note, `>` migrée), une courte section de gratitude par entrée, des dossiers mensuels et un rituel de bilan mensuel. Livré avec deux semaines complètes d'exemple (du 25 mai au 7 juin 2026) et le bilan mensuel de mai rédigé.

## Structure des dossiers

```
journal-template/
├── Commencez ici.md                       ← à lire d'abord (avec la légende du logging)
├── Journal/
│   └── 2026/
│       ├── 05/                            ← 7 entrées + "2026-05 Bilan.md"
│       └── 06/                            ← 7 entrées
└── Modèles/
    ├── Entrée de journal (bullet journal).md ← le modèle par défaut des notes quotidiennes
    ├── Entrée de journal (prose).md          ← variante longue en prose
    ├── Entrée de journal (Templater).md      ← ajoute les liens préc./suiv.
    └── Bilan mensuel.md
```

## Installation

1. Décompressez le téléchargement.
2. Ouvrez Obsidian → **Ouvrir un dossier comme vault** → sélectionnez le dossier décompressé.
3. Faites confiance au vault quand Obsidian le demande (il ne contient que des réglages JSON bruts).
4. Ouvrez `Commencez ici.md`, puis cliquez sur l'icône calendrier pour l'entrée du jour.

Pour l'utiliser dans un vault existant, copiez `Journal/` et `Modèles/` et réglez Daily notes sur le dossier `Journal`, le format `YYYY/MM/YYYY-MM-DD` et le modèle `Modèles/Entrée de journal (bullet journal)`.

## Plugins

Requis : aucun.

Facultatifs :

- **Templater** — dates dynamiques et liens vers le jour précédent/suivant pour la variante Templater. https://obsidian.md/plugins?id=templater-obsidian

## Licence

MIT. Utilisez-le, modifiez-le, publiez-le — aucune attribution requise.

Modèle par Vaultorial — https://vaultorial.com/fr/modele-de-journal/
