# AGENTS.md

This repository contains a Codex-compatible skill at:

- `skills/ljg-xray-paper/SKILL.md`

## Scope

- Keep the analytical behavior in `skills/ljg-xray-paper/SKILL.md` unchanged unless explicitly requested.
- Codex adaptation should be done through metadata and packaging files (for example, `agents/openai.yaml` and repository docs).

## Structure

- `skills/ljg-xray-paper/SKILL.md`: skill prompt and execution logic.
- `skills/ljg-xray-paper/agents/openai.yaml`: Codex UI metadata.
- `.claude-plugin/*`: legacy Claude plugin metadata retained for backward compatibility.
