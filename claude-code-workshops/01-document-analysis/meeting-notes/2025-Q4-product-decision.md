# Product Decision Meeting — Rewards Platform Selection
**Date:** October 28, 2025
**Attendees:** Elena Rodriguez (CEO), Sarah Chen (VP Product), Marcus Williams (Head of Partnerships), Priya Patel (Analytics Lead), James O'Brien (CFO), David Kim (CTO), Lisa Tran (Customer Experience)

## Agenda
Review vendor evaluation and make final platform selection decision.

## Discussion

**Marcus** presented the vendor evaluation (see separate document). His recommendation was Vendor B (RewardStack) based on superior platform capabilities and built-in analytics.

**David** raised integration concerns with Vendor B. Our core banking system runs on a legacy stack that isn't in RewardStack's standard connector library. He estimated the integration could take 6-7 months rather than the quoted 5, based on similar past projects. "Every vendor underestimates integration with our stack."

**James** presented the financial analysis:
- Vendor A (LoyaltyCore): $2.1M over 3 years, but add ~$400K/year for supplementary analytics = **$3.3M effective 3-year cost**
- Vendor B (RewardStack): $2.8M over 3 years, analytics included = **$2.8M effective 3-year cost**
- However, Vendor A is offering a 15% early renewal discount that expires December 31. If we don't renew, we lose the discount and face a 20% price increase at contract end (March 2026).

**Elena** asked about the customer impact of delay. Priya shared that every quarter of delay costs approximately $1.1M in continued churn at current rates.

**Sarah** argued for Vendor B on strategic grounds: "We're not just buying a loyalty platform. We're buying the ability to iterate. RewardStack lets us A/B test reward structures. LoyaltyCore means we're locked into whatever we launch."

## Decision

**Selected: Vendor A (LoyaltyCore)** — with conditions.

Despite Marcus's recommendation of Vendor B, the team chose Vendor A for the following reasons:

1. **Contract timing:** The early renewal discount saves $315K and avoids a 20% price increase. Missing the December 31 deadline creates significant cost risk.
2. **Speed to market:** 5 months vs 8+ months. At $1.1M/quarter churn cost, the 3-month difference has real financial impact (~$825K).
3. **Integration risk:** David's assessment that RewardStack integration would likely take longer than quoted tipped the risk calculus.
4. **Mitigation plan:** James proposed allocating $200K from Q1 budget for a standalone analytics layer to address LoyaltyCore's reporting gaps. This brings the effective cost closer to parity while maintaining the faster timeline.

**Elena's closing comment:** "I hear the strategic argument for RewardStack, and I don't disagree. But we're losing customers now. We need to move fast, and LoyaltyCore gets us there sooner with less risk. We can always re-evaluate platforms in 3 years."

## Action Items
- [ ] James to initiate LoyaltyCore contract renewal by November 15
- [ ] David to assign integration lead and begin technical planning
- [ ] Sarah to finalize 3-tier rewards structure for LoyaltyCore implementation
- [ ] Marcus to notify WestJet of upcoming changes (90-day notice)
- [ ] Priya to define analytics requirements for supplementary reporting layer
- [ ] Legal to review updated LoyaltyCore contract terms

## Target Timeline
- Contract signed: December 2025
- Development start: January 2026
- Testing: April 2026
- Launch: May 2026

---
*Notes taken by Lisa Tran. Distributed to all attendees.*
