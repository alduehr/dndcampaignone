# CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md — Master Cartographic Authority

---
type: region
secrecy: mixed
status: static
region: Orrun
factions: []
level_range: 1-20
related: [FULL_WORLD_MAP_COORDINATES.md, WORLD_MAP_COORDINATES.md, FULL_WORLD_MAP_AUTHORITY.md, WORLD_MAP_AUTHORITY.md, PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md, MAP_FEATURE_REGISTRY.md, ROADS_RIVERS_AND_ROUTES_AUTHORITY.md, WATER_AND_SHORELINE_AUTHORITY.md, MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md, FULL_CONTINENT_SETTLEMENT_ANCHORS.md, REGION_INDEX.md, ../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md]
tags: [type:map, secrecy:mixed, function:cartography, coordinates, route-geometry, terrain-polygon, water-geometry, orrun, full-continent, authority]
---

> **Secrecy classification:** This file is **mixed**. The player-safe render layer (§13) is safe to render to the player; §14 (DM-only render layer) names hidden subsurface features (Concord Deep, Under-Shrine / Drowned Keystone, Hollow Court seat) only to forbid rendering them. **Never hand this file directly to the player**; use it to generate/audit player-safe and DM-only maps.

## AI Use

This is the **single master cartographic authority** for the continent of **Orrun** (world of **Vael**). It consolidates the existing coordinate, route, water, terrain, and settlement-anchor files into one deterministic geometry reference so a mapper can render player-safe and DM-only maps without guessing. Load it when:
- Generating or commissioning any full-continent or regional map.
- Resolving where a feature sits relative to others.
- Building image-generation prompts (use with `PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md` for label authority).

**This file does not invent new geography.** It resolves the geometry already established in `FULL_WORLD_MAP_COORDINATES.md`, `WORLD_MAP_COORDINATES.md`, `FULL_WORLD_MAP_AUTHORITY.md`, `WORLD_MAP_AUTHORITY.md`, and `MAP_DESCRIPTION.md` into explicit polylines, polygons, and points. Where a feature only had a centroid before, this file derives a polyline/polygon consistent with that centroid and the established adjacencies, and marks it **DERIVED**. No travel time, region description, or label is changed.

---

## §1. Map Scale and Orientation

- **World:** Vael. **Continent of play:** Orrun.
- **Orientation:** **North = top, west = left.** (X = 0 west, X = 100 east; Y = 0 north/top, Y = 100 south/bottom — see §2.)
- **Scale:** one full-continent grid unit ≈ **8–12 miles**; corner-to-corner ≈ **2–3 months' travel** by road. The NW campaign cluster's internal scale is finer (one campaign-grid unit ≈ 2–2.6 miles; corner-to-corner of the cluster ≈ 200–260 miles / ~12 days).
- **Canonical travel unit:** the **established day-count** (see `MAP_DESCRIPTION.md`, `TRAVEL_ROUTES_RING1.md`), not miles. Mileage here is a drawing aid only.

---

## §2. Full-Continent Coordinate System (authoritative — single convention)

The full-continent grid is **0–100 on both axes**. **There is one coordinate convention used throughout this file, all render manifests, and all settlement-anchor files:**

- **(0,0) = NW corner (top-left); X = 0 west, X = 100 east; Y = 0 north (top), Y = 100 south (bottom).**

This is the render convention. All coordinates in this file, in `FULL_WORLD_MAP_COORDINATES.md`, `PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md`, `FULL_CONTINENT_SETTLEMENT_ANCHORS.md`, and every region/settlement map packet use this convention. A mapper can place features directly from coordinates in any of these files without conversion.

The NW campaign cluster occupies render-grid **X 8–40, Y 8–42** (upper-left quarter). It is the only high-detail zone. The campaign-area grid in `WORLD_MAP_COORDINATES.md` is a ~3× zoom on this corner; see §15 for the transform.

---

## §3. Continent Outline (major cape/bay features)

Orrun is a large continent that tilts from a **cold, broken NW frontier** to a **warm, rich S/SE**. Render convention coastline, clockwise from the NW corner:

> **Confidence columns (geographic-certainty context only — see §16):** HIGH/MEDIUM/LOW labels in this file's tables indicate geographic certainty, NOT render-readiness. For render-confidence, use `MAP_FEATURE_REGISTRY.md` (four-status taxonomy: AUTHORITATIVE / DERIVED_CANON / NOT_MAP_AUTHORITATIVE / CARTOGRAPHY_BLOCKER). This note applies to all confidence columns in §3–§12b.

