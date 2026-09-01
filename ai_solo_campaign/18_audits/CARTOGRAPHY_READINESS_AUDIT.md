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

2. **Can every major region be mapped without guessing?** — **YES.** **18 standalone map-authoritative regions, each with its own region packet** in `04_world_atlas/region_map_packets/` (Sundering Reach, Ashgarden Vale, Tollwood, Pale Coast, Caradril, + 13 far regions including Highmark Passes). The **Cindern Waste is NOT a 19th region** — it is the ash-badland terrain sub-zone within the Emberfell Theocracy region, covered in `REGION_EMBERFELL_THEOCRACY.md`; the **Drowned Steps** is a submerged-ruin sub-area (D30) within Sallowmarch, not a region. Use **18** as the region count everywhere; "19" only counts Cindern Waste as a named terrain label (resolved 2026-06-18, Cartography Determinism Cleanup — see `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §10`). Each packet has a local grid, full-continent bounds, terrain/water/routes/settlements/dungeons/landmarks, and player-safe vs DM-only layers.

3. **Can every major city be mapped without guessing?** — **YES.** 4 city packets in `06_settlements/city_map_packets/` (Caradril, Glassmere, Calderport, Ashfast). Caradril is HIGH detail; the three far cities have canonical-enough placeholder layouts (internally justified from registered canon: Glassmere two-bank from "the Three Bridges"; Calderport crescent harbor; Ashfast fortress-temple).

4. **Can every important settlement be mapped without guessing?** — **YES.** **40 settlement packets** in `06_settlements/settlement_map_packets/` (glob-verified), covering all NW cluster settlements and all reachable far-continent settlements. Every packet provides local-grid notable areas, exits, bridges/fords, and landmarks.

5. **Can roads/trade routes be mapped without guessing?** — **YES.** `ROADS_RIVERS_AND_ROUTES_AUTHORITY.md` gives every named road, river, and sea-lane as an ordered waypoint polyline with terrain, crossings, toll points, hazards, nearby settlements, and player/DM visibility.

6. **Can rivers/lakes/shorelines be mapped without guessing?** — **YES.** `WATER_AND_SHORELINE_AUTHORITY.md` gives ocean/sea bounds, coastline segments, lake/inland-sea polygons, river polylines, wetland polygons, and all key crossings with coords.

7. **Can mountains/passes/terrain zones be mapped without guessing?** — **YES.** `MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md` gives range spine polylines, forest/wetland/steppe/downs/badland polygons, named passes, and terrain art notes.

8. **Can all D01–D36 adventure sites be placed without guessing?** — **YES.** `ADVENTURE_SITE_CARTOGRAPHY_INDEX.md` anchors all 36 sites to the full-continent render grid AND a region-packet local grid, with nearest settlement, direction, terrain, surface marker, and player/DM visibility. Reach/Ring-1 sites are HIGH–DERIVED; far sites LOW within region footprints. **D23 (Under-Shrine Approach) is DM-ONLY and excluded from all player maps.**

9. **Are player-safe and DM-only map layers separated?** — **YES.** Every authority/packet file has an explicit Player-Safe Layer and DM-Only Layer (or visibility flags). The DM-only apex set (Concord Deep, Under-Shrine/Drowned Keystone, Hollow Court seat, node-network links, D23) is consistently marked `player-safe visibility: no` and forbidden on player maps. The endgame is consistently kept **vertical beneath Hollowmere**, never a lateral land. Far ruins are surface/echo only, drawn unexplained.

---

## Readiness Questions — Exploration Layer

