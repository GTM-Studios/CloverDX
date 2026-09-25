# Decisions

Log of material decisions made on this engagement. Append at the bottom, chronological — never rewrite an existing entry.

## 2026-09-18 — Engagement repo launched from GTM Studios template

**Decision (GTM's own):** created `GTM-Studios/CloverDX` from the `client-engagement-template`, replacing the lightweight `clients/cloverdx/` folder as the canonical source of truth for this engagement.

**Source:** bootstrap of this repo; template at `studio/templates/client-engagement-repo/`.

**Status:** Active.

---

## 2026-09-23 — CloverDX weekly sync rescheduled to Friday; Albin proposing Friday to Ross

**Decision (client-facing, in-progress — Albin x Ross):** the CloverDX weekly sync, moved off its original slot, is now being proposed for **Friday** — Albin asked Leo whether to suggest Friday, Leo agreed, and Albin proposed Friday to Ross at CloverDX (pending Ross confirmation). Feeds and partly resolves the C-sync reschedule thread.

**Source:** `communications/internal/slack/2026-09-23-cloverdx-slack-morning-digest.md` (morning digest 2026-09-23, #cloverdx-internal `C0ABLAVBVDJ`).

**Status:** Active — Friday proposed to Ross, client to confirm.

---

## 2026-09-24 — Strategic shift to awareness-stage framework for high-value/hard-persona deals

**Decision (GTM's own, Leo):** straight outbound does not work for high-value deals with difficult personas; Leo will develop a new **awareness-stage framework** to combine with current targeting (CloverDX pipeline). U0ACAB6GNN4 called it a likely "game changer" once refined. Engages the Clay job-change signal gap as a build dependency.

**Source:** `communications/internal/slack-huddle/2026-09-24-cloverdx-huddle-notes-clay-enrichment.md` (huddle C0ABLAVBVDJ).

**Status:** Active — framework to be developed and presented by Leo.

---

## 2026-09-24 (2nd) — Web-visitor contact-level tracking ask + job-change signal resolution (CloverDX, GTM-authored)

**Decision (GTM's own, Leo):** ask Clay support whether the **built-in website-visitor providers can track at CONTACT
level** (currently company-level only) — intent confirmed contact-level ("Yes second one"). New action **A9**
(clickup `124f7bm4f6j`). **Also:** the job-change signal gap (A7) was root-caused with Clay support — **signals must be
run first** before pulling data (a workbook-table signal can't detect job changes in an Audience); new signal set up.

**Source:** `communications/internal/slack/2026-09-24-cloverdx-slack-audiences-stage-mapping-job-change-resolution-web-visitor-tracking.md` (#cloverdx-internal `C0ABLAVBVDJ`).

**Status:** Active — A9 queued to Albin (ask support); A7 mostly resolved, monitor rebuilt signal.

---

## 2026-09-25 — Audience segmentation framework (3 segments) + workflow/account-agent prep for client call

**Decision (GTM's own, Leo):** audience segmentation framework structured by familiarity — **segment 1 "know us"**, **segment 2 "using Informatica but don't know us"**, **segment 3 "cold fit"**; enriched accounts land in segments by signals (competitor usage / no signals). Prior straight outbound failed; relationship-based outbound succeeded → **nurture-first strategy**. Workflows will move accounts between segments on triggers (job changes, ad opens), driven by chat-prompted logic. **Account agents** combine tables with skills (web search, contact finding) for inbound handling — feature requires an upgrade before implementation. Preps the next CloverDX client call: U0ACAB6GNN4 to build a sample workflow + account agent by 11:00 (**A10**); Leo to finalize audiences + presentation (**A12**).

**Source:** `communications/internal/slack-huddle/2026-09-25-cloverdx-huddle-notes-audience-segmentation-framework.md` (huddle `#cloverdx-internal` `C0ABLAVBVDJ`).

**Status:** Active — prep tasks in flight for the client call.

---

## 2026-09-25 (2nd) — Prospect-research workflow + field standardization + LinkedIn Ads API (CloverDX, GTM-authored)

**Decision (GTM's own, Leo + U0ACAB6GNN4):** U0ACAB6GNN4's **prospect research workflow** is the intake arm — tracks prospect web visits (filter by page path + domain) to surface companies already aware of the product, uses AI (4 Mini) on domain+page-type inputs to flag **forcing factors** and suggest **outreach angles** (competitor-page visitor = "stage one competitor"). **Field standardization:** Leo to standardize fields across **all Clay accounts**; presets for a new field using the **warm / nurture / air cover / direct** framework, auto-populated with **segment tracking** by value. **LinkedIn Marketing API:** when an account lands in a segment, a workflow triggers to push it to a **predefined LinkedIn ad campaign via API** (U0ACAB6GNN4 aligned, automated ad deployment). Adds actions **A13** (update workflow + follow-up call) and **A14** (verify segment-push capability).

**Source:** `communications/internal/slack-huddle/2026-09-25-cloverdx-huddle-notes-prospect-research-workflow.md` (huddle `#cloverdx-internal` `C0ABLAVBVDJ`).

**Status:** Active — A13/A14 queued to U0ACAB6GNN4.

---

## 2026-09-25 (3rd) — Cloud MCP ↔ Clay connection + project ownership transfer to U0ACAB6GNN4 (CloverDX, GTM-authored)

**Decision (GTM's own, Leo):** **project ownership transferred** to U0ACAB6GNN4 — Marketing work with Laura and Kate to translate results more directly; Leo flagged uncertainty on project duration. **Cloud MCP ↔ Clay:** client has a custom-built brain and wants to connect its cloud MCP to its Clay workspace; team will implement Jay's changes on their table and **automate his manual cloud-check step via a Clay connection** (removes manual verification). **Accountability concern:** Leo wants the client left **with no excuses for non-delivery** — flagged ambiguity on the "sequence" issue (Matt: still problematic; Kate: they'll fix themselves), and possible misalignment given extensive feedback vs only **5 dials**. Adds actions **A15** (summary email + context to Kate re MCP server connection, `124f7bm4h8c`), **A16** (investigate + implement cloud MCP ↔ Clay connection, `124f7bm4h8d`), **A17** (Leo calls Ross re project progress, `124f7bm4h8e`).

**Source:** `communications/internal/slack-huddle/2026-09-25-cloverdx-huddle-notes-cloud-mcp-ownership-transfer.md` (huddle `#cloverdx-internal` `C0ABLAVBVDJ`).

**Status:** Active — A15/A16 queued to U0ACAB6GNN4, A17 to Leo.
