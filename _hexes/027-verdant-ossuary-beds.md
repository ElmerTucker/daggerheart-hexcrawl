---
hex_id: "027"
title: "Verdant Ossuary Beds"
terrain_type: "moss gardens"
region: "The Bone Gardens"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript area filled with subtle details waiting to be uncovered."
  impulses:
    - "Hide secrets in plain sight"
    - "Draw attention to overlooked elements"
  difficulty: 11
  potential_adversaries:
    - "Curious passerby"
    - "Wandering animal"
  features:
    - name: "Unremarkable Facade"
      type: "Passive"
      fear_cost: null
      description: "Any search or investigation rolls made here are at disadvantage until a clue is found or a PC spends extra time observing."
      questions:
        - "What subtle hint reveals that something is amiss here?"
        - "Which common object holds an unexpected secret?"
    - name: "Hidden Detail"
      type: "Action"
      fear_cost: 1
      description: "The GM may introduce a new, previously unnoticed clue or object, requiring a successful Cunning check (difficulty 11) to discover its significance."
      questions:
        - "What new clue draws the party’s suspicion?"
        - "How does the environment subtly shift to reveal more?"
    - name: "Fleeting Glimpse"
      type: "Reaction"
      fear_cost: null
      description: "When a PC fails an investigation check, they catch a brief, ambiguous sign—granting advantage on their next attempt if they pursue it immediately."
      questions:
        - "What shadow or sound provides a second chance?"
        - "How does the environment reward persistence?"

encounters:
  - name: "Mossback Carrion Beetles"
    fear: "A hidden swarm erupts from a bone mound, threatening to strip flesh and supplies if disturbed."
    hope: "The beetles can be harvested for chitin plates and their sweet-smelling, edible larvae if approached carefully."

factions:
  - name: "The Ossuary Foragers"
    description: "A loose group of scavengers and herbalists harvesting rare mosses and bone-lichen, wary of outsiders but willing to trade."

points_of_interest:
  - "A towering femur pillar draped in glowing moss, rumored to conceal a hidden alcove"

npcs:
  - name: "Sprig Moll"
    role: "Forager and Moss Tender"
    description: "A quick-witted youth who knows every patch of edible moss and is always on the lookout for new recipes and rare spores."

adventure_sites:
  - name: "The Glowroot Hollow"
    description: "A shallow, root-choked cave beneath the largest bone pillar, filled with rare phosphorescent moss, strange insects, and signs of a lost expedition."

tags:
  - "bone"
  - "moss"
  - "hidden-resources"
  - "edible-insects"
  - "foraging"
  - "scavengers"

created_at: "2026-02-04"
---
