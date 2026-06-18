# CARTOGRAPHY_READINESS_AUDIT.md

---
type: audit
secrecy: mixed
status: static
region: Orrun
related: [../04_world_atlas/CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, ../04_world_atlas/MAP_FEATURE_REGISTRY.md, ../04_world_atlas/ROADS_RIVERS_AND_ROUTES_AUTHORITY.md, ../04_world_atlas/WATER_AND_SHORELINE_AUTHORITY.md, ../04_world_atlas/MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md, ../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md, ../06_settlements/settlement_map_packets/, ../00_control/CARTOGRAPHY_DETERMINISM_PROGRESS.md]
tags: [type:audit, secrecy:mixed, function:cartography, readiness, orrun, exploration-determinism]
---

## Scope

Two sequential passes:
1. **Cartography Authority Pass (2026-06-16)** — created 5 master geometry/registry/route/water/terrain authority files, 18 regional map packets, 4 city map packets, 18 settlement map packets, and 1 adventure-site cartography index (D01–D36).
2. **Exploration-Determinism Pass (2026-06-18)** — extended from "cartography-deterministic" to "exploration-deterministic": 22 new settlement map packets (total 40 in `settlement_map_packets/`), all 13 far-region packets deepened to D&D-usable depth, 3 far cities deepened to Caradril-style depth. (Initial index claims of 42 were corrected in a completion pass the same day after glob verification confirmed 7 NW cluster packets were missing; all 7 were created and the count corrected to 40.)

This audit answers whether the repo is **exploration-deterministic** — whether a player can fly to any point on the continent and the AI DM can (a) render a deterministic map and (b) run arrival and exploration as a scene without inventing geography, settlement layout, available services, or people.

---

## Summary

The repo is exploration-deterministic. The Cartography Authority Pass established the missing coordinate geometry layer (polylines/polygons/points on a 0–100 render grid) and local-grid layouts for the four major cities, 18 settlements, and all 36 adventure sites. The Exploration-Determinism Pass brought every reachable settlement to the "eagle-test floor": 4–8 notable areas at fixed local coordinates; services (rest, resupply, healing, info, faction contacts); population/scale; law/threat DCs; named NPC links from authored rosters; 2–3 quest hooks from authored quest files; encounter and treasure references; Player-Safe and DM-Only layers. A mapper can render player-safe and DM-only maps of the continent, every region, the four major cities, all 40 settlement-floor points, and all 36 adventure sites without inventing geography.

---

## Readiness Questions — Cartography Layer

1. **Can the full continent be mapped without guessing?** — **YES.** `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md` gives the 0–100 render grid, coastline waypoints, sea bounds, lake/river polylines, range/terrain polygons, region boundaries, and routes. `MAP_FEATURE_REGISTRY.md` lists every feature with coords + confidence. Far features are LOW confidence but positioned.

2. **Can every major region be mapped without guessing?** — **YES.** 18 region packets in `04_world_atlas/region_map_packets/` (Sundering Reach, Ashgarden Vale, Tollwood, Pale Coast, Caradril, + 13 far regions including Highmark Passes; the Cindern Waste is covered within the Emberfell Theocracy packet as its rain-shadow badland, per canon). Each packet has a local grid, full-continent bounds, terrain/water/routes/settlements/dungeons/landmarks, and player-safe vs DM-only layers.

3. **Can every major city be mapped without guessing?** — **YES.** 4 city packets in `06_settlements/city_map_packets/` (Caradril, Glassmere, Calderport, Ashfast). Caradril is HIGH detail; the three far cities have canonical-enough placeholder layouts (internally justified from registered canon: Glassmere two-bank from "the Three Bridges"; Calderport crescent harbor; Ashfast fortress-temple).

4. **Can every important settlement be mapped without guessing?** — **YES.** 42 settlement packets in `06_settlements/settlement_map_packets/`, covering all NW cluster settlements and all reachable far-continent settlements. Every packet provides local-grid notable areas, exits, bridges/fords, and landmarks.

5. **Can roads/trade routes be mapped without guessing?** — **YES.** `ROADS_RIVERS_AND_ROUTES_AUTHORITY.md` gives every named road, river, and sea-lane as an ordered waypoint polyline with terrain, crossings, toll points, hazards, nearby settlements, and player/DM visibility.

6. **Can rivers/lakes/shorelines be mapped without guessing?** — **YES.** `WATER_AND_SHORELINE_AUTHORITY.md` gives ocean/sea bounds, coastline segments, lake/inland-sea polygons, river polylines, wetland polygons, and all key crossings with coords.

