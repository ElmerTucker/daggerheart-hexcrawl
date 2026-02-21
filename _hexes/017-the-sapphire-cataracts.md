---
hex_id: "017"
title: "The Sapphire Cataracts"
terrain_type: "cavern"
region: "The Weeping Gallery"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript area with subtle details waiting to be uncovered."
  impulses:
    - "Hide secrets just out of sight"
    - "Encourage careful observation"
  difficulty: 11
  potential_adversaries:
    - "Wandering animal"
    - "Curious local"
  features:
    - name: "Unremarkable Facade"
      type: "Passive"
      fear_cost: null
      description: "PCs must succeed on a Discovery check to notice anything unusual; otherwise, the environment appears mundane."
      questions:
        - "What minor detail hints at something hidden?"
        - "How does the environment subtly resist examination?"
    - name: "Obscured Clues"
      type: "Action"
      fear_cost: 1
      description: "The GM may spend 1 Fear to further obscure a clue or complicate a search, increasing the next relevant check’s difficulty by 2."
      questions:
        - "What natural feature cleverly conceals information?"
        - "How does the environment momentarily distract the PCs?"
    - name: "Subtle Resistance"
      type: "Reaction"
      fear_cost: null
      description: "When a PC attempts to forcefully alter or disturb the environment, they risk drawing unwanted attention or triggering a minor hazard."
      questions:
        - "What small consequence makes the PCs reconsider their approach?"
        - "Who or what might notice the PCs' disturbance?"

encounters:
  - name: "Azure Eel Migration"
    fear: "A surge of razor-finned eels blocks passage, potentially shocking or biting anyone in their way."
    hope: "The party can harvest delicious, energizing eel fillets or rare electric glands if cautious."

factions:
  - name: "The Deepwater Foragers"
    description: "A band of amphibious gatherers harvesting rare aquatic plants and organisms, fiercely defending their territory from poachers."

points_of_interest:
  - "Glittering Sapphire Veil (cascading mineral curtain across a waterfall pool)"

npcs:
  - name: "Vella of the Pools"
    role: "Deepwater Forager Scout"
    description: "A vigilant, web-footed scout who knows every eddy and hidden den in the Cataracts."

adventure_sites:
  - name: "The Submerged Archive"
    description: "A collapsed ruin beneath the waterfall, filled with preserved scrolls and relics, accessible only during rare dry seasons or with clever aquatic traversal."

tags:
  - "water"
  - "mineral"
  - "rare ingredients"
  - "tier 4"

created_at: "2026-02-04"
---
