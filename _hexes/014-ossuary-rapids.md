---
hex_id: "014"
title: "Ossuary Rapids"
terrain_type: "bone fields"
region: "The Weeping Gallery"

environment:
  name: "Ossuary Rapids"
  tier: 2
  type: "Exploration"
  description: "Rushing underground streams cut through jagged bone deposits, creating dangerous but resource-rich bone fields awash with water, mist, and necromantic resonance."
  impulses:
    - "Reveal resources amid danger"
    - "Test skillful traversal and observation"
  difficulty: 14
  potential_adversaries:
    - "Necrophage Eels"
    - "Bonepicker Ghouls"
  features:
    - name: "Churning Streams"
      type: "Hazard"
      fear_cost: 1
      description: "Swift, unpredictable currents filled with shattered bone. Crossing or harvesting here risks being swept away or slashed."
      questions:
        - "What valuable resource is just out of easy reach, across the current?"
        - "How do the bones and water conceal lurking creatures?"
    - name: "Necromantic Resonance"
      type: "Environmental"
      fear_cost: null
      description: "The bones vibrate faintly with lingering energy. Offer clues to magical remains, or hint at reanimation threats."
      questions:
        - "What magical effect lingers near the bone piles?"
        - "What signs suggest recent necromantic activity?"
    - name: "Mist-Clad Boneyards"
      type: "Terrain"
      fear_cost: null
      description: "Dense, humid mist limits vision and muffles sound. Movement is risky without careful mapping or teamwork."
      questions:
        - "How does the mist mask danger or opportunity?"
        - "What sounds echo through the bone fields, real or imagined?"

encounters:
  - name: "Necrophage Eel Swarm"
    fear: "The eels overwhelm, dragging explorers beneath the current and forcing them to abandon gear or risk being consumed."
    hope: "The party harvests precious necromantic eel organs and rare bone-embedded pearls for food and crafting."

factions:
  - name: "Syndicate of the White Maw"
    description: "Bone traders and necromantic artisans comb the rapids for fresh materials, fiercely defending their claimed harvest zones from rivals."

points_of_interest:
  - "Shattered Bone Arch: A massive, natural arch of interlocked bones spanning a turbulent stream."

npcs:
  - name: "Gresa Tibbs"
    role: "White Maw Bone Prospector"
    description: "Gruff and quick-witted, Gresa brokers rare finds and guides outsiders—for the right price—while keeping one eye on the Syndicate’s rivals."

adventure_sites:
  - name: "The Sunken Ossuary"
    description: "An underwater vault filled with ancient, enchanted bones and sealed necromantic relics. Accessible only during rare periods of low water."

tags:
  - "resource-rich"
  - "hazardous"
  - "necromancy"
  - "faction-conflict"
  - "bonecraft"

created_at: "2026-02-04"
---
