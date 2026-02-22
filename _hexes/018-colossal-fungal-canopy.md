---
hex_id: "018"
title: "Colossal Fungal Canopy"
terrain_type: "fungal forest"
region: "The Great Descent"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript area awaits, its secrets hidden in plain sight."
  impulses:
    - "Invite careful observation"
    - "Conceal small discoveries"
  difficulty: 11
  potential_adversaries:
    - "Curious wanderer"
    - "Hidden trap"
  features:
    - name: "Unremarkable Setting"
      type: "Passive"
      fear_cost: null
      description: "Checks to notice anything unusual are made with Disadvantage."
      questions:
        - "What might be overlooked by a casual glance?"
        - "How does the mundane appearance mask something important?"
    - name: "Subtle Clue"
      type: "Action"
      fear_cost: 1
      description: "Reveal a faint hint or detail to the party, requiring a successful Wit check to interpret."
      questions:
        - "What clue is almost missed?"
        - "How could a minor detail reveal a larger secret?"
    - name: "Unexpected Find"
      type: "Reaction"
      fear_cost: null
      description: "When a character searches thoroughly, they stumble upon a hidden object or passage."
      questions:
        - "What do they discover that no one else has found?"
        - "How does this discovery alter their perception of the place?"

encounters:
  - name: "Sporeback Monarch"
    fear: "The colossal spore-laden beast is disturbed and unleashes a choking cloud of toxic spores, threatening to suffocate or poison the party."
    hope: "The party can harvest rare, luminescent spore clusters from its trail, useful for powerful alchemy and cuisine."

factions:
  - name: "Mycelian Gatherers"
    description: "A secretive enclave of fungal-kin and their allies, harvesting unique growths while fiercely guarding this canopy from outsiders and rival factions."

points_of_interest:
  - "A hollowed-out titan mushroom, echoing with mysterious, flute-like calls"

npcs:
  - name: "Bleth the Sporesinger"
    role: "Mycelian Scout"
    description: "A quick-moving, bioluminescent scout who uses song to communicate with the fungal forest and warn of intruders."

adventure_sites:
  - name: "The Luminous Overhang"
    description: "A precarious platform of interwoven fungi arching out over the abyss, rumored to be home to rare edible mosses and the eggs of the Sporeback Monarch."

tags:
  - "bioluminescent"
  - "dangerous flora"
  - "rare ingredients"
  - "verticality"

created_at: "2026-02-04"
---
