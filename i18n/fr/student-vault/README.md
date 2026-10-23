# Vault étudiant pour Obsidian

Un vault Obsidian pour gérer le travail universitaire, organisé par semestre et par matière, avec un tableau de bord Dataview qui fait remonter chaque échéance et chaque examen à venir depuis le frontmatter des notes. Livré avec deux matières d'exemple, douze notes remplies entre cours, préparation d'examens et lectures, et trois modèles.

## Structure des dossiers

```
student-vault/
├── Commencez ici.md       ← lisez ceci en premier
├── Tableau de bord.md     ← Dataview : échéances + examens, auto-construit
├── Printemps 2026/
│   ├── Biologie 101/      ← cours, préparation d'examen, notes de lecture
│   └── Statistiques 201/  ← cours, préparation d'examen, notes de lecture
└── Modèles/               ← Note de cours / Préparation d'examen / Note de lecture
```

## Comment ça marche

Les notes portent les champs `due` et `type` dans leur frontmatter. `Tableau de bord.md` interroge tout le vault : un tableau des échéances (tout ce qui a un `due` futur), un tableau des examens (`type: exam`) et une ventilation par matière. Modifiez une date dans une note et le tableau de bord la reflète aussitôt. Ajoutez une matière en copiant un dossier de matière ; ajoutez un semestre avec un nouveau dossier `Saison AAAA/`.

## Installation

1. Décompressez le téléchargement.
2. Ouvrez Obsidian → **Ouvrir un dossier comme coffre** → sélectionnez le dossier décompressé.
3. Désactivez le mode restreint quand on vous le demande, puis installez Dataview (lien ci-dessous) et activez-le.
4. Ouvrez `Tableau de bord.md` — les tableaux devraient se peupler à partir des notes d'exemple.

## Plugins

- **Requis :** Dataview — https://obsidian.md/plugins?id=dataview — alimente le tableau de bord.
- **Optionnel :** Calendar — https://obsidian.md/plugins?id=calendar — vue mensuelle compagnon des notes quotidiennes.

## Licence

MIT. Utilisez-le, modifiez-le, bâtissez dessus — usage personnel ou commercial. Aucune attribution requise.

Modèle par Vaultorial — https://vaultorial.com/fr/vault-etudiant/
