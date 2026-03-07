---
hex_id: "031"
title: "Caustic Ossuary Plains"
terrain_type: "bone fields"
region: "The Bitter Depths"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript area filled with subtle secrets waiting to be uncovered."
  impulses:
    - "Conceal hidden details"
    - "Reward careful observation"
  difficulty: 11
  potential_adversaries:
    - "Curious wanderer"
    - "Minor lurking threat"
  features:
    - name: "Unremarkable Facade"
      type: "Passive"
      fear_cost: null
      description: "All Investigation and Perception rolls to notice something out of place are made at difficulty 11."
      questions:
        - "What is the most easily overlooked detail here?"
        - "How do signs of disturbance subtly reveal themselves?"
    - name: "Faint Clues"
      type: "Action"
      fear_cost: 1
      description: "Reveal a subtle clue or object to a searching character, granting them advantage on their next Investigation roll in this environment."
      questions:
        - "What hint could spark further curiosity?"
        - "Who or what left this clue behind?"
    - name: "Sudden Distraction"
      type: "Reaction"
      fear_cost: null
      description: "When a character focuses too intently, create a minor distraction, causing disadvantage on their next roll to notice hidden elements."
      questions:
        - "What unexpected sound or movement draws attention away?"
        - "How does the environment mask its own secrets?"

encounters:
  - name: "Acid-Worn Marrow Gnashers"
    fear: "A pack of bone-crunching scavengers ambushes the party, drawn by the scent of exposed flesh and spilled alchemical reagents."
    hope: "The gnashers, if distracted or appeased, can be lured away, leaving behind valuable marrow and acid-resilient bone shards."

factions:
  - name: "The Bonepickers"
    description: "A roving band of resourceful scavengers searching for rare, acid-etched bones and glands to sell or craft into gear. Here, they're extracting caustic marrow from exposed boneyards."

points_of_interest:
  - "A tangle of titanic, fossilized ribcages forming natural bridges over toxic runnels."

npcs:
  - name: "Farris Vell"
    role: "Bonepicker Leader"
    description: "Cautious, whip-smart, and scarred by acid burns. Always on the lookout for potential allies or rivals."

adventure_sites:
  - name: "The Lurid Bonepile"
    description: "A massive mound of acid-bleached bones where rare marrow creatures nest and the runoff glows with bioluminescence. Rumored to hide precious, unspoiled artifacts."

tags:
  - "toxic"
  - "bone"
  - "scavenger"
  - "acid"

created_at: "2026-02-04"
---
