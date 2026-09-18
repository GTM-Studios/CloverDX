# icp/

**Statement of truth.** Everything in this folder must be a fact confirmed by the client — a direct quote or statement from a call, email, or Slack message. Nothing GTM-authored, assumed, or designed goes in here unless the client has explicitly agreed to it. If it's our own interpretation, hypothesis, or working design rather than something the client actually said, it does not belong in this folder.

**⚠ Known structural weakness.** A vertical folder can hold GTM-authored files alongside `icp.md` (qualification logic, sourcing channels, Peter Parker prompts, enrichment specs, segment breakdowns). Each declares its own status in its header, so the fact/design split is preserved *per file* — but not by folder location, which is what this README claims. This matters because a header doesn't travel with a claim once it's quoted elsewhere: a GTM research note read out of `icp/` can be mistaken for client fact (it already happened once — see `AGENTS.md`, "Citing is not verifying").

**Until resolved: read the header, don't trust the folder.**

One subfolder per active vertical (see `client-context.md`), each with a single `icp.md`:

- `EXAMPLE-VERTICAL/icp.md`
