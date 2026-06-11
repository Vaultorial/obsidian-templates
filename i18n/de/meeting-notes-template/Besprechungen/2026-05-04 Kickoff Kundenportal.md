---
type: teammeeting
date: 2026-05-04
project: Kundenportal
attendees:
  - Sarah Chen
  - Priya Nair
  - Marcus Webb
---

# Kickoff Kundenportal

Interner Kickoff für die Build-Phase des Kundenportals von Brightleaf Insurance. Die Discovery endete Ende April; diese Besprechung verwandelt die Erkenntnisse in einen funktionierenden Plan.

## Agenda

1. Rückblick: worauf uns die Discovery festgelegt hat
2. Sprint-Taktung und Rollen
3. Technische Unbekannte, die zuerst zu spiken sind
4. Was der Kunde sieht, und wann

## Notizen

- Umfang aus der Discovery: Versicherungsnehmer können den Schadenstatus prüfen, Dokumente zu einem offenen Schaden hochladen und dem Schadenteam Nachrichten schreiben. Ausdrücklich draußen: Zahlungen und Policenänderungen — frühestens Phase zwei.
- Rollen: Priya verantwortet das Portal-Frontend, Marcus die API-Schicht und die Integration mit Brightleafs Policensystem, Sarah die Kundenbeziehung und das Backlog.
- Zwei technische Unbekannte, die es vor dem Festlegen von Sprint 1 zu spiken lohnt: wie das Policensystem Schadensereignisse bereitstellt, und ob Brightleafs Identitätsanbieter den von uns skizzierten Login-Flow unterstützt.
- Vereinbart, nur funktionierende Software zu demonstrieren — niemals Folien-Demos für den Kunden. Bringt ein Sprint nichts Vorführbares, sagen wir das.

## Entscheidungen

- Zwei-Wochen-Sprints ab dem 2026-05-04; kundenseitige Demo jeden zweiten Freitag.
- Sprint-Reviews sind intern am Montag nach jedem Sprint; das Kundengespräch folgt am Donnerstag.
- Der Auth-Spike bekommt die ersten drei Tage von Sprint 1, bevor irgendeine UI-Arbeit beginnt.

## Aktionspunkte

- [x] Marcus — Auth- und Schadensereignis-Spike dokumentiert 📅 2026-05-07 ✅ 2026-05-07
- [x] Sarah — Sprint-1-Backlog mit Helen bei Brightleaf abgestimmt 📅 2026-05-06 ✅ 2026-05-05
- [x] Priya — Portal-UI-Gerüst und Design-Tokens im Repo 📅 2026-05-08 ✅ 2026-05-08
- [ ] Sarah — das Demo-Tag-Logistik-Einseiter für die Kundenseite schreiben 📅 2026-06-12
