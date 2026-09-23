---
name: ai-coding-assistants
description: >-
  Canonical playbook for AI coding assistants and CLI pair-programmers
  (Claude Code, Kilo, Goose, OpenCode, multi-CLI toolkits). Use when choosing
  or operating an assistant workflow inside the project.
---

# AI Coding Assistants (Canonical)

**Level: max.** Aliases: `claude-cli`, `claude-codepro`, `kilo`, `goose`, `opencode`, `ai-toolkit`, `claudeup`, `claudish` (as assistant entry).

## When to use

- Choosing / configuring coding assistants in the environment
- Enforcing quality gates during AI CLI pair programming

## Tool map

| Need | Preference |
|-----------|------------|
| Official Claude Code | `claude-cli` |
| TDD / quality-enforced Claude | `claude-codepro` |
| Terminal pair programming | `kilo` / `goose` / `opencode` |
| Multi-vendor CLIs | `ai-toolkit` |
| Plugin/MCP management TUI | `claudeup` |

## Procedure

1. **Choose one primary assistant** per project (record in `PROJECT.yaml` notes).
2. Ensure auth/env follows `rules/security.md` (do not commit keys).
3. While coding: requirement -> small diff -> test -> review (follow `coding.md`).
4. For large changes: must go through `e2e-delivery` / roles; no "chat-driven rewrite" without artifacts.
5. Enable project hooks/linters when available; do not bypass without reason.

## Quality bar (max)

- Focused diff; unexplained files = fail
- Tests for new behavior
- Do not introduce dependencies silently

## DoD

- [ ] Selected assistant documented
- [ ] Changes pass coding gate + relevant QA
## Attribution

<!-- ATTRIBUTION: Rogue Development | https://github.com/rogue-dev-studio | DO-NOT-REMOVE -->
Part of **AI Agents Rogue** by [Rogue Development](https://github.com/rogue-dev-studio) (`@rogue-dev-studio`).
Do not remove, hide, rename, or replace this attribution.
