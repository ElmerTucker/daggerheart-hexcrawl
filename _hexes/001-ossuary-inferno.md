---
hex_id: "001"
title: "Ossuary Inferno"
terrain_type: "lava tubes"
region: "The Bone Gardens"

environment:
  name: "Ossuary Inferno"
  tier: 4
  type: "Exploration"
  description: "Searing heat, rivers of molten bone, necromantic energies suffusing skeletal structures."
  impulses:
    - "Conceal subtle clues"
    - "Encourage cautious movement"
  difficulty: 11
  potential_adversaries:
    - "Curious animal"
    - "Distracted local"
  features:
    - name: "Unremarkable Terrain"
      type: "Passive"
      fear_cost: null
      description: "Checks to notice hidden details require careful observation; characters gain advantage on Search if they spend extra time."
      questions:
        - "What detail do the characters almost miss?"
        - "How does the environment reward thoroughness?"
    - name: "Subtle Distraction"
      type: "Action"
      fear_cost: 1
      description: "Cause a faint noise or minor event (like a breeze or distant voice) to draw attention away from a clue, increasing the difficulty of a single Search roll by 2."
      questions:
        - "What minor event could pull focus from the main objective?"
        - "Who or what causes the distraction?"
    - name: "Trace Evidence"
      type: "Reaction"
      fear_cost: null
      description: "When a character investigates a specific spot, reveal a barely noticeable hint or sign pointing to something hidden or important."
      questions:
        - "What tiny sign hints at a larger story?"
        - "How can this clue change the party’s direction?"

encounters:
  - name: "Molten Bone Warden"
    fear: "The skeletal warden animates rivers of molten bone to trap or incinerate trespassers, driving them into dangerous side tunnels."
    hope: "The party negotiates with or subdues the warden, learning secrets about the necromantic currents and gaining access to rare crafting bone."

factions:
  - name: "The Ivory Cult"
    description: "A group of necromancers harvesting bones and soul-ash, seeking to animate greater bone constructs. Here, they perform rituals and fiercely defend their claimed lava tubes."

points_of_interest:
  - "A bridge of fused bone arching over a glowing river of molten marrow"

npcs:
  - name: "Sable Marrow"
    role: "Bone Cult Ritualist"
    description: "A gaunt, intense necromancer who studies the flows of molten bone and barters necromantic secrets for rare reagents."

adventure_sites:
  - name: "The Pyre Crucible"
    description: "A chamber where bone and soul-ash are fused by volcanic heat, used for both dangerous rituals and forging powerful bonecraft gear."

tags:
  - "necromancy"
  - "lava"
  - "bone"
  - "high-danger"
  - "resource-rich"

created_at: "2026-02-04"
---
