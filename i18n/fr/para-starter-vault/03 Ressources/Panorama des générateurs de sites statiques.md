---
type: ressource
created: 2026-02-21
tags: [ressource, web]
---

# Panorama des générateurs de sites statiques

Note de référence créée pendant les recherches pour [[Lancement du site personnel]]. Gardée dans Ressources plutôt que dans le dossier du projet parce qu'elle survivra au projet — la prochaine refonte du site en voudra aussi.

## Ce qu'est un générateur de site statique

Un outil qui prend des fichiers texte (en général du Markdown) plus des gabarits, et produit un dossier de HTML fini. Pas de base de données, pas de code côté serveur à l'exécution — le résultat s'héberge partout où l'on peut servir des fichiers.

## Ce que j'ai comparé, et l'impression laissée

- **Hugo** — un seul binaire, builds très rapides, le templating demande un temps d'adaptation.
- **Eleventy** — basé sur JavaScript, flexible, très peu d'a priori sur la structure.
- **Astro** — modèle à composants, plus de pièces mobiles qu'un site de cinq pages n'en demande.
- **Jekyll** — le vétéran ; correct, mais je n'ai de Ruby nulle part ailleurs dans ma vie.

## Décision (21/02/2026)

Eleventy. Raison : mes notes sont déjà en Markdown, je lis ses gabarits sans manuel, et le build est assez simple pour que le moi du futur le comprenne encore dans deux ans. Décision consignée ici pour que la note de projet ([[Lancement du site personnel]]) reste une affaire d'actions, pas de recherche.
