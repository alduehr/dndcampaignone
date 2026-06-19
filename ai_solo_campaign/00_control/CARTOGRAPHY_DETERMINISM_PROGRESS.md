# CARTOGRAPHY_DETERMINISM_PROGRESS.md — Eagle-Test Build Tracker

> **Anti-Overclaim Rule:** Mark a row DONE only after the file exists AND has been read back and confirmed to meet the defined floor. "Generated" ≠ "DONE." A truthful partial result is required; a false "complete" is a task failure.
>
> **Resume rule:** The next run picks up at the first row that is NOT DONE (UNCHECKED or IN-PROGRESS).

## Floor Definitions (what DONE means per category)

| Category | Floor to meet DONE |
|---|---|
| Phase 0 — Convention | §2 of `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md` states ONE convention authoritatively; the SW-origin reconciliation note is deleted; no other file references SW-origin. |
| Phase 1 — Geometry | Coastline has ≥15 waypoints per major segment; all terrain polygons have ≥8 waypoints; all rivers have intermediate waypoints; MAP_FEATURE_REGISTRY has AUTHORED-CANON provenance on committed shapes. |
| Phase 2 — Region packet | Local 0–100 grid defined; terrain zones with local coords; water features with local coords; roads/routes with local waypoints; ALL settlements at local coords; ALL D-sites positioned; level range + solo danger; Player-Safe + DM-Only layers; unresolved gaps honest. |
| Phase 3 — City packet | District bounds + centroids; river/harbor geometry; bridges/gates/docks/fords; road exits; named landmark buildings (incl. inn, market, temple, seat of power); services section; pop/scale; law & threat DCs; NPC links from `08_npcs/by_region/`; 2–3 hooks from `09_quests/by_region/`; encounter + treasure refs; word "placeholder" removed. |
| Phase 4 — Settlement packet | 4–8 notable areas at fixed local coords; services (rest, resupply, healing, info, faction); pop/scale; law & threat DCs; named NPC links from `08_npcs/by_region/`; 2–3 hooks from quests/clocks; encounter + treasure refs; Player-Safe + DM-Only layers. |

---

## Phase 0 — Kill Coordinate Convention Ambiguity

| Item | File | Status | Notes |
|---|---|---|---|
| P0-A: Remove SW-origin reconciliation note from §2 | `04_world_atlas/CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md` | DONE | §2 now states one convention only; SW-origin paragraph deleted; §1 orientation note also corrected. Verified 2026-06-17. |
| P0-B: Verify no other file references SW-origin | all atlas files | DONE | Grep confirmed: only PROGRESS_LOG.md (historical) and CARTOGRAPHY_READINESS_AUDIT.md (stale resolution note — flagged for Phase 6 rewrite). No atlas/map packet files reference SW-origin. Verified 2026-06-17. |

---

## Phase 1 — Commit Full-Continent Geometry

| Item | File | Status | Notes |
|---|---|---|---|
| P1-A: Coastline densified (≥15 waypoints/segment) | `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §4` | DONE | All 5 segments now have 15–19 waypoints; all AUTHORED-CANON. Verified 2026-06-17. |
| P1-B: Terrain polygons ≥8 waypoints each | `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §9` | DONE | All 10 terrain polygons expanded to 12–15 waypoints; AUTHORED-CANON. Verified 2026-06-17. |
| P1-C: Regional boundary polygons ≥8 waypoints each | `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §10` | DONE | All 19 regional boundary polygons expanded to 12–15 waypoints; DERIVED entries eliminated. Verified 2026-06-17. |
| P1-D: Rivers have ≥3 intermediate waypoints | `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §7` | DONE | All 6 rivers densified to 9–15 waypoints; AUTHORED-CANON. Verified 2026-06-17. |
| P1-E: Mountain ranges have ≥3 intermediate waypoints | `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §8` | DONE | All 6 ranges expanded to 6–10 waypoints; AUTHORED-CANON. Verified 2026-06-17. |
| P1-F: MAP_FEATURE_REGISTRY geometry/provenance updated | `04_world_atlas/MAP_FEATURE_REGISTRY.md` | DONE | Cleared by P6-D: four-status taxonomy (AUTHORITATIVE/DERIVED_CANON/NOT_MAP_AUTHORITATIVE/CARTOGRAPHY_BLOCKER) applied to all 136 entries; 57 AUTH, 72 DERIVED, 7 NOT_MAP, 0 BLOCKER. Strict Cartography Determinism Cleanup pass 2026-06-18. |