| Segment | Description | Confidence |
|---|---|---|
| NW corner | The Pale Coast headlands meet the Pale Sea; sea-cliffs and shingle coves. | HIGH |
| N edge | The Highmark Spine wall rises behind a short cold-N coast on the Sunder Ocean. | MEDIUM |
| NE corner | The Karran Teeth reach the N/NE; little coast; rugged frontier. | LOW |
| E edge | The Hethewood and Hethe drainage; the Hethe reaches the Calm Reach in the SE. | LOW |
| SE corner | The Glass Coast (volcanic glass) against the Calm Reach; the warm-rich corner. | LOW |
| S edge | The Hollow Gulf (major bay) at the Mardenflow/Glasswater delta; the Drowned Steps offshore. | LOW |
| SW edge | The Sallow Marches delta; then up the W coast toward the Wracking Straits. | LOW |
| Far-W margin | The Wracking Straits narrow toward open ocean; the Sundered Isles lie off-grid W. | LOW |

**Major bays/capes (render points):** the Hollow Gulf (66,92), the Stillwater harbor-lake inlet (34,35), the Verdance sea-mouth (15,32), the Wracking Straits (2,64).

---

## §4. Coastline Segments (ordered render-grid waypoints)

Draw the W and S coasts as a single continuous shoreline; the N coast is short. Waypoints are ordered N→S down the W coast, then W→E along the S coast. **All geometry is AUTHORED-CANON (committed); a renderer needs zero shape decisions.**

| Coast segment | Ordered waypoints (x,y) | Provenance | Notes |
|---|---|---|---|
| W coast (Pale Sea) | (12,18) Cobble Strand cove → (12,20) → (11,21) headland indent → (12,22) Wrackmouth approach → (12,23) Wrackmouth → (12,25) cove S → (13,26) shore bend → (14,28) → (14,30) coast turn → (15,32) Verdance mouth → (13,36) coast recedes → (11,40) → (10,44) → (10,45) → (8,50) coast turns W → (5,55) → (5,58) → (3,61) cape bend → (2,64) Wracking Straits | AUTHORED-CANON (NW HIGH; far MEDIUM) | 19 waypoints; sea-cliffs and shingle near cluster, open coast south |
| N coast (Sunder Ocean) | (20,6) → (22,5) → (25,5) → (28,5) → (30,6) pass inlet → (33,5) → (36,5) → (38,5) → (42,5) → (44,5) → (47,5) → (50,4) → (53,5) → (57,5) → (60,5) → (63,5) → (65,5) | AUTHORED-CANON (LOW) | 17 waypoints; short cold coast behind the Spine/Teeth |
| S coast W half (Sallow Marches/Sunmark) | (36,86) → (37,87) → (38,88) → (40,90) → (41,91) → (42,89) bay edge → (44,90) → (46,90) → (47,89) → (48,89) → (50,88) → (51,88) → (52,87) → (53,87) → (55,86) Mardenflow delta edge | AUTHORED-CANON (LOW) | 15 waypoints; marshy delta coast |
| S coast Hollow Gulf | (55,86) → (57,88) → (58,89) → (59,90) → (60,92) → (62,93) → (64,93) → (65,92) Calderport crescent → (66,92) Hollow Gulf mouth → (67,92) → (68,91) → (69,91) Saltgate headland → (70,91) → (72,91) → (74,90) | AUTHORED-CANON (LOW) | 15 waypoints; major bay with two port headlands |
| SE coast (Glass Coast / Calm Reach) | (74,90) → (76,89) → (78,88) → (80,87) → (82,85) → (84,83) → (86,80) Glass Coast → (87,78) → (88,75) → (88,72) → (89,68) → (90,65) → (90,62) → (89,58) → (88,55) Hethe mouth | AUTHORED-CANON (LOW) | 15 waypoints; volcanic-glass coast into warm sea |

---

## §5. Sea / Ocean Boundaries (label-body centroids and fill bounds)

| Body | Type | Centroid (x,y) | Fill bounds | Confidence |
|---|---|---|---|---|
| The Pale Sea | ocean | (4,30) | X 0–10, Y 5–60 (W margin) | HIGH |
| The Sunder Ocean | ocean | (50,2) | X 20–70, Y 0–6 (N margin) | MEDIUM |
| The Calm Reach | warm sea | (82,92) | X 70–95, Y 85–98 (SE/S margin) | MEDIUM |
| The Hollow Gulf | major bay | (66,92) | X 60–72, Y 88–96 | LOW |
| The Wracking Straits | strait | (2,64) | X 0–5, Y 58–70 (far-W) | LOW |

---

## §6. Major Lakes / Harbor-Lakes / Inland Seas (polygon waypoints)

| Water feature | Type | Centroid | Polygon waypoints (x,y) | Shore notes | Confidence |
|---|---|---|---|---|---|
| The Stillwater | harbor-lake | (34,35) | (33,34)→(35,33)→(36,35)→(35,37)→(33,36) | Small lake at the E end of Caradril where the Verdance widens; Caradril on its W/N shore. | HIGH |
| Hollowmere basin | flooded basin | (24,23) | (23,22)→(25,22)→(25,24)→(23,24) | Dark flooded sink; Hollowmere rings its rim. Drowned shrine interior is DM-only (§14). | HIGH |
| Orchardmere lake | lake | (25,32) | (24,31)→(26,31)→(26,33)→(24,33) | Small Vale lake; Orchardmere on its shore. | MEDIUM |
| The Saltmere | inland salt sea | (60,70) | (56,67)→(64,67)→(66,71)→(62,75)→(56,73) | Brackish inland sea; ringed by the Saltmere Reaches (label on land), Ghostmark Range, Bonepan Flats. | LOW |

