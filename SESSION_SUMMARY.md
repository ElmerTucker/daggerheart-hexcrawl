# Daggerheart Hexcrawl - Session Summary

## What We've Built

### GitHub Infrastructure (Complete)
- **Repo:** https://github.com/ElmerTucker/daggerheart-hexcrawl
- **Live Site:** https://elmertucker.github.io/daggerheart-hexcrawl/
- Jekyll-based GitHub Pages site with Daggerheart-themed styling
- Hex layout template rendering all schema fields correctly
- Sample hex: The Scorched Hollow (demonstrates full schema)

### Schema (Complete)
Corrected to match actual Daggerheart rules:
- Environment stat blocks with: name, tier, type, description, impulses, difficulty, potential_adversaries, features
- Features have: name, type (Passive/Action/Reaction), fear_cost, description, questions
- Hex includes: environment, encounters (Fear/Hope), factions, points_of_interest, npcs, adventure_sites, tags

### n8n Workflows (In Progress - Need Fixing)
Two workflow JSON files in `/n8n/` directory:
- `hex-generator-workflow.json` - Main workflow
- `environment-generator-workflow.json` - Sub-workflow for environment stat blocks

**Problem:** The exported JSON doesn't match your n8n version's node schemas. Nodes show up broken when imported.

**Solution in progress:** Setting up n8n MCP server so Claude can build workflows directly in your n8n instance.

## Issue Tracker Status

| Issue | Title | Status |
|-------|-------|--------|
| #1 | Create hex crawl GitHub repo + GitHub Pages site | ✅ Closed |
| #2 | Design n8n agentic workflow for hex generation | 🔄 In Progress |
| #3 | Build n8n GitHub + Discord posting pipeline | ⏳ Blocked by #2 |
| #4 | Add search and vector DB integration | ⏳ Future |
| #5 | Refine hex schema based on Daggerheart source | ✅ Done (merged into #2 work) |

## Campaign Context (Beast Feast)

- Monster Hunter meets Delicious in Dungeon
- Setting: Plover Caves / Southern Depths
- Regions: The Jasmine Reaches, The Bitter Depths, The Forgotten Vaults, The Descent Shafts, The Titan's Tomb, Halfway Station, The Great Descent, The Weeping Gallery, The Bone Gardens

## Daggerheart Environment Generation Guide

You provided a detailed guide for environment stat blocks. Key points:
- Tiers 1-4 with matching difficulties (11/14/17/20)
- Types: Exploration, Social, Traversal, Event
- Features ordered: Passive → Action → Reaction
- Each feature must have GM inspiration questions
- Fear costs only on impactful Action features

The full guide is embedded in the workflow JSON system prompts.

## Next Steps

1. **Restart Claude Code** to activate the n8n MCP server
2. **Resume this conversation** by saying:
   ```
   Continue working on the daggerheart-hexcrawl project. We were setting up n8n
   workflows for hex generation. The n8n MCP should now be connected. Please use
   it to build the Environment Generator workflow directly in my n8n instance.
   ```
3. **After workflows are built:**
   - Test the environment generator
   - Test the full hex generator
   - Move on to Issue #3 (GitHub + Discord posting)

## Key Files

```
/home/elmer/daggerheart-hexcrawl/
├── _config.yml                 # Jekyll config
├── _layouts/
│   ├── default.html
│   └── hex.html                # Hex page template (updated for correct schema)
├── _hexes/
│   └── 001-the-scorched-hollow.md  # Sample hex (updated schema)
├── assets/css/style.css        # Daggerheart theme CSS
├── index.html                  # Hex index page
├── README.md                   # Schema documentation
├── n8n/
│   ├── hex-generator-workflow.json         # Main workflow (needs rebuild)
│   └── environment-generator-workflow.json # Sub-workflow (needs rebuild)
└── SESSION_SUMMARY.md          # This file
```

## MCP Configuration

Added to `~/.claude/settings.json`:
```json
{
  "mcpServers": {
    "n8n": {
      "command": "npx",
      "args": ["n8n-mcp"],
      "env": {
        "MCP_MODE": "stdio",
        "N8N_API_URL": "https://n8n.elmertucker.space",
        "N8N_API_KEY": "[configured]"
      }
    }
  }
}
```

## Workflow Architecture (To Build)

```
┌─────────────────┐
│  Manual Trigger │ ← Optional: prompt, region, terrain, tier
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Set Defaults   │ ← Random region/tier if not provided
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Get Next Hex   │ ← Query GitHub for highest existing hex ID
│  ID from GitHub │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│   AI Agent      │ ← GPT-4.1 with Beast Feast context
│   (OpenAI)      │
│                 │ ── Tool: Generate Environment (sub-workflow)
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Validate JSON  │ ← Ensure schema compliance
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Output         │ ← Ready for Issue #3 (GitHub + Discord)
└─────────────────┘
```
