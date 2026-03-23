# Claw Machine Catalog

Curated skills and tools for [Claw Machine](https://github.com/rob-linton/clawmachine).

## How It Works

This repo serves as the default catalog for Claw Machine. When configured, the system auto-syncs skills and tools from this repo on startup.

### Setup

In Claw Machine Settings, set **Catalog URL** to:
```
https://raw.githubusercontent.com/rob-linton/claw-catalog/main/catalog.json
```

Then click **Sync Catalog** or restart the API server.

## Available Skills

| ID | Name | Description |
|----|------|-------------|
| `create-skill` | Create Agent Skill | Creates new Agent Skills following the agentskills.io specification |

## Available Tools

| ID | Name | Description |
|----|------|-------------|
| `gh-cli` | GitHub CLI | GitHub CLI for repo operations and API access |

## Contributing

To add a skill or tool:

1. Create a directory under `skills/` or `tools/`
2. Add the required files (`SKILL.md` + `manifest.json` for skills, `TOOL.json` + `manifest.json` for tools)
3. Update `catalog.json` with the new entry
4. Submit a PR

See [SKILL-FORMAT.md](https://github.com/rob-linton/clawmachine/blob/main/Documents/SKILL-FORMAT.md) and [TOOL-FORMAT.md](https://github.com/rob-linton/clawmachine/blob/main/Documents/TOOL-FORMAT.md) for package format specifications.