---

## §7. River Polylines (source → mouth, ordered render-grid waypoints)

All rivers drawn as single polylines through ordered waypoints. Label each **once** (see render manifest §5). **All geometry is AUTHORED-CANON.**

| River | Ordered waypoints (x,y) | Source → mouth | Provenance |
|---|---|---|---|
| Verdance | (48,46) upland source → (46,44) → (44,42) → (40,40) → (38,38) → (34,35) Caradril/Stillwater → (28,35) → (24,33) → (20,33) → (15,32) Pale Sea mouth | rises in Verdance Reaches interior; widens at Caradril/Stillwater; reaches the Pale Sea | AUTHORED-CANON (cluster HIGH; upper MEDIUM) |
| Glasswater | (58,40) Greatspine source → (58,43) → (57,46) → (56,48) → (55,50) Glassmere → (57,55) → (58,60) → (59,66) → (60,72) → (61,78) → (62,83) → (63,86) → (64,88) Hollow Gulf delta | the continent's largest river; the main commercial artery; runs through the Glassmere League | AUTHORED-CANON (LOW) |
| Mirewend | (25,16) Sunder Heights source → (25,18) → (25,20) → (25,21) → (24,22) → (24,23) Hollowmere basin → (24,25) → (24,28) → (25,32) → (26,36) → (28,40) Mirewend Sinks drain | the Reach's slow peat-dark artery; floods autumn; feeds the basin | AUTHORED-CANON (cluster HIGH) |
| Ammet | (28,28) Vale headwaters → (27,29) → (26,29) → (25,30) Tilbrook → (25,31) → (25,32) Orchardmere → (24,32) → (22,32) → (18,32) joins Verdance | the Vale's river; mill-driven | AUTHORED-CANON (MEDIUM) |
| Mardenflow | (52,64) Marrowdowns source → (52,66) → (53,68) → (53,71) → (54,74) → (55,76) → (56,78) → (57,80) → (58,83) → (58,84) Sallow Marches delta → (60,87) → (62,89) → (63,90) → (64,91) → (65,92) Hollow Gulf | drains the southern plains into the Gulf delta; floods seasonally | AUTHORED-CANON (LOW) |
| Hethe | (74,22) Karran Teeth source → (73,24) → (74,26) → (74,28) → (75,30) → (76,32) → (76,34) → (77,36) → (77,40) → (78,44) → (79,47) → (80,50) Calm Reach mouth | eastern trade river; toll-contested; drains the Hethewood/Hethewald country | AUTHORED-CANON (LOW) |

---

## §8. Mountain Range Polylines (ordered spine waypoints)

**All geometry is AUTHORED-CANON.**

| Range | Ordered waypoints (x,y) | Provenance | Notes |
|---|---|---|---|
| The Highmark Spine | (26,10) W end → (28,10) → (30,9) → (33,9) → (35,9) → (38,8) → (41,8) → (44,8) E end | AUTHORED-CANON (W MEDIUM; E LOW) | 8 waypoints; cold N barrier |
| The Sunder Heights | (21,18) → (22,17) → (24,16) → (24,15) → (26,14) → (28,13) | AUTHORED-CANON (HIGH) | 6 waypoints; Reach highland belt |
| The Karran Teeth | (70,20) → (71,18) → (73,17) → (74,16) → (77,14) → (80,13) | AUTHORED-CANON (LOW) | 6 waypoints; NE rugged frontier |
| The Greatspine / Sundering Wall | (50,38) NW end → (52,40) → (54,43) → (56,46) → (58,48) → (60,51) → (62,53) → (62,56) → (66,60) → (70,64) SE end | AUTHORED-CANON (LOW) | 10 waypoints; continental cordillera |
| The Emberfells | (76,57) → (77,58) → (79,59) → (80,60) → (82,62) → (84,64) | AUTHORED-CANON (LOW) | 6 waypoints; volcanic highland |
| The Ghostmark Range | (53,70) → (55,71) → (57,72) → (58,72) → (61,73) → (63,74) | AUTHORED-CANON (LOW) | 6 waypoints; low eroded ring S of the Saltmere |

---

## §9. Forest / Wetland / Badland / Highland / Steppe Polygons

Each polygon is an ordered ring of render-grid waypoints. **All geometry is AUTHORED-CANON; a renderer needs zero shape decisions.**

