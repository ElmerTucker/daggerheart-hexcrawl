---
hex_id: "024"
title: "The Acid-Mist Vaults"
terrain_type: "cavern"
region: "The Bitter Depths"

environment:
  name: "The Acid-Mist Vaults"
  tier: 4
  type: "Exploration"
  description: "A cavern choked with drifting acidic mists, slick stone, and the ruins of ancient alchemical workshops. Danger and rare reagents linger in the air."
  impulses:
    - "Corrode the unwary"
    - "Reveal rare alchemical treasures to the bold"
  difficulty: 18
  potential_adversaries:
    - "Acid-Drake Broodmother"
    - "Caustic Slime Swarm"
    - "Alchemical Revenant"
  features:
    - name: "Acidic Mists"
      type: "Passive"
      fear_cost: null
      description: "Continuous exposure deals minor damage and quickly corrodes metal if not protected. Visibility is reduced, muffling sound and obscuring movement."
      questions:
        - "What precious gear is threatened by the acidic air?"
        - "How do the mists shift and swirl, revealing or hiding dangers?"
    - name: "Alchemical Ruins"
      type: "Action"
      fear_cost: 2
      description: "Players can search the crumbling remains of alchemical workshops for potent reagents or long-lost recipes, risking exposure to unstable chemicals."
      questions:
        - "What rare substance or recipe is uncovered?"
        - "What active hazard remains in the ruins?"
    - name: "Unstable Terrain"
      type: "Reaction"
      fear_cost: 1
      description: "The slick, corroded stone fractures or gives way underfoot, potentially dropping explorers into deeper, more hostile pockets of acid or forgotten storage vaults."
      questions:
        - "Who or what is separated from the group by a sudden collapse?"
        - "What new danger or opportunity is revealed below?"

encounters:
  - name: "Caustic Slime Swarm"
    fear: "The swarm engulfs a party member, threatening to dissolve gear and flesh unless quickly repelled."
    hope: "Defeated slimes yield rare acid glands prized by alchemists and crafters."

factions:
  - name: "The Emerald Crucible"
    description: "A secretive cabal of alchemists and scavengers seeking rare reagents and lost knowledge in the acid-choked ruins. They guard their finds jealously and trap their territory against intruders."

points_of_interest:
  - "A shattered containment vault, its glass murals etched with chemical formulas and faded arcane runes."

npcs:
  - name: "Sibyl Greenhand"
    role: "Emerald Crucible Alchemist"
    description: "Cautious and shrouded in protective gear, Sibyl negotiates for rare materials but brooks no theft or sabotage."

adventure_sites:
  - name: "The Sunken Crucible"
    description: "A partially collapsed workshop beneath the main vault, rumored to contain a legendary acid-resistant forge and experimental mutagens."

tags:
  - "acid"
  - "alchemical"
  - "hazardous"
  - "rare-materials"
  - "ruins"

created_at: "2026-02-04"
---
