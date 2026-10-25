# Vault diagramme de Gantt — Modèle Obsidian

Des diagrammes de Gantt tirés de vos notes : chaque tâche est une note avec des dates de début et de fin dans ses propriétés, et une requête DataviewJS en fait un diagramme de Gantt Mermaid par projet, avec une section par phase. Deux projets d'exemple, un exemple statique sans plugin et un modèle de tâche sont inclus.

## Structure

```
gantt-chart-template/
├── Commencez ici.md                ← à lire en premier
├── Calendrier.md                   ← les diagrammes générés
├── Exemple de Gantt statique.md    ← diagramme écrit à la main, sans plugin
├── Projets/                        ← 2 projets d'exemple, 14 tâches datées
└── Modèles/                        ← note de tâche vierge
```

## Installation

1. Téléchargez et décompressez le modèle : **Décompresser → Obsidian → Ouvrir le dossier comme vault**.
2. Quand Obsidian le demande, activez les plugins communautaires pour ce vault.
3. Installez Dataview, activez *JavaScript queries* dans ses réglages, puis ouvrez `Calendrier.md`.

## Plugins

**Obligatoires**

- Dataview — https://obsidian.md/plugins?id=dataview

## Licence

MIT. Utilisez-le, modifiez-le, partagez-le ; l'attribution est appréciée mais pas obligatoire.

Modèle de Vaultorial — https://vaultorial.com/fr/modele-diagramme-de-gantt/
