# Q1 2026 Kickoff — Rewards Program Restructuring
**Date:** January 8, 2026
**Attendees:** Sarah Chen (VP Product), David Kim (CTO), Marcus Williams (Head of Partnerships), Priya Patel (Analytics Lead), James O'Brien (CFO), Rachel Foster (CCO), Lisa Tran (Customer Experience), Tom Nguyen (Engineering Lead)

## Status Update

### What's Done
- ✅ LoyaltyCore contract renewed and signed (December 18, 2025)
- ✅ 3-tier structure finalized: Essentials → Preferred → Premium
- ✅ WestJet notified of changes (November 28 — within 90-day requirement)
- ✅ Engineering lead assigned (Tom Nguyen)
- ✅ Compliance Issue #1 (tier migration notification) — resolved
- ✅ Q1 budget allocated: $200K for analytics layer, $150K for LoyaltyCore custom development

### What's In Progress
- 🔄 LoyaltyCore technical integration planning (Tom — on track)
- 🔄 Customer communication drafts under Compliance review
- 🔄 Supplementary analytics platform evaluation (Priya)

### What's Blocked
- ⛔ **Compliance Issue #2 (Points Conversion Fairness) — STILL PENDING**
  - Amir's legal analysis was due December 15 but has been delayed
  - The edge case for Silver-tier customers with >50,000 points remains unresolved
  - **This is a launch blocker.** We cannot migrate customers until the conversion formula is legally approved.
  - Rachel confirmed: "We will not approve go-live without resolution of this issue."
  - New target: January 31, 2026

## Revised Timeline

| Milestone | Original Date | Revised Date | Status |
|-----------|--------------|--------------|--------|
| Contract signed | Dec 2025 | Dec 18, 2025 | ✅ Done |
| Development start | Jan 2026 | Jan 15, 2026 | 🔄 Slight delay (waiting on compliance) |
| Points conversion approved | — | Jan 31, 2026 | ⛔ Blocker |
| Testing | Apr 2026 | Apr 2026 | On track (if blocker resolved) |
| Customer notifications sent | — | Mar 15, 2026 | Dependent on compliance approval |
| Launch | May 2026 | May 2026 | At risk if blocker not resolved by Jan 31 |

## Key Decisions Made
1. **Analytics platform:** Priya recommended Metabase (open-source) connected to our data warehouse rather than a commercial tool. James approved — saves ~$120K vs. commercial options.
2. **Parallel run:** David confirmed LoyaltyCore can support a 30-day parallel run. Both old and new structures will be active during transition.
3. **Customer segmentation for rollout:** Lisa proposed a phased rollout — Premium tier first (smallest group, highest engagement), then Preferred, then Essentials. Sarah approved.

## Risks
1. **Compliance blocker** — If points conversion isn't resolved by Jan 31, the May launch is at risk. Mitigation: Sarah to escalate to Elena if no resolution by Jan 20.
2. **WestJet integration** — Marcus flagged that WestJet's technical team is slow to respond. If their API changes aren't ready, we may need to launch without co-brand integration and add it post-launch.
3. **Customer backlash** — Eliminating 2 tiers will upset some customers regardless of how fair the conversion is. Lisa is preparing a FAQ and training customer service team.

## Action Items
- [ ] Amir: Deliver points conversion legal opinion by January 31 (CRITICAL)
- [ ] Tom: Complete LoyaltyCore integration spec by January 22
- [ ] Sarah: Escalate compliance blocker to Elena if unresolved by January 20
- [ ] Marcus: Follow up with WestJet technical team weekly
- [ ] Priya: Deploy Metabase instance and connect to data warehouse by February 15
- [ ] Lisa: Complete customer service training materials by March 1

---
*Notes taken by Lisa Tran. This is a CONFIDENTIAL internal document.*
