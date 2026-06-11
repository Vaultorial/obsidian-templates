---
type: appel-client
date: 2026-05-14
project: Portail client
attendees:
  - Sarah Chen
  - Marcus Webb
  - Helen Brody (Brightleaf)
  - Tom Aldridge (Brightleaf)
---

# Appel client Brightleaf

Appel bimensuel programmé avec Brightleaf Insurance avant la première démo de sprint. Helen est la directrice des opérations et sponsor du projet ; Tom dirige l'équipe sinistres qui pilotera le portail.

## Ordre du jour

1. Avancement du sprint 1, honnêtement
2. Groupe pilote et calendrier
3. Contraintes de téléversement de documents
4. Planification de la revue de sécurité

## Notes

- Sarah a parcouru le sprint 1 : l'exploration de l'authentification a réussi contre le tenant de test du fournisseur d'identité ; l'écran d'état de sinistre lit des données en direct du système de polices de staging. Plus lent qu'espéré : les événements de sinistre arrivent par lots la nuit, donc l'état « en direct » est en réalité « à hier soir » — Tom a confirmé que cela correspond à la façon dont l'équipe sinistres travaille déjà, ce qui désamorce le problème.
- Pilote : Tom propose son équipe sinistres plus une poignée d'assurés de confiance plutôt qu'un lancement progressif public. Helen a approuvé — plus petit, plus sûr, retour plus rapide.
- Téléversement de documents : les règles de conservation de Brightleaf exigent que les téléversements atterrissent dans leur entrepôt documentaire, pas le nôtre. Marcus a confirmé que l'entrepôt a une API d'ingestion ; les limites de taille et les types de fichiers autorisés seront fournis par l'équipe de Tom.
- Revue de sécurité : l'équipe de sécurité interne de Brightleaf a besoin de trois semaines de préavis et d'un questionnaire complété. La réserver maintenant pour fin juin garde la date du pilote réaliste.

## Décisions

- Le groupe pilote est l'équipe sinistres plus des assurés invités ; début visé la dernière semaine de juin.
- Les documents téléversés vont directement dans l'entrepôt documentaire de Brightleaf ; le portail ne garde que des références.
- Revue de sécurité réservée pour la semaine du 2026-06-22 ; questionnaire à la charge de Marcus.

## Actions

- [x] Tom Aldridge — envoyer les types de fichiers et limites de taille autorisés pour les téléversements 📅 2026-05-20 ✅ 2026-05-19
- [x] Marcus — demander les identifiants de l'API de l'entrepôt documentaire pour le staging 📅 2026-05-18 ✅ 2026-05-18
- [ ] Marcus — compléter le questionnaire de sécurité 📅 2026-06-15
- [ ] Helen Brody (Brightleaf) — désigner les assurés de confiance pour le pilote 📅 2026-06-17
- [ ] Sarah — diffuser les critères de réussite du pilote pour validation 📅 2026-06-19
