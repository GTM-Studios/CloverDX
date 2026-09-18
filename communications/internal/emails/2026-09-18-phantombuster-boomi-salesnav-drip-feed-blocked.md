# CloverDX: PhantomBuster "Boomi - SalesNav - Drip Feed" blocked — no Sales Navigator — 2026-09-18

Source: Gmail `1a0b2f65bfd6c8ed`, Subject: "Your automation didn't go all the way — here's a quick fix" from PhantomBuster (`notifications@mg.phantombuster.com`), received 2026-09-18 05:21 UTC. To: Sid Suresh, Leo Bran, Albin Beqiri.

## Summary
PhantomBuster automation **"CloverDx - Boomi - SalesNav - Drip Feed"** (automation id 5704928670514197) failed to complete. Reason given: **"You don't have a Sales Navigator account. Please upgrade your plan to begin extraction."**

## Status signal (GTM-authored, internal)
BLOCKER on the CloverDX SalesNav drip-feed / outbound lead-gen pipeline: the Phantom can't extract without a connected Sales Navigator account. Second of two SalesNav-blocked automations this week. [ASSUMPTION] a tooling/config gap (SalesNav access not provisioned), not a CloverDX-side instruction.

## Flag for Leo
- Resolve whether a Sales Navigator account should be provisioned, or park the drip feed. Do not pick a winner/act on provisioning silently.

*(verified 2026-09-18, Gmail read)*