| Zone | Type | Polygon waypoints (x,y) — ordered ring | Provenance |
|---|---|---|---|
| Tollwood | forest | (29,18)→(31,17)→(34,17)→(36,18)→(37,21)→(36,25)→(35,26)→(33,27)→(30,27)→(28,25)→(28,21)→(29,18) | AUTHORED-CANON (HIGH) — 12 pts |
| Hethewood | great forest | (64,32)→(68,31)→(72,31)→(76,31)→(80,32)→(81,36)→(81,40)→(80,44)→(78,46)→(74,47)→(70,47)→(66,46)→(64,43)→(64,38)→(64,32) | AUTHORED-CANON (LOW) — 15 pts |
| Sunmark Wilds | warm forest | (38,75)→(41,74)→(44,74)→(47,74)→(50,75)→(51,78)→(51,82)→(50,86)→(47,87)→(44,87)→(41,86)→(38,85)→(37,82)→(37,78)→(38,75) | AUTHORED-CANON (LOW) — 15 pts |
| Greyfens | fog marsh | (19,23)→(20,22)→(22,22)→(24,22)→(25,23)→(25,25)→(25,27)→(25,28)→(23,29)→(21,28)→(20,27)→(19,25)→(19,23) | AUTHORED-CANON (HIGH) — 13 pts |
| Mirewend Sinks | boglands | (24,36)→(27,35)→(30,35)→(33,35)→(34,36)→(35,38)→(35,41)→(34,44)→(31,45)→(28,45)→(25,44)→(24,42)→(24,39)→(24,36) | AUTHORED-CANON (LOW) — 14 pts |
| Sallow Marches | deltaic wetland | (52,80)→(55,79)→(58,79)→(61,79)→(64,80)→(64,83)→(64,86)→(64,90)→(62,91)→(59,91)→(56,91)→(53,90)→(52,87)→(52,83)→(52,80) | AUTHORED-CANON (LOW) — 15 pts |
| Cindern Waste | ash badland | (80,62)→(83,61)→(86,61)→(89,62)→(90,64)→(90,67)→(90,72)→(88,73)→(85,73)→(82,72)→(80,70)→(79,67)→(80,62) | AUTHORED-CANON (LOW) — 13 pts |
| Bonepan Flats | salt badland | (51,70)→(53,69)→(56,69)→(59,69)→(61,70)→(62,72)→(62,75)→(61,78)→(59,79)→(56,79)→(53,78)→(51,76)→(51,73)→(51,70) | AUTHORED-CANON (LOW) — 14 pts |
| Marrowdowns (terrain) | chalk downs | (45,60)→(47,59)→(50,59)→(53,59)→(55,60)→(56,63)→(56,67)→(55,70)→(52,71)→(49,71)→(47,70)→(45,67)→(44,63)→(45,60) | AUTHORED-CANON (LOW) — 14 pts |
| Wender Steppe | cold steppe | (40,12)→(43,11)→(47,11)→(51,11)→(55,12)→(56,15)→(56,19)→(55,22)→(52,23)→(48,23)→(44,23)→(41,22)→(40,19)→(40,15)→(40,12) | AUTHORED-CANON (LOW) — 15 pts |

---

## §10. Regional Boundary Polygons (all map-authoritative regions)

Area-fill bounds (render-grid). Far regions are faint fills. **All polygons are AUTHORED-CANON committed rings; no "infer from centroid" derivation remains.** Boundary waypoints are ordered clockwise from the NW corner of each region.

> **Definitive region count (resolved 2026-06-18, Cartography Determinism Cleanup):** there are **18 standalone map-authoritative regions, each with its own region map packet** in `04_world_atlas/region_map_packets/` (the 5 NW/cluster regions — Sundering Reach, Ashgarden Vale, Tollwood, Pale Coast, Caradril — plus 13 far regions, the last of which is the optional Highmark Passes). The table below has 19 rows because the last row, **Cindern Waste, is NOT a standalone region** — it is the ash-badland **terrain sub-zone within the Emberfell Theocracy region** (its rain-shadow), listed here for its boundary polygon and covered in `region_map_packets/REGION_EMBERFELL_THEOCRACY.md`, not in its own packet. Likewise **the Drowned Steps** is a submerged-ruin sub-area (adventure site D30) **within the Sallowmarch Protectorate**, not a region. Use **18** as the region/packet count everywhere; "19" only when counting Cindern Waste as a named terrain label.

