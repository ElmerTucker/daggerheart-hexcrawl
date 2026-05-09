---
hex_id: "022"
title: "Prismalight Chasm"
terrain_type: "crystal formation"
region: "The Descent Shafts"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript space filled with hidden details waiting to be uncovered."
  impulses:
    - "Conceal secrets within the ordinary"
    - "Reward careful observation"
  difficulty: 11
  potential_adversaries:
    - "Curious townsfolk"
    - "Wandering animal"
  features:
    - name: "Unremarkable Facade"
      type: "Passive"
      fear_cost: null
      description: "All perception and investigation rolls to notice hidden elements are made at disadvantage unless aided by a clue or tool."
      questions:
        - "What subtle clue hints at something more?"
        - "How does the environment discourage casual exploration?"
    - name: "Reveal the Unseen"
      type: "Action"
      fear_cost: 2
      description: "The GM may spend 2 Fear to present a sudden revelation, drawing attention to a previously unnoticed detail or passage."
      questions:
        - "What secret is revealed, and who notices first?"
        - "How does the revelation shift the party’s focus?"
    - name: "Unexpected Obstacle"
      type: "Reaction"
      fear_cost: null
      description: "When a PC searches or investigates, a mundane object becomes a minor obstacle, requiring another check or causing a brief delay."
      questions:
        - "What everyday item proves unexpectedly troublesome?"
        - "How does this obstacle hint at greater mysteries?"

encounters:
  - name: "Crystalline Lurker"
    fear: "The Lurker ambushes climbers, using mimicry to blend with crystal ledges and knock explorers to a deadly fall."
    hope: "The Lurker's crystal carapace can be harvested for rare armor plating or ground into a spice that enhances rations with a refreshing mineral tang."

factions:
  - name: "Sable Guild"
    description: "Expert crafters and resource prospectors marking crystal veins; they harvest both for trade and for their signature glasswork tools."

points_of_interest:
  - "A suspended crystal bridge glittering with luminous moss"

npcs:
  - name: "Tarn Virell"
    role: "Sable Guild Scout"
    description: "Wiry and sharp-eyed, Tarn charts new ledges and tags stable routes for the guild, but is quick to warn others away from unstable paths."

adventure_sites:
  - name: "The Prismal Vault"
    description: "A shattered crystal chamber halfway down the chasm, containing the fossilized remains of an ancient beast and mysterious glassware."

tags:
  - "crystal"
  - "verticality"
  - "valuable resources"
  - "hazardous traversal"

created_at: "2026-02-04"
---
