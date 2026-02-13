---
hex_id: "009"
title: "Scorched Mycelium Tunnels"
terrain_type: "lava tubes"
region: "The Bitter Depths"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript area that offers little apparent character but may conceal hidden details."
  impulses:
    - "Conceal its true nature"
    - "Encourage careful observation"
  difficulty: 11
  potential_adversaries:
    - "Wandering bandit"
    - "Curious animal"
  features:
    - name: "Unremarkable Setting"
      type: "Passive"
      fear_cost: null
      description: "All Investigation and Perception checks to find something out of the ordinary are made with one Disadvantage."
      questions:
        - "What subtle clue breaks the monotony of this space?"
        - "How do the characters realize something is amiss?"
    - name: "Fleeting Glimpse"
      type: "Action"
      fear_cost: 1
      description: "A shadow or brief movement distracts the party, forcing them to reroll their next Investigation or Perception check and take the lower result."
      questions:
        - "What causes the distraction?"
        - "Does the glimpse hint at danger or opportunity?"
    - name: "Hidden Detail"
      type: "Reaction"
      fear_cost: null
      description: "When a character fails a search or investigation check, reveal a minor but intriguing detail that suggests a deeper secret."
      questions:
        - "What does the revealed detail hint at?"
        - "How do the characters interpret this new information?"

encounters:
  - name: "Fume-Crawler Ambush"
    fear: "A sudden attack from heat-adapted, acidic-spraying crustaceans catches the party off-guard, risking burns and ruined gear."
    hope: "Keen perception spots the camouflaged predators early, allowing for a strategic hunt and a haul of rare, spicy meat and heat-resistant carapace."

factions:
  - name: "The Glaze-Born"
    description: "A reclusive group of fungal cultivators collecting rare heat-loving spores and acidic run-off for powerful concoctions. They fiercely protect their patches from outsiders."

points_of_interest:
  - "A patch of glowing, heat-resistant mushrooms dripping with acidic dew—valuable for alchemy and monster cuisine."

npcs:
  - name: "Cordy Emberlock"
    role: "Glaze-Born Sporescout"
    description: "A masked, irritable mycologist who guards the best fungal growths and trades only for rare ingredients or unique monster parts."

adventure_sites:
  - name: "The Boiling Sump"
    description: "A bubbling, acidic hot spring collecting in a collapsed lava bubble, home to unusual minerals and dangerous creatures. Risk and reward for any who try to harvest its bounty."

tags:
  - "fungus"
  - "acid"
  - "resource-rich"
  - "predators"
  - "hazard"

created_at: "2026-02-04"
---
