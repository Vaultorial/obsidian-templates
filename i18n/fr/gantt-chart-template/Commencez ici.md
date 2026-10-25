# Commencez ici

Ce vault dessine des diagrammes de Gantt à partir de vos notes. Chaque tâche est une note avec une date `start` et une date `end` dans ses propriétés, et la note [[Calendrier]] transforme chaque tâche en barre : un diagramme par projet, une section par phase. Déplacez une date et le diagramme se redessine. Rien à exporter, et chaque tâche reste un simple fichier Markdown que vous pouvez lier, étiqueter et rédiger.

## Ce que contient le vault

- `Projets/` — deux projets d'exemple avec des tâches datées : un déménagement de bureaux et une refonte de site web, avec des tâches terminées, en cours et critiques, et des jalons.
- [[Calendrier]] — les diagrammes générés et la liste des tâches qui n'ont pas encore de date.
- [[Exemple de Gantt statique]] — un diagramme de Gantt Mermaid écrit à la main, sans plugin, avec la syntaxe expliquée.
- `Modèles/Tâche` — une note de tâche vierge avec toutes les propriétés.

## Plugins à activer

1. **Dataview** (obligatoire pour le [[Calendrier]]). Installez-le depuis les plugins communautaires.
2. Dans les réglages de Dataview, activez **JavaScript queries**.
3. Obsidian dessine les diagrammes avec Mermaid, intégré d'origine. Si une note demande s'il faut afficher les diagrammes Mermaid dans ce vault, autorisez-le.

Le plugin natif **Modèles** est déjà activé et pointe vers `Modèles/`.

## Propriétés d'une tâche

- `project` et `phase` déterminent le diagramme et la section où va la barre.
- `start` et `end` sont des dates au format AAAA-MM-JJ. Une tâche sans `start` reste hors du diagramme.
- `status` : `terminée`, `en cours` ou `à faire`.
- `critical: true` dessine la barre en rouge, `milestone: true` un losange à la date de début.

## Premiers pas

1. Activez Dataview et les JavaScript queries, puis ouvrez le [[Calendrier]] en mode lecture.
2. Ouvrez n'importe quelle tâche de `Projets/Déménagement des bureaux/`, changez sa date `end` et revenez au [[Calendrier]].
3. Pour votre propre projet : créez un dossier dans `Projets/`, ajoutez des notes de tâche avec le modèle Tâche et remplissez les dates.
