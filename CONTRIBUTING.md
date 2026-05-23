# Contributing & the public/private rule

This handbook is public. Most of it is maintained by AI agents working from MODULR's internal source of truth. Whether you're an agent or a human, **read this before adding or editing anything.**

## The one rule that matters: the firewall

This repo is the **public** half of MODULR. There is a **private** half (client work, our CRM, our numbers) that lives elsewhere and **must never cross into this repo.**

Before committing anything, ask: *does this name a client, expose client data, list a prospect, or show real money/comp?*

**If yes → it does NOT go here. Full stop.**

### Never commit to this repo

- ❌ **Client names** — not in examples, not in case studies, not in passing. Anonymize: "a founder-led education brand," "a SaaS client," "a RevOps engagement."
- ❌ **Client data** — their lists, metrics, emails, account IDs, portal numbers, anything they gave us.
- ❌ **Prospect / target lists** — who we're pitching is private.
- ❌ **Specific deal sizes or client retainer amounts** — our *published rates* (rack/floor) are fine; what a *specific client* pays is not.
- ❌ **Revenue, burn, or financial performance numbers**
- ❌ **Individual compensation**
- ❌ **Anything under an NDA**

### Fine to commit

- ✅ Methodology, frameworks, how we think
- ✅ Our positioning, values, POV
- ✅ Our published pricing (rack rate, floor)
- ✅ Our sales process and playbooks (the *method*, not the *targets*)
- ✅ Aggregate, anonymized proof stats we already use publicly
- ✅ How we work, how we're structured, what we believe

**When in doubt, leave it out.** It's far cheaper to omit something than to leak a client.

## How to make a change

1. Edit the relevant markdown file under `handbook/`.
2. Run the firewall check in your head (or grep — see below).
3. Commit with a clear message.
4. Open a PR if you're external; founders/agents with write access can push to `main`.

### A quick self-check before pushing

```bash
# From repo root — scans for the obvious leak categories.
# Update the client/prospect name list as the roster changes.
grep -rinE "CLIENT_NAME_1|CLIENT_NAME_2|PROSPECT_NAME" handbook/ && echo "⚠️  POSSIBLE LEAK — review before pushing" || echo "✅ clean"
```

(The real list of names to scan for lives in the private workspace, not here — because even the watchlist is a hint about who our clients are.)

## Style

- Plain markdown. One `#` H1 per file (the title).
- Keep it tight. We practice what we preach about anti-boring writing — see [Writing Rules](handbook/voice-and-style/writing-rules.md).
- Link between docs with relative paths.
