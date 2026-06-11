---
type: client-call
date: 2026-05-14
project: Client Portal
attendees:
  - Sarah Chen
  - Marcus Webb
  - Helen Brody (Brightleaf)
  - Tom Aldridge (Brightleaf)
---

# Brightleaf Client Call

Scheduled fortnightly call with Brightleaf Insurance ahead of the first sprint demo. Helen is the ops director and project sponsor; Tom leads the claims team that will pilot the portal.

## Agenda

1. Sprint 1 progress, honestly
2. Pilot group and timeline
3. Document upload constraints
4. Security review scheduling

## Notes

- Sarah walked through sprint 1: auth spike succeeded against the identity provider's test tenant; claim-status screen reads live data from the staging policy system. Slower than hoped: claim events arrive in batches overnight, so "live" status is really "as of last night" — Tom confirmed that matches how the claims team already works, which defuses the issue.
- Pilot: Tom proposes his claims team plus a handful of friendly policyholders rather than a public soft launch. Helen agreed — smaller, safer, faster feedback.
- Document upload: Brightleaf's retention rules require uploads to land in their document store, not ours. Marcus confirmed the store has an ingestion API; size limits and allowed file types to be provided by Tom's team.
- Security review: Brightleaf's internal security team needs three weeks' notice and a completed questionnaire. Booking it now for late June keeps the pilot date realistic.

## Decisions

- Pilot group is the claims team plus invited policyholders; target start in the last week of June.
- Uploaded documents go directly to Brightleaf's document store; the portal keeps only references.
- Security review booked for the week of 2026-06-22; questionnaire owned by Marcus.

## Action items

- [x] Tom Aldridge — send allowed file types and size limits for uploads 📅 2026-05-20 ✅ 2026-05-19
- [x] Marcus — request document store API credentials for staging 📅 2026-05-18 ✅ 2026-05-18
- [ ] Marcus — complete the security questionnaire 📅 2026-06-15
- [ ] Helen Brody (Brightleaf) — nominate the friendly policyholders for the pilot 📅 2026-06-17
- [ ] Sarah — circulate the pilot success criteria for sign-off 📅 2026-06-19