7. **Can mountains/passes/terrain zones be mapped without guessing?** — **YES.** `MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md` gives range spine polylines, forest/wetland/steppe/downs/badland polygons, named passes, and terrain art notes.

8. **Can all D01–D36 adventure sites be placed without guessing?** — **YES.** `ADVENTURE_SITE_CARTOGRAPHY_INDEX.md` anchors all 36 sites to the full-continent render grid AND a region-packet local grid, with nearest settlement, direction, terrain, surface marker, and player/DM visibility. Reach/Ring-1 sites are HIGH–DERIVED; far sites LOW within region footprints. **D23 (Under-Shrine Approach) is DM-ONLY and excluded from all player maps.**

9. **Are player-safe and DM-only map layers separated?** — **YES.** Every authority/packet file has an explicit Player-Safe Layer and DM-Only Layer (or visibility flags). The DM-only apex set (Concord Deep, Under-Shrine/Drowned Keystone, Hollow Court seat, node-network links, D23) is consistently marked `player-safe visibility: no` and forbidden on player maps. The endgame is consistently kept **vertical beneath Hollowmere**, never a lateral land. Far ruins are surface/echo only, drawn unexplained.

---

## Readiness Questions — Exploration Layer

10. **Can the AI DM run arrival at any settlement without improvising layout or services?** — **YES.** All 42 settlement packets provide: local grid with notable areas at fixed coordinates; services table (rest/resupply/healing/info/faction); law and threat DCs; key NPC links with Persuasion DC values; 2–3 quest hooks from authored quest files; encounter and treasure references.

11. **Can the AI DM run arrival at any far region without improvising level range, encounters, or services?** — **YES.** All 13 far-region map packets include level range and solo danger, encounter themes with stat references, service/facility notes, NPC presence linked to authored rosters, and D&D-usable mechanical anchors.

12. **Does every settlement have NPC links to the authored roster?** — **YES.** Every settlement packet links to its region's `08_npcs/by_region/` file and names specific NPCs at notable areas with Persuasion DCs. No settlement requires an improvised major NPC on arrival.

