# Planificateur quotidien (time blocking) — Modèle Obsidian

Un planificateur quotidien en time blocking pour Obsidian : trois tâches les plus importantes, une timeline heure par heure en syntaxe Day Planner (`- [ ] 09:00 - 10:30 Deep work : brouillon du rapport`) et un rituel de clôture en fin de journée. Livré avec trois journées d'exemple réalistes et une note d'aperçu de la semaine.

## Structure des dossiers

```
daily-planner-template/
├── Commencez ici.md                ← à lire en premier
├── Planificateur/                  ← une note par jour + aperçu de la semaine
│   ├── 2026-06-08.md … 2026-06-10.md
│   └── Semaine du 2026-06-08.md
└── Modèles/
    ├── Planificateur quotidien.md  ← appliqué automatiquement aux nouvelles notes
    └── Aperçu de la semaine.md
```

## Installation

1. Décompressez le téléchargement.
2. Ouvrez Obsidian → **Ouvrir un dossier comme coffre** → sélectionnez le dossier décompressé.
3. Faites confiance au vault quand il vous le demande (il ne contient que des réglages JSON simples).
4. Ouvrez `Commencez ici.md`, puis créez la note du jour depuis l'icône calendrier du bandeau latéral.

Pour l'utiliser dans un vault existant, copiez-y `Planificateur/` et `Modèles/` et pointez Daily notes vers le dossier `Planificateur`, format `YYYY-MM-DD`, modèle `Modèles/Planificateur quotidien`.

## Plugins

Requis : aucun — tout fonctionne comme de simples listes à cocher avec les plugins natifs.

Facultatif (recommandé) :

- **Day Planner** — affiche les blocs de la timeline comme un emploi du temps visuel avec un repère « maintenant » en direct. https://obsidian.md/plugins?id=obsidian-day-planner

## Licence

MIT. Utilisez-le, modifiez-le, publiez-le — aucune attribution requise.

Modèle par Vaultorial — https://vaultorial.com/fr/modele-planificateur-quotidien/