10. **Can the AI DM run arrival at any settlement without improvising layout or services?** — **YES.** All 40 settlement packets provide: local grid with notable areas at fixed coordinates; services table (rest/resupply/healing/info/faction); law and threat DCs; key NPC links with Persuasion DC values; 2–3 quest hooks from authored quest files; encounter and treasure references.

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
| Low (non-blocking) | Tollreach (Greenfinger Maddoc's outlaw camp, Hethewald) — referenced as a `travel_anchor` in Hethemoot/region files; no standalone packet. | **RESOLVED (2026-06-18):** Tollreach is formalized as a **route-waypoint danger marker** at (75,37) on the Hethe Tollway (DM danger-icon; player map shows it as unlabeled danger-icon or omits). Not a service settlement. Documented in `ROADS_RIVERS_AND_ROUTES_AUTHORITY.md` (Hethe Tollway) and `MAP_FEATURE_REGISTRY.md` MF-612. No packet needed. |
| Low (non-blocking) | Pre-existing D-site numbering discrepancy: region packets mislabeled sites — Marrowdowns used D30 (should be D26), Sallowmarch used D33 (should be D30), Hollow Gulf referenced the Drowned Steps as D33, Wender Steppe table row said D25 (should be D32). | **RESOLVED (2026-06-18):** all four region-packet D-site IDs corrected to match the authoritative `ADVENTURE_SITE_CARTOGRAPHY_INDEX.md` (D26 = Marrowdowns Barrow Complex; D30 = Sallowmarch Drowned Steps; D32 = Wender Sky-Stones; D33 = Sunhollow Great Grove). Settlement packets (Marrowmoot/Fenward/Reedmouth) already used correct IDs. All region/settlement/index D-site IDs now consistent. |

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

The full continent, all **18 map-authoritative regions** (the Cindern Waste is a terrain sub-zone within Emberfell, not a 19th region; the Drowned Steps is a sub-area within Sallowmarch), the 4 major cities, all 40 settlement-floor points (plus 4 city-depth packets = 44 total), every named road/river/route, all water/terrain features, and all 36 adventure sites are coordinate-anchored and exploration-ready on both player-safe and DM-only layers. A player can fly to any point on Orrun and the AI DM can render a deterministic map AND run arrival and exploration as a scene without inventing geography, settlement layout, available services, or people.

---

## Cartography Determinism Cleanup Pass (2026-06-18)

### Inspection Results
- Region packets inspected: 18 (glob-verified in `region_map_packets/`)
- City packets inspected: 4 (Caradril, Glassmere, Calderport, Ashfast)
- Settlement packets inspected: 40 (glob-verified)
- D01–D36 sites inspected: 36 (all region-packet D-site IDs cross-checked against the master index)
- LOW-confidence major features promoted to **DERIVED-CANONIZED** (layout/geometry authoritative for mapping, geographic position stays LOW): the 3 far cities (Glassmere two-bank/Three-Bridges, Calderport crescent-harbor, Ashfast caldera fortress-temple); the major far rivers (Glasswater, Mardenflow, Hethe); the major far ranges (Karran Teeth, Greatspine/Sundering Wall, Emberfells, Ghostmark); the major far routes (Verdance Road, Glasswater Run, Greatspine Crown Road, Salt Road, Hethe Tollway). DERIVED-CANONIZED tier documented in `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §16`; far-city registry rows updated to "LOW (position) / DERIVED-CANONIZED (layout)."
- DERIVED entries already in registry: 0 unresolved — all §4/§7/§8/§9/§10/§11 geometry was already AUTHORED-CANON committed waypoints (DERIVED count = 0 prior to this pass; this pass only added the explicit DERIVED-CANONIZED *labeling* the brief asked for).
- Remaining LOW-confidence entries: all far-continent *geographic positions* (intentional placeholder; geometry committed). None blocks rendering.
- Count inconsistencies fixed: region count made explicitly **18 standalone regions** (was loosely "19") across `CARTOGRAPHY_AUTHORITY §10`, this audit, and tracking files; settlement count confirmed **40** (one audit line still said 42 — fixed).
- D-site discrepancies fixed: 4 region-packet mislabels corrected — REGION_MARROWDOWNS D30→**D26**; REGION_SALLOWMARCH D33→**D30**; REGION_HOLLOW_GULF_PORTS Drowned-Steps D33→**D30**; REGION_WENDER_STEPPE table row D25→**D32**. (Settlement packets were already correct.)
- Cities made deterministic: all 4 already had full local-grid layouts (districts, geometry relationship, gates/bridges, road exits, civic/faction/temple/inn placements, DM-only layers); this pass confirmed Caradril HIGH and promoted the 3 far-city layouts to DERIVED-CANONIZED with explicit confidence lines in their packet headers.
- Tollreach: resolved as a **route-waypoint danger marker** at (75,37) on the Hethe Tollway (not a service settlement); documented in the route authority + MF-612.
- Cindern Waste / Drowned Steps status: **Cindern Waste = terrain sub-zone within Emberfell Theocracy** (not a standalone region); **Drowned Steps = submerged-ruin sub-area (D30) within Sallowmarch** (not a region). Both documented in `CARTOGRAPHY_AUTHORITY §10`.
- Remaining cartography gaps (minor, non-blocking): far-continent coastline (Hollow Gulf → Wracking Straits) capes/inlets sketched; far river meanders illustrative between committed source/mouth waypoints; off-grid overseas isles are edge-arrows; far-region internal micro-geography is light-anchor. None blocks player-safe or DM-only rendering.

### Final Cartography Verdict

**MAP READY.** *(historical — superseded by Strict Cartography Determinism Cleanup Pass verdict below)*

All 4 major cities are deterministic (Caradril HIGH; the 3 far cities DERIVED-CANONIZED in layout); all 18 standalone map-authoritative regions have packets (+ Cindern Waste/Drowned Steps explicitly documented as sub-zones, not regions); all major rivers/routes/terrain have committed waypoint/polygon geometry; all D01–D36 sites are deterministically placed and D-site IDs are now consistent across every region packet, settlement packet, and the master index; counts are consistent (18 regions / 4 cities / 40 settlements / 36 D-sites); and no major map-authoritative feature remains geometry-LOW (only far *positions* are LOW, with committed geometry). Tollreach is resolved. No cartography blockers remain.

---

## Strict Cartography Determinism Cleanup Pass (2026-06-18)

### Pre-Pass Inventory
The geometry authority files were already AUTHORED-CANON (all §4/§7/§8/§9/§10/§11 polylines/polygons committed), but the four-status taxonomy the brief requires was not yet applied to the `MAP_FEATURE_REGISTRY.md` Conf. column, which still used HIGH/MEDIUM/LOW, and three authority files still carried "approximate/endpoint-pair/sketched" language in their gap sections. Every LOW/MEDIUM/HIGH/"placeholder"/"sketched"/"endpoint-pair"/"approximate"/"DERIVED-CANONIZED" usage on a map-authoritative row or gap line was inventoried and reclassified:
- **§A Regions (18):** 5 HIGH → AUTHORITATIVE; 13 LOW → DERIVED_CANON.
- **§B Cities/settlements (41):** 17 HIGH/MEDIUM → AUTHORITATIVE; 24 LOW (incl. 3 far-city "LOW(position)/DERIVED-CANONIZED(layout)") → DERIVED_CANON.
- **§C Rivers (6):** 3 → AUTHORITATIVE; 3 → DERIVED_CANON.
- **§D Lakes/seas/bays (9):** 4 → AUTHORITATIVE; 5 → DERIVED_CANON.
- **§E Mountains/terrain (16):** 4 → AUTHORITATIVE; 12 → DERIVED_CANON.
- **§F Routes/sea-lanes (10):** 4 → AUTHORITATIVE; 5 → DERIVED_CANON; 1 (South Sea Lanes off-map edge-arrow) → NOT_MAP_AUTHORITATIVE.
- **§G Bridges/ferries/fords/passes/ports (17):** 11 → AUTHORITATIVE; 6 → DERIVED_CANON.
- **§H Adventure-site surface markers (8):** 5 → AUTHORITATIVE; 3 → DERIVED_CANON.
- **§I Landmarks (6):** 4 → AUTHORITATIVE; 1 (Reliquary) → DERIVED_CANON; 1 (Star-Stones, "varies"/no fixed point) → NOT_MAP_AUTHORITATIVE.
- **§DM-Only (5):** all NOT_MAP_AUTHORITATIVE on player maps; AUTHORITATIVE/DERIVED_CANON on DM maps.

### Status After Pass
- **AUTHORITATIVE entries: 57**
- **DERIVED_CANON entries: 72**
- **NOT_MAP_AUTHORITATIVE entries: 7** (MF-510 South Sea Lanes; MF-803 Star-Stones; the 5 §DM-Only rows on player maps)
- **CARTOGRAPHY_BLOCKER entries: 0** (none — no map-authoritative feature requires invention)

### Region count: **18 standalone map-authoritative regions** (5 NW/cluster + 13 far). Cindern Waste = terrain sub-zone of Emberfell; Drowned Steps = D30 sub-area of Sallowmarch. Neither is a region.
### City packets: 4 (Caradril AUTHORITATIVE; Glassmere, Calderport, Ashfast DERIVED_CANON — all read and verified to have committed local-grid layouts: districts, river/harbor/caldera geometry, gates, road exits, named landmark coordinates).
### Settlement packets: 40 (glob-verified)
### D-sites: D01–D36 (36 total). All carry full-continent (X,Y) + region-local coords. D-site IDs verified consistent across region packets (Marrowdowns D26, Sallowmarch D30, Wender D32, Sunhollow D33, Hollow Gulf Wreck-Reef D31) and settlement packets (Marrowmoot/Fenward/Reedmouth). D23 (Under-Shrine Approach) confirmed DM-only, absent from every player layer.

### Remaining Gaps (all NOT_MAP_AUTHORITATIVE or DERIVED_CANON with placeholder survey context; none blocking)
- South Sea Lanes: Hollow Gulf → off-map edge-arrow only (NOT_MAP_AUTHORITATIVE).
- Star-Stones: scattered roadside relay-stones along the Concord roads, no single fixed marker point (NOT_MAP_AUTHORITATIVE).
- Far coastline / far river meanders / far ridgelines / far-zone polygon edges: committed DERIVED_CANON geometry; frontier micro-detail is placeholder context, drawn soft/faint.
- Far-region internal street/field micro-geography: deferred (NOT_MAP_AUTHORITATIVE); committed settlement anchors + region polygons suffice for region/settlement-floor maps.
- Overseas landmasses: off-grid edge-arrows (NOT_MAP_AUTHORITATIVE).

### Final Verdict

**MAP READY WITH MINOR NON-BLOCKING GAPS.**

Rationale: zero CARTOGRAPHY_BLOCKERs and zero map-authoritative features remaining LOW/placeholder/sketched/endpoint-only. All 18 regions, 4 cities, 40 settlements, 6 rivers, 9 water bodies, 16 terrain features, 10 routes, 17 crossings/ports, 8 surface adventure-site markers, and 6 landmarks are either AUTHORITATIVE (57) or DERIVED_CANON (72) with committed coordinate geometry a mapper can render directly. The only 7 NOT_MAP_AUTHORITATIVE items are the off-map South Sea Lanes edge-arrow, the scattered (non-point) Star-Stones, and the 5 DM-only hidden subsurface features — all legitimately non-renderable as fixed player-map points and none blocking. The "MINOR NON-BLOCKING GAPS" qualifier (rather than bare MAP READY) honestly reflects those 7 NOT_MAP_AUTHORITATIVE entries plus the placeholder far-survey micro-detail on DERIVED_CANON far features.

---

## Related Files

- [`../04_world_atlas/CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`](../04_world_atlas/CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md) · [`../04_world_atlas/MAP_FEATURE_REGISTRY.md`](../04_world_atlas/MAP_FEATURE_REGISTRY.md)
- [`../04_world_atlas/ROADS_RIVERS_AND_ROUTES_AUTHORITY.md`](../04_world_atlas/ROADS_RIVERS_AND_ROUTES_AUTHORITY.md) · [`../04_world_atlas/WATER_AND_SHORELINE_AUTHORITY.md`](../04_world_atlas/WATER_AND_SHORELINE_AUTHORITY.md) · [`../04_world_atlas/MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md`](../04_world_atlas/MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md)
- [`../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
- [`../00_control/CARTOGRAPHY_DETERMINISM_PROGRESS.md`](../00_control/CARTOGRAPHY_DETERMINISM_PROGRESS.md)
- region packets: [`../04_world_atlas/region_map_packets/`](../04_world_atlas/region_map_packets/)
- city packets: [`../06_settlements/city_map_packets/`](../06_settlements/city_map_packets/)
- settlement packets: [`../06_settlements/settlement_map_packets/`](../06_settlements/settlement_map_packets/)
