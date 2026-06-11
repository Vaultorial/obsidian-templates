# Kit de démarrage MOC

Un vault de démarrage Obsidian pour organiser ses notes avec des cartes de contenu (MOC). Il est livré entièrement travaillé : une carte d'accueil, trois MOC thématiques (productivité, apprentissage, écriture) et quinze notes interconnectées en dessous — ouvrez la vue graphique et l'arbre à trois niveaux est déjà là.

## Structure des dossiers

```
moc-template/
├── Commencez ici.md    ← à lire d'abord
├── Home MOC.md         ← niveau 1 : le point d'entrée unique
├── MOCs/               ← niveau 2 : une carte par thème (3 exemples)
├── Notes/              ← niveau 3 : une idée par note, à plat (15 exemples)
└── Modèles/            ← modèle de MOC avec les conventions de liaison
```

## Conventions utilisées partout

- **Home MOC → MOC → note** : la page d'accueil ne renvoie qu'à des MOC ; les MOC renvoient aux notes avec une ligne de contexte chacune ; les notes renvoient `Up:` à leur MOC et latéralement aux notes liées.
- Les notes vivent à plat dans `Notes/` — ce sont les cartes qui portent la structure, pas l'arborescence de dossiers.

## Installation

1. Décompressez le téléchargement.
2. Ouvrez Obsidian → **Ouvrir un dossier comme vault** → sélectionnez le dossier décompressé.
3. Si Obsidian interroge sur le mode restreint, gardez-le — ce vault n'utilise aucun plugin communautaire.
4. Activez le plugin natif **Templates** (Réglages → Plugins natifs) pour utiliser le modèle de MOC.

## Plugins

- **Requis :** aucun. Fonctionne entièrement avec les plugins natifs.
- **Facultatifs :** aucun.

## Licence

MIT. Utilisez-le, modifiez-le, construisez dessus — à titre personnel ou commercial. Aucune attribution requise.

Modèle par Vaultorial — https://vaultorial.com/fr/modele-moc/