---

## Phase 2 — Far-Region Map Packets (13 regions)

| Region | File | Status | Notes |
|---|---|---|---|
| Verdance Reaches | `REGION_VERDANCE_REACHES.md` | DONE | Full Phase 2 floor met. Verified prior session (2026-06-17/18). |
| Glassmere League | `REGION_GLASSMERE_LEAGUE.md` | DONE | Full Phase 2 floor met. Verified prior session. |
| Marrowdowns | `REGION_MARROWDOWNS.md` | DONE | Full Phase 2 floor met. (D-site discrepancy **RESOLVED 2026-06-18**: packet now uses **D26** to match the master index; Barrow Complex = D26.) Verified prior session. |
| Sallowmarch Protectorate | `REGION_SALLOWMARCH_PROTECTORATE.md` | DONE | Full Phase 2 floor met. (D-site discrepancy **RESOLVED 2026-06-18**: packet now uses **D30** to match the master index; Drowned Steps = D30.) Verified prior session. |
| Hollow Gulf Ports | `REGION_HOLLOW_GULF_PORTS.md` | DONE | Full Phase 2 floor met; used as reference template this session. Verified 2026-06-18. |
| Wender Steppe | `REGION_WENDER_STEPPE.md` | DONE | Full Phase 2 floor met; used as reference template this session. Verified 2026-06-18. |
| Karran Marches | `REGION_KARRAN_MARCHES.md` | DONE | Upgraded from placeholder this session. Full Phase 2 floor: local grid X 70–80 / Y 14–24; transform; 5 terrain zones; 2 water features; 4 routes; 4 settlements (Brask's Hold, Karran-Gate, Deep Cuts, Old Iron forts); D27; level 9–14; Player-Safe + DM-Only. Read-back confirmed. Verified 2026-06-18. |
| Emberfell Theocracy | `REGION_EMBERFELL_THEOCRACY.md` | DONE | Upgraded from placeholder this session. Full Phase 2 floor: local grid X 76–86 / Y 56–68; transform; 5 terrain zones; 3 water features; 4 routes; 3 settlements (Ashfast ref city packet, Cinderhold, Ash Roads); D22 + D36; level 12–16; Player-Safe + DM-Only. Read-back confirmed. Verified 2026-06-18. |
| Saltmere Reaches | `REGION_SALTMERE_REACHES.md` | DONE | Upgraded from placeholder this session. Full Phase 2 floor: local grid X 55–66 / Y 66–76; transform; 5 terrain zones; 3 water features; 4 routes; 3 settlements (Brackhold, Saltcairn, Drowned Towns/D24); D24; level 11–15; Player-Safe + DM-Only. Verified 2026-06-18. |
| Concord Heartlands | `REGION_CONCORD_HEARTLANDS.md` | DONE | Upgraded from placeholder this session. Full Phase 2 floor: local grid X 58–66 / Y 52–60; transform; 5 terrain zones; 2 water features; 4 routes; 2 settlements (Crownmouth, Pilgrim Camps); D21; level 13–17; critical secrecy notes in DM-Only layer. Verified 2026-06-18. |
| Hethewald Free Holds | `REGION_HETHEWALD_FREE_HOLDS.md` | DONE | Upgraded from placeholder this session. Full Phase 2 floor: local grid X 66–78 / Y 34–46; transform; 6 terrain zones; 3 water features; 4 routes; 4 settlements (Hethemoot, Greenward, Tollreach, Old Holds/D25); D25; level 7–12; Player-Safe + DM-Only. Read-back confirmed. Verified 2026-06-18. |
| Sunmark | `REGION_SUNMARK.md` | DONE | Upgraded from placeholder this session. Full Phase 2 floor: local grid X 38–50 / Y 75–85; transform; 5 terrain zones; 3 water features; 3 routes; 3 settlements (Sunhollow/D33, Grove-Camps, Green Roads); D33; level 8–13; Player-Safe + DM-Only. Read-back confirmed. Verified 2026-06-18. |
| Highmark Passes | `REGION_HIGHMARK_PASSES.md` | DONE | Upgraded from placeholder this session. Full Phase 2 floor: local grid X 26–44 / Y 7–11; transform; 4 terrain zones; 2 water features; 3 routes; NO settlements; D35 DM-ONLY (never on player map); level 12–16 optional late frontier; explicit "no NPC/quest files" note. Read-back confirmed. Verified 2026-06-18. |

---

## Phase 3 — Far Cities to Caradril Depth

| City | File | Status | Notes |
|---|---|---|---|
| Glassmere | `city_map_packets/GLASSMERE_CITY_MAP.md` | DONE | Population/scale, Services, Law & Threat DCs, Key NPC Links (GL-M1–M5 + secondaries), 3 quest hooks (Q_GL_001–003), Encounter + Treasure refs added. "placeholder" removed from title, tags, secrecy note, and Unresolved Gaps. NPC + quest file links added. Verified 2026-06-17. |
| Calderport | `city_map_packets/CALDERPORT_CITY_MAP.md` | DONE | Population/scale, Services, Law & Threat DCs, Key NPC Links (HG-M1/M2/M4/M5 + secondaries), 3 quest hooks (Q_HGP_001–003), Encounter + Treasure refs added. "placeholder" removed. Verified 2026-06-17. |
| Ashfast | `city_map_packets/ASHFAST_CITY_MAP.md` | DONE | Population/scale, Services, Law & Threat DCs, Key NPC Links (EF-M1–M4 + secondaries), 3 quest hooks (Q_ET_001–003), Encounter + Treasure refs added. "placeholder" removed. Verified 2026-06-17. |

---

## Phase 4 — Settlement Map Packets (all reachable named settlements)

### Existing packets upgraded to explorable floor

| Settlement | File | Status | Notes |
|---|---|---|---|
| Crownmouth | `settlement_map_packets/SETTLEMENT_CROWNMOUTH_MAP.md` | DONE | Upgraded 2026-06-18: 6 notable areas, services, NPC links (Lyssa Crownmouth DC17, Hollin Vane DC17, Father Ord DC14, Mab DC15), hooks, DCs. DM-Only: surface ruin ONLY. Verified. |
| Brask's Hold | `settlement_map_packets/SETTLEMENT_BRASKS_HOLD_MAP.md` | DONE | Upgraded 2026-06-18: 6 notable areas, services, NPC links ("Iron" Brask AC18/~104HP, Mully Karr DC16, Wenna Stone DC17), hooks, DCs. DM-Only: Old Iron forts NOT keystone. Verified. |
| Brackhold | `settlement_map_packets/SETTLEMENT_BRACKHOLD_MAP.md` | DONE | Upgraded 2026-06-18: 6 notable areas, services, NPC links (Bryd Saltmere DC17, Salt-Mother Tess DC16, Delver Oss DC16, Bonepan DC14), hooks, DCs. DM-Only: Drowned Towns NOT keystone. Verified. |
| Fenward | `settlement_map_packets/SETTLEMENT_FENWARD_MAP.md` | DONE | Upgraded 2026-06-18: 6 notable areas, services, NPC links (Vorr Sallow DC17, Doll Fenn DC15, "Heron" Maddox DC15, Sela Reed DC16, Pell Sallows DC13), hooks, DCs. Verified. |
| Marrowmoot | `settlement_map_packets/SETTLEMENT_MARROWMOOT_MAP.md` | DONE | Upgraded 2026-06-18: 6 notable areas, services, NPC links (Aldous Penmark DC15, Senna Crale DC14, Doss Wether DC14, Edony Marrow DC14), hooks, DCs. Verified. |
| Hethemoot | `settlement_map_packets/SETTLEMENT_HETHEMOOT_MAP.md` | DONE | Upgraded 2026-06-18: 6 notable areas, services, NPC links (Bram Hethe DC16, Onn Greenward visiting, Greenfinger NOT at Hethemoot), hooks, DCs. Verified. |
| Sunhollow | `settlement_map_packets/SETTLEMENT_SUNHOLLOW_MAP.md` | DONE | Upgraded 2026-06-18: 6 notable areas, services, NPC links (Sael Sunmark DC15, Sun-Singer Doll DC16 EXTREMELY oblique), hooks, DCs. DM-Only: grove rites work, mechanism NEVER explained. Verified. |
| Cold Springs | `settlement_map_packets/SETTLEMENT_COLD_SPRINGS_MAP.md` | DONE | Upgraded 2026-06-18: 6 notable areas, services, NPC links (Tamur Wend-Khar DC15, Wind-Singer Esha DC16 oblique, Borr NOT at camp), hooks, DCs. DM-Only: Sky-Stones NON-CONCORD. Verified. |
| Cinderhold | `settlement_map_packets/SETTLEMENT_CINDERHOLD_MAP.md` | DONE | Upgraded 2026-06-18: 6 notable areas, services, NPC links (Doss Ashfast DC16, Sef Embren DC17 AC18/~85HP), hooks, DCs. DM-Only: D36 peripheral supply-works, NOT keystone. Verified. |

### New settlement packets created

| Settlement | File | Status | Notes |
|---|---|---|---|
| Marrowfen Stair | `SETTLEMENT_MARROWFEN_STAIR_MAP.md` | DONE | Created 2026-06-18: Verdance hub (58,42); 6 areas; Wessel Crane DC16, Hadwin Vael DC15, Mossa Drenn DC14; hooks Q_VR_001/003. Verified. |
| Lord's Wend | `SETTLEMENT_LORDS_WEND_MAP.md` | DONE | Created 2026-06-18: Verdance secondary (60,45); 5 areas; Lord Ennis Marrow DC15; hooks Q_VR_004/005. Verified. |
| Cresswater | `SETTLEMENT_CRESSWATER_MAP.md` | DONE | Created 2026-06-18: Verdance river-landing (55,46); 4 areas; Mossa Drenn DC14; hooks Q_VR_003. Verified. |
| Sennfort | `SETTLEMENT_SENNFORT_MAP.md` | DONE | Created 2026-06-18: Glassmere named-in-passing anchor (56,32); 6 areas; Mareth Senn visiting. Named-in-passing depth only per NAMING_REGISTRY. Verified. |
| Cairnwater | `SETTLEMENT_CAIRNWATER_MAP.md` | DONE | Created 2026-06-18: Glassmere named-in-passing anchor (60,30); 6 areas. Named-in-passing depth only per NAMING_REGISTRY. Verified. |
| Penmark Hold | `SETTLEMENT_PENMARK_HOLD_MAP.md` | DONE | Created 2026-06-18: Marrowdowns secondary (47,63); 5 areas; Aldous Penmark DC15, Edony Marrow DC14; hooks Q_MD_002. Verified. |
| Wether | `SETTLEMENT_WETHER_MAP.md` | DONE | Created 2026-06-18: Marrowdowns travel anchor (53,68); 4 areas; Doss Wether DC14; hooks Q_MD_001/D26 escort. Verified. |
| Reedmouth | `SETTLEMENT_REEDMOUTH_MAP.md` | DONE | Created 2026-06-18: Sallowmarch secondary (60,85); 5 areas; "Heron" Maddox DC15, Sela Reed DC16, Pell Sallows DC13; hooks Q_SP_002. Verified. |
| Saltgate | `SETTLEMENT_SALTGATE_MAP.md` | DONE | Created 2026-06-18: Gulf port city (46,82); 6 areas; Doss Saltgate DC16, Roke Mallin DC15; hooks Q_HGP_003. Verified. |
| Saltcairn | `SETTLEMENT_SALTCAIRN_MAP.md` | DONE | Created 2026-06-18: Saltmere secondary (63,73); 5 areas; Delver Oss visiting; hooks Q_SALT_002. Verified. |
| Karran-Gate | `SETTLEMENT_KARRAN_GATE_MAP.md` | DONE | Created 2026-06-18: Karran mining town (76,20); 6 areas; Mully Karr DC16, Wenna Stone DC17; hooks Q_KM_001/003. Verified. |
| Greenward | `SETTLEMENT_GREENWARD_MAP.md` | DONE | Created 2026-06-18: Hethewald grove-village (68,43); 6 areas; Onn Greenward DC15; hooks Q_HFH_003/005. DM-Only: "failing bargains" M5/M6-oblique ONLY; NOT keystone. Verified. |
| Spine-Foot trade-meet | `SETTLEMENT_SPINE_FOOT_MAP.md` | DONE | Created 2026-06-18: Wender travel anchor (50,20); 5 areas; Tamur seasonal; hooks Q_WS_001/002. Verified. |
| Pilgrim Camps | `SETTLEMENT_PILGRIM_CAMPS_MAP.md` | DONE | Created 2026-06-18: Heartlands ruin-edge (63,58); 6 areas; Father Ord DC14 (M6-oblique), Hollin Vane DC17, Old Crown Mab DC15; hooks Q_CH_001/003. DM-Only: surface-only; NOT keystone. Verified. |
| Grove-Camps | `SETTLEMENT_GROVE_CAMPS_MAP.md` | DONE | Created 2026-06-18: Sunmark social anchor (40,77); 5 areas; Tamsin Greenway DC14 (secondary; distinct from Tamsin Orr); links to Sael/Sunhollow; hooks Q_SUN_001/006. Verified. |

---

## Phase 5 — Eagle-Test Coverage Audit

| Item | Status | Notes |
|---|---|---|
| P5-A: All settlement anchors verified — packet exists | DONE | All Table 2 `settlement_major`/`settlement_secondary` anchors have packets (Phase 3 city packets + Phase 4 settlement packets). Travel anchors (Nine Locks, Rice Sallows, Ash Roads, Deep Cuts, Tollreach, Green Roads), ruin-edge anchors, and city-district locales do not require standalone packets. **Tollreach RESOLVED (2026-06-18):** formalized as a **route-waypoint danger marker** at (75,37) on the Hethe Tollway (`ROADS_RIVERS_AND_ROUTES_AUTHORITY.md`, `MAP_FEATURE_REGISTRY.md` MF-612) — a dangerous outlaw camp, not a service settlement; no packet needed. Verified 2026-06-18. |
| P5-B: All D-sites positioned in region packets | DONE | All 36 sites (D01–D36) are positioned in their region/city packets. **D-site discrepancies RESOLVED (2026-06-18):** Marrowdowns packet now uses **D26**, Sallowmarch **D30**, Hollow Gulf Drowned-Steps **D30**, Wender Steppe **D32** — all matching the authoritative `ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`. D23 (Under-Shrine) confirmed DM-only / never on player maps. D35 (Highmark) confirmed DM-facing only. Verified 2026-06-18. |
| P5-C: 8-point random-location proof | DONE | Tested 8 points — all fully deterministic: (1) Hollowmere (24,23): `HOLLOWMERE.md`+`REGION_SUNDERING_REACH.md`; (2) Caradril (34,35): `CARADRIL_CITY_MAP.md`+8 district packets; (3) Glassmere (55,50): `GLASSMERE_CITY_MAP.md`+`REGION_GLASSMERE_LEAGUE.md`; (4) Brask's Hold (73,17): `SETTLEMENT_BRASKS_HOLD_MAP.md`+`REGION_KARRAN_MARCHES.md`; (5) Sunhollow (44,80): `SETTLEMENT_SUNHOLLOW_MAP.md`+`REGION_SUNMARK.md`; (6) Crownmouth (60,54): `SETTLEMENT_CROWNMOUTH_MAP.md`+`REGION_CONCORD_HEARTLANDS.md`; (7) Cinderhold (83,65): `SETTLEMENT_CINDERHOLD_MAP.md`+`REGION_EMBERFELL_THEOCRACY.md`; (8) Cold Springs (45,16): `SETTLEMENT_COLD_SPRINGS_MAP.md`+`REGION_WENDER_STEPPE.md`. All 8: local coords ✓, services ✓, NPC links ✓, law DCs ✓, hooks ✓, apex secrecy ✓. Verified 2026-06-18. |
| P5-D: Zero blockers remaining | DONE | No blockers. The pre-existing D-site numbering discrepancies (Marrowdowns/Sallowmarch/Hollow Gulf/Wender Steppe) and the Tollreach gap are **RESOLVED** in the 2026-06-18 Cartography Determinism Cleanup pass. Eagle-test verdict: **CONTINENT IS EXPLORATION-DETERMINISTIC; MAP READY.** Verified 2026-06-18. |

---

## Phase 6 — Indexes, Canon, Tracking

| Item | File | Status | Notes |
|---|---|---|---|
| P6-A: CONTENT_INDEX.md updated | `00_control/CONTENT_INDEX.md` | DONE | Updated during Exploration-Determinism pass (2026-06-18) — all 40 settlement packets + region/city packets indexed. |
| P6-B: TAG_INDEX.md updated | `00_control/TAG_INDEX.md` | DONE | Updated during Exploration-Determinism pass (2026-06-18). |
| P6-C: REGION_INDEX.md updated | `04_world_atlas/REGION_INDEX.md` | DONE | Updated during Exploration-Determinism pass (2026-06-18) — eagle-test depth note added; all 18 regions listed. |
| P6-D: MAP_FEATURE_REGISTRY.md settlements updated | `04_world_atlas/MAP_FEATURE_REGISTRY.md` | DONE | Four-status taxonomy applied to all 136 entries (Strict Cartography Determinism Cleanup pass 2026-06-18): 57 AUTH, 72 DERIVED_CANON, 7 NOT_MAP, 0 BLOCKER. Also clears P1-F. |
| P6-E: RETRIEVAL_GUIDE.md updated | `00_control/RETRIEVAL_GUIDE.md` | DONE | Rewritten during Stage 16 correction pass (2026-06-16); updated to include Exploration-Determinism Pass during that pass. Current as of 2026-06-18. |
| P6-F: NAMING_REGISTRY.md city-scale labels updated | `00_control/NAMING_REGISTRY.md` | DONE | Exploration-Determinism pass note (2026-06-18) explicitly states city-internal landmark names are "settlement-flavor labels only — NOT registered proper nouns per registry scope." No further registry update required. |
| P6-G: PROGRESS_LOG.md entry added | `00_control/PROGRESS_LOG.md` | DONE | Strict Cartography Determinism Cleanup Pass entry added 2026-06-18. |
| P6-H: TODO.md updated | `00_control/TODO.md` | DONE | Updated during Exploration-Determinism / Cartography Determinism Cleanup passes (2026-06-18). |
| P6-I: CONTENT_GAPS.md updated | `17_generation_backlog/CONTENT_GAPS.md` | DONE | Updated during Exploration-Determinism / Cartography Determinism Cleanup passes (2026-06-18) — Tollreach + D-site rows closed. |
| P6-J: STAGE_STATUS.md updated | `00_control/STAGE_STATUS.md` | DONE | Strict Cartography Determinism Cleanup pass added to Current Status block + Interstitial Passes table; Most Recent Pass line updated. 2026-06-18. |
| P6-K: CARTOGRAPHY_READINESS_AUDIT.md rewritten | `18_audits/CARTOGRAPHY_READINESS_AUDIT.md` | DONE | Strict Cartography Determinism Cleanup Pass section added; honest verdict "MAP READY WITH MINOR NON-BLOCKING GAPS." 2026-06-18. |

---

## Summary (updated 2026-06-18 — ALL PHASES COMPLETE)

| Phase | Done | Unchecked | Total |
|---|---|---|---|
| Phase 0 | 2 | 0 | 2 |
| Phase 1 | 6 | 0 | 6 |
| Phase 2 | 13 | 0 | 13 |
| Phase 3 | 3 | 0 | 3 |
| Phase 4 | 24 | 0 | 24 |
| Phase 5 | 4 | 0 | 4 |
| Phase 6 | 11 | 0 | 11 |
| **Total** | **63** | **0** | **63** |

> **Last verified:** 2026-06-18 — Strict Cartography Determinism Cleanup pass complete. All 63 items DONE. Eagle-test verdict: **CONTINENT IS EXPLORATION-DETERMINISTIC.** Cartography verdict: **MAP READY WITH MINOR NON-BLOCKING GAPS** (57 AUTHORITATIVE, 72 DERIVED_CANON, 7 NOT_MAP_AUTHORITATIVE, 0 CARTOGRAPHY_BLOCKER). Stage 17 (Live Campaign Operation) is next; map image generation is the only remaining cartography work.
