# CloverDX — Audiences deep-dive: audience-to-stage mapping, job-change signal resolution, web-visitor contact-level tracking

**Source:** `#cloverdx-internal` / team channel (channel `C0ABLAVBVDJ`, weekly CloverDX sync), 2026-09-23 12:30 → 2026-09-24 15:02 BST. Slack sweep `1790252483`→`1790261550` (thread). GTM-authored (Leo Branica × Albin Beqiri). Follows the 09-24 13:15 huddle (`slack-huddle/2026-09-24-cloverdx-huddle-notes-clay-enrichment.md`).

## Content

**1. Audience-to-awareness-stage mapping direction (Leo, feeds A8).**
Leo (09-24 12:24): "Ok this what I am thinking", "How can we create an audience and map them out to each stage" → definitions
"solution aware means using a cloud solution  Product aware is using informatica"; "accounts that change jobs could be in the
most aware" and running ads, not just outbound (12:26–12:30); "This is what I am thinking - let me know if that makes sense" (12:59). Extends the awareness-stage framework (A8) into the Audiences build.

**2. Job-change signal in Clay Audiences — root-caused and resolved (updates A7 blocker).**
- Albin (12:31): taking all HubSpot people + checking for job changes → "0 results … even though we've done these job changes signals before in Clay." Test: "Brandon Powers", changed job Aug 31.
- Possible cause: `Name` field empty / full-name matching (12:31); "45k contacts being enriched with full name" (13:06).
- **Clay support answer (13:42–14:48):** the original job-change signal was created in a workbook referencing a table, so it cannot detect job changes in an Audience — **signals must be run first before pulling the data**. Albin confirmed "It works that way" (14:48); new signal set up (Clay workbook `wb_0sx0zx8y8y4jDfuTSPS`). **A7 blocker partially cleared** — people-segment job-change filters now work via run-signals-first.

**3. Web-visitor contact-level tracking — ask queued to Clay support (NEW action A9).**
Leo (14:52): "could you also ask support does the built in web site visitors providers, do they allow you to track people?"
Albin clarified (14:54–14:56): other providers such as RB2B vs tracking visits at **contact** level (currently company-level only,
per the 13:15 huddle finding). Leo confirmed intent = contact-level (15:02: "Yes second one") → **A9**: Albin to ask Clay support
whether built-in website-visitor providers support contact-level tracking.

## Classifications
- All GTM-authored — no client-confirmed fact on this thread.
- Cross-refs: `slack/2026-09-23-cloverdx-slack-morning-digest.md`, `slack-huddle/2026-09-24-cloverdx-huddle-notes-clay-enrichment.md`, `ACTION-ITEMS.md` A7/A8/A9.