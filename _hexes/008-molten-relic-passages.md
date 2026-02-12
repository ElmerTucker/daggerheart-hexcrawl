---
hex_id: "008"
title: "Molten Relic Passages"
terrain_type: "lava tubes"
region: "The Forgotten Vaults"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "An unremarkable area holds subtle details awaiting discovery."
  impulses:
    - "Conceal hidden clues"
    - "Invite careful observation"
  difficulty: 11
  potential_adversaries:
    - "Roving animal"
    - "Curious bystander"
  features:
    - name: "Subtle Details"
      type: "Passive"
      fear_cost: null
      description: "Characters must succeed on a Difficulty 11 Insight or Awareness roll to notice anything out of the ordinary."
      questions:
        - "What small sign hints at something more?"
        - "How do the senses reveal hidden elements?"
    - name: "Overlooked Clue"
      type: "Action"
      fear_cost: 1
      description: "A crucial piece of information is obscured until characters spend extra time searching or ask the right questions."
      questions:
        - "What does a second look reveal?"
        - "How does impatience hinder discovery?"
    - name: "Echoes of Activity"
      type: "Reaction"
      fear_cost: null
      description: "When a character investigates, faint evidence of recent activity becomes apparent, granting advantage on the next search roll for the party."
      questions:
        - "What traces of passage are barely noticeable?"
        - "How does the environment subtly respond to attention?"

encounters:
  - name: "Scavenger Skulk"
    fear: "Ambushed by a swarm of heat-adapted cave rats, the party must fend off biting attackers and salvage what supplies they can."
    hope: "The rats reveal the location of a hidden cache of edible fungus and mineral-rich ore, accessible if the party approaches with caution."

factions:
  - name: "The Ember Seekers"
    description: "A small band of relic hunters scouring the lava tubes for ancient, heat-tempered artifacts. They’re defensive and wary of outsiders, hoping to claim a legendary fireproof pan said to be lost here."

points_of_interest:
  - "Cracked obsidian altar embedded with faintly glowing runes"

npcs:
  - name: "Vennan Kesh"
    role: "Relic Hunter Scout"
    description: "Lean, soot-stained, and ever-watchful, Vennan maps the passages and warns his companions of lurking predators and rival factions."

adventure_sites:
  - name: "The Flowstone Pantry"
    description: "A collapsed ancient kitchen where heat-loving fungi and edible crystal growths flourish among forgotten cookware and charred bones."

tags:
  - "relics"
  - "fungus"
  - "rats"
  - "hidden"

created_at: "2026-02-04"
---
