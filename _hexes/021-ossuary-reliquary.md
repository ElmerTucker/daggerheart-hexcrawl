---
hex_id: "021"
title: "Ossuary Reliquary"
terrain_type: "ancient ruins"
region: "The Bone Gardens"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript area that invites curiosity through its subtle ambiguity."
  impulses:
    - "Encourage cautious investigation"
    - "Conceal minor secrets"
  difficulty: 11
  potential_adversaries:
    - "Wandering critter"
    - "Hidden trap"
  features:
    - name: "Blank Canvas"
      type: "Passive"
      fear_cost: null
      description: "Clues and details only become apparent after deliberate searching or careful observation."
      questions:
        - "What faint sign hints at something hidden here?"
        - "How does the environment subtly resist being understood?"
    - name: "Fleeting Detail"
      type: "Action"
      fear_cost: 1
      description: "A minor, easily overlooked element draws attention elsewhere or distracts the party, making the next search roll more difficult (Disadvantage)."
      questions:
        - "What small distraction diverts the party’s focus?"
        - "How does this moment of distraction affect the group's confidence?"
    - name: "Echoes of Presence"
      type: "Reaction"
      fear_cost: null
      description: "When a player makes a bold declaration or action, a subtle environmental response (like a distant sound or shifting air) hints at unseen aspects."
      questions:
        - "What unexpected response does the environment offer?"
        - "How do the characters interpret this ambiguous sign?"

encounters:
  - name: "Necrotic Bone Scavengers"
    fear: "A swarm of skeletal carrion beetles erupts from broken sarcophagi, gnawing at gear and flesh, drawn by the scent of the living."
    hope: "Successfully driving off the beetles reveals a lode of bone shards and preserved marrow, ripe for harvesting and use in cooking or crafting."

factions:
  - name: "The Ossuary Compact"
    description: "A loose alliance of bone-mages and scavenger clans seeking necromantic reagents and ancient relics among the ruins. Here, they sift through the reliquary, looking for rare corpse-flowers and spirit-imbued marrow."

points_of_interest:
  - "A shattered reliquary altar, its surface etched with glyphs that faintly glow in the presence of necromantic magic"

npcs:
  - name: "Sable Thurn"
    role: "Bone-mage Relic Hunter"
    description: "A gaunt, pragmatic mage intent on recovering a lost spirit-bound jawbone rumored to grant speech with the dead."

adventure_sites:
  - name: "The Labyrinth of Skulls"
    description: "A winding passageway formed by stacked skulls and bone fragments. Rumored to be haunted by restless spirits and containing hidden caches of valuable remains."

tags:
  - "necromancy"
  - "bonecrafting"
  - "ancient ruins"
  - "scavengers"

created_at: "2026-02-04"
---
