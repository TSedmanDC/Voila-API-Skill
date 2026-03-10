# Voila API Claude Code Plugin

A comprehensive guide and toolset for integrating with the Voila API (by Despatch Cloud). This plugin provides Claude with full knowledge of Voila's REST schemas, shipment flows, and courier management.

## Features

- **Full API Documentation:** Exhaustive schemas for labeling, tracking, pricing, and webhooks.
- **Smart Shipping Flows:** Guidance on automating courier selection.
- **Bundled Scripts:** Node.js and Python scripts for listing couriers and getting specifics.
- **Playground Credentials:** Pre-configured for the Voila API playground.

## Installation

### For Claude Code

To use this as a plugin in Claude Code:

1. **Local Development Mode:**
   Run Claude Code pointing to this directory:
   ```bash
   claude --plugin-dir /path/to/Voila-API
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

1. **Direct Folder Reference:**
   You can reference this folder directly in your Cursor rules or by telling Cursor to "use the @Voila-API folder as a skill".

2. **Packaged Skill:**
   If you use the `skill-creator` tool, you can package this directory into a `.skill` file for easier distribution.

## API Configuration

- **Base URL:** `https://app.heyvoila.io`
- **Playground Credentials:**
  - `api-user`: `VoilaPlayground`
  - `api-token`: `vtkpuslqfrdhwbio`

## Directory Structure

```text
Voila-API/
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

## License

MIT
