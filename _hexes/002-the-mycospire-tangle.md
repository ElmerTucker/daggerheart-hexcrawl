---
hex_id: "002"
title: "The Mycospire Tangle"
terrain_type: "fungal forest"
region: "The Descent Shafts"

environment:
  name: "Mycospire Tangle"
  tier: 3
  type: "Traversal"
  description: "Dense fungal forest threaded with vertical stalks and hanging spore-veils, requiring careful climbing and navigation"
  impulses:
    - "Obscure safe paths"
    - "Reward clever climbing or navigation"
    - "Conceal danger among beauty"
  difficulty: 17
  potential_adversaries:
    - "Spore-maddened chasm gliders"
    - "Fungal ambushers"
    - "Territorial fungal colonies"
  features:
    - name: "Vertical Fungal Pillars"
      type: "Traversal"
      fear_cost: 2
      description: "Navigating the forest requires perilous climbing between thick, slippery stalks, with spore clouds obscuring handholds and vision."
      questions:
        - "What rare fungus can only be reached by scaling the tallest stalks?"
        - "What lurks in the shadows between the columns?"
    - name: "Spore Veil Hazards"
      type: "Hazard"
      fear_cost: 1
      description: "Disturbed veils release clouds that can induce hallucinations or drowsiness if inhaled."
      questions:
        - "Who among the party is most vulnerable to these spores?"
        - "What visions or memories do the spores awaken?"
    - name: "Hidden Mycogroves"
      type: "Discovery"
      fear_cost: null
      description: "Careful navigation can reveal pockets of edible or medicinal mushrooms, as well as traces of prior explorers."
      questions:
        - "Which resource is desperately needed by the group?"
        - "What signs of another faction or lost party are found here?"

encounters:
  - name: "Spore-Maddened Chasm Glider"
    fear: "The creature swoops from above, scattering spores as it attacks, threatening to knock explorers into the depths below."
    hope: "The glider can be frightened off or harvested for unique wing membranes prized for crafting lightweight armor."

factions:
  - name: "The Green Veil"
    description: "A secretive band of fungal cultivators who harvest rare spores and fiercely guard their hidden groves from outsiders."

points_of_interest:
  - "A bioluminescent fungal bridge spanning a deep shaft"

npcs:
  - name: "Mosa the Spore-Warden"
    role: "Fungal forest guide and negotiator"
    description: "A wary, masked member of the Green Veil with deep knowledge of edible and dangerous fungi, offering guidance—at a price."

adventure_sites:
  - name: "The Hanging Mycarium"
    description: "A suspended, web-like fungal garden cultivated by the Green Veil; entry is by negotiation or stealth, but its rare edibles fetch a high price."

tags:
  - "verticality"
  - "fungus"
  - "navigation"
  - "resources"
  - "territorial"

created_at: "2026-02-04"
---
