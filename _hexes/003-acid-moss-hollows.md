---
hex_id: "003"
title: "Acid-Moss Hollows"
terrain_type: "moss gardens"
region: "The Bitter Depths"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript area filled with subtle details waiting to be uncovered."
  impulses:
    - "Encourage investigation"
    - "Reveal hidden information"
  difficulty: 11
  potential_adversaries:
    - "Bored Attendant"
    - "Wandering Animal"
  features:
    - name: "Quiet Ambience"
      type: "Passive"
      fear_cost: null
      description: "All Investigation rolls gain advantage due to the lack of distractions."
      questions:
        - "What subtle signs of activity are present?"
        - "How does the quiet affect the party's mood?"
    - name: "Fleeting Clues"
      type: "Action"
      fear_cost: 1
      description: "A sudden change or movement provides a fleeting clue; the GM may offer a hint or reveal a detail to the most attentive character."
      questions:
        - "What unexpected change draws the party's attention?"
        - "Who notices the clue first?"
    - name: "Echoing Step"
      type: "Reaction"
      fear_cost: null
      description: "When a PC makes a loud noise, their actions echo, drawing attention and possibly revealing their presence."
      questions:
        - "Who or what hears the noise?"
        - "Does this new attention help or hinder the party?"

encounters:
  - name: "Mossback Caustisaur"
    fear: "The Caustisaur attacks intruders, releasing acidic mist and trampling anything in its path, threatening to destroy valuable resources and injure the party."
    hope: "If approached carefully and fed with specific spores, the Caustisaur becomes docile, allowing safe harvest of its valuable venom glands and moss-ridden scales."

factions:
  - name: "The Verdant Order"
    description: "Botanist-hunters mapping the moss gardens for rare reagents and toxic flora; fiercely defend their claimed patches against rivals."

points_of_interest:
  - "Luminescent Spore Pools"

npcs:
  - name: "Selenya Pitch"
    role: "Order Scout"
    description: "A quick-witted botanist skilled in identifying edible mosses and mitigating acid burns; always seeking new fungal recipes."

adventure_sites:
  - name: "The Fume Vault"
    description: "An ancient, sealed chamber shrouded in acidic vapors, rumored to hold preserved plants and toxic relics from a forgotten age."

tags:
  - "toxic"
  - "harvestable"
  - "bioluminescence"
  - "territorial predator"

created_at: "2026-02-04"
---
