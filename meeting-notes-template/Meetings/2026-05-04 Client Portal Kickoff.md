---
type: team-meeting
date: 2026-05-04
project: Client Portal
attendees:
  - Sarah Chen
  - Priya Nair
  - Marcus Webb
---

# Client Portal Kickoff

Internal kickoff for the build phase of the Brightleaf Insurance client portal. Discovery wrapped at the end of April; this meeting turns the findings into a working plan.

## Agenda

1. Recap: what discovery committed us to
2. Sprint cadence and roles
3. Technical unknowns to spike first
4. What the client sees, and when

## Notes

- Scope from discovery: policyholders can check claim status, upload documents to an open claim, and message the claims team. Explicitly out: payments and policy changes — phase two at the earliest.
- Roles: Priya owns the portal frontend, Marcus owns the API layer and the integration with Brightleaf's policy system, Sarah runs the client relationship and the backlog.
- Two technical unknowns worth spiking before sprint 1 commits: how the policy system exposes claim events, and whether Brightleaf's identity provider supports the login flow we sketched.
- Agreed to demo working software only — no slide demos to the client, ever. If a sprint produces nothing demoable, we say so.

## Decisions

- Two-week sprints starting 2026-05-04; client-facing demo every other Friday.
- Sprint reviews are internal on the Monday after each sprint; the client call follows on Thursday.
- The auth spike gets the first three days of sprint 1 before any UI work starts.

## Action items

- [x] Marcus — auth and claim-events spike written up 📅 2026-05-07 ✅ 2026-05-07
- [x] Sarah — sprint 1 backlog agreed with Helen at Brightleaf 📅 2026-05-06 ✅ 2026-05-05
- [x] Priya — portal UI scaffold and design tokens in the repo 📅 2026-05-08 ✅ 2026-05-08
- [ ] Sarah — write the demo-day logistics one-pager for the client side 📅 2026-06-12
