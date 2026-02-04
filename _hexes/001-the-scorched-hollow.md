---
hex_id: "001"
title: "The Scorched Hollow"
terrain_type: "lava tubes"
region: "The Bitter Depths"

environment:
  name: "The Scorched Hollow"
  tier: 2
  type: "Traversal"
  description: "A network of ancient lava tubes where residual heat creates shimmering air and the walls glow with veins of cooling magma."
  impulses:
    - "Vent pressure through sudden steam eruptions"
    - "Collapse unstable passages"
    - "Draw creatures to warmth"
  difficulty: 14
  potential_adversaries:
    - "Ember Wurm"
    - "Magma Crawler"
    - "Heat-Drunk Scavengers"
    - "Obsidian Golem"
  features:
    - name: "Residual Heat"
      type: "Passive"
      fear_cost: null
      description: "The ambient temperature is dangerously high. Characters without heat protection must mark a Stress at the end of each scene spent in the Hollow."
      questions:
        - "What signs of previous expeditions lie half-melted into the walls?"
        - "How do the native creatures tolerate this heat?"
    - name: "Steam Vent Eruption"
      type: "Action"
      fear_cost: 2
      description: "A vent erupts violently. All characters in Close range must make an Agility roll against the Difficulty or take 2d8+2 physical damage from scalding steam."
      questions:
        - "What treasures were revealed when the vent cleared debris?"
        - "Did the eruption open a new passage or seal one off?"
    - name: "Unstable Ground"
      type: "Reaction"
      fear_cost: null
      description: "When a character fails a movement-related roll, the thin crust beneath them cracks. They must succeed on an additional Agility roll or fall into a pocket of extreme heat, taking 2d6+3 damage and becoming Restrained until pulled free."
      questions:
        - "What lies in the cavity below—bones, treasure, or something worse?"
        - "How do the vibrations from the collapse affect nearby creatures?"

encounters:
  - name: "The Ember Wurm's Domain"
    fear: "The wurm bursts from the wall, separating the party. Its molten body ignites the air, and smaller magma crawlers swarm from the tunnels it leaves behind."
    hope: "The party spots the wurm's heat signature before it strikes. They find a recently-shed scale worth 3 handfuls of gold and locate the wurm's abandoned nest, rich with thermal crystals."
  - name: "Scavenger Band"
    fear: "Heat-maddened scavengers ambush from above, their skin crusted with mineral deposits that grant them fire resistance. They fight without regard for their own safety, seeking to drag victims into the deeper tunnels."
    hope: "The scavengers recognize the party as fellow hunters, not prey. They're willing to trade information about the safest routes and the locations of harvestable creature dens for water and cooling supplies."

factions:
  - name: "The Ember Collective"
    description: "A cult of fire-worshippers who believe the Southern Depths house a slumbering fire god. They harvest magma creatures for ritual purposes and guard the deepest heat vents."
  - name: "Halfway Station Prospectors"
    description: "Miners from the settlement above who venture here for thermal crystals and rare heat-forged metals. They maintain emergency supply caches throughout the tubes."

points_of_interest:
  - "The Breathing Fissure: A massive crack that rhythmically vents hot air, as if the earth itself is exhaling"
  - "Crystal Grotto: A chamber where intense heat has formed natural thermal crystals worth significant gold to alchemists"
  - "The Cooled Flow: An ancient lava river now solidified into a stable pathway through the most dangerous sections"

npcs:
  - name: "Keth the Firewalker"
    role: "Ember Collective Acolyte"
    description: "A scarred human who has undergone ritual burning to prove devotion. Secretly doubts the faith but fears the Collective too much to leave. Will trade information for protection."
  - name: "Prospector Mags"
    role: "Crystal Hunter"
    description: "A grizzled dwarf who knows every safe path through the Hollow. Lost her team to an Ember Wurm last season and hunts alone now, half-seeking revenge, half-seeking death."

adventure_sites:
  - name: "The Wurm Nest"
    description: "A chamber where an Ember Wurm has made its lair, surrounded by the bones of its prey and studded with valuable thermal crystals. The wurm is currently dormant but stirs at vibrations."
  - name: "The Collective Shrine"
    description: "A hidden temple where the Ember Collective performs their rituals. Contains records of the deeper tunnels and a map to 'The Heart of Fire'—their prophesied god's resting place."

tags:
  - "tier-2"
  - "traversal"
  - "lava"
  - "creatures"
  - "faction-conflict"
  - "harvesting"

created_at: "2026-02-03"
---
