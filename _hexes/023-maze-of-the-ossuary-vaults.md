---
hex_id: "023"
title: "Maze of the Ossuary Vaults"
terrain_type: "bone fields"
region: "The Forgotten Vaults"

environment:
  name: "Ossuary Maze"
  tier: 2
  type: "Exploration"
  description: "A labyrinthine expanse of ancient bones and crumbling vaults, echoing with the memories of long-dead beasts and the whispers of necromantic power."
  impulses:
    - "Hide secrets within mundane elements"
    - "Invite curiosity through subtle clues"
  difficulty: 11
  potential_adversaries:
    - "Wandering animal"
    - "Curious local"
  features:
    - name: "Subtle Details"
      type: "Passive"
      fear_cost: null
      description: "Characters who spend time observing may discover hidden objects or information with a successful Discovery roll."
      questions:
        - "What easily overlooked element holds a secret?"
        - "How do these details reward thorough investigation?"
    - name: "Hidden Clue"
      type: "Action"
      fear_cost: 1
      description: "Reveal a hidden clue that hints at something greater, granting advantage to the next investigation check if noticed."
      questions:
        - "What form does this clue take?"
        - "How does it connect to a larger mystery?"
    - name: "Overlooked Hazard"
      type: "Reaction"
      fear_cost: null
      description: "When a character ignores their surroundings, a minor hazard (such as a loose stone or sudden noise) causes them to make a Reflex roll or take 1d6+1 damage."
      questions:
        - "What small danger is easily missed here?"
        - "How do the characters react to being caught off guard?"

encounters:
  - name: "Bone Warden Revenant"
    fear: "The Bone Warden animates skeletal remains to attack intruders or seal exits, turning the maze against the party."
    hope: "The party appeases or outwits the revenant, gaining access to its knowledge of hidden vault passages and a cache of preserved monster marrow."

factions:
  - name: "The Marrow Syndicate"
    description: "A secretive group that harvests rare bone materials and necromantic reagents. They are mapping the ossuary for lucrative relics and monster remains."

points_of_interest:
  - "Collapsed vault door with runic bone wardings"

npcs:
  - name: "Veshka the Bone Scribe"
    role: "Cartographer and Marrow Syndicate agent"
    description: "A shifty goblin with bone spectacles, tirelessly mapping the maze and trading information for rare ossified treasures."

adventure_sites:
  - name: "The Spiral Ossuary"
    description: "A spiral staircase of interlocked monster ribs descends into a sealed chamber rumored to house a legendary necromantic recipe and rare skeletal monsters."

tags:
  - "bones"
  - "maze"
  - "necromancy"
  - "secrets"
  - "ancient ruins"

created_at: "2026-02-04"
---
