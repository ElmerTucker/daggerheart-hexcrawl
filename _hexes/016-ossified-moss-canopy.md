---
hex_id: "016"
title: "Ossified Moss Canopy"
terrain_type: "moss gardens"
region: "The Titan's Tomb"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript area holds subtle secrets waiting to be uncovered."
  impulses:
    - "Conceal hidden details from casual observation"
    - "Encourage careful investigation"
  difficulty: 11
  potential_adversaries:
    - "Suspicious passerby"
    - "Minor magical anomaly"
  features:
    - name: "Unremarkable Facade"
      type: "Passive"
      fear_cost: null
      description: "Checks to notice hidden objects or clues are made at disadvantage unless specifically searching."
      questions:
        - "What clues might be overlooked at first glance?"
        - "How does the environment subtly mislead observers?"
    - name: "Subtle Movement"
      type: "Action"
      fear_cost: 1
      description: "A shadow or noise draws attention away from a vital clue, increasing difficulty to discover it by 2 for one round."
      questions:
        - "What causes a minor distraction here?"
        - "Who or what benefits from the PCs missing something?"
    - name: "Echoes of the Past"
      type: "Reaction"
      fear_cost: null
      description: "When a PC investigates thoroughly, faint traces of past events become apparent, offering a helpful hint or context."
      questions:
        - "What memory or evidence lingers here?"
        - "How does this clue change the party’s approach?"

encounters:
  - name: "Mossback Chiroptid Swarm"
    fear: "The swarm descends, overwhelming intruders and leaving them covered in spore burns and lacerations."
    hope: "The party harvests rare Mossback guano and finds abandoned chiroptid nests full of edible larvae and bioluminescent moss."

factions:
  - name: "Bonegarden Tenders"
    description: "A collective of moss-farmers and bone-harvesters who cultivate rare mosses for food and medicine, defending the area from poachers."

points_of_interest:
  - "A massive rib arch draped in glowing moss, humming with latent necromantic energy"

npcs:
  - name: "Tessik Khol"
    role: "Bonegarden Tender Overseer"
    description: "A stoic, moss-stained dwarf with a thick accent and encyclopedic knowledge of medicinal mosses and bonecraft."

adventure_sites:
  - name: "The Ossuary Steps"
    description: "A staircase of giant vertebrae spiraling through a living moss canopy, rumored to hide relics of the ancient Titan and rare fungal species."

tags:
  - "harvestable"
  - "bioluminescent"
  - "necromantic"
  - "moss"
  - "bone"
  - "faction presence"

created_at: "2026-02-04"
---
