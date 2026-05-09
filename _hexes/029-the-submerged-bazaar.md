---
hex_id: "029"
title: "The Submerged Bazaar"
terrain_type: "underground lake"
region: "Halfway Station"

environment:
  name: "Unnamed Environment"
  tier: 1
  type: "Exploration"
  description: "A nondescript area inviting investigation and subtle discovery."
  impulses:
    - "Reveal hidden details"
    - "Encourage careful observation"
  difficulty: 11
  potential_adversaries:
    - "Minor wildlife"
    - "Curious onlooker"
  features:
    - name: "Subtle Clues"
      type: "Passive"
      fear_cost: null
      description: "Characters who spend time searching find minor hints or objects that may aid future checks."
      questions:
        - "What overlooked detail catches a character's eye?"
        - "How does a clue tie to a character’s background?"
    - name: "Unexpected Find"
      type: "Action"
      fear_cost: 1
      description: "Reveal a hidden compartment, loose floorboard, or secret note granting advantage on the next Discovery check."
      questions:
        - "What unexpected item is uncovered?"
        - "How might this discovery change the party’s approach?"
    - name: "Shifting Details"
      type: "Reaction"
      fear_cost: null
      description: "When a player makes a misstep or overlooks something, subtly change or obscure a minor detail, increasing the environment's difficulty by 1 until the end of the scene."
      questions:
        - "What detail becomes harder to notice?"
        - "Who realizes something has changed, and how?"

encounters:
  - name: "Lake Leviathan Bounty"
    fear: "A massive, ancient aquatic beast surfaces, threatening to capsize market rafts and send traders or hunters plunging into the depths."
    hope: "Successfully cooperating with traders and skilled fishers, the party helps subdue or appease the leviathan, earning rare monster parts and trade privileges."

factions:
  - name: "Gleamgill Brokers"
    description: "A merchant syndicate specializing in the trade of aquatic monster parts and rare lake-harvested ingredients. Their influence keeps the peace, but they're always watching for profit."
  - name: "The Salt-Eyed Order"
    description: "Ritualist fishers who believe the lake is sacred and resist over-harvesting. They broker limited access to deeper water resources in exchange for respect and offerings."

points_of_interest:
  - "Floating market platforms built from scavenged bones and giant fungal stalks"
  - "Submerged ruins beneath crystal-clear water, only visible by torchlight"

npcs:
  - name: "Marrin Tidebound"
    role: "Market Warden"
    description: "Gruff but fair, Marrin arbitrates disputes and enforces trade rules on the floating bazaar. Veteran monster-hunter with a missing hand."
  - name: "Eshri of the Salt-Eyed"
    role: "Lake Oracle"
    description: "Mysterious, masked ritualist who claims to commune with the spirits of the water. Offers cryptic advice and warnings."

adventure_sites:
  - name: "The Sunken Archive"
    description: "A partially-flooded vault below the bazaar, rumored to contain weathered journals, maps, and preserved monster specimens lost during a great deluge."

tags:
  - "market"
  - "aquatic"
  - "trade"
  - "danger"
  - "faction-territory"

created_at: "2026-02-04"
---
