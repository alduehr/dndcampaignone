# SETTLEMENT_GROVE_CAMPS_MAP.md — Settlement Map Packet

---
type: settlement
secrecy: player-safe
status: static
region: Sunmark
settlement: The Grove-Camps
level_range: 8-13
related: [../../04_world_atlas/region_map_packets/REGION_SUNMARK.md, ../../04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../../08_npcs/by_region/SUNMARK_NPCS.md, ../../09_quests/by_region/SUNMARK_QUESTS.md]
tags: [type:map, secrecy:player-safe, function:cartography, settlement-map, map-packet, grove-camps, sunmark]
---

> **Secrecy classification:** Player-safe. The Grove-Camps are the dispersed settlements of the Sunmark grove-keeper tribes — a social anchor positioned between Sunhollow and the outside world. No apex content; the faith is presented as simply working without explanation.

## Settlement: The Grove-Camps (Sunmark — dispersed grove-tribe settlements)

- **Local grid:** 0–100 (X east, Y south); (0,0) = NW corner. Not a single concentrated settlement — the Grove-Camps are a cluster of 5–8 small tribal camp-villages within a few hours' walk of each other in the warm forest. This packet represents the primary contact-camp at the Sunhollow approach.
- **Full-continent position:** render-grid (40,77) — the approximate center of the cluster; Sunhollow is nearby E (44,80; hours).
- **Population / scale:** ~400–700 across the full camp-cluster; the primary contact-camp holds ~100–150. Dispersal across the grove is a cultural and practical choice (not weakness).
- **Water/road relationship:** in the **Sunmark Wilds** warm forest; multiple small streams; the **Green Roads** (pilgrimage paths) lead NE (to Sunhollow, 44,80; hours), N (toward Marrowdowns; days–weeks), and E (toward the Hollow Gulf coast; days).

## Layout / Notable Areas (primary contact-camp)

| Area | Local | Notes |
|---|---|---|
| The Welcome-Shelter | (45,40) | the camp's meeting-shelter for visitors; where travelers are first received |
| The Grove-Keeper's Long-Tent | (35,50) | the camp-elder's tent; the local decision-point (not Sael — that's at Sunhollow) |
| The Craft-Ground | (65,55) | basket-making, medicines, bark-cloth; where the camp's daily work happens |
| The Healer's Fire | (50,65) | grove-faith healer; the best first aid on the Green Roads |
| The Green Roads junction | (55,30) | the Green Roads crossroads; three paths meet here |

## Entrances / Exits

| Exit | Local edge | Leads to |
|---|---|---|
| Green Roads (NE to Sunhollow) | (75,0) | Sunhollow / D33 (44,80; hours) |
| Green Roads (N) | (30,0) | Marrowdowns (weeks; long walk) |
| Green Roads (E, to Gulf) | (100,50) | Hollow Gulf coast approaches (days) |
| Forest interior (W) | (0,60) | deeper Sunmark Wilds (unguided; wilderness) |

## Services

| Service | Where | Details |
|---|---|---|
| Rest | Welcome-Shelter (45,40) | free for respectful visitors; safe by grove-keeper protocol |
| Resupply | Craft-Ground (65,55) | healing herbs, food, water, forest provisions; no weapons or metal |
| Healing | Healer's Fire (50,65) | grove-faith; mundane + 1st-level divine; freely given; DC 13 to ask properly |
| Information | Grove-Keeper's Long-Tent or Green Roads junction | camp-elder (DC 13); Green Roads travelers (DC 12) |
| Faction contact | Welcome-Shelter | grove-keeper tribes; the camp-elder directs to Sael at Sunhollow for major matters |

## Law and Threat DCs

- **Entering the Grove-Camps:** respectful approach; same protocol as Sunhollow — weapons sheathed, Persuasion DC 13. Even more informal than Sunhollow; the camp-elder is welcoming.
- **Disrespecting the Healer's Fire:** the camp mobilizes (50+ grove-keepers from nearby camps; DC 14 to explain before escalation).
- **Being directed toward Sunhollow:** the camp-elder always sends serious matters to Sael (DC 13 to understand this is respectful, not a brush-off).

## Key NPC Links

| NPC | Role | Location | Notes |
|---|---|---|---|
| Grove-Keeper Sael Sunmark | grove head | at Sunhollow (44,80), not the Grove-Camps | the camp-elder directs all major matters to Sael |
| Greenway-Warden Tamsin Greenway | road-captain; secondary NPC | Green Roads junction (55,30; patrols) | DC 14; knows the Green Roads better than anyone; guards pilgrims |

## Quest Hooks

- **Q_SUN_001 — The Saw at the Grove (early warning):** Ledger logging-scouts are spotted on the E Green Roads before reaching Sunhollow; the camp-elder reports it to arriving travelers (L8; on-ramp to the Sunmark arc).
- **Q_SUN_006 — Green Roads escort:** Greenway-Warden Tamsin needs a companion to accompany a pilgrim-group safely to Sunhollow (minor; L8+; establishes the camp's social connections).
- **Healer's Fire access:** the best first-aid between the Marrowdowns and the Sunmark coast (free healing; earns trust for Sunhollow approach; L8+).

## Encounter / Treasure References

- Encounter: grove-keeper warriors if threatened (**Tribal Warrior-like**, AC 13–14, significant numbers in hours); Green Roads bandits (rare; Doss Sunward's logging-scouts are not combat-oriented); see L8+ forest encounter lines.
- Treasure: `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` Tier 2 (L6–11) — grove-faith gifts (healing herb kits, forest provisions, safe-guide to Sunhollow); no monetary rewards here.

## Player-Safe Layer

The warm forest camp; the welcoming shelter; the healer's fire; the Green Roads junction with its three paths; the camp-elder's direction toward Sunhollow for anything important. A gentle, open, non-threatening first contact point with the Sunmark grove culture.

## Related Files

- Region: [`../../04_world_atlas/region_map_packets/REGION_SUNMARK.md`](../../04_world_atlas/region_map_packets/REGION_SUNMARK.md)
- Grove-heart: [`SETTLEMENT_SUNHOLLOW_MAP.md`](SETTLEMENT_SUNHOLLOW_MAP.md)
- NPCs: [`../../08_npcs/by_region/SUNMARK_NPCS.md`](../../08_npcs/by_region/SUNMARK_NPCS.md)
- Quests: [`../../09_quests/by_region/SUNMARK_QUESTS.md`](../../09_quests/by_region/SUNMARK_QUESTS.md)
