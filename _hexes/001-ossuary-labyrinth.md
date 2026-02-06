---
hex_id: "001"
title: "Ossuary Labyrinth"
terrain_type: "ancient ruins"
region: "The Bone Gardens"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript area where subtle details hide beneath the surface."
  impulses:
    - "Conceal hidden elements"
    - "Challenge observation and perception"
  difficulty: 11
  potential_adversaries:
    - "Small lurking creatures"
    - "Unseen traps"
  features:
    - name: "Unremarkable Facade"
      type: "Passive"
      fear_cost: null
      description: "The environment appears ordinary, requiring a successful Cunning roll (Difficulty 11) to notice anything out of place."
      questions:
        - "What subtle clues hint at something unusual?"
        - "How does the environment mislead the senses?"
    - name: "Overlooked Obstacle"
      type: "Action"
      fear_cost: 1
      description: "The GM may introduce a minor hidden hazard (e.g., loose stone, sudden dip) that forces a PC to make a Quickness or Fortitude roll to avoid 1d6+1 damage or being delayed."
      questions:
        - "What unnoticed hazard surprises the party?"
        - "How does the environment respond to movement or investigation?"
    - name: "Hidden Discovery"
      type: "Reaction"
      fear_cost: null
      description: "When a PC investigates thoroughly or asks a probing question, reveal a concealed item, passage, or clue relevant to their goal."
      questions:
        - "What secret is revealed by careful observation?"
        - "How does this discovery shift the party’s understanding of the area?"

encounters:
  - name: "Bone Warden's Patrol"
    fear: "The Bone Warden animates skeletal guardians, attacking intruders and raising chilling alarms that draw more threats."
    hope: "The Bone Warden can be reasoned with or distracted, allowing the party to discover a cache of rare necromantic reagents embedded in the remains."

factions:
  - name: "Mortuary Guild"
    description: "This secretive guild harvests arcane bones and marrow, seeking to control the Bone Gardens’ necromantic power. Here, their scouts search for relics and keep rivals at bay."

points_of_interest:
  - "Collapsed Noble Crypt with unbroken seals"

npcs:
  - name: "Veshra the Ossuary Witch"
    role: "Caretaker and bone mage"
    description: "An enigmatic figure weaving spells from marrow and spirit, offering knowledge in exchange for rare remains or stories."

adventure_sites:
  - name: "Chamber of the Whispering Skulls"
    description: "A vast rotunda where animated skulls murmur secrets of the past, guarded by spectral sentinels. Brave explorers may learn lost recipes or forbidden rites."

tags:
  - "necromantic"
  - "maze"
  - "resource-rich"
  - "dangerous"
  - "ancient"

created_at: "2026-02-04"
---
