# Commencez ici

Bienvenue. Ce vault est un planificateur quotidien en time blocking : chaque jour reçoit trois priorités (le **Top 3**), une timeline de blocs au format Day Planner et une **Clôture** de deux minutes en fin de journée. Trois journées remplies et un aperçu de la semaine sont inclus, pour voir une semaine réelle et imparfaite — y compris des blocs qui ont dû être déplacés.

## Comment le vault est organisé

- `Planificateur/` — une note par jour (`YYYY-MM-DD`) plus une note simple d'aperçu hebdomadaire (`Semaine du 2026-06-08`). Les exemples couvrent du lundi au mercredi, 8–10 juin 2026 ; le mercredi est volontairement en milieu de journée, l'après-midi encore non coché.
- `Modèles/` — `Planificateur quotidien` (appliqué automatiquement aux nouvelles notes quotidiennes) et `Aperçu de la semaine`.

Le plugin natif **Daily notes** est configuré pour créer les notes du planificateur dans `Planificateur/` à partir du modèle.

## La méthode, en quatre règles

1. **Le Top 3 d'abord.** Si seules ces trois choses se font, la journée était bonne. Choisissez-les avant de regarder votre agenda.
2. **Bloquez la timeline.** Utilisez des lignes `- [ ] 09:00 - 10:30 Deep work : telle chose` sous *Planning du jour*. Les blocs sont des paris, pas des promesses — déplacez-les quand la réalité s'en mêle, n'abandonnez pas la liste.
3. **Un bloc profond avant le déjeuner.** Protégez-le comme un rendez-vous client.
4. **La clôture, toujours.** Cochez ce qui a eu lieu, notez ce qui passe à demain, fermez l'ordinateur. C'est la clôture qui fait que la planification de demain prend cinq minutes au lieu de trente.

## Premiers pas

1. Lisez les trois journées d'exemple dans l'ordre — le lundi s'est déroulé comme prévu, le mardi non, le mercredi est en cours. Ce contraste est tout l'intérêt.
2. Ouvrez la note du jour (icône calendrier ou `Ouvrir la note quotidienne du jour`). Le modèle se charge tout seul.
3. Écrivez votre Top 3, bloquez la matinée, commencez.

## Plugins

- **Day Planner** (facultatif mais recommandé) — transforme les lignes de la timeline en emploi du temps visuel avec un repère « maintenant » dans la barre latérale, et affiche votre journée sous forme de frise. Installez-le, gardez ses réglages par défaut, et il récupérera automatiquement les tâches `- [ ] HH:mm - HH:mm` de vos notes quotidiennes.

Tout le reste relève des plugins natifs, déjà configurés.

> [!tip] Estimez de moitié
> Si le time blocking est nouveau pour vous, rendez chaque bloc deux fois moins ambitieux que ce qui vous semble juste. Deux blocs profonds honnêtes de 90 minutes valent mieux qu'un emploi du temps fantasme qui s'effondre à 10 h 15.
