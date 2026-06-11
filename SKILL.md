---
name: clickup-operator
description: Route ClickUp ideas, to-dos, and project work with operator-style defaults. Use when the user wants tasks or ideas created, moved, assigned, due-dated, promoted into project lists, or read back from ClickUp without unnecessary confirmation.
---

# ClickUp Operator

This root entrypoint exists so the package remains directly usable while also exposing the dual-runtime packaging layout.

## Package shape

- Shared runtime logic lives in [core/SKILL.md](core/SKILL.md).
- OpenClaw-specific wrapper files live in [openclaw/](openclaw/README.md).
- Claude Code-specific wrapper files live in [claude-code/](claude-code/README.md).
- Maintainer-only packaging and validation docs live in [maintainer/](maintainer/README.md).

## Runtime behavior

For actual skill behavior, read and follow [core/SKILL.md](core/SKILL.md).

If this package is being installed into a specific runtime:

- OpenClaw / ClawHub should use the wrapper in [openclaw/skills/clickup-operator/SKILL.md](openclaw/skills/clickup-operator/SKILL.md).
- Claude Code should use the wrapper in [claude-code/.claude/skills/clickup-operator/SKILL.md](claude-code/.claude/skills/clickup-operator/SKILL.md).
