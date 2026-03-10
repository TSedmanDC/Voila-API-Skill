# Voila API Claude Code Plugin

A comprehensive guide and toolset for integrating with the Voila API (by The Despatch Company). This plugin provides Claude with full knowledge of Voila's REST schemas, shipment flows, and courier management.

## Features

- **Full API Documentation:** Exhaustive schemas for labeling, tracking, pricing, and webhooks.
- **Smart Shipping Flows:** Guidance on automating courier selection.
- **Bundled Scripts:** Node.js and Python scripts for listing couriers and getting specifics.

## API Configuration

- **Base URL:** `https://app.heyvoila.io`

## Installation

### For Claude Code

To use this as a plugin in Claude Code:

1. **Local Development Mode:**
   Run Claude Code pointing to the plugin root directory:
   ```bash
   claude --plugin-dir /path/to/plugin-root
   ```

2. **Permanent Installation:**
   Copy the contents of this folder into your Claude Code plugins directory (usually `~/.claude/plugins/voila-api`).

3. **Usage:**
   Once loaded, you can ask Claude about Voila API endpoints or use the namespaced skill:
   ```text
   /voila-api:help
   ```

### For Cursor

To use this as a skill in Cursor:

1. **Copy Skill Folder:**
   Copy the `skills/voila-api` folder into your project's `.cursor/skills` directory.

2. **Verify Detection:**
   Ensure the skill is detected in **Cursor Settings** > **Rules, Skills, Subagents** > **Skills**. Once detected, Cursor will have access to the Voila API knowledge.

## Directory Structure

```text
.
├── .claude-plugin/     # Plugin metadata
│   └── plugin.json
├── skills/
│   └── voila-api/     # Main skill content
│       ├── SKILL.md    # Entry point & Overview
│       ├── endpoints/  # Detailed API route documentation
│       ├── scripts/    # Ready-to-use API scripts
│       └── evals/      # Test cases and assertions
└── README.md           # This file
```
