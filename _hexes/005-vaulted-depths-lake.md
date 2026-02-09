---
hex_id: "005"
title: "Vaulted Depths Lake"
terrain_type: "underground lake"
region: "The Forgotten Vaults"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript area invites careful observation and patient searching."
  impulses:
    - "Present subtle clues"
    - "Reward thorough investigation"
  difficulty: 11
  potential_adversaries:
    - "Wandering creature"
    - "Hidden trap"
  features:
    - name: "Unremarkable Setting"
      type: "Passive"
      fear_cost: null
      description: "Characters must succeed on an Insight roll to notice anything out of the ordinary; otherwise, the environment appears plain."
      questions:
        - "What detail hints at something unusual?"
        - "How does the environment conceal its secrets?"
    - name: "Concealed Detail"
      type: "Action"
      fear_cost: 1
      description: "Reveal a subtle clue or hidden object to a character who searches carefully or asks specific questions."
      questions:
        - "What clue, if discovered, could change the party's approach?"
        - "How is this detail protected or camouflaged?"
    - name: "Echoes of Movement"
      type: "Reaction"
      fear_cost: null
      description: "When a character disturbs the environment, faint sounds or shifting shadows reveal potential hidden dangers or opportunities."
      questions:
        - "What does the sound or movement suggest about the environment?"
        - "Who or what else might be present here?"

encounters:
  - name: "Ancient Lake Leviathan"
    fear: "The leviathan attacks suddenly, dragging a party member into the depths, flooding the chamber, or collapsing a section of the vault."
    hope: "The party manages to avoid notice or pacify the leviathan, gaining access to rare leviathan scales, meat, and ancient relics on its back."

factions:
  - name: "The Deep Vault Seekers"
    description: "A small expedition of treasure-divers and ruin scholars, searching for lost relics beneath the water, wary of both monsters and rival scavengers."

points_of_interest:
  - "Collapsed stone promenade leading into dark water"
  - "Half-sunken statue of a forgotten ruler"
  - "Thin, glowing lichen on the ceiling illuminating the lake"

npcs:
  - name: "Curator Vilenn"
    role: "Deep Vault Seeker leader"
    description: "A cautious scholar with encyclopedic knowledge of vault relics, desperate to recover a specific lost artifact rumored to be near the lake’s heart."

adventure_sites:
  - name: "Sunken Archive"
    description: "An underwater library containing magically preserved records and ancient scrolls, accessible only by skilled swimmers or those with clever aquatic solutions."

tags:
  - "aquatic"
  - "ruins"
  - "ancient"
  - "dangerous"
  - "resource-rich"

created_at: "2026-02-04"
---
