# Exemple de Gantt statique

Un diagramme de Gantt écrit à la main, sans aucun plugin. Obsidian dessine lui-même les diagrammes Mermaid, ce bloc fonctionne donc dans n'importe quel vault. Utilisez-le pour un plan ponctuel, et le [[Calendrier]] quand les dates vivent dans vos notes de tâche.

```mermaid
gantt
    title Lancement de produit
    dateFormat YYYY-MM-DD
    axisFormat %d/%m
    excludes weekends
    section Recherche
    Étude de marché :done, r1, 2026-11-02, 8d
    Analyse de la concurrence :active, r2, after r1, 5d
    section Développement
    Prototype :crit, b1, after r2, 10d
    Test bêta :b2, after b1, 6d
    section Lancement
    Jour du lancement :milestone, m1, after b2, 0d
```

## Comment fonctionne la syntaxe

- `dateFormat` indique comment les dates sont écrites dans les lignes de tâche, `axisFormat` comment elles s'affichent sur l'axe.
- Chaque ligne s'écrit `nom :étiquettes, id, début, fin-ou-durée`. Les étiquettes sont facultatives : `done`, `active`, `crit` et `milestone`.
- `after id` fait démarrer une tâche quand une autre se termine : si vous déplacez la première, les suivantes suivent.
- `excludes weekends` fait compter uniquement les jours ouvrés dans des durées comme `5d`.
