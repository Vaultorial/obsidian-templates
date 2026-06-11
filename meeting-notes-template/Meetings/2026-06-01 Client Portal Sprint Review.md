---
type: team-meeting
date: 2026-06-01
project: Client Portal
attendees:
  - Sarah Chen
  - Priya Nair
  - Marcus Webb
---

# Client Portal Sprint Review

Internal review of sprint 2 (2026-05-18 to 2026-05-29), the Monday after sprint close.

## Agenda

1. What shipped vs what we committed
2. The test data problem
3. Demo prep for Friday
4. Risks for the pilot date

## Notes

- Shipped: claim-status screen complete including the overnight-batch caveat copy, messaging thread UI working end to end on staging, upload UI built but running against a mock.
- Not shipped: upload against the real document store. Credentials arrived 2026-05-27, too late in the sprint — carried to sprint 3 with the integration already scoped.
- Test data: Brightleaf's anonymized claims extract is stuck with their data protection officer. Without it we demo on synthetic claims that look nothing like real ones. Marcus proposed generating a richer synthetic set from the claim-event schema instead of waiting; agreed.
- Priya runs Friday's demo solo, per the plan from the last 1-on-1. Dry run on Thursday.
- Pilot risk check: security review (week of 2026-06-22) and policyholder nominations are the two external dependencies. Both have owners on the Brightleaf side; Sarah chases gently mid-week.

## Decisions

- Stop waiting on the anonymized extract for demos; invest half a day in a synthetic data generator and revisit when the real extract clears.
- Upload integration is the first item of sprint 3; nothing else starts until it is end-to-end on staging.

## Action items

- [x] Marcus — synthetic claims generator producing realistic demo data 📅 2026-06-03 ✅ 2026-06-03
- [x] Priya — Thursday dry run of the solo demo with Sarah as audience 📅 2026-06-04 ✅ 2026-06-04
- [ ] Marcus — upload flow working against the real document store on staging 📅 2026-06-12
- [ ] Sarah — status nudge to Helen on the security review and pilot nominations 📅 2026-06-11
