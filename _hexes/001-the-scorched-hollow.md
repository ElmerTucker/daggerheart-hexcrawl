---
hex_id: "001"
title: "The Scorched Hollow"
biome: "volcanic"
tier: 1
description: |
  A desolate valley where ancient volcanic activity has left the earth scarred and smoldering. Fissures vent acrid smoke, and the ground crunches underfoot with layers of black glass and ash. Despite the harsh conditions, strange heat-loving creatures have adapted to thrive here, and rumors speak of valuable minerals exposed by the geological upheaval.

  The air shimmers with heat, making distant shapes dance and waver. Travelers must watch their step—thin crusts of cooite stone often conceal pockets of scalding steam or unstable ground that can give way without warning.

environment_stat_block:
  damage_thresholds:
    minor: 3
    major: 7
    severe: 12
  features:
    - "Volcanic vents release scalding steam unpredictably"
    - "Ground is unstable; thin cruite crust may collapse"
    - "Extreme heat causes exhaustion without proper preparation"
    - "Obsidian formations provide cover but can shatter dangerously"
  instincts:
    - "The environment vents steam when creatures approach fissures"
    - "Tremors cause unstable ground to collapse"
    - "Heat intensifies during confrontations, forcing movement"

encounters:
  - name: "Ember Wraith Ambush"
    fear: "The wraiths drag a party member into a fissure, dealing severe damage and separating them from the group. The heat intensifies, and more wraiths emerge from the smoke."
    hope: "A wraith's core is exposed during the attack—destroying it causes a chain reaction that disperses the others and reveals a cache of volcanic glass worth 3 handfuls of gold."
    adversaries:
      - "Ember Wraith (3)"
      - "Smoldering Husk"
  - name: "The Obsidian Merchant"
    fear: "The merchant is actually a con artist who leads the party into a trap—the 'rare obsidian' is worthless, and hired thugs emerge from hiding to rob them."
    hope: "The merchant is genuine and grateful for safe passage. They offer to trade rare volcanic glass weapons at a significant discount and share knowledge of a safer route through the hollow."
    adversaries: []

npcs:
  - name: "Vel'kora the Ash-Touched"
    role: "Hermit Alchemist"
    description: "A burn-scarred dwarf who chose exile in the Hollow to study its unique properties. She knows the safe paths and can identify valuable minerals, but her mind has been affected by years of isolation and toxic fumes."
  - name: "Scorch"
    role: "Fire Elemental Guide"
    description: "A small, semi-sentient flame that has taken a liking to travelers. It can lead parties safely around the worst hazards, but it's easily distracted by anything flammable and may wander off at inopportune moments."

loot:
  domain: "Arcana"
  items:
    - "Obsidian Blade (volcanic glass dagger, +1 damage, shatters on critical fail)"
    - "Firewalker's Salve (3 uses, grants resistance to heat for 1 hour)"
    - "Ember Heart Gem (rare, glows with inner fire, component for fire magic)"
    - "Ash-Woven Cloak (provides advantage on stealth in smoky environments)"

landmarks:
  - "The Crying Fissure: A massive crack in the earth that constantly vents steam, creating an eerie wailing sound"
  - "Obsidian Spire: A towering natural formation of volcanic glass that serves as a navigation point"
  - "The Cooled Flow: A river of solidified lava that provides the only stable path through the valley's center"

travel_hazards:
  - "Steam Vent Fields: Random vents can erupt, requiring Agility checks to avoid burns"
  - "Unstable Ground: Areas of thin crust over hollow chambers may collapse under weight"
  - "Heat Exhaustion: Without protection, travelers must rest frequently or suffer fatigue"
  - "Toxic Fumes: Low-lying areas accumulate poisonous gases; staying too long causes disorientation"

community_ties:
  - "The Emberforge Clan maintains a small outpost at the Hollow's edge, trading in volcanic materials"
  - "A circle of druids monitors the volcanic activity, believing a slumbering fire elemental rests beneath"
  - "Smugglers use the Hollow's dangers as cover for moving illegal goods between territories"

connections: []

tags:
  - "volcanic"
  - "tier-1"
  - "hazardous"
  - "minerals"
  - "elementals"
  - "undead"

created_at: "2026-02-03"
---
