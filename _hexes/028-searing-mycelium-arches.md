---
hex_id: "028"
title: "Searing Mycelium Arches"
terrain_type: "lava tubes"
region: "The Jasmine Reaches"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript area filled with subtle details awaiting discovery."
  impulses:
    - "Conceal hidden elements"
    - "Encourage careful observation"
  difficulty: 11
  potential_adversaries:
    - "Wandering animal"
    - "Curious local"
  features:
    - name: "Subtle Details"
      type: "Passive"
      fear_cost: null
      description: "Characters searching this environment must succeed on an Investigation (Difficulty 11) to notice anything out of the ordinary."
      questions:
        - "What overlooked clue could change the party’s perspective?"
        - "How does the environment reward persistent observation?"
    - name: "Hidden Obstacle"
      type: "Action"
      fear_cost: 1
      description: "The GM may reveal a concealed hazard or trap, requiring a Reflex save (Difficulty 11) or the character takes 1d6+1 damage."
      questions:
        - "What unexpected danger lies just beneath the surface?"
        - "How can the environment foreshadow this hazard?"
    - name: "Echoes of Movement"
      type: "Reaction"
      fear_cost: null
      description: "When a character makes a loud noise, the environment reacts by drawing attention to their presence, potentially alerting adversaries."
      questions:
        - "Who or what notices the disturbance?"
        - "How does the environment amplify or muffle sounds?"

encounters:
  - name: "Lava Mycelial Behemoth"
    fear: "The creature attacks the party, its heated tendrils causing burning wounds and threatening to collapse sections of the tunnels."
    hope: "The party harvests rare fireproof fungal spores and a chunk of the Behemoth’s carapace—valuable for fire resistance potions or armor."

factions:
  - name: "Glowspore Foragers"
    description: "A small, cautious band of fungal gatherers seeking rare ingredients; they lay traps for monsters and rivals, fiercely guarding prime patches."

points_of_interest:
  - "Luminescent archways of heat-loving fungus, some edible, some dangerously toxic"

npcs:
  - name: "Tessa Fumehands"
    role: "Glowspore Forager Leader"
    description: "Wiry, soot-stained, and fiercely protective of her crew, she trades in exotic fungi and claims territory with cunning traps."

adventure_sites:
  - name: "The Ember Spore Bloom"
    description: "A cavern where rare fire-resistant mushrooms erupt in vibrant color—guarded by natural hazards and claimed by territorial creatures."

tags:
  - "foraging"
  - "fungus"
  - "heat"
  - "danger"
  - "rare-ingredients"

created_at: "2026-02-04"
---
