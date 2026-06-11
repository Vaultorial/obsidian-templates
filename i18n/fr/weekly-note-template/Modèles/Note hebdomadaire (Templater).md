---
week: <% tp.file.title %>
start: <% moment(tp.file.title, "GGGG-[W]WW").startOf("isoWeek").format("YYYY-MM-DD") %>
end: <% moment(tp.file.title, "GGGG-[W]WW").endOf("isoWeek").format("YYYY-MM-DD") %>
type: hebdomadaire
---

# <% tp.file.title %> — <% moment(tp.file.title, "GGGG-[W]WW").startOf("isoWeek").format("D") %>–<% moment(tp.file.title, "GGGG-[W]WW").endOf("isoWeek").format("D MMMM YYYY") %>

← [[<% tp.date.now("GGGG-[W]WW", -7, tp.file.title, "GGGG-[W]WW") %>]] | [[<% tp.date.now("GGGG-[W]WW", 7, tp.file.title, "GGGG-[W]WW") %>]] →

## Plan de la semaine

**Objectif :**

- [ ]
- [ ]
- [ ]

## Bilan

### Réussites

-

### Chiffres

| Indicateur | Cible | Réel |
| ---------- | ----- | ---- |
|            |       |      |

### Reporté

-

### Objectif de la semaine prochaine

-

> [!note]- Comment utiliser ce modèle
> Variante Templater. La plage de la semaine et les liens précédent/suivant se déduisent du nom du fichier : nommez la note `2026-W24` (semaine ISO) et appliquez le modèle via Templater. Réglage : installez Templater et définissez `Modèles` comme son dossier de modèles. Supprimez ce callout de votre copie.
