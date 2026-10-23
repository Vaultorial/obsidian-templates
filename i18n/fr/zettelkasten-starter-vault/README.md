# Vault Zettelkasten de démarrage — Modèle pour Obsidian

Un vault de démarrage pour la méthode Zettelkasten dans Obsidian, déjà peuplé d'un exemple en état de marche : quatorze notes liées sur l'apprentissage et la mémoire qui montrent le pipeline complet éphémère → littérature → permanente, les identifiants horodatés et un index comme point d'entrée.

## Structure des dossiers

```
zettelkasten-starter-vault/
├── Commencez ici.md   ← à lire en premier
├── Index.md           ← point d'entrée vers les notes permanentes
├── Éphémères/         ← captures rapides, traitées puis supprimées (3 exemples)
├── Littérature/       ← une note par source, vos propres mots (3 exemples)
├── Permanentes/       ← une idée par note, identifiants horodatés (8 exemples)
└── Modèles/           ← modèles de note éphémère / de littérature / permanente
```

Les notes permanentes se nomment `YYYYMMDDHHMM Titre.md` (par exemple `202605141030 Écrire ses notes avec ses propres mots.md`). L'identifiant rend chaque note adressable de façon unique et garde les noms de fichiers stables même quand les titres évoluent.

## Installation

1. Décompressez le téléchargement.
2. Ouvrez Obsidian → **Ouvrir un dossier comme coffre** → sélectionnez le dossier décompressé.
3. Activez le plugin natif **Templates** si besoin (Paramètres → Modules principaux) ; il pointe déjà vers `Modèles`.
4. Optionnel : installez Templater (ci-dessous) et le modèle de note permanente générera son identifiant horodaté automatiquement.

## Plugins

- **Requis :** aucun — le vault fonctionne d'emblée avec les plugins natifs.
- **Optionnel :** Templater — https://obsidian.md/plugins?id=templater-obsidian — remplit seul l'identifiant `YYYYMMDDHHMM` et les dates des modèles. Sans lui, tapez l'identifiant à la main.

## Licence

MIT. Utilisez-le, modifiez-le, bâtissez dessus — usage personnel ou commercial. Aucune attribution requise.

Modèle par Vaultorial — https://vaultorial.com/fr/vault-zettelkasten/
