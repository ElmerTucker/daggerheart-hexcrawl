---
hex_id: "015"
title: "Glittering Spireways"
terrain_type: "crystal formation"
region: "The Great Descent"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript area filled with subtle details waiting to be noticed."
  impulses:
    - "Conceal small secrets"
    - "Encourage careful observation"
  difficulty: 11
  potential_adversaries:
    - "Curious onlooker"
    - "Hidden animal"
  features:
    - name: "Unremarkable Facade"
      type: "Passive"
      fear_cost: null
      description: "Checks to notice hidden objects or details are made at disadvantage."
      questions:
        - "What subtle clue hints at something more beneath the surface?"
        - "How does the environment mask its secrets?"
    - name: "Shifting Shadows"
      type: "Action"
      fear_cost: 1
      description: "Obscure a clue or pathway, increasing the difficulty of the next investigation or search roll by 2."
      questions:
        - "What causes the environment to shift unexpectedly?"
        - "How do the shadows mislead or distract the characters?"
    - name: "Revealing Glint"
      type: "Reaction"
      fear_cost: null
      description: "When a character fails a search or investigation roll, a fleeting detail appears, granting advantage on the next attempt by any character."
      questions:
        - "What accidental motion or change brings the detail to light?"
        - "How do the characters interpret this unexpected hint?"

encounters:
  - name: "Crystalback Skitterer Ambush"
    fear: "A pack of Crystalback Skitterers erupts from the facets, showering the bridge with razor shards and risking a deadly fall."
    hope: "The Skitterers are after the bright cave moths, not the party, leaving behind edible larvae and valuable carapace fragments."

factions:
  - name: "The Prism Guild"
    description: "Explorers and prospectors seeking rare crystals and minerals. They mark safe paths and collect samples, wary of damaging the spireways."

points_of_interest:
  - "Luminous Bridge: A natural crystal bridge that glows faintly, humming with magical resonance."

npcs:
  - name: "Delven Rusk"
    role: "Prism Guild Scout"
    description: "A wiry, bright-eyed scout mapping safe routes and cataloging edible cave flora, eager to trade information for supplies."

adventure_sites:
  - name: "Veiled Crevice"
    description: "A hidden fissure beneath the bridge, filled with bioluminescent fungi, rare insects, and signs of an ancient campsite."

tags:
  - "crystal"
  - "traversal"
  - "verticality"
  - "resource-rich"
  - "hazardous"

created_at: "2026-02-04"
---
