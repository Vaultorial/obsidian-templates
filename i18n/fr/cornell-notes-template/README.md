# Modèle de notes Cornell pour Obsidian

Un vault Obsidian qui met en œuvre la méthode Cornell de prise de notes avec de simples callouts et un unique snippet CSS : une colonne d'indices à gauche, les notes à droite, un bandeau de résumé en dessous. Aucun plugin communautaire. Livré avec deux modèles (Cornell générique et une variante Notes de cours avec métadonnées de matière) et trois notes d'exemple entièrement rédigées.

## Structure des dossiers

```
cornell-notes-template/
├── Commencez ici.md          ← à lire d'abord
├── Notes/                    ← 3 notes de cours d'exemple remplies
├── Modèles/                  ← Note Cornell + Notes de cours (Cornell)
└── .obsidian/snippets/
    └── cornell.css           ← la disposition à deux colonnes (préactivée)
```

## Comment ça marche

Chaque note utilise trois callouts — `[!cue]`, `[!notes]`, `[!summary]` — et le snippet `cornell.css` les dispose comme la page Cornell classique : colonne d'indices flottée (32 %), notes à côté, résumé dégagé en dessous, se repliant en blocs empilés sur les fenêtres étroites. Le snippet est préactivé via `appearance.json` ; il se bascule dans Réglages → Apparence → Snippets CSS.

La variante Notes de cours ajoute le frontmatter `course`, `professor` et `date` pour que les notes de cours restent triables et cherchables par matière.

## Installation

1. Décompressez le téléchargement.
2. Ouvrez Obsidian → **Ouvrir un dossier comme vault** → sélectionnez le dossier décompressé.
3. Gardez le mode restreint si on vous le demande — il n'y a aucun plugin communautaire ici.
4. Ouvrez une note dans `Notes/` en vue de lecture ; vous devriez voir deux colonnes. Sinon, activez le snippet **cornell** dans Réglages → Apparence → Snippets CSS.

## Plugins

- **Requis :** aucun. Seulement le plugin natif Templates (préconfiguré sur le dossier `Modèles`).
- **Facultatifs :** aucun.

## Licence

MIT. Utilisez-le, modifiez-le, construisez dessus — à titre personnel ou commercial. Aucune attribution requise.

Modèle par Vaultorial — https://vaultorial.com/fr/modele-notes-cornell/
