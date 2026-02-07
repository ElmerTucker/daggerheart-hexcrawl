---
hex_id: "004"
title: "Verdant Ossuary Beds"
terrain_type: "moss gardens"
region: "The Bone Gardens"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript area waiting to reveal its secrets to the observant."
  impulses:
    - "Conceal hidden details"
    - "Reward curiosity"
  difficulty: 11
  potential_adversaries:
    - "Wandering Wildlife"
    - "Unseen Observer"
  features:
    - name: "Unremarkable Facade"
      type: "Passive"
      fear_cost: null
      description: "Characters must succeed on an Investigation check (DC 11) to notice anything unusual or potentially important in this area."
      questions:
        - "What might be overlooked by a casual glance?"
        - "Is there something quietly out of place?"
    - name: "Subtle Clue"
      type: "Action"
      fear_cost: 1
      description: "The GM can reveal a faint sign, sound, or scent that hints at something hidden; a successful Insight roll uncovers a minor secret or leads to a new discovery."
      questions:
        - "How does the clue connect to a larger mystery?"
        - "Who or what left this subtle sign?"
    - name: "Unveiled Discovery"
      type: "Reaction"
      fear_cost: null
      description: "When a character thoroughly searches or interacts with the environment, a previously hidden object, passage, or detail is revealed."
      questions:
        - "What unexpected thing do the characters find?"
        - "How does this discovery change the party's understanding of the area?"

encounters:
  - name: "Bonecap Stalker Foraging"
    fear: "The mossy ground conceals a territorial predator, the Bonecap Stalker; if startled, it attacks from beneath the moss with venomous fangs."
    hope: "Careful observation reveals the creature’s burrow, enabling safe harvest of rare bone-moss and edible fungi—or perhaps a nonviolent encounter."

factions:
  - name: "The Ossuary Tenders"
    description: "A secretive cult devoted to maintaining the balance of life and death in the Bone Gardens. Here, they collect rare mosses for rituals and watch for trespassers."

points_of_interest:
  - "A fossilized ribcage arching overhead, draped in glowing green moss and shelf-fungi"

npcs:
  - name: "Brother Lymm"
    role: "Ossuary Tender Acolyte"
    description: "A quiet, moss-stained figure tending to luminescent growths, eager to barter for fresh monster marrow or rare spores."

adventure_sites:
  - name: "The Verdant Ribcage"
    description: "A living mausoleum where rare edible mosses and necromantic mushrooms thrive on ancient bone; hidden caches and tunnels beckon explorers."

tags:
  - "harvest"
  - "necromancy"

created_at: "2026-02-04"
---
