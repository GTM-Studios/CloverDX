# 2026-09-24 — CloverDX huddle: Clay enrichment & signal-gap + awareness-stage shift

**Huddle:** 24/09/2026, 14:15–14:24 BST, `#cloverdx-internal` (C0ABLAVBVDJ). AI notes canvas `F0C41SDRSKX`, transcript `F0C4AH8FA76`.
**Attendees:** U0ACAB6GNN4 (Clay operator) and U0AB49S6806 (Leo).
**Type:** GTM-internal coordination carrying real CloverDX engagement work. **No client-confirmed fact originated here** — all rows GTM-authored.

## Summary

- **HubSpot name-field population:** U0ACAB6GNN4 found HubSpot contacts have first/last names but a blank full-name field; built a workflow (AI agent) to auto-populate it across **45,000 contacts** [4:01].
- **Job-change signal gap (key finding):** applying a job-change filter to a people segment returns *"no records found"* despite LinkedIn showing Brandon Powers moving to Global Wet Link [1:19][2:30]. U0AB49S6806 + U0ACAB6GNN4 suspect a Clay bug or config needing support contact [3:31][4:49]. Web-visit signals work correctly — the non-detection is inconsistent [3:25].
- **Web-visit granularity:** web-visit signals appear only at **company** level, not individual people level — filtering returns all people from visited companies, not specific visitors [5:16][5:24]. Path filtering (demo/trial/pricing) works at company level [6:33].
- **Strategic shift (GTM, Leo):** straight outbound doesn't work for high-value deals with difficult personas — new **awareness-stage framework** to combine with current targeting [U0AB49S6806 7:48][7:57]. U0ACAB6GNN4 expects it to be a "game changer" once refined [8:17].

## Action items

1. **U0ACAB6GNN4** — contact Clay support to clarify why job-change signals aren't detected in people segment [7:20]. Status: open.
2. **U0AB49S6806 (Leo)** — develop and present the new awareness-stage framework for U0ACAB6GNN4 to integrate [8:34]. Status: open.

## Risks / flags

- Clay job-change signal non-detection blocks people-level job-change targeting (ties into PhantomBuster "Current Customers Job Changes" automation) — external (Clay), unverified until support responds.
- Web-visit signals company-level only caps path filtering precision — external tool limitation.
- Conflicting with repo AGENTS.md: CloverDX is **repo-only** task tracking (no ClickUp sync). See flag in digest.

Source: `~/gtm-studios/inbox/slack-huddles/20260924_132507__headphones__Huddle_notes__24_09_2026_in___C0ABLAVBVDJ_.html` (canvas). Huddle: `https://gtmstudios.slack.com/archives/C0ABLAVBVDJ/p1790255723991829`.
