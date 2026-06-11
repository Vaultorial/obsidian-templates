---
type: kundengespräch
date: 2026-05-14
project: Kundenportal
attendees:
  - Sarah Chen
  - Marcus Webb
  - Helen Brody (Brightleaf)
  - Tom Aldridge (Brightleaf)
---

# Kundengespräch Brightleaf

Geplanter zweiwöchentlicher Call mit Brightleaf Insurance vor der ersten Sprint-Demo. Helen ist die Betriebsleiterin und Projekt-Sponsorin; Tom leitet das Schadenteam, das das Portal pilotieren wird.

## Agenda

1. Sprint-1-Fortschritt, ehrlich
2. Pilotgruppe und Zeitplan
3. Einschränkungen beim Dokumenten-Upload
4. Terminierung der Sicherheitsprüfung

## Notizen

- Sarah ging Sprint 1 durch: Der Auth-Spike war gegen den Test-Tenant des Identitätsanbieters erfolgreich; der Schadenstatus-Screen liest Live-Daten aus dem Staging-Policensystem. Langsamer als erhofft: Schadensereignisse kommen über Nacht in Stapeln, der "Live"-Status ist also eigentlich "Stand letzte Nacht" — Tom bestätigte, dass das dem entspricht, wie das Schadenteam ohnehin arbeitet, was das Problem entschärft.
- Pilot: Tom schlägt sein Schadenteam plus eine Handvoll wohlgesinnter Versicherungsnehmer statt eines öffentlichen Soft-Launches vor. Helen stimmte zu — kleiner, sicherer, schnelleres Feedback.
- Dokumenten-Upload: Brightleafs Aufbewahrungsregeln verlangen, dass Uploads in ihrem Dokumentenspeicher landen, nicht in unserem. Marcus bestätigte, dass der Speicher eine Ingest-API hat; Größenlimits und erlaubte Dateitypen liefert Toms Team.
- Sicherheitsprüfung: Brightleafs internes Sicherheitsteam braucht drei Wochen Vorlauf und einen ausgefüllten Fragebogen. Sie jetzt für Ende Juni zu buchen, hält das Pilotdatum realistisch.

## Entscheidungen

- Pilotgruppe ist das Schadenteam plus eingeladene Versicherungsnehmer; Zielstart in der letzten Juniwoche.
- Hochgeladene Dokumente gehen direkt in Brightleafs Dokumentenspeicher; das Portal behält nur Referenzen.
- Sicherheitsprüfung gebucht für die Woche des 2026-06-22; Fragebogen verantwortet Marcus.

## Aktionspunkte

- [x] Tom Aldridge — erlaubte Dateitypen und Größenlimits für Uploads senden 📅 2026-05-20 ✅ 2026-05-19
- [x] Marcus — Zugangsdaten für die Dokumentenspeicher-API für Staging anfragen 📅 2026-05-18 ✅ 2026-05-18
- [ ] Marcus — den Sicherheitsfragebogen ausfüllen 📅 2026-06-15
- [ ] Helen Brody (Brightleaf) — die wohlgesinnten Versicherungsnehmer für den Piloten benennen 📅 2026-06-17
- [ ] Sarah — die Pilot-Erfolgskriterien zur Freigabe verteilen 📅 2026-06-19
