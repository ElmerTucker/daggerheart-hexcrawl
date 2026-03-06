---
hex_id: "030"
title: "Lake Vitriol"
terrain_type: "underground lake"
region: "The Bitter Depths"

environment:
  name: "Acidic Lake of the Deep"
  tier: 4
  type: "Exploration"
  description: "A nondescript area filled with subtle clues and quiet mysteries awaiting discovery."
  impulses:
    - "Conceal hidden details"
    - "Invite careful observation"
  difficulty: 11
  potential_adversaries:
    - "Curious local"
    - "Wandering beast"
  features:
    - name: "Subtle Clues"
      type: "Passive"
      fear_cost: null
      description: "Characters who closely examine their surroundings may notice faint traces, hidden objects, or overlooked details with a successful Exploration roll."
      questions:
        - "What detail stands out upon closer inspection?"
        - "How does the environment reward patience and observation?"
    - name: "Echoes of Movement"
      type: "Action"
      fear_cost: 1
      description: "The GM may introduce a faint sound, shifting shadow, or minor disturbance, prompting players to investigate or feel watched."
      questions:
        - "What draws the characters’ attention unexpectedly?"
        - "Does the disturbance hint at danger or opportunity?"
    - name: "Hidden Obstruction"
      type: "Reaction"
      fear_cost: null
      description: "When a character attempts to move quickly or act without caution, they may stumble over a concealed obstacle, slowing their progress or causing minor inconvenience."
      questions:
        - "What unexpected hazard slows the characters down?"
        - "How does the environment subtly punish haste?"

encounters:
  - name: "Vitriol Serpent"
    fear: "The colossal acid serpent bursts from the water, spitting corrosive venom and threatening to drag hunters beneath the burning waves."
    hope: "The serpent is distracted by a rare mineral cluster, allowing a skilled hunter to harvest acid-hardened scales and rare organ-glands."

factions:
  - name: "The Causticfaith"
    description: "A zealous group that worships the lake’s corrosive power, gathering acid-touched relics and fiercely defending the shore from trespassers."

points_of_interest:
  - "Shoreline of crystallized bone and mineral, pocked with bubbling acid vents"

npcs:
  - name: "Mist-Tongue Zara"
    role: "Hermit-Guide"
    description: "A mutated loner whose skin shimmers with acid scars; Zara knows safe paths and which creatures taste best after proper soaking."

adventure_sites:
  - name: "The Searing Jetty"
    description: "A precarious platform of rusted metal and petrified wood jutting into the lake, used by hunters to fish for acid-resistant prey or lower cages into the depths."

tags:
  - "acid"
  - "lake"
  - "mutation"
  - "rare-resources"
  - "tier-4"

created_at: "2026-02-04"
---
