---
type: reunion-equipe
date: 2026-06-01
project: Portail client
attendees:
  - Sarah Chen
  - Priya Nair
  - Marcus Webb
---

# Revue de sprint du portail client

Revue interne du sprint 2 (2026-05-18 au 2026-05-29), le lundi suivant la clôture du sprint.

## Ordre du jour

1. Ce qui a été livré face à ce qu'on avait engagé
2. Le problème des données de test
3. Préparation de la démo pour vendredi
4. Risques pour la date du pilote

## Notes

- Livré : écran d'état de sinistre complet, y compris le texte de la réserve sur le lot nocturne, UI du fil de messagerie fonctionnant de bout en bout sur le staging, UI de téléversement construite mais tournant contre un mock.
- Non livré : téléversement contre l'entrepôt documentaire réel. Les identifiants sont arrivés le 2026-05-27, trop tard dans le sprint — reporté au sprint 3 avec l'intégration déjà cadrée.
- Données de test : l'extrait anonymisé des sinistres de Brightleaf est bloqué chez leur délégué à la protection des données. Sans lui, on démontre sur des sinistres synthétiques qui ne ressemblent en rien aux vrais. Marcus a proposé de générer un jeu synthétique plus riche à partir du schéma d'événements de sinistre plutôt que d'attendre ; approuvé.
- Priya anime la démo de vendredi en solo, conformément au plan du dernier 1-on-1. Répétition jeudi.
- Vérification des risques du pilote : la revue de sécurité (semaine du 2026-06-22) et les désignations d'assurés sont les deux dépendances externes. Les deux ont des responsables côté Brightleaf ; Sarah relance doucement en milieu de semaine.

## Décisions

- Cesser d'attendre l'extrait anonymisé pour les démos ; investir une demi-journée dans un générateur de données synthétiques et réévaluer quand l'extrait réel est débloqué.
- L'intégration du téléversement est le premier point du sprint 3 ; rien d'autre ne démarre tant qu'elle n'est pas de bout en bout sur le staging.

## Actions

- [x] Marcus — générateur de sinistres synthétiques produisant des données de démo réalistes 📅 2026-06-03 ✅ 2026-06-03
- [x] Priya — répétition du jeudi de la démo en solo avec Sarah en public 📅 2026-06-04 ✅ 2026-06-04
- [ ] Marcus — flux de téléversement fonctionnant contre l'entrepôt documentaire réel sur le staging 📅 2026-06-12
- [ ] Sarah — relance d'état à Helen sur la revue de sécurité et les désignations du pilote 📅 2026-06-11
