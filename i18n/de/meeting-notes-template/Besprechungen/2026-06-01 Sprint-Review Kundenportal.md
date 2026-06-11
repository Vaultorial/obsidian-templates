---
type: teammeeting
date: 2026-06-01
project: Kundenportal
attendees:
  - Sarah Chen
  - Priya Nair
  - Marcus Webb
---

# Sprint-Review Kundenportal

Interner Review von Sprint 2 (2026-05-18 bis 2026-05-29), am Montag nach Sprint-Ende.

## Agenda

1. Was ausgeliefert wurde gegen das, was wir zugesagt hatten
2. Das Testdaten-Problem
3. Demo-Vorbereitung für Freitag
4. Risiken für das Pilotdatum

## Notizen

- Ausgeliefert: Schadenstatus-Screen vollständig inklusive des Über-Nacht-Stapel-Hinweistexts, Messaging-Thread-UI funktioniert end-to-end auf Staging, Upload-UI gebaut, läuft aber gegen einen Mock.
- Nicht ausgeliefert: Upload gegen den echten Dokumentenspeicher. Zugangsdaten kamen am 2026-05-27, zu spät im Sprint — mit bereits umrissener Integration in Sprint 3 übertragen.
- Testdaten: Brightleafs anonymisierter Schadensauszug steckt bei ihrem Datenschutzbeauftragten fest. Ohne ihn demonstrieren wir auf synthetischen Schäden, die nichts mit echten zu tun haben. Marcus schlug vor, statt zu warten ein reichhaltigeres synthetisches Set aus dem Schadensereignis-Schema zu generieren; zugestimmt.
- Priya leitet Freitags Demo allein, gemäß dem Plan aus dem letzten 1-on-1. Generalprobe am Donnerstag.
- Pilot-Risikocheck: die Sicherheitsprüfung (Woche des 2026-06-22) und die Versicherungsnehmer-Nennungen sind die zwei externen Abhängigkeiten. Beide haben Verantwortliche auf der Brightleaf-Seite; Sarah hakt zur Wochenmitte sanft nach.

## Entscheidungen

- Aufhören, für Demos auf den anonymisierten Auszug zu warten; einen halben Tag in einen synthetischen Datengenerator investieren und neu bewerten, wenn der echte Auszug freigegeben ist.
- Die Upload-Integration ist der erste Punkt von Sprint 3; nichts anderes startet, bis sie auf Staging end-to-end läuft.

## Aktionspunkte

- [x] Marcus — synthetischer Schadensgenerator, der realistische Demo-Daten erzeugt 📅 2026-06-03 ✅ 2026-06-03
- [x] Priya — Donnerstags-Generalprobe der Solo-Demo mit Sarah als Publikum 📅 2026-06-04 ✅ 2026-06-04
- [ ] Marcus — Upload-Flow läuft gegen den echten Dokumentenspeicher auf Staging 📅 2026-06-12
- [ ] Sarah — Status-Stupser an Helen zur Sicherheitsprüfung und den Pilot-Nennungen 📅 2026-06-11
