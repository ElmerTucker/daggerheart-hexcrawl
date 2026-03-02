---
hex_id: "026"
title: "Smoldering Passage"
terrain_type: "lava tubes"
region: "The Descent Shafts"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript area, its details waiting to be uncovered by curious explorers."
  impulses:
    - "Conceal secrets within its ordinary surroundings"
    - "Encourage careful observation and interaction"
  difficulty: 11
  potential_adversaries:
    - "Wandering critter"
    - "Unseen observer"
  features:
    - name: "Unremarkable Facade"
      type: "Passive"
      fear_cost: null
      description: "All Investigation and Perception rolls to notice anything out of the ordinary are made with Disadvantage."
      questions:
        - "What subtle clue hints at something hidden?"
        - "How does the environment reward patient observation?"
    - name: "Hidden Detail"
      type: "Action"
      fear_cost: 1
      description: "The GM may reveal a minor secret, clue, or hidden object to a PC who interacts creatively with the scenery."
      questions:
        - "What discovery shifts the party’s understanding of this place?"
        - "How does the environment react to keen attention?"
    - name: "Fleeting Glimpse"
      type: "Reaction"
      fear_cost: null
      description: "When a PC fails an Investigation or Perception roll, they catch a brief glimpse or hear a faint sound that suggests there is more than meets the eye."
      questions:
        - "What ephemeral sign teases the presence of something more?"
        - "How might a failed roll still encourage further exploration?"

encounters:
  - name: "Molten Shellbacks"
    fear: "A cluster of lava-armored shellbacks emerges from a fissure, defending their territory with bursts of scalding steam and molten spit."
    hope: "Careful observation reveals the shellbacks are distracted by certain mineral fungi, allowing a clever party to bypass or harvest them for heat-resistant plates and rare ingredients."

factions:
  - name: "The Ember-Bound Cartel"
    description: "A small crew of scavengers harvesting rare minerals and glowing fungi for trade at Halfway Station, wary of intruders and territorial over profitable veins."

points_of_interest:
  - "A collapsed vent choked with luminescent, heat-loving fungi—the air shimmers with residual warmth."

npcs:
  - name: "Bramm Tindle"
    role: "Cartel Fungi Harvester"
    description: "A nervous, soot-stained dwarf constantly wiping sweat from his brow. Will trade fungal samples for water and news, but is quick to warn of heat hazards deeper in the tubes."

adventure_sites:
  - name: "Sulfurous Chamber"
    description: "A pocket of toxic gas and brittle crystals partially blocks the way; bypassing or harvesting its resources requires ingenuity and caution."

tags:
  - "hazardous terrain"
  - "resource-rich"
  - "faction presence"
  - "heat"
  - "fungi"

created_at: "2026-02-04"
---
