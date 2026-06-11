# Claude Code Lane

This folder contains the Claude Code-facing wrapper for ClickUp Operator.

## Install target

Copy the `.claude/` contents into the target project or user Claude Code environment.

Expected runtime entrypoint:

- `.claude/skills/clickup-operator/SKILL.md`

## Claude Code model

- `CLAUDE.md` is for persistent context and project-level instructions.
- `SKILL.md` is for reusable procedures and capabilities that Claude loads when relevant.

This package uses that split directly:

- `.claude/skills/clickup-operator/SKILL.md` is the reusable skill entrypoint
- `.claude/CLAUDE.md` is an optional helper note showing how a project might reference the skill

## Notes

- The actual reusable skill logic lives in [../core/SKILL.md](../core/SKILL.md).
- Maintainer-only validation and internal packaging notes live in [../maintainer/README.md](../maintainer/README.md).
