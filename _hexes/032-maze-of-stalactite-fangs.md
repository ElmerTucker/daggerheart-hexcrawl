---
hex_id: "032"
title: "Maze of Stalactite Fangs"
terrain_type: "stalactite maze"
region: "The Titan's Tomb"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript area invites careful observation and subtle discovery."
  impulses:
    - "Conceal minor secrets"
    - "Encourage quiet exploration"
  difficulty: 11
  potential_adversaries:
    - "Wandering animal"
    - "Hidden trap"
  features:
    - name: "Subtle Details"
      type: "Passive"
      fear_cost: null
      description: "Characters must succeed on a Sense check to notice hidden features, clues, or minor changes in the environment."
      questions:
        - "What detail could easily be overlooked here?"
        - "How does the environment subtly hint at a deeper mystery?"
    - name: "Background Movement"
      type: "Action"
      fear_cost: 1
      description: "The GM can introduce a minor event (a faint sound, a shadow passing, a gentle breeze) that distracts or misdirects the characters, imposing Disadvantage on their next check to observe or search."
      questions:
        - "What small event could draw attention away from something important?"
        - "How does the environment keep the characters on edge?"
    - name: "Unstable Ground"
      type: "Reaction"
      fear_cost: null
      description: "When a character interacts with the environment recklessly, loose stones or uneven footing may cause them to stumble, requiring an Agility check to avoid minor harm or delay."
      questions:
        - "What part of the environment is unexpectedly hazardous?"
        - "How does a character’s actions trigger a subtle danger?"

encounters:
  - name: "Bone-Latch Hermit"
    fear: "The hermit attacks intruders with bone-tipped spears and leads them into pit traps."
    hope: "The hermit offers cryptic guidance in exchange for food or rare marrow fungus, revealing hidden paths."

factions:
  - name: "Gravetide Foragers"
    description: "A band of scavengers seeking monster bones and marrow for culinary and alchemical use, wary of rivals and defensive of their discovered deposits."

points_of_interest:
  - "A nest of luminous cave moths clinging to a natural bone archway"

npcs:
  - name: "Chara of the Ivory Staff"
    role: "Wandering Bone Collector"
    description: "A resourceful, eccentric scavenger who trades in rare bone fragments and knows the maze’s shifting paths."

adventure_sites:
  - name: "Fossilized Jaw Bridge"
    description: "A crossing formed from the petrified jawbone of an ancient beast—treacherous footing but rich in harvestable bone moss and marrow-filled crevices."

tags:
  - "traversal"
  - "bone-resources"
  - "hidden-paths"
  - "factions"

created_at: "2026-02-04"
---
