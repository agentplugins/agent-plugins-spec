# Agent Plugins

Agent Plugins is an open, vendor-neutral standard for packaging reusable components that extend AI agents into distributable plugins. The published 1.0 specification defines a portable package format for Agent Skills and MCP servers; the 1.1.0 working draft adds portable hooks.

This README is a non-normative introduction. The versioned specification defines the portable contract.

## Status

Agent Plugins Specification 1.0.0 is the current published release. Agent Plugins Specification 1.1.0 is a working draft.

## Quick Start

The smallest useful plugin is a directory with one skill:

```text
hello-plugin/
├── plugin.json
└── skills/
    └── greet/
        └── SKILL.md
```

In `plugin.json`:

```json
{
  "$schema": "https://agent-plugins.org/schemas/1.0.0/plugin.schema.json",
  "name": "hello-plugin"
}
```

In `skills/greet/SKILL.md`:

```markdown
---
name: greet
description: Greet the user and offer help.
---

Greet the user and offer help.
```

A client that supports skills can load the plugin by reading `plugin.json` and discovering `skills/greet/SKILL.md`. How the client exposes the skill to users or models is outside the Agent Plugins specification.

## Project Documents

- [Agent Plugins Specification 1.0.0](./spec/1.0.0.md)
- [1.0.0 schemas](./schemas/1.0.0/)
- [Agent Plugins Specification 1.1.0 (working draft)](./spec/1.1.0.md)
- [1.1.0 schemas](./schemas/1.1.0/)
- [Technical Charter](./GOVERNANCE.md)
- [Future considerations](./FUTURE_CONSIDERATIONS.md)
