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
