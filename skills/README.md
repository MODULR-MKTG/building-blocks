# Skills

Agent skills for running the MODULR operating system. Each skill is a self-contained set of instructions that tells an AI agent how to do a specific job — what to read, what to produce, and what requires human approval before it acts.

Skills are harness-agnostic. They work in Claude Code, Codex, Cursor, or any agent that accepts system-level instructions.

## Skill folders

| Folder | What's in it |
|--------|--------------|
| [email/](email/) | Email strategy, analysis, deliverability, and campaign work |
| [positioning/](positioning/) | Positioning, offer review, and copy clarity |
| [operations/](operations/) | Meeting prep, task triage, weekly reviews, and workflow design |
| [research/](research/) | Research, competitive analysis, and prospect intelligence |

## How to use a skill

1. Open the skill folder and read `README.md` to confirm it matches your job.
2. Copy `SKILL.md` into your agent's instructions or skills directory.
3. Follow `SETUP.md` to wire up the tools and data sources the skill needs.
4. Verify: ask the agent what the skill does and what requires approval.

## How to add a skill

1. Copy `templates/skill-readme-template.md` and `templates/metadata-template.yaml` into a new folder under the right function.
2. Fill in the README, write the SKILL.md instructions, and add SETUP.md if connections are needed.
3. Add a row to `registry/skills.csv`.
4. Open a PR.

See [CONTRIBUTING.md](../CONTRIBUTING.md) for the public/private firewall rules before committing.