| Region | Center (x,y) | Boundary polygon (x,y) — ordered ring | Provenance |
|---|---|---|---|
| Sundering Reach | (24,23) | (20,19)→(22,18)→(25,18)→(27,18)→(28,19)→(29,22)→(29,26)→(28,28)→(25,28)→(22,28)→(20,26)→(20,23)→(20,19) | AUTHORED-CANON (HIGH) — 13 pts |
| Ashgarden Vale | (25,31) | (21,28)→(23,27)→(26,27)→(28,27)→(30,28)→(31,31)→(31,33)→(30,35)→(27,36)→(25,36)→(22,35)→(21,33)→(21,30)→(21,28) | AUTHORED-CANON (HIGH) — 14 pts |
| Tollwood | (32,22) | (29,18)→(31,17)→(34,17)→(36,18)→(37,21)→(36,25)→(35,26)→(33,27)→(30,27)→(28,25)→(28,21)→(29,18) | AUTHORED-CANON (HIGH) — 12 pts |
| Pale Coast | (14,21) | (10,17)→(12,16)→(15,16)→(17,17)→(18,18)→(18,22)→(18,25)→(17,26)→(14,27)→(11,26)→(10,23)→(10,19)→(10,17) | AUTHORED-CANON (HIGH) — 13 pts |
| Caradril (city-state hinterland) | (34,35) | (31,32)→(33,31)→(35,31)→(37,32)→(38,34)→(38,37)→(37,38)→(35,38)→(33,38)→(31,37)→(31,34)→(31,32) | AUTHORED-CANON (HIGH) — 12 pts |
| Verdance Reaches | (42,42) | (38,38)→(40,37)→(43,37)→(46,37)→(48,38)→(49,41)→(49,45)→(48,48)→(45,49)→(42,49)→(39,48)→(38,45)→(38,41)→(38,38) | AUTHORED-CANON (LOW) — 14 pts |
| Glassmere League | (55,50) | (50,45)→(53,44)→(56,44)→(59,44)→(60,45)→(61,48)→(61,52)→(60,55)→(57,56)→(54,56)→(51,55)→(50,52)→(50,48)→(50,45) | AUTHORED-CANON (LOW) — 14 pts |
| Marrowdowns | (50,66) | (45,60)→(47,59)→(50,59)→(53,59)→(55,60)→(56,63)→(56,67)→(55,70)→(52,71)→(49,71)→(47,70)→(45,67)→(44,63)→(45,60) | AUTHORED-CANON (LOW) — 14 pts |
| Saltmere Reaches | (60,70) | (55,66)→(58,65)→(62,65)→(64,65)→(66,66)→(67,69)→(67,73)→(66,76)→(63,77)→(60,77)→(57,77)→(55,74)→(55,70)→(55,66) | AUTHORED-CANON (LOW) — 14 pts |
| Sallowmarch Protectorate | (58,84) | (53,80)→(55,79)→(58,79)→(61,79)→(63,80)→(63,83)→(63,86)→(63,88)→(60,89)→(57,89)→(54,88)→(53,85)→(53,82)→(53,80) | AUTHORED-CANON (LOW) — 14 pts |
| Hollow Gulf Ports | (66,90) | (60,86)→(62,85)→(65,85)→(68,85)→(70,85)→(72,86)→(73,89)→(72,93)→(70,94)→(66,94)→(62,94)→(60,92)→(59,89)→(60,86) | AUTHORED-CANON (LOW) — 14 pts |
| Wender Steppe | (46,16) | (40,12)→(43,11)→(47,11)→(51,11)→(55,12)→(56,15)→(56,19)→(55,22)→(52,23)→(48,23)→(44,23)→(41,22)→(40,19)→(40,15)→(40,12) | AUTHORED-CANON (LOW) — 15 pts |
| Karran Marches | (74,18) | (70,14)→(72,13)→(75,13)→(78,13)→(80,14)→(81,17)→(81,21)→(80,24)→(77,25)→(74,25)→(71,24)→(70,21)→(70,17)→(70,14) | AUTHORED-CANON (LOW) — 14 pts |
| Emberfell Theocracy / Ashfast | (80,62) | (76,56)→(79,55)→(82,55)→(84,55)→(86,56)→(87,59)→(87,63)→(86,67)→(84,69)→(81,69)→(78,68)→(76,65)→(76,60)→(76,56) | AUTHORED-CANON (LOW) — 14 pts |
| Concord Heartlands / Ruin'd Crown | (62,56) | (58,52)→(60,51)→(63,51)→(65,51)→(66,52)→(67,55)→(67,58)→(66,60)→(63,61)→(61,61)→(59,60)→(58,58)→(58,54)→(58,52) | AUTHORED-CANON (LOW) — 14 pts |
| Hethewald Free Holds | (72,40) | (66,34)→(68,33)→(72,33)→(76,33)→(78,34)→(79,37)→(79,41)→(78,45)→(75,47)→(72,47)→(69,46)→(66,44)→(65,40)→(66,36)→(66,34) | AUTHORED-CANON (LOW) — 15 pts |
| Sunmark | (44,80) | (38,75)→(41,74)→(44,74)→(47,74)→(50,75)→(51,78)→(51,82)→(50,85)→(47,86)→(44,86)→(41,86)→(38,85)→(37,82)→(37,78)→(38,75) | AUTHORED-CANON (LOW) — 15 pts |
| Highmark Passes (late frontier) | (30,8) | (26,7)→(29,6)→(33,6)→(37,6)→(41,6)→(44,7)→(44,9)→(42,11)→(38,11)→(34,11)→(30,11)→(27,10)→(26,9)→(26,7) | AUTHORED-CANON (LOW) — 14 pts |
| Cindern Waste (within Emberfell) | (84,66) | (80,62)→(83,61)→(86,61)→(89,62)→(90,64)→(90,67)→(90,72)→(88,73)→(85,73)→(82,72)→(80,70)→(79,67)→(80,62) | AUTHORED-CANON (LOW) — 13 pts |