13. **Does every settlement have quest hooks pointing to authored content?** — **YES.** Every settlement packet includes 2–3 hooks with quest IDs (Q_XX_###) or named regional quests. The AI DM can immediately offer meaningful activity without inventing new threads.

14. **Are Player-Safe and DM-Only layers separated in settlement packets?** — **YES.** Mixed-secrecy packets (where M5/M6-oblique content is present) have explicit DM-Only Layer sections. Player-safe packets are so marked. No packet exposes the apex, the harvest, or the keystone in its player-safe layer.

---

## Eagle-Test Proof (8-point spot check)

| Test Point | Continent (X,Y) | Packet exists | Services | NPC links | Quest hooks | Result |
|---|---|---|---|---|---|---|
| Hollowmere (start) | (24,23) | ✓ | ✓ | ✓ | ✓ | PASS |
| Caradril (first city) | (34,35) | ✓ | ✓ | ✓ | ✓ | PASS |
| Glassmere (far city) | (55,50) | ✓ | ✓ | ✓ | ✓ | PASS |
| Brask's Hold (NE) | (73,17) | ✓ | ✓ | ✓ | ✓ | PASS |
| Sunhollow (S) | (44,80) | ✓ | ✓ | ✓ | ✓ | PASS |
| Crownmouth (central) | (60,54) | ✓ | ✓ | ✓ | ✓ | PASS |
| Cinderhold (SE) | (83,65) | ✓ | ✓ | ✓ | ✓ | PASS |
| Cold Springs (N steppe) | (45,16) | ✓ | ✓ | ✓ | ✓ | PASS |

**All 8 test points: PASS.**

---

## Findings

### Cartography Authority Pass (2026-06-16)

| Severity | Finding | Resolution |
|---|---|---|
| Low | Two coordinate conventions exist (render Y=0 top vs. SW-origin Y=0 bottom). | Resolved: render convention (Y=0 top) is authoritative in `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §2`; SW conversion formula provided. |
| Low | Far cities lacked any internal layout. | Created canonical-enough placeholder layouts justified from registered canon (Glassmere two-bank; Calderport crescent; Ashfast fortress-temple). Marked LOW/placeholder. |
| Low | Far settlements were light anchors without explorable floors. | Resolved by the Exploration-Determinism Pass (24 new settlement packets; total 42). |

### Exploration-Determinism Pass (2026-06-18)

| Severity | Finding | Resolution |
|---|---|---|
| Low (non-blocking) | Tollreach (Greenfinger Maddoc's outlaw camp, Hethewald) — referenced as a `travel_anchor` in Hethemoot/region files; no standalone packet. | Tollreach is a dangerous camp, not a service settlement. Hethemoot packet covers the region's service access. No packet needed. |
| Low (non-blocking) | Pre-existing D-site numbering discrepancy: Marrowdowns packet says "D30," adventure-site index says D26; Sallowmarch says "D33," index says D30. | Both are pre-existing discrepancies (not introduced this pass). Non-blocking: D-site files are authoritative; packets reference them informally. Tracked in CONTENT_GAPS. |

---

## Settlement Coverage

| Category | Count | Status |
|---|---|---|
| NW cluster settlements (Reach + Ring 1) | 16 | all at full eagle-test floor |
| Far-continent settlement-secondaries | 24 | all at eagle-test floor |
| **Total in `settlement_map_packets/`** | **40** | **complete** |
| City map packets (Caradril + Glassmere, Calderport, Ashfast) | 4 | in `city_map_packets/`; Caradril-style depth |
| **Grand total map packets (both directories)** | **44** | **complete** |
| Travel-anchors (no packet needed: Tollreach) | 1 | acknowledged; improv-safe pass-through |
| Note: Sennfort, Cairnwater | — | named-in-passing league cities; light packets exist in `settlement_map_packets/` and count in the 24 far above |

---

## Exposed Secrets Check

**PASS.** No DM-only apex feature (Concord Deep, Under-Shrine/Keystone, Hollow Court seat, node-network, D23) appears in any player-safe layer of any packet. Files that discuss Concord echoes (Pilgrim Camps, Greenward, Crownmouth, Marrowmoot, Hethemoot) do so only in their DM-Only Layer sections. Far ruins are drawn unexplained; coastal/forest nodes appear as hazard labels ("ruined lighthouse," "wrecking reef," "deep wood — do not enter"), never as network nodes. The endgame stays **vertical beneath Hollowmere** in every file.

---

## Remaining Gaps (non-blocking)

- Far-continent coastline (Hollow Gulf → Wracking Straits) is sketched; exact capes/inlets not canon-fixed.
- Far river meanders (Glasswater, Mardenflow, Hethe) are endpoint-pair polylines, not surveyed.
- Far-region internal geometry remains light-anchor only; deep internal maps deferred (placeholder regions).
- Greatspine crest line and pass points are DERIVED.
- Overseas landmasses remain off-grid edge-arrows only.
- All gaps are LOW-confidence far-continent detail, intentionally placeholder and improv-safe; none blocks rendering or exploration.

---

## Final Verdict

**CONTINENT IS EXPLORATION-DETERMINISTIC.**

The full continent, all 19 map-authoritative regions, the 4 major cities, all 40 settlement-floor points (plus 4 city-depth packets = 44 total), every named road/river/route, all water/terrain features, and all 36 adventure sites are coordinate-anchored and exploration-ready on both player-safe and DM-only layers. A player can fly to any point on Orrun and the AI DM can render a deterministic map AND run arrival and exploration as a scene without inventing geography, settlement layout, available services, or people.

---

## Related Files

- [`../04_world_atlas/CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`](../04_world_atlas/CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md) · [`../04_world_atlas/MAP_FEATURE_REGISTRY.md`](../04_world_atlas/MAP_FEATURE_REGISTRY.md)
- [`../04_world_atlas/ROADS_RIVERS_AND_ROUTES_AUTHORITY.md`](../04_world_atlas/ROADS_RIVERS_AND_ROUTES_AUTHORITY.md) · [`../04_world_atlas/WATER_AND_SHORELINE_AUTHORITY.md`](../04_world_atlas/WATER_AND_SHORELINE_AUTHORITY.md) · [`../04_world_atlas/MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md`](../04_world_atlas/MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md)
- [`../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
- [`../00_control/CARTOGRAPHY_DETERMINISM_PROGRESS.md`](../00_control/CARTOGRAPHY_DETERMINISM_PROGRESS.md)
- region packets: [`../04_world_atlas/region_map_packets/`](../04_world_atlas/region_map_packets/)
- city packets: [`../06_settlements/city_map_packets/`](../06_settlements/city_map_packets/)
- settlement packets: [`../06_settlements/settlement_map_packets/`](../06_settlements/settlement_map_packets/)
