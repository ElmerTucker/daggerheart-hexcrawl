---
hex_id: "013"
title: "Molten Reliquary Passages"
terrain_type: "lava tubes"
region: "The Forgotten Vaults"

environment:
  name: "Molten Reliquary Passages"
  tier: 3
  type: "Exploration"
  description: "Ancient lava-scarred tunnels wind through forgotten vaults, flickering with geothermal light and haunted by echoes of lost civilizations."
  impulses:
    - "Conceal hidden details"
    - "Encourage curious investigation"
  difficulty: 11
  potential_adversaries:
    - "Wandering animal"
    - "Cautious traveler"
  features:
    - name: "Unremarkable Ground"
      type: "Passive"
      fear_cost: null
      description: "All Investigation rolls are made with one fewer die unless time is taken to carefully search."
      questions:
        - "What is overlooked at first glance?"
        - "How does the environment mask important information?"
    - name: "Fleeting Glimpse"
      type: "Action"
      fear_cost: 1
      description: "A shadow, movement, or brief anomaly draws attention, prompting a Presence roll (Difficulty 11) to notice or interpret it; on a failure, the opportunity is missed."
      questions:
        - "What passes by unnoticed unless someone is watching closely?"
        - "How does this fleeting clue change the party's perception of the area?"
    - name: "Hidden Obstacle"
      type: "Reaction"
      fear_cost: null
      description: "When a PC moves quickly or without caution, reveal a minor hazard (such as loose stones or tangled roots) requiring an Agility roll (Difficulty 11) to avoid stumbling."
      questions:
        - "What subtle hazards does the environment conceal?"
        - "What does a stumble here reveal or disrupt?"

encounters:
  - name: "Vault Stalker Ambush"
    fear: "A pack of obsidian-scaled predators erupts from shadowed fissures, forcing the party into a desperate battle or a perilous retreat."
    hope: "The party spots the telltale heat shimmer of the stalkers in time, setting a clever trap or harvesting rare stalker glands prized for fire-resistant oils."

factions:
  - name: "The Emberbound"
    description: "A reclusive guild of fire-mage scavengers, seeking relics and geothermal energy sources in the ancient vaults, wary of intruders and fiercely territorial."

points_of_interest:
  - "A partially-collapsed reliquary studded with cooling magma and ancient, heat-warped artifacts"

npcs:
  - name: "Master Zevius"
    role: "Emberbound Relic-Seeker"
    description: "A wiry, heat-scarred elf obsessed with restoring lost magitech, willing to barter or sabotage rivals."

adventure_sites:
  - name: "The Fumarole Archives"
    description: "A hidden chamber where geothermal vents keep ancient scrolls petrified in crystal, guarded by unstable steam traps and cryptic mechanisms."

tags:
  - "lava"
  - "ruins"
  - "predators"
  - "ancient tech"
  - "magical hazards"

created_at: "2026-02-04"
---
