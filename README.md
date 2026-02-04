# Daggerheart Hex Crawl

Daily hex crawl content for [Daggerheart](https://darringtonpress.com/daggerheart/) TTRPG, auto-generated and posted to Discord.

**Campaign:** Beast Feast (Monster Hunter meets Delicious in Dungeon)
**Setting:** The Plover Caves - Southern Depths

## Hex JSON Schema

Each hex is stored as a Markdown file with YAML front matter in `_hexes/`. The schema follows Daggerheart rules:

```yaml
---
hex_id: "001"                    # Unique identifier (zero-padded numeric)
title: "The Scorched Hollow"     # Display name
terrain_type: "lava tubes"       # Environment type
region: "The Bitter Depths"      # Southern Depths region

environment:                     # Daggerheart environment stat block
  name: "The Scorched Hollow"
  tier: 2                        # 1-4 (matches party level range)
  type: "Traversal"              # Exploration | Social | Traversal | Event
  description: "One evocative sentence."
  impulses:                      # What the environment "wants" to do
    - "Vent pressure through steam eruptions"
    - "Collapse unstable passages"
  difficulty: 14                 # Tier-based: T1=11, T2=14, T3=17, T4=20
  potential_adversaries:
    - "Ember Wurm"
    - "Magma Crawler"
  features:                      # Ordered: Passive, Action, Reaction
    - name: "Feature Name"
      type: "Passive"            # Passive | Action | Reaction
      fear_cost: null            # null or 1-3 for Action features
      description: "Mechanical effect."
      questions:                 # GM inspiration prompts
        - "Question for the GM?"

encounters:                      # Random encounters with Fear/Hope outcomes
  - name: "Encounter Name"
    fear: "What happens on Fear result"
    hope: "What happens on Hope result"

factions:                        # Groups with presence in this hex
  - name: "Faction Name"
    description: "Their goals and activities here"

points_of_interest:              # Notable locations
  - "Description of location"

npcs:                            # Important characters
  - name: "NPC Name"
    role: "Their role"
    description: "Brief description"

adventure_sites:                 # Potential adventure locations
  - name: "Site Name"
    description: "What makes this interesting"

tags:                            # Searchable tags
  - "tier-2"
  - "traversal"

created_at: "2026-02-03"         # ISO date
---
```

## Southern Depths Regions

- **The Jasmine Reaches** - Fragrant fungal gardens
- **The Bitter Depths** - Toxic, acidic environments
- **The Forgotten Vaults** - Ancient storage and ruins
- **The Descent Shafts** - Vertical passages, climbing hazards
- **The Titan's Tomb** - Massive skeletal remains, bone structures
- **Halfway Station** - Settlement and trading post
- **The Great Descent** - Main thoroughfare downward
- **The Weeping Gallery** - Water features, underground streams
- **The Bone Gardens** - Ossuary-like, necromantic energy

## Daggerheart Environment Rules

### Tiers and Difficulty
| Tier | Levels | Base Difficulty | Damage Range |
|------|--------|-----------------|--------------|
| 1 | 1 | 10-11 | 1d6+1 to 1d8+3 |
| 2 | 2-4 | 13-14 | 2d6+3 to 2d10+2 |
| 3 | 5-7 | 16-17 | 3d8+3 to 3d10+1 |
| 4 | 8-10 | 19-20 | 4d8+3 to 4d10+10 |

### Environment Types
- **Exploration**: Mystery, discovery, investigation
- **Social**: Interpersonal challenges, negotiations
- **Traversal**: Physical obstacles, movement hazards
- **Event**: Dramatic occurrences, battles, disasters

### Feature Types (must appear in this order)
1. **Passive**: Always active, no cost
2. **Action**: GM uses on their turn, may cost Fear (1-3)
3. **Reaction**: Triggered by PC actions

## Project Structure

```
daggerheart-hexcrawl/
├── _config.yml          # Jekyll configuration
├── _layouts/
│   ├── default.html     # Base layout
│   └── hex.html         # Individual hex page layout
├── _hexes/              # Hex content files
│   └── 001-the-scorched-hollow.md
├── assets/css/
│   └── style.css        # Daggerheart-themed styling
├── n8n/                 # n8n workflow exports
│   ├── hex-generator-workflow.json
│   └── environment-generator-workflow.json
├── index.html           # Hex index page
└── README.md
```

## n8n Workflows

### Hex Generator (`n8n/hex-generator-workflow.json`)
Main workflow that generates complete hexes:
- Accepts optional prompt, region, terrain, tier parameters
- Queries GitHub for next hex ID
- Uses AI agent with environment generation tool
- Outputs validated JSON

### Environment Generator (`n8n/environment-generator-workflow.json`)
Sub-workflow called as a tool:
- Generates Daggerheart-compliant environment stat blocks
- Validates feature structure and ordering
- Returns structured JSON

**Setup:**
1. Import both workflows into n8n
2. Update credential IDs for GitHub and OpenAI
3. Configure the Environment Generator as a tool in the main workflow

## Local Development

```bash
gem install bundler jekyll
bundle exec jekyll serve
```

## License

Hex content is original creative work. Daggerheart is a trademark of Darrington Press.
