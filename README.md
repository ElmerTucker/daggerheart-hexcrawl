# Daggerheart Hex Crawl

Daily hex crawl content for [Daggerheart](https://darringtonpress.com/daggerheart/) TTRPG, auto-generated and posted to Discord.

## Hex JSON Schema

Each hex is stored as a Markdown file with YAML front matter in `_hexes/`. The schema supports all Daggerheart-specific mechanics:

```yaml
---
hex_id: "001"                    # Unique identifier (string for sorting flexibility)
title: "The Scorched Hollow"     # Display name
biome: "volcanic"                # Environment type (volcanic, forest, desert, swamp, mountain, coast, plains, tundra, urban)
tier: 1                          # Difficulty tier (1-4)
description: |                   # Full narrative description (markdown supported)
  Multi-paragraph description of the hex...

environment_stat_block:          # Daggerheart environment mechanics
  damage_thresholds:
    minor: 3
    major: 7
    severe: 12
  features:                      # Environmental features that affect gameplay
    - "Feature description"
  instincts:                     # How the environment "acts" during scenes
    - "Instinct description"

encounters:                      # Potential encounters with Fear/Hope outcomes
  - name: "Encounter Name"
    fear: "What happens on Fear result"
    hope: "What happens on Hope result"
    adversaries:                 # List of enemies (can be empty for social encounters)
      - "Enemy name"

npcs:                            # Notable NPCs in this hex
  - name: "NPC Name"
    role: "Their role/occupation"
    description: "Brief description"

loot:                            # Treasure and rewards
  domain: "Arcana"               # Daggerheart domain (Arcana, Blade, Bone, Codex, Grace, Midnight, Sage, Splendor, Valor)
  items:
    - "Item description"

landmarks:                       # Notable locations within the hex
  - "Landmark description"

travel_hazards:                  # Dangers when traveling through
  - "Hazard description"

community_ties:                  # Connections to factions, settlements, organizations
  - "Connection description"

connections: []                  # Links to adjacent hexes (populated by future vector search)

tags:                            # Searchable tags
  - "tag-name"

created_at: "2026-02-03"         # ISO date string
---
```

## Project Structure

```
daggerheart-hexcrawl/
├── _config.yml          # Jekyll configuration
├── _layouts/
│   ├── default.html     # Base layout
│   └── hex.html         # Individual hex page layout
├── _hexes/              # Hex content files (Markdown with YAML front matter)
│   └── 001-the-scorched-hollow.md
├── assets/
│   └── css/
│       └── style.css    # Daggerheart-themed styling
├── index.html           # Hex index page
└── README.md
```

## Local Development

```bash
# Install Jekyll
gem install bundler jekyll

# Serve locally
bundle exec jekyll serve

# Build for production
bundle exec jekyll build
```

## Adding New Hexes

1. Create a new file in `_hexes/` named `{hex_id}-{slug}.md`
2. Add YAML front matter following the schema above
3. Commit and push—GitHub Pages will rebuild automatically

## Automation

This repo is designed to receive automated commits from an n8n workflow that:
1. Generates hex content using an AI agent
2. Commits the hex JSON to this repo
3. Posts a Discord webhook with the hex summary and link

See issues #2 and #3 for workflow implementation details.

## License

Hex content is original creative work. Daggerheart is a trademark of Darrington Press.