> Sunder Heights is a Reach wilderness highland, not a separate political region; its polygon is in §8/§9.

---

## §11. Long-Distance Road / Trade-Route Polylines

| Route | Type | Ordered waypoints (x,y) | Player-safe | Confidence |
|---|---|---|---|---|
| Verdance Road | land | (34,35) Caradril → (40,40) → (55,50) Glassmere | yes | LOW |
| Glasswater Run | river/road corridor | (55,50) Glassmere → (60,66) → (66,90) Hollow Gulf Ports | yes | LOW |
| Greatspine Crown Road *(contested)* | mountain pass | (55,50) Glassmere → (62,56) Concord Heartlands → south | yes (mark contested) | LOW |
| Salt Road | land | (14,21) Pale Coast → (37,54) → (60,70) Saltmere Reaches | yes | LOW |
| Hethe Tollway | land | (74,18) Karran Marches → (77,34) → (80,50) Calm Reach coast | yes | LOW |
| South Road | land (in-cluster) | (24,26) Candlewick → (25,30) Tilbrook → (25,32) Orchardmere → (40,33) downs → (34,35) Caradril | yes | HIGH |
| East Road | land (in-cluster) | (27,23) Kettle Bridge → (30,22) Tollstone Cross → (33,22) Hartfell → (34,35) Caradril | yes | HIGH |
| Pale Road | land (in-cluster) | (20,22) Saltmargin → (13,20) Cobble Strand → (12,23) Wrackmouth | yes | HIGH |

---

## §12. Sea-Lane Routes

| Sea route | Ordered waypoints (x,y) | Player-safe | Confidence |
|---|---|---|---|
| Pale Coast Sea-Route | (12,23) Wrackmouth → (15,32) Verdance mouth → up-Verdance → (34,35) Stillwater/Caradril → (continues S past cluster) | yes (avoid the Skerries ~10,22 — gated) | HIGH |
| South Sea Lanes | (66,90) Hollow Gulf → off-map S (edge-arrow "to overseas lands") | yes (dashed arrows) | LOW |

**Ports and river mouths (named render points):** Wrackmouth port (12,23); the Verdance sea-mouth (15,32); the Stillwater quays (34,35); Calderport (65,89); Saltgate (69,91); the Mardenmouth wharves (63,88); Reedmouth (60,85).

---

## §12b. Bridges, Ferries, Fords, Locks, Passes, Toll Points

| Feature | Type | Position (x,y) | Route | Confidence |
|---|---|---|---|---|
| Kettle Bridge (Mirewend crossing) | bridge / toll-town | (27,23) | East Road, Mirewend | HIGH |
| Reedford (central ford) | ford | (25,24) | in-Reach road | MEDIUM |
| Sashe's Crossing | fen ford/guide-crossing | (22,25) Greyfens edge | Greyfens | MEDIUM |
| The Drowned Mile (flooded causeway) | flooded ford-stretch | (26,24) | Concord road | MEDIUM |
| The Green Mile (drowned road) | washed-out causeway | (30,22) | East Road, Tollwood | MEDIUM |
| Tollstone Cross (toll-station) | road toll point | (30,22) | East Road | MEDIUM |
| The Greenward Toll-Station | Concord road-node toll | (31,22) | East Road | LOW |
| Verdance mouth ferry (to up-river) | sea→river transfer | (15,32) | Pale Coast Sea-Route | MEDIUM |
| Caradril river-bridges (×2) + ferry | city bridges/ferry | (34,35) | intra-city (see CARADRIL_CITY_MAP) | HIGH |
| The Nine Locks | lock-staircase | (43,43) | Verdance Road | LOW |
| The Three Bridges (Glassmere) | city river-crossings | (55,50) | intra-Glassmere | LOW |
| Tollreach (Hethe toll-camp) | river toll point | (75,37) | Hethe Tollway | LOW |
| Highmark passes | mountain passes | (30,8)/(40,8) | far-N frontier | LOW |
| Greatspine passes (Crown Road) | mountain passes | (60,52) | Crown Road | LOW |

---

## §13. Player-Safe Render Layer (features that appear on the player map)

All of the following may be rendered and labeled on a player-facing map (per `PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md`):

