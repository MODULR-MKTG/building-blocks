# Install

## Claude Code / Codex

Copy this folder into your agent's skills directory. In Claude Code, add the `SKILL.md` contents to your project-level agent instructions or `.claude/skills/` folder.

## Cursor

Use the contents of `SKILL.md` as a Cursor rule or agent instruction.

## Any other agent harness

Copy `SKILL.md` into your system prompt, project instructions, or agent memory layer. The skill is harness-agnostic — it's just instructions.

## Verify

Ask the agent: *"What does this skill do, what inputs does it need, and what requires human approval before it acts?"*

If the agent can answer all three correctly, it's loaded.

## Connections

See `SETUP.md` for the specific tools, credentials, and data sources this skill needs to function. Most skills require at minimum:

- A source (email archive, CRM, calendar, task list)
- An output destination (Docs, Slack, or file)
- Any API keys listed in `SETUP.md`
