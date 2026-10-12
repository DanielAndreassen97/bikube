# AGENTS.md

Drovr: A macOS kanban board where every card is a live terminal, for running many coding agents side by side.

Built with Software Factory's workflow: read `docs/agents/workflow.md` before starting on an item, and `docs/agents/stack.md` for the stack picked at creation and its guidelines. Domain terms are in `CONTEXT.md`, decisions in `docs/adr/`.

Not scaffolded yet. The first item (v1) sets the stack up with the `bootstrap` skill, and then:
- fills in `.claude/check.sh` with everything that must be green
- adds `.github/workflows/ci.yml` with a job named `check` that runs `.claude/check.sh` (the rulesets require it)
- records the stack in `docs/adr/0001-stack.md` and the commands in this file

This file is for every coding agent; `CLAUDE.md` imports it.
