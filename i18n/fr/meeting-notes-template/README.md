# Pack de notes de réunion — modèle Obsidian

Trois modèles de notes de réunion à toute épreuve pour Obsidian — réunion d'équipe, 1-on-1 et appel client — avec un frontmatter structuré, une disposition cohérente ordre du jour/notes/décisions/actions, et un tableau de bord Dataview qui fait remonter chaque réunion et chaque action ouverte. Inclut quatre réunions d'exemple remplies issues d'un même projet pour que le tableau de bord fonctionne dès la première ouverture.

Les actions utilisent la syntaxe de date du plugin Tasks (`- [ ] Responsable — action 📅 2026-06-15`), de sorte qu'elles peuvent être reprises directement dans un vault GTD avec le plugin Tasks.

## Structure

```
meeting-notes-template/
├── Commencez ici.md                ← lisez ceci en premier
├── Tableau de bord des réunions.md ← Dataview : par type, par projet, actions ouvertes
├── Modèles/
│   ├── Réunion d'équipe.md
│   ├── 1-on-1.md
│   ├── Appel client.md
│   ├── Daily standup.md
│   └── Rétrospective.md
└── Réunions/                       ← six exemples remplis, un même projet cohérent
    ├── 2026-05-04 Lancement du portail client.md
    ├── 2026-05-11 1-on-1 Sarah et Priya.md
    ├── 2026-05-14 Appel client Brightleaf.md
    ├── 2026-05-19 Daily standup du portail client.md
    ├── 2026-06-01 Revue de sprint du portail client.md
    └── 2026-06-02 Rétrospective de sprint du portail client.md
```

## Installation

1. Téléchargez et décompressez le modèle : **Décompresser → Obsidian → Ouvrir un dossier comme coffre**.
2. Quand Obsidian le demande, activez les plugins communautaires pour ce vault.
3. Installez Dataview et ouvrez `Tableau de bord des réunions.md` en mode lecture.

## Plugins

**Requis**

- Dataview — https://obsidian.md/plugins?id=dataview

**Optionnels**

- Templater — https://obsidian.md/plugins?id=templater-obsidian (remplacez les variables Templates natif par des dynamiques si vous l'utilisez déjà)

## Licence

MIT. Utilisez-le, modifiez-le, partagez-le — attribution appréciée mais non requise.

Modèle par Vaultorial — https://vaultorial.com/fr/modele-notes-de-reunion/
