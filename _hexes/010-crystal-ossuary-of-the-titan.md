---
hex_id: "010"
title: "Crystal Ossuary of the Titan"
terrain_type: "crystal formation"
region: "The Titan's Tomb"

environment:
  name: "Crystal Ossuary"
  tier: 3
  type: "Exploration"
  description: "Vast crystal formations grow among ancient titan bones, refracting eerie light and hiding both resources and threats."
  impulses:
    - "Reveal hidden dangers or treasures in the crystal lattice"
    - "Mask valuable resources behind refracted illusions"
  difficulty: 17
  potential_adversaries:
    - "Shardback Crystal Lizard"
    - "Spectral Bonekeeper"
    - "Titan Remnant Wraith"
  features:
    - name: "Refracting Maze"
      type: "Passive"
      fear_cost: null
      description: "Crystals scatter light in dazzling patterns, making navigation and perception challenging unless party members employ clever tactics or special equipment."
      questions:
        - "What hidden denizen moves unseen through the shifting lights?"
        - "How might light be manipulated to reveal a secret?"
    - name: "Bone-Locked Cache"
      type: "Action"
      fear_cost: 2
      description: "Buried among fossilized titan bones, rare crafting materials and edible crystal fungus can be harvested with effort and care."
      questions:
        - "What rare ingredient could be pried from the ancient marrow?"
        - "Who else seeks these resources?"
    - name: "Resonant Howl"
      type: "Reaction"
      fear_cost: 1
      description: "Sudden noises or strikes against the crystals can trigger haunting echoes, potentially attracting hostile attention or causing environmental tremors."
      questions:
        - "What creature is lured by the crystalline howl?"
        - "Does something ancient stir in response?"

encounters:
  - name: "Shardback Crystal Lizard Ambush"
    fear: "The lizards' camouflage leaves the party surrounded and overwhelmed, risking injury or loss of gathered materials."
    hope: "Careful observation reveals their presence, allowing the party to either hunt the lizards for valuable crystal armor plates or avoid them entirely."

factions:
  - name: "The Crystalline Circle"
    description: "A guild of crafters and harvesters vying for control of unique crystalline resources—both for crafting advanced gear and culinary purposes. Their scouts monitor intruders, wary of trespass."

points_of_interest:
  - "The Titan's Eye: A massive geode embedded in a skull cavity, rumored to pulse with necromantic energy"

npcs:
  - name: "Verrit Shardtongue"
    role: "Crystal Circle Scout"
    description: "A wary, quick-footed elf who trades crystal fragments for information and guides, but distrusts outsiders."

adventure_sites:
  - name: "The Bone-Locked Cache"
    description: "A fossilized titan ribcage cradles a nest of rare fungi, crystalline minerals, and remnants of ancient tools—ripe for discovery, if one can bypass the aggressive lizard pack."

tags:
  - "crystals"
  - "ossuary"
  - "rare ingredients"
  - "territorial factions"
  - "light hazards"

created_at: "2026-02-04"
---
