# SETTLEMENT_SENNFORT_MAP.md — Settlement Map Packet

---
type: settlement
secrecy: player-safe
status: static
region: Glassmere League
settlement: Sennfort
level_range: 9-14
related: [../../04_world_atlas/region_map_packets/REGION_GLASSMERE_LEAGUE.md, ../../04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../../08_npcs/by_region/GLASSMERE_LEAGUE_NPCS.md, ../../09_quests/by_region/GLASSMERE_LEAGUE_QUESTS.md, ../../06_settlements/city_map_packets/GLASSMERE_CITY_MAP.md]
tags: [type:map, secrecy:player-safe, function:cartography, settlement-map, map-packet, sennfort, glassmere-league]
---

> **Secrecy classification:** Player-safe. Sennfort is a smaller Glassmere League city — a named-in-passing anchor, not deep-built. Full political depth is at Glassmere city. No apex content here.

## Settlement: Sennfort (Glassmere League — secondary league city)

- **Local grid:** 0–100 (X east, Y south); (0,0) = NW corner. Upriver walled city on the Glasswater; compact mercantile center; Glassmere road W.
- **Full-continent position:** render-grid (56,32).
- **Population / scale:** ~3,000–5,000; a secondary Glassmere League city; full civic structure but smaller than Glassmere. Not deep-built.
- **Water/road relationship:** on the **Glasswater** upstream from Glassmere (57,36); the river is navigable here (shallow-draft barges only); the **League Road** runs W–E (Cairnwater 60,30 to Glassmere 57,36).

## Layout / Notable Areas

| Area | Local | Notes |
|---|---|---|
| The League-Gate | (20,50) | main city gate; League toll collected; standard inspection |
| The Factor's Hall | (45,35) | local league-factor's offices; commercial licensing |
| The Glasswater Quay | (65,65) | shallow-draft barge dock; N route toward Cairnwater |
| The Market Square | (50,55) | standard market; League-regulated trade |
| The Three Thresholds Chapel | (35,65) | Threshold faith; standard civic shrine |
| The Traveler's Inn | (60,45) | safe mid-quality rest; 3sp/night |

## Entrances / Exits

| Exit | Local edge | Leads to |
|---|---|---|
| League Road (W) | (0,50) | Cairnwater (60,30; days) |
| League Road (E) | (100,50) | Glassmere (57,36; days) |
| Glasswater (S, by barge) | (65,100) | Glassmere downstream (faster) |
| Upriver track (N) | (50,0) | Concord Heartlands approaches (weeks) |

## Services

| Service | Where | Details |
|---|---|---|
| Rest | Traveler's Inn (60,45) | 3sp/night; safe; League-standard quality |
| Resupply | Market Square (50,55) | League-regulated standard market; most goods available |
| Healing | Three Thresholds Chapel (35,65) | mundane + 2nd-level divine; Persuasion DC 13 |
| Information | Factor's Hall or Market | Factor (DC 15); Market news (DC 12) |
| Faction contact | Factor's Hall | Glassmere League commercial arm; Remnant chapter-house minor presence |

## Law and Threat DCs

- **Entering Sennfort:** League-gate inspection; standard toll (1gp) or Persuasion DC 13.
- **Commercial activity without League license:** Factor's fine (5gp) or Persuasion DC 14.
- **Violent act:** city watch (30 guards, **Guard-like**, AC 14); standard League city response.

## Key NPC Links

| NPC | Role | Location | Notes |
|---|---|---|---|
| (unnamed local factor) | League commercial authority | Factor's Hall | secondary NPC; Persuasion DC 15; not in NAMING_REGISTRY (background figure) |
| Reliquary-Lector Mareth Senn | Glassmere Remnant chapter-head | visiting from Glassmere (seasonal) | Persuasion DC 17; the Sennfort name-connection is coincidence (per NAMING_REGISTRY) |

## Quest Hooks

- **Leg of the Glassmere arc:** Sennfort is a transit stop on the way to/from Glassmere; League politics and the Reliquary-Lector's visits make it a secondary complication.
- **Q_GL_XXX — Sennfort waypoint hook:** local League-factional dispute (wool-tax; upriver access rights); on-ramp into Glassmere League politics (L9+).

## Encounter / Treasure References

- Encounter: city watch (**Guard-like**, AC 14); League road-bandit suppression (the road between Sennfort and Cairnwater needs policing occasionally; Veteran-like, L9+).
- Treasure: `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` Tier 2–3 League trade rewards; Factor's commercial payment.

## Unresolved Map Gaps

Sennfort is a "named-in-passing" anchor per `NAMING_REGISTRY.md`. Full district-depth is not required; this packet provides eagle-test landing capacity only. The Reliquary and Three Bridges (Glassmere's key landmarks) are not here — see `GLASSMERE_CITY_MAP.md`.

## Related Files

- Region: [`../../04_world_atlas/region_map_packets/REGION_GLASSMERE_LEAGUE.md`](../../04_world_atlas/region_map_packets/REGION_GLASSMERE_LEAGUE.md)
- City: [`../../06_settlements/city_map_packets/GLASSMERE_CITY_MAP.md`](../../06_settlements/city_map_packets/GLASSMERE_CITY_MAP.md)
- NPCs: [`../../08_npcs/by_region/GLASSMERE_LEAGUE_NPCS.md`](../../08_npcs/by_region/GLASSMERE_LEAGUE_NPCS.md)
- Quests: [`../../09_quests/by_region/GLASSMERE_LEAGUE_QUESTS.md`](../../09_quests/by_region/GLASSMERE_LEAGUE_QUESTS.md)
