---
hex_id: "006"
title: "Vault of Verdant Shadows"
terrain_type: "fungal forest"
region: "The Forgotten Vaults"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript place filled with subtle details waiting to be uncovered."
  impulses:
    - "Present hidden clues"
    - "Obscure important information"
  difficulty: 11
  potential_adversaries:
    - "Curious passerby"
    - "Wandering animal"
  features:
    - name: "Unremarkable Facade"
      type: "Passive"
      fear_cost: null
      description: "All search or investigation attempts are made at disadvantage unless a character spends time carefully observing."
      questions:
        - "What subtle detail gives away something important?"
        - "How might an overlooked feature change the situation?"
    - name: "Hidden Discovery"
      type: "Action"
      fear_cost: 1
      description: "Reveal a small but meaningful secret or clue to a character who takes initiative, granting them advantage on their next Exploration roll within this environment."
      questions:
        - "What secret is uncovered that shifts the party's perspective?"
        - "Who notices the clue first?"
    - name: "Faint Distraction"
      type: "Reaction"
      fear_cost: null
      description: "When a character rushes or becomes impatient, introduce an innocuous distraction that delays progress or causes them to overlook something important."
      questions:
        - "What causes the character to lose focus?"
        - "How does the delay affect their plans?"

encounters:
  - name: "Spore-Cloaked Stalker"
    fear: "The party is ambushed by a camouflaged fungal predator, risking injury and the spread of hallucinogenic spores."
    hope: "The party spots the stalker in time to harvest rare, potent spores and gain a valuable monster part."

factions:
  - name: "The Mycoliths"
    description: "A reclusive fungal-kin society cultivating unique mushrooms and jealously guarding ancient relics buried beneath the moss."

points_of_interest:
  - "A collapsed vault door covered in phosphorescent lichen, concealing a trove of ancient supplies."

npcs:
  - name: "Senior Sporekeeper Mirrun"
    role: "Fungal Scholar and Relic Warden"
    description: "A spindly, masked humanoid devoted to cataloging new fungal lifeforms and keeping intruders away from the most dangerous mushrooms and relics."

adventure_sites:
  - name: "The Relic Glade"
    description: "A clearing where massive bioluminescent mushrooms have grown around a half-buried, rune-etched vault—ripe for harvesting but fiercely protected by local creatures and Mycolith guardians."

tags:
  - "bioluminescent"
  - "ancient ruins"
  - "fungal creatures"
  - "hidden threats"
  - "valuable resources"

created_at: "2026-02-04"
---
