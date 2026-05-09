---
hex_id: "025"
title: "The Ivory Thicket"
terrain_type: "bone fields"
region: "The Titan's Tomb"

environment:
  name: "The Ivory Thicket"
  tier: 2
  type: "Exploration"
  description: "Dense bone spires and tangled marrow thickets, haunted by scavengers and echoing with the low groans of shifting remains."
  impulses:
    - "Conceal what lies within the bone labyrinth"
    - "Entangle the unwary among shifting ivory"
    - "Draw scavengers and bone-harvesters to the choicest remains"
  difficulty: 13
  potential_adversaries:
    - "Marrow Mites (bone-boring insects)"
    - "Ivory Vultures (large, flightless carrion birds)"
    - "Bonepicker Outcasts"
  features:
    - name: "Bone Labyrinth"
      type: "Passive"
      fear_cost: null
      description: "Navigators must succeed on a Cunning or Grace roll (Difficulty 13) to avoid becoming disoriented or separated among the bone spires."
      questions:
        - "What eerie shapes loom out of the ivory mist?"
        - "How does the labyrinth shift with the movement of the party?"
    - name: "Groaning Remains"
      type: "Action"
      fear_cost: 2
      description: "Pressure on certain bones releases deep, resonant groans that can attract predators or alert lurking scavengers nearby."
      questions:
        - "Who or what responds to the haunting sounds?"
        - "Can the party use the bones’ resonance to their advantage?"
    - name: "Marrow Cache"
      type: "Reaction"
      fear_cost: null
      description: "Those who search carefully may discover hidden caches of rich marrow or rare monster bone fragments, valuable for cooking or crafting."
      questions:
        - "What unique creature left these remains?"
        - "How can the party use these resources?"

encounters:
  - name: "Ivory Vulture Scavenging"
    fear: "A flock of Ivory Vultures aggressively defends a fresh kill, swarming intruders and risking injury or infection with disease-ridden beaks."
    hope: "Careful negotiation or distraction grants access to fresh marrow and rare vulture plumes, prized in both cuisine and crafting."

factions:
  - name: "The Bonepicker Outcasts"
    description: "A desperate band eking out survival by harvesting bone and marrow, fiercely territorial and suspicious of outsiders, but open to trade for tools or food."

points_of_interest:
  - "Spiral Ossuary—an enormous ribcage structure hollowed out into a shelter and lookout"

npcs:
  - name: "Grelka"
    role: "Bonepicker Outcast Leader"
    description: "Stubborn and shrewd, adorned with bone jewelry and wielding a marrow-saw, determined to protect her people and their marrow caches."

adventure_sites:
  - name: "The Marrow Vault"
    description: "A partly-collapsed chamber beneath splintered vertebrae, rumored to contain preserved remains from a legendary beast—ripe for harvest, but crawling with dangerous marrow mites."

tags:
  - "bonecrafting"
  - "scavenging"
  - "hazardous"
  - "resource-rich"

created_at: "2026-02-04"
---
