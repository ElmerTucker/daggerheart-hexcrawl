---
hex_id: "011"
title: "Verdant Scented Canopy"
terrain_type: "moss gardens"
region: "The Jasmine Reaches"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript space holds subtle secrets waiting to be uncovered."
  impulses:
    - "Encourage careful observation"
    - "Hide information in plain sight"
  difficulty: 11
  potential_adversaries:
    - "None"
    - "Wandering Animal"
  features:
    - name: "Unremarkable Facade"
      type: "Passive"
      fear_cost: null
      description: "At first glance, nothing stands out here—Perception or Insight rolls are required to notice hidden details."
      questions:
        - "What clues are overlooked by the casual observer?"
        - "How does the environment reward patient investigation?"
    - name: "Subtle Clue"
      type: "Action"
      fear_cost: 1
      description: "On the GM’s turn, reveal a vague hint or minor secret to a character who deliberately searches or interacts with the environment."
      questions:
        - "What small clue changes a player’s understanding of the space?"
        - "How does this clue connect to a larger mystery?"
    - name: "Unexpected Discovery"
      type: "Reaction"
      fear_cost: null
      description: "When a PC attempts an unusual action, reveal a hidden compartment, item, or piece of information."
      questions:
        - "What is revealed that no one expected?"
        - "How does this discovery alter the party’s next steps?"

encounters:
  - name: "Aromatic Mosslurker"
    fear: "The Mosslurker's camouflage allows it to ambush the party, causing injuries or disrupting foraging."
    hope: "Careful observation lets the party notice the Mosslurker first, gaining valuable rare moss and edible fungi from its trail."

factions:
  - name: "Frondward Seekers"
    description: "A band of scavenger explorers cataloging aromatic mosses to brew potent curatives and unique perfumes. They have marked trails and guarded caches here."

points_of_interest:
  - "Perfumed Overhang: A ledge where condensation drips into a natural basin, infusing water with potent fungal essences."

npcs:
  - name: "Tamsin Loor"
    role: "Moss tender and field chef"
    description: "A gentle, stoic herbalist who gathers mosses and brews invigorating teas for passing adventurers. She shares recipes in exchange for rare finds."

adventure_sites:
  - name: "Hidden Spore Cache"
    description: "A concealed hollow beneath thick moss containing ancient jars of preserved spores, highly valuable for cooking or crafting—if the Mosslurker's lair is avoided."

tags:
  - "moss"
  - "aromatic"
  - "foraging"
  - "hidden life"
  - "faction presence"

created_at: "2026-02-04"
---