- **Regions:** all five authored (Sundering Reach, Ashgarden Vale, Tollwood, Pale Coast, Caradril) + all far placeholders drawn faint.
- **Seas/water:** Pale Sea, Sunder Ocean, Calm Reach, Hollow Gulf, Saltmere, Wracking Straits, Stillwater, Hollowmere basin (dark water, no depth), Orchardmere lake.
- **Rivers:** Verdance, Glasswater, Mirewend, Ammet, Mardenflow, Hethe.
- **Mountains/terrain:** Highmark Spine, Sunder Heights, Karran Teeth, Greatspine/Sundering Wall, Emberfells, Ghostmark Range, Tollwood, Hethewood, Sunmark Wilds, Greyfens, Mirewend Sinks, Sallow Marches, Cindern Waste, Bonepan Flats, Marrowdowns, Wender Steppe.
- **Routes:** all of §11 + §12 (route geometry is player-safe).
- **Settlements:** every `render_on_reference_map=true` anchor in `FULL_CONTINENT_SETTLEMENT_ANCHORS.md`.
- **Adventure sites:** only those marked **player-map visibility: visible** in `ADVENTURE_SITE_CARTOGRAPHY_INDEX.md` (surface ruins/landmarks drawn as labeled hazard landmarks — e.g. "deep wood — do not enter," "wrecking reef," "ruined lighthouse"), never as nodes.

---

## §14. DM-Only Render Layer (NEVER on player maps)

The following are **DM-only** and must never appear on a player-facing map — not as a label, line, area, depth annotation, or implication:

- **The Concord Deep** — subsurface node-network, hub at (24,24) beneath the basin. No surface label.
- **The Under-Shrine / Drowned Keystone** — endgame, **directly below Hollowmere (24,23), deepest Z** (vertical, not lateral).
- **The Hollow Court seat** — beneath the basin; DM-only.
- **The node-network links** — keystone basin ↔ Deep Adit (Harrowgast) ↔ Sunken Tollhouse (Kettle Bridge) ↔ Saint Veddow's Tomb (Vale) ↔ Drowned Lamp/Skerry Shrine (Coast) ↔ Sunken Wards (Caradril) ↔ Tollwood deep — render only on DM Layer 2/7.
- **Adventure site D23 (Under-Shrine Approach)** — DM-only; never on any map shared with the player.
- The endgame is **vertical (down beneath the NW cluster)**, never a distant land. Far ruins (Concord Heartlands, Saltmere Drowned Towns, etc.) are drawn only as broken, unexplained **surface** ruin-country.

See `WORLD_MAP_LAYERS.md` Layers 2 and 7 for the full DM-only geography.

---

## §15. Campaign-Cluster ↔ Full-Continent Transform

The campaign-area grid (`WORLD_MAP_COORDINATES.md`, 0–100, NW quarter only) embeds into this full-continent grid in the NW corner:

```
full_X = 8 + (campaign_X * 0.32)      → campaign 0–100 maps to full 8–40 on X
full_Y = 8 + (campaign_Y * 0.34)      → campaign 0–100 maps to full 8–42 on Y
```

Spot-checks (campaign → full): Hollowmere (50,45) → (24.0,23.3); Caradril (82,80) → (34.2,35.2); Wrackmouth (14,44) → (12.5,23.0). For **fine intra-cluster placement**, use the campaign grid in `WORLD_MAP_COORDINATES.md`; for **continental placement**, use this file's render grid.

---

## §16. Confidence and Provenance Summary (geometry features)

All polygons, polylines, and coastline segments in §4, §7, §8, §9, and §10 are now **AUTHORED-CANON** — committed waypoint rings and polylines that fully specify shape without renderer inference. Confidence ratings below indicate the underlying geographic certainty (HIGH = derived from campaign play; LOW = far-continent placeholder geometry), not the geometry's specificity.

> **Four-status confidence standard (Strict Cartography Determinism Cleanup, 2026-06-18):** the canonical per-feature confidence taxonomy lives in `MAP_FEATURE_REGISTRY.md` and uses exactly four statuses — **AUTHORITATIVE** (coordinate-anchored by direct authorship), **DERIVED_CANON** (committed map position reasoned from named anchors + region context; a mapper must use it), **NOT_MAP_AUTHORITATIVE** (background/off-map/too-vague; non-blocking; draw soft or omit), **CARTOGRAPHY_BLOCKER** (cannot place without invention; blocks MAP READY — current count **0**). The HIGH/MEDIUM/LOW labels retained in this file's geometry tables are **geographic-certainty context only**, not render-confidence; the registry's four-status column is the render-confidence authority. No map-authoritative feature in this file remains DERIVED/placeholder/sketched — all geometry is committed AUTHORED-CANON.

