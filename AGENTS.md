# AGENTS.md

Operating manual for any AI agent working in this repository.

## Project Manager role

When asked to act as project manager for this engagement (or when new content has landed in `communications/`), do the following:

1. **Read the new content** — calls, Slack threads, or emails under `communications/client/` or `communications/internal/`.
2. **Extract** action items (who owns what, by when if stated), decisions made, and open questions/risks.
3. **Log decisions** in `decisions.md` (append at the bottom, chronological — never rewrite an existing entry).
4. **Update ICP files** in `icp/` only if the new content adds a genuinely client-confirmed fact — see the statement-of-truth rule in `icp/README.md`. Don't touch them for GTM's own analysis or hypotheses.
5. **Flag, don't decide.** If something is ambiguous or consequential, surface it rather than resolving it silently.

**Execution: manual only.** This role runs when invoked in a session — there is no scheduled/autonomous routine processing this repo on its own. Nothing here is running unattended.

**Task tracking: repo-only.** This role keeps `decisions.md` and the repo's own files current. It does not create, update, or sync tasks in ClickUp or any other external tracker. The ClickUp reference below is for context only.

## Answering questions about this engagement

**Search before you answer.** Never answer from memory, from `client-context.md` alone, or from what a previous session left in context. `client-context.md` and `decisions.md` are summaries — the underlying facts live in the communications and ICP files, and those are more current. Read the actual files.

**Sweep every folder that could hold the answer**, not just the first one that looks right:

| Folder | What's in it |
|---|---|
| `client-context.md` | Who the client is, what they sell, their verticals — orientation, not a citable source |
| `decisions.md` | Chronological log of material decisions, each with its own source pointer |
| `communications/client/` | `calls/`, `emails/`, `slack/` — anything from the client. **The only place client-confirmed facts originate.** |
| `communications/internal/` | `slack/`, `slack-huddle/`, `calls/` — GTM Studios only: our reasoning, QA findings, tooling decisions |
| `icp/<vertical>/icp.md` | Client-confirmed targeting facts only (statement of truth — see `icp/README.md`) |
| `icp/<vertical>/` (other files) | GTM-authored: qualification logic, Peter Parker prompts, sourcing channels, enrichment specs, segment breakdowns |
| `gtm-studios-work/lead-lists/` | The lists we produced |
| `gtm-studios-work/handover-documents/` | What Leo hands to the GTM engineer |
| `gtm-studios-work/peter-parker-runs/` | Scraper runs — inputs, prompt as run, results, data-quality warnings |
| `onboarding/pre-sales/` | Discovery, demo and scoping transcripts from before the deal closed |
| `onboarding/onboarding-documentation/` | Kickoff-onward material — strategy, verticals detail, lead scoring |
| `onboarding/statement-of-work/` | Signed SoW and amendments — the contractual scope |
| `session-context/` | What previous AI sessions did, and what they left open |

Minimum sweep for any substantive question: `decisions.md`, **both** sides of `communications/`, and the relevant `icp/<vertical>/` folder. Add `onboarding/` for anything touching original scope or commercials, and `gtm-studios-work/` for anything about lists, runs, or data quality.

Files are date-prefixed (`YYYY-MM-DD-`). **Read newest-first, and say so when a later file supersedes an earlier one** — a client instruction from September overrides the same topic from August.

## Referencing facts in answers

Every factual claim carries its source inline, as a repo-relative path in backticks — the convention `decisions.md` already uses:

> <client contact> approved the shortlist apart from two exclusions (`communications/client/slack/YYYY-MM-DD-<topic>.md`).

- **Quote the client verbatim** where their exact wording carries the decision. Paraphrase drifts — a close-name match on a targeted list vs. a genuinely different company is precisely this failure mode.
- **Label whose fact it is:** client-confirmed (from `communications/client/` or an `icp.md`) vs. GTM-authored (everything else). Never let our hypothesis read as their instruction.
- **Say "not in the repo"** when it isn't there. An uncited claim is a guess, and a guess stated as fact here ends up in a client deliverable. If the sweep comes up empty, say so and flag it as a question for the client.
- **Flag contradictions instead of picking a winner** — surface both sources with their dates and let Leo resolve it.

## Citing is not verifying

**A citation proves a claim was written down before. It says nothing about whether the claim is true.** This distinction has already caused one real error: a market/partner relationship was described in a sourcing-channels file as "an actual browsable directory," correctly labelled as GTM research, and cited correctly into a client-facing handover sheet. It was a **vendor** marketplace. The citation rule above passed it cleanly.

So, on top of citing:

- **Client facts are checkable; GTM research is not.** A client fact carries a speaker, a date, and a verbatim quote — three ways to test it. A GTM-authored claim about the outside world (a directory exists, a tool behaves a certain way, a company is of a certain type) carries none of that. **Treat every such claim as unverified until it says otherwise.**
- **Stamp external claims when you write them:** `*(verified <date>, <how>)*` or `*(unverified — not yet checked)*`. Without a stamp, assume unverified.
- **Never increase confidence when copying a claim between files.** If the source says "worth checking," the destination says "worth checking" — not "best available." Each hop must preserve the hedge or add new evidence to justify dropping it. Silent confidence inflation across two or three hops turns a maybe into a fact with nobody having checked anything.
- **Verify before promoting into a deliverable.** Anything leaving this repo — a handover sheet, a client document, a brief — must have its GTM-authored external claims checked first, not merely cited. Inside the repo, an unverified note is fine if labelled. In a deliverable someone will act on, it is not.
- **When a claim turns out to be wrong, fix it at the source too**, not only in the document where it surfaced. Otherwise the next person inherits it again.

**⚠ Known structural weakness.** `icp/README.md` declares the whole folder a client-only statement of truth with "a single `icp.md`" per vertical, but a vertical folder may hold GTM-authored files alongside `icp.md` (qualification logic, sourcing channels, prompts, enrichment specs). Each declares its own status in its header, so the boundary holds only as long as you read headers — and headers don't travel with a quoted claim. **Check the header of any file in `icp/` before treating its contents as client fact; folder location is not the signal here.**

## Configuration — sources this role reads from

**Slack channels:**
- Internal (GTM Studios + CloverDX BD): `#cloverdx-internal`, Channel ID `C0ABLAVBVDJ` *(from routing.json / digest)*
- External (client): Channel ID `C0AFQ85E1AB` *(from Leo; client-side, Kate Pidgeon et al.)*

**Email:**
- Inbox: Leo's Gmail (`leo@gotomarketstudios.com`)
- Scope: threads with `@cloverdx.com` counterparts
- Excludes pure scheduling/calendar-acceptance emails and auto-replies unless they carry a substantive decision or action item

**ClickUp (reference only, not synced to):**
- Workspace ID: `90152153946`
- Space: "CloverDX" (Space ID `90159041715`) — one space, **multiple department lists**:
  - List: "Original Project" (Kate & Jake's) — List ID `901519248410`
  - List: "Intel 360" (Pavel's) — List ID `901524267426`
  - List: "New Business Team Project" (Ross's) — List ID `901524267505`

*These identifiers carry over from the prior repo for this same engagement — confirm they're still current if anything's changed since.*
