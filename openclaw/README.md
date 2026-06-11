# OpenClaw / ClawHub Lane

This folder contains the OpenClaw-facing wrapper for ClickUp Operator.

## Install target

Install the contents of `skills/clickup-operator/` into the target OpenClaw skills directory.

Expected runtime entrypoint:

- `skills/clickup-operator/SKILL.md`

## What this wrapper does

- exposes the ClickUp Operator skill to OpenClaw in a native skill shape
- preserves OpenClaw-compatible frontmatter and agent metadata
- delegates actual behavior to the shared core package

## Notes

- The actual reusable skill logic lives in [../core/SKILL.md](../core/SKILL.md).
- Maintainer-only validation and internal packaging notes live in [../maintainer/README.md](../maintainer/README.md).
