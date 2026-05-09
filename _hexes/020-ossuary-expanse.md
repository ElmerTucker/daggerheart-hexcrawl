---
hex_id: "020"
title: "Ossuary Expanse"
terrain_type: "bone fields"
region: "The Titan's Tomb"

environment:
  name: "Ossuary Expanse"
  tier: 3
  type: "Exploration"
  description: "Vast fields of gigantic bones, silt, and calcified remains. Eerie quiet punctuated by the creaks of shifting skeletal monuments."
  impulses:
    - "Reveal ancient secrets among the bones"
    - "Challenge movement with unstable footing and hidden traps"
    - "Confront explorers with skeletal predators and scavengers"
  difficulty: 16
  potential_adversaries:
    - "Bone scavenger pack"
    - "Skeletal colossus remnant"
    - "Territorial necromancer"
  features:
    - name: "Shifting Bone Monoliths"
      type: "Passive"
      fear_cost: null
      description: "Massive bones groan and shift, sometimes collapsing or opening new passages. Navigating safely requires careful Study or Traverse."
      questions:
        - "What sound or movement signals a coming shift?"
        - "How might explorers take advantage of newly revealed paths?"
    - name: "Calcified Spoil Pockets"
      type: "Action"
      fear_cost: 2
      description: "Pockets of valuable but hazardous mineral deposits or monster remains trapped in bone. Harvesting them risks collapse or exposure to toxins."
      questions:
        - "What rare resource tempts the party?"
        - "What threat lurks within the calcified mass?"
    - name: "Necromantic Residue"
      type: "Reaction"
      fear_cost: 1
      description: "Residual magic animates small bone fragments or draws the attention of necromancers."
      questions:
        - "What evidence hints at restless spirits?"
        - "How does this magic alter the local ecosystem?"

encounters:
  - name: "Bone Scavenger Ambush"
    fear: "A pack of skeletal beasts erupts from the silt, threatening to overwhelm the party and scatter their supplies."
    hope: "Defeating or driving off the scavengers yields rare marrow, bone shards, and a clear path to deeper treasures."

factions:
  - name: "The Ossuary Guild"
    description: "Bone-harvesters and necromantic crafters, the Guild patrols the Expanse for resources and will fiercely defend lucrative finds from outsiders."

points_of_interest:
  - "A towering ribcage arch, festooned with fungus and hanging charms from previous expeditions"

npcs:
  - name: "Griselle Marrowshank"
    role: "Ossuary Guild Forewoman"
    description: "Gruff, one-legged, and fiercely protective of her crew. Knows every bone formation and is rumored to have a pact with a bone spirit."

adventure_sites:
  - name: "The Titan's Jaw"
    description: "A colossal jawbone forms a natural bridge over a chasm. Hidden compartments and necromantic runes suggest ancient rituals or lost treasures."

tags:
  - "bone"
  - "necromancy"
  - "hazard"
  - "resource-rich"
  - "guild-territory"

created_at: "2026-02-04"
---
