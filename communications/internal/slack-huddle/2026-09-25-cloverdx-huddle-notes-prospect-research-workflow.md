# 2026-09-25 — CloverDX huddle: prospect-research workflow, field standardization, LinkedIn Ads API

**Huddle:** 25/09/2026, 10:29:36–10:37:12 BST, `#cloverdx-internal` (C0ABLAVBVDJ). AI notes canvas `F0C48RGGBJP`, transcript `F0C4H0VH8DP`.
**Attendees:** U0ACAB6GNN4 (Clay operator/engineer) and U0AB49S6806 (Leo).
**Type:** GTM-internal prep for the CloverDX client call — follow-on to the 09:25 audience-segmentation huddle. **No client-confirmed fact originated here** — all rows GTM-authored.

## Summary

- **Prospect identification & research workflow (U0ACAB6GNN4):** tracks web visits from prospects, filtering by **page path + domain** to identify companies already aware of the product [0:42]. Uses AI (**4 Mini**) with **domain name + page type** as inputs to judge whether a company faces **forcing factors to change** and to suggest **outreach angles** [1:25]. Example output: a company visiting a **competitor page** classified **"stage one competitor"** — high engagement, potential interest in switching tools [2:55].
- **Field standardization & segment creation (Leo):** standardize fields across **all Clay accounts** so every company has consistent field availability [6:00]. U0ACAB6GNN4 proposed presets for a **new field** using Leo's existing framework: **warm, nurture, air cover, direct** [6:23]. System should populate the field **automatically** and enable **segment tracking** by assigned value [6:43].
- **LinkedIn Marketing API integration (Leo):** once an account lands in a segment, trigger a workflow to push it to a **predefined LinkedIn marketing campaign via API** [6:47]. U0ACAB6GNN4 confirmed alignment with this approach for **automated ad deployment** [7:08].

## Action items

1. **U0ACAB6GNN4** — update the prospect-research workflow and join a follow-up call to discuss next steps [7:17]. Status: open → **A13**.
2. **U0ACAB6GNN4** — verify whether the system can push companies to different segments [4:19] (gates the LinkedIn Ads API trigger). Status: open → **A14**.

## Risks / flags

- The **segment → LinkedIn Ads campaign** trigger depends on the system being able to **push accounts between segments** — unverified (ties to A14).
- **Field presets (warm/nurture/air-cover/direct)** only useful if fields are consistent across **all** Clay accounts — Leo driving standardization [ASSUMPTION until implemented].

Source: `~/gtm-studios/inbox/slack-huddles/20260925_093742__headphones__Huddle_notes__25_09_2026_in___C0ABLAVBVDJ_.html` (canvas). Huddle: `https://gtmstudios.slack.com/archives/C0ABLAVBVDJ/p1790328575286559`.
