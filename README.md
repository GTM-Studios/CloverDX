# CloverDX — engagement repo

Canonical source of truth for the CloverDX GTM engagement.

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
