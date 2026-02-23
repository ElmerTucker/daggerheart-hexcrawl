---
hex_id: "019"
title: "Labyrinth of Hanging Blades"
terrain_type: "stalactite maze"
region: "The Forgotten Vaults"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript area offering subtle details for those who choose to look closer."
  impulses:
    - "Conceal its true nature"
    - "Reward patient observation"
  difficulty: 11
  potential_adversaries:
    - "Wandering animal"
    - "Hidden thief"
  features:
    - name: "Unremarkable Facade"
      type: "Passive"
      fear_cost: null
      description: "All Investigation and Perception rolls to notice anything unusual suffer Disadvantage."
      questions:
        - "What detail is almost always overlooked?"
        - "How do signs of prior passage blend into the background?"
    - name: "Sudden Subtlety"
      type: "Action"
      fear_cost: 1
      description: "The environment shifts slightly, hiding clues or evidence; a player must pass a Presence or Insight check (Difficulty 11) or miss a crucial detail."
      questions:
        - "What small change makes something harder to find?"
        - "Who or what triggers this sudden subtlety?"
    - name: "Overlooked Clue"
      type: "Reaction"
      fear_cost: null
      description: "When a PC fails a check by 2 or less, they notice a faint anomaly hinting at something more if they follow up."
      questions:
        - "What faint anomaly draws their attention?"
        - "How does following up change their perception of the area?"

encounters:
  - name: "Vault Stalker Ambush"
    fear: "A Vault Stalker (a chitinous, camouflaged predator) drops from above, threatening to separate and wound the party."
    hope: "Defeating or driving off the Stalker yields rare, alchemically useful carapace and scent sacs."

factions:
  - name: "Candlelight Syndicate"
    description: "A group of smugglers and relic-thieves using the maze to hide stolen goods and ambush rivals. They're currently scouting new hiding spots."

points_of_interest:
  - "A cluster of unlooted, half-collapsed vault lockers tangled among the stalactites"

npcs:
  - name: "Mira 'Spindlefingers'"
    role: "Relic-Scavenger"
    description: "A wiry, sharp-eyed member of the Syndicate, Mira knows the twisting mazes well and trades information for monster parts or food."

adventure_sites:
  - name: "The Shattered Reliquary"
    description: "A long-lost, rune-locked chamber rumored to hold a preserved Keeper's heart and ancient recipes. Traps and lingering guardian spirits make approach perilous."

tags:
  - "navigation"
  - "hidden treasures"
  - "predators"
  - "ancient ruins"

created_at: "2026-02-04"
---
