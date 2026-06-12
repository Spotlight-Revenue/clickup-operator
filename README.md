# ClickUp Operator

ClickUp Operator is a reusable skill package for routing ClickUp ideas, to-dos, and project work with clean operator defaults and minimal back-and-forth.

This package is structured as one shared skill core with two runtime-specific install lanes:

- OpenClaw / ClawHub
- Claude Code

## Current release

This package is live on ClawHub and GitHub as the first public release of ClickUp Operator.

Core routing behavior was validated against a live ClickUp setup during packaging, and the repo is structured for both OpenClaw / ClawHub and Claude Code install paths.

## Folder layout

```text
clickup-operator/
├── README.md
├── SKILL.md
├── core/
│   ├── SKILL.md
│   ├── examples/
│   ├── references/
│   └── templates/
├── openclaw/
│   ├── README.md
│   └── skills/
│       └── clickup-operator/
│           ├── SKILL.md
│           └── agents/
├── claude-code/
│   ├── README.md
│   └── .claude/
│       ├── CLAUDE.md
│       └── skills/
│           └── clickup-operator/
│               └── SKILL.md
└── maintainer/
    ├── README.md
    ├── references/
    └── validation/
```

## What lives where

`core/`

- portable operator logic
- routing rules
- setup behavior
- portable templates
- reusable examples

`openclaw/`

- OpenClaw / ClawHub install shape
- OpenClaw-specific wrapper entrypoint
- OpenClaw agent metadata

`claude-code/`

- Claude Code install shape
- Claude-specific wrapper entrypoint
- optional `CLAUDE.md` helper note

`maintainer/`

- internal install notes
- public packaging notes
- validation and smoke-test material

## Quick install lanes

For OpenClaw / ClawHub, start in [openclaw/README.md](openclaw/README.md).

For Claude Code, start in [claude-code/README.md](claude-code/README.md).

For the shared skill logic, start in [core/SKILL.md](core/SKILL.md).