> **DERIVED_CANON tier (formerly "DERIVED-CANONIZED"; renamed in Strict Cartography Determinism Cleanup pass 2026-06-18):** every far-continent **major feature** that was derived from registered narrative/lore rather than from campaign play — the three far cities (**Glassmere** two-bank/Three-Bridges layout; **Calderport** crescent-harbor layout; **Ashfast** caldera fortress-temple layout), the major far rivers (**Glasswater, Mardenflow, Hethe**), the major far ranges (**Karran Teeth, Greatspine/Sundering Wall, Emberfells, Ghostmark Range**), and the major far routes (**Verdance Road, Glasswater Run, Greatspine Crown Road, Salt Road, Hethe Tollway**) — is now **DERIVED_CANON**: its committed waypoint geometry (in §4/§7/§8/§9/§11 here, and in the route/water/terrain authority files and city packets) is **authoritative for mapping**, even though its underlying geographic confidence stays LOW. A "LOW" tag on these rows means "place it where stated; the exact far-survey detail is placeholder," NOT "geometry missing." The far city layouts are derived per each city packet's stated derivation basis (Glassmere from "the Three Bridges" two-bank canon; Calderport from harbor-crescent canon; Ashfast from fortress-temple-against-caldera canon). Minor/unpinnable far features (off-grid overseas isles, diffuse Fever Channels, the Saltmere's shifting waterline) remain **NOT_MAP_AUTHORITATIVE** and are drawn soft/faint without precise borders.

| Provenance / Confidence | Count | Notes |
|---|---|---|
| AUTHORED-CANON / HIGH | ~24 | NW cluster regions/water/routes/rivers; Pale Sea; Stillwater; Hollowmere basin; Mirewend; South/East/Pale Roads; Pale Coast Sea-Route |
| AUTHORED-CANON / MEDIUM | ~16 | NW-adjacent coastline, Sunder Ocean, Calm Reach, Ammet, Highmark Spine W, Orchardmere lake, in-cluster fords/crossings |
| AUTHORED-CANON / LOW | ~70 | All far-continent regions, rivers, ranges, terrain polygons, far routes, far lakes/seas, far bridges/passes — geometry committed per Phase 1 of the Cartography Determinism build |
| DERIVED | 0 | Eliminated; all features now have explicit waypoints |

---

## §17. Map Gaps (four-status classification)

All map-authoritative geometry is committed; the items below are either DERIVED_CANON (committed for mapping, with placeholder far-survey context) or NOT_MAP_AUTHORITATIVE (off-grid/optional — draw soft or omit, non-blocking).

1. **Far-continent coastline** (Hollow Gulf → Wracking Straits) — **DERIVED_CANON**: §4 gives committed ordered waypoints; the exact frontier cape/inlet detail is placeholder context. A mapper draws the committed waypoints.
2. **Far river courses** (Glasswater mid-course, Hethe, Mardenflow) — **DERIVED_CANON**: §7 gives committed source→waypoint→mouth polylines (each passing through its named settlements as waypoints); meander micro-detail between committed waypoints is illustrative context.
3. **Greatspine/Sundering Wall crest line** — **DERIVED_CANON**: §8 gives a committed NW–SE spine polyline; the Crown Road pass point (60,52) is committed.
4. **Far-region internal micro-geography** (settlement spread within a far region beyond the committed anchor points) — **NOT_MAP_AUTHORITATIVE**: deep internal street/field maps are deferred; the committed settlement anchors and region polygons are sufficient to render region and settlement-floor maps (see far-region packets).
5. **Overseas landmasses** (Surren, Iron Skards, Sundered Isles) — **NOT_MAP_AUTHORITATIVE**: off-grid edge-arrows only; not part of the Orrun render.

All items are **non-blocking** for player-safe and DM-only continent/region/city/settlement rendering. **CARTOGRAPHY_BLOCKER count: 0.**

## Related Files

- [`MAP_FEATURE_REGISTRY.md`](MAP_FEATURE_REGISTRY.md) · [`ROADS_RIVERS_AND_ROUTES_AUTHORITY.md`](ROADS_RIVERS_AND_ROUTES_AUTHORITY.md) · [`WATER_AND_SHORELINE_AUTHORITY.md`](WATER_AND_SHORELINE_AUTHORITY.md) · [`MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md`](MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md)
- [`FULL_WORLD_MAP_COORDINATES.md`](FULL_WORLD_MAP_COORDINATES.md) · [`WORLD_MAP_COORDINATES.md`](WORLD_MAP_COORDINATES.md) · [`PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md`](PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md)
- [`FULL_CONTINENT_SETTLEMENT_ANCHORS.md`](FULL_CONTINENT_SETTLEMENT_ANCHORS.md) · [`REGION_INDEX.md`](REGION_INDEX.md) · [`WORLD_MAP_LAYERS.md`](WORLD_MAP_LAYERS.md)
- [`../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
- region map packets: [`region_map_packets/`](region_map_packets/) · city packets: [`../06_settlements/city_map_packets/`](../06_settlements/city_map_packets/) · settlement packets: [`../06_settlements/settlement_map_packets/`](../06_settlements/settlement_map_packets/)
