---
type: reunion-equipe
date: 2026-05-04
project: Portail client
attendees:
  - Sarah Chen
  - Priya Nair
  - Marcus Webb
---

# Lancement du portail client

Lancement interne de la phase de build du portail client de Brightleaf Insurance. La découverte s'est terminée fin avril ; cette réunion transforme les conclusions en un plan de travail.

## Ordre du jour

1. Récapitulatif : ce à quoi la découverte nous a engagés
2. Cadence des sprints et rôles
3. Inconnues techniques à explorer en premier
4. Ce que le client voit, et quand

## Notes

- Périmètre issu de la découverte : les assurés peuvent consulter l'état de leur sinistre, téléverser des documents vers un sinistre ouvert et envoyer des messages à l'équipe sinistres. Explicitement hors périmètre : les paiements et les changements de police — phase deux au plus tôt.
- Rôles : Priya pilote le frontend du portail, Marcus la couche d'API et l'intégration avec le système de polices de Brightleaf, Sarah gère la relation client et le backlog.
- Deux inconnues techniques à explorer avant d'engager le sprint 1 : comment le système de polices expose les événements de sinistre, et si le fournisseur d'identité de Brightleaf supporte le flux de connexion que nous avons esquissé.
- Convenu de ne démontrer que du logiciel qui fonctionne — jamais de démos sur diapositives au client. Si un sprint ne produit rien de démontrable, on le dit.

## Décisions

- Sprints de deux semaines à partir du 2026-05-04 ; démo face au client un vendredi sur deux.
- Les revues de sprint sont internes le lundi suivant chaque sprint ; l'appel client suit le jeudi.
- L'exploration de l'authentification prend les trois premiers jours du sprint 1 avant tout travail d'UI.

## Actions

- [x] Marcus — exploration de l'authentification et des événements de sinistre documentée 📅 2026-05-07 ✅ 2026-05-07
- [x] Sarah — backlog du sprint 1 convenu avec Helen chez Brightleaf 📅 2026-05-06 ✅ 2026-05-05
- [x] Priya — échafaudage de l'UI du portail et design tokens dans le dépôt 📅 2026-05-08 ✅ 2026-05-08
- [ ] Sarah — écrire la note de logistique du jour de démo pour le côté client 📅 2026-06-12
