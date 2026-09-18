# {CLIENT NAME} — engagement repo

Canonical source of truth for the {CLIENT NAME} GTM engagement.

Read `AGENTS.md` before working in here — it defines how to ingest communications,
log decisions, and answer questions about this account.

- `communications/` — client + internal comms (calls, emails, Slack)
- `decisions.md` — append-only log of material decisions
- `icp/` — client-confirmed targeting facts (statement of truth)
- `gtm-studios-work/` — lead lists, handover docs, scraper runs
- `onboarding/` — signed SoW + onboarding material
- `session-context/` — AI-session records

Ingestion writes into `communications/` and `decisions.md` via the GTM Studios
pipeline (Krisp/Meet calls, Slack sweep, Gmail). See `~/gtm-studios/agent/systems.md`.

---

## Template bootstrap

This repo was created from the GTM Studios **client engagement template** (derived
from the OV engagement, which defined the canonical structure). To bring it online:

1. Fill in `client-context.md` (who they are, what they sell, ICP shape, key contacts).
2. Fill in `status.md` current state and `ACTION-ITEMS.md` open work.
3. Fill the `Configuration` section at the bottom of `AGENTS.md` (Slack channels,
   email scope, ClickUp IDs) with this client's real identifiers.
4. Replace every `{CLIENT ...}` placeholder below the filename.
5. Point ingestion at this repo (Krisp webhook, Slack sweep, Gmail scope) per
   `~/gtm-studios/agent/systems.md`.
6. Delete this bootstrap section.
