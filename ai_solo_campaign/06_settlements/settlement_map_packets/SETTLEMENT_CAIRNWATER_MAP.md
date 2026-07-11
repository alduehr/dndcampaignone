# SETTLEMENT_CAIRNWATER_MAP.md — Settlement Map Packet

---
type: settlement
secrecy: player-safe
status: static
region: Glassmere League
settlement: Cairnwater
level_range: 9-14
related: [../../04_world_atlas/region_map_packets/REGION_GLASSMERE_LEAGUE.md, ../../04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../../08_npcs/by_region/GLASSMERE_LEAGUE_NPCS.md, ../../09_quests/by_region/GLASSMERE_LEAGUE_QUESTS.md, ../../06_settlements/city_map_packets/GLASSMERE_CITY_MAP.md]
tags: [type:map, secrecy:player-safe, function:cartography, settlement-map, map-packet, cairnwater, glassmere-league]
---

> **Secrecy classification:** Player-safe. Cairnwater is a smaller Glassmere League city — named-in-passing, not deep-built. Full political depth at Glassmere city. No apex content.

## Settlement: Cairnwater (Glassmere League — secondary league city, W corridor)

- **Local grid:** 0–100 (X east, Y south); (0,0) = NW corner. Walled city at the W end of the League Road; gateway from the Concord Heartlands and Karran Marches into the League.
- **Full-continent position:** render-grid (60,30).
- **Population / scale:** ~4,000–6,000; larger than Sennfort; the western-approach gateway; League's frontier-facing city.
- **Water/road relationship:** on the upper **Glasswater** (smaller at this point); the **League Road** runs E (to Sennfort 56,32, then Glassmere 57,36); the **Heartlands Track** leads NE (toward Concord Heartlands, weeks); the **Karran Road** leads N (toward Karran Marches, weeks).

## Layout / Notable Areas

| Area | Local | Notes |
|---|---|---|
| The West Gate | (15,50) | main frontier gate; heavier inspection than interior League cities |
| The Factor's House | (40,35) | league commercial authority; frontier-trade licensing |
| The Market (covered) | (60,50) | covered market; frontier goods including salvage and raw ore |
| The Armorer's Row | (70,40) | weapons and armor; frontier-frontier trade |
| The Customs House | (35,65) | Compact-adjacent inspection post; relic and salvage declaration |
| The River House Inn | (55,65) | rest; 3sp/night; the major meeting-place |

## Entrances / Exits

| Exit | Local edge | Leads to |
|---|---|---|
| League Road (E) | (100,50) | Sennfort (56,32; days), then Glassmere |
| Heartlands Track (NE) | (100,20) | Concord Heartlands (63,56; weeks) |
| Karran Road (N) | (55,0) | Karran Marches (weeks; dangerous) |
| Glasswater (S, headwaters) | (60,100) | river narrows; local farmland only |

## Services

| Service | Where | Details |
|---|---|---|
| Rest | River House Inn (55,65) | 3sp/night; safe; League-standard |
| Resupply | Covered Market (60,50) | frontier goods; armor, weapons, salvage-equipment; most standard goods |
| Healing | Factor's House (affiliated healer) | mundane + 2nd-level divine; DC 14 |
| Information | Factor's House or Market | Factor (DC 15); frontier travelers (DC 12) |
| Faction contact | Customs House | Compact-adjacent; Remnant chapter minor presence; Heartlands expedition-contacts |

## Law and Threat DCs

- **Entering Cairnwater:** West Gate inspection (frontier-facing: stricter); League permit or Persuasion DC 15.
- **Carrying salvage / relics:** Customs House declaration required; DC 15 to declare honestly; DC 17 to smuggle past (riskier here than at Sennfort).
- **Violent act:** city watch (40 guards at frontier-strength, **Guard/Veteran-like**, AC 14–16).

## Key NPC Links

| NPC | Role | Location | Notes |
|---|---|---|---|
| (unnamed frontier factor) | League gateway authority | Factor's House | secondary NPC; DC 15; frontier-focused |
| Reclaimer-Captain Wenna Stone | Remnant NE expedition | periodic (en route from Karran) | Persuasion DC 17; turnable; passes through Cairnwater |

## Quest Hooks

- **Local hook — "The Frontier Salvage"** (no developed quest file; improv-safe; routes into `../../09_quests/by_region/GLASSMERE_LEAGUE_QUESTS.md` threads): a Heartlands expedition has brought something through the West Gate that the Customs House wants held; multiple parties want it (L11+).
- **Wenna Stone passage:** Cairnwater is where Wenna Stone resupplies before/after the Karran Marches expedition; a contact point for Q_KM_003 (L12+).

## Encounter / Treasure References

- Encounter: frontier road-bandits between Cairnwater and the Heartlands/Karran approaches (Veteran-like, CR 5–9; L9+); Heartlands rival-expedition teams (Veteran-like).
- Treasure: `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` Tier 2–3 frontier and League-contract rewards.

## Unresolved Map Gaps

Cairnwater is a "named-in-passing" anchor per `NAMING_REGISTRY.md`. Full district-depth is not required; this packet provides eagle-test landing capacity only.

## Related Files

- Region: [`../../04_world_atlas/region_map_packets/REGION_GLASSMERE_LEAGUE.md`](../../04_world_atlas/region_map_packets/REGION_GLASSMERE_LEAGUE.md)
- City: [`../../06_settlements/city_map_packets/GLASSMERE_CITY_MAP.md`](../../06_settlements/city_map_packets/GLASSMERE_CITY_MAP.md)
- NPCs: [`../../08_npcs/by_region/GLASSMERE_LEAGUE_NPCS.md`](../../08_npcs/by_region/GLASSMERE_LEAGUE_NPCS.md)
- Quests: [`../../09_quests/by_region/GLASSMERE_LEAGUE_QUESTS.md`](../../09_quests/by_region/GLASSMERE_LEAGUE_QUESTS.md)
