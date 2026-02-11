---
hex_id: "007"
title: "The Blooming Market Groves"
terrain_type: "fungal forest"
region: "Halfway Station"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript area with subtle details waiting to be uncovered."
  impulses:
    - "Conceal hidden truths"
    - "Invite close observation"
  difficulty: 11
  potential_adversaries:
    - "Wandering creature"
    - "Secretive local"
  features:
    - name: "Unremarkable Facade"
      type: "Passive"
      fear_cost: null
      description: "Perception and Investigation rolls to notice anything unusual have disadvantage unless the search is careful or methodical."
      questions:
        - "What is easily overlooked here?"
        - "What faint clues hint at something more?"
    - name: "Reveal Subtle Clue"
      type: "Action"
      fear_cost: 2
      description: "A small detail catches a PC’s attention, granting advantage on their next search or investigation in this area."
      questions:
        - "What draws a fleeting glance?"
        - "How does the environment reward patient curiosity?"
    - name: "Shift the Ordinary"
      type: "Reaction"
      fear_cost: null
      description: "When a PC interacts with the environment in an unexpected way, something minor but revealing changes or is uncovered."
      questions:
        - "How does the environment respond to creative thinking?"
        - "What new lead emerges from an unusual action?"

encounters:
  - name: "Negotiation with Guild Foragers"
    fear: "Foragers catch PCs poaching rare ingredients, risking conflict, trade ban, or extortion."
    hope: "Foragers welcome the PCs and share tips, rare samples, or access to secluded groves if impressed or bribed."

factions:
  - name: "Sporewalkers' Guild"
    description: "Expert foragers who regulate the harvesting and sale of fungal ingredients, keen to maintain their monopoly and wary of outsiders."
  - name: "Mycelian Brokers"
    description: "Shadowy traders moving rare monster parts and black market spores; here to make deals, scout new clients, and manipulate local politics."

points_of_interest:
  - "Bioluminescent trading stalls grown from living mushrooms"
  - "A hidden spore-locked vault storing rare ingredients"

npcs:
  - name: "Pellim Sporehand"
    role: "Senior Forager"
    description: "Gruff leader of the Sporewalkers' Guild, knows every edible and toxic fungus in the groves and brooks no fools."
  - name: "Marrow Silkvein"
    role: "Black Market Broker"
    description: "Soft-spoken, calculating, and always ready to cut a deal for rare monster parts—legal or not."

adventure_sites:
  - name: "The Spore-Crypt"
    description: "A sealed, fungus-choked archive rumored to contain ancient recipes, monster specimens, and rare spores—dangerous to the unprepared."

tags:
  - "trading post"
  - "fungal ecology"
  - "faction intrigue"
  - "resource-rich"
  - "underground market"

created_at: "2026-02-04"
---
