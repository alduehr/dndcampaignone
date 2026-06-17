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
- **Orientation:** **North = top, west = left.** (X increases east; Y increases north on the authoring axis described in §2 — see the axis note carefully.)
- **Scale:** one full-continent grid unit ≈ **8–12 miles**; corner-to-corner ≈ **2–3 months' travel** by road. The NW campaign cluster's internal scale is finer (one campaign-grid unit ≈ 2–2.6 miles; corner-to-corner of the cluster ≈ 200–260 miles / ~12 days).
- **Canonical travel unit:** the **established day-count** (see `MAP_DESCRIPTION.md`, `TRAVEL_ROUTES_RING1.md`), not miles. Mileage here is a drawing aid only.

---

## §2. Full-Continent Coordinate System (authoritative)

The full-continent grid is **0–100 on both axes**. Two conventions are in play across the repo; this file states both and uses the **render convention** for all geometry so a mapper can place features directly.

- **Render convention (used in this file and all render manifests):** (0,0) = **NW corner** (top-left); X = 0 west, X = 100 east; **Y = 0 north (top), Y = 100 south (bottom)**. This matches `FULL_WORLD_MAP_COORDINATES.md`, `PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md`, and `FULL_CONTINENT_SETTLEMENT_ANCHORS.md`. **All coordinates in this file use this convention.**
- **Task SW-origin convention (for reference only):** the cartography-pass brief describes (0,0) = SW corner with Y increasing northward. To convert a render-convention point to the SW-origin convention: `y_sw = 100 − y_render`. Example: Hollowmere render (24,23) = SW-origin (24,77). **Mappers should use the render convention (Y=0 at top) for consistency with every existing atlas file.** The SW note exists only so the brief's framing is reconciled.

The NW campaign cluster occupies render-grid **X 8–40, Y 8–42** (upper-left quarter). It is the only high-detail zone. The campaign-area grid in `WORLD_MAP_COORDINATES.md` is a ~3× zoom on this corner; see §15 for the transform.

---

## §3. Continent Outline (major cape/bay features)

Orrun is a large continent that tilts from a **cold, broken NW frontier** to a **warm, rich S/SE**. Render convention coastline, clockwise from the NW corner:

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

Draw the W and S coasts as a single continuous shoreline; the N coast is short. Waypoints are ordered N→S down the W coast, then W→E along the S coast.

| Coast segment | Ordered waypoints (x,y) | Confidence |
|---|---|---|
| W coast (Pale Sea) | (12,18) Cobble Strand cove → (12,23) Wrackmouth → (14,28) → (15,32) Verdance mouth → (10,45) → (5,58) → (2,64) Wracking Straits | MEDIUM (NW HIGH near cluster) |
| N coast (Sunder Ocean) | (20,6) → (35,5) → (50,4) → (65,5) (behind the Highmark Spine / Karran Teeth) | LOW |
| S coast (W half — Sallow Marches/Sunmark) | (40,90) → (50,88) → (55,86) Mardenflow delta edge | LOW |
| S coast (Hollow Gulf) | (60,92) → (66,92) Hollow Gulf mouth → (72,91) Saltgate headland | LOW |
| SE coast (Glass Coast / Calm Reach) | (78,88) → (86,80) Glass Coast → (90,70) → (88,55) Hethe mouth | LOW |

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

All rivers drawn as single polylines through ordered waypoints. Label each **once** (see render manifest §5).

| River | Ordered waypoints (x,y) | Source → mouth | Confidence |
|---|---|---|---|
| Verdance | (48,46) interior/upland source → (40,40) → (34,35) Caradril/Stillwater → (24,33) → (15,32) Pale Sea mouth | rises in the interior toward Glassmere country; widens at the Stillwater; reaches the Pale Sea S of the Pale Coast | HIGH (cluster) / MEDIUM (upper) |
| Glasswater | (58,40) Greatspine source → (55,50) Glassmere → (60,66) → (64,88) Hollow Gulf delta | the continent's largest river; the main commercial artery | LOW |
| Mirewend | (25,16) Sunder Heights source → (24,23) Hollowmere basin → (24,28) → (28,40) Mirewend Sinks drain (NW system) | the Reach's slow peat-dark artery; floods in autumn | HIGH (cluster) |
| Ammet | (28,28) Vale headwaters (toward Tollwood) → (25,30) Tilbrook → (25,32) Orchardmere → joins the Verdance / drains coastally | the Vale's river | MEDIUM |
| Mardenflow | (52,64) Marrowdowns source → (55,76) → (58,84) Sallow Marches delta → (66,92) Hollow Gulf | drains the southern plains; floods seasonally | LOW |
| Hethe | (74,22) Karran Teeth source → (76,32) → (78,40) → (80,50) Calm Reach mouth | eastern trade river; toll-contested | LOW |

---

## §8. Mountain Range Polylines (ordered spine waypoints)

| Range | Ordered waypoints (x,y) | Confidence |
|---|---|---|
| The Highmark Spine | (26,10) W end → (35,9) → (44,8) E end | MEDIUM (W) / LOW (E) |
| The Sunder Heights | (21,18) → (24,15) → (28,13) (highland belt below the Highmark Spine) | HIGH |
| The Karran Teeth | (70,20) → (74,16) → (80,13) | LOW |
| The Greatspine / Sundering Wall | (50,38) NW end → (58,48) → (62,56) → (70,64) SE end | LOW |
| The Emberfells | (76,57) → (80,60) → (84,64) (volcanic highland) | LOW |
| The Ghostmark Range | (53,70) → (58,72) → (63,74) (low eroded ring S of the Saltmere) | LOW |

---

## §9. Forest / Wetland / Badland / Highland / Steppe Polygons

Each polygon is an ordered ring of render-grid waypoints (loose/faint for far placeholders).

| Zone | Type | Polygon waypoints (x,y) | Confidence |
|---|---|---|---|
| Tollwood | forest | (29,18)→(36,18)→(36,26)→(29,26) | HIGH |
| Hethewood | great forest | (64,32)→(80,32)→(80,46)→(64,46) | LOW |
| Sunmark Wilds | warm forest | (38,75)→(50,75)→(50,86)→(38,86) | LOW |
| Greyfens | fog marsh | (19,23)→(25,23)→(25,28)→(19,28) | HIGH |
| Mirewend Sinks | boglands | (24,36)→(34,36)→(34,44)→(24,44) | LOW |
| Sallow Marches | deltaic wetland | (52,80)→(64,80)→(64,90)→(52,90) | LOW |
| Cindern Waste | ash badland | (80,62)→(90,62)→(90,72)→(80,72) | LOW |
| Bonepan Flats | salt badland | (51,70)→(61,70)→(61,78)→(51,78) | LOW |
| Marrowdowns | chalk downs | (45,60)→(55,60)→(55,70)→(45,70) | LOW |
| Wender Steppe | cold steppe | (40,12)→(55,12)→(55,22)→(40,22) | LOW |

---

## §10. Regional Boundary Polygons (all map-authoritative regions)

Loose area-fill bounds (render-grid). Far placeholders are faint. Boundaries derived from centroids + adjacency in the render manifest §6; marked DERIVED where a footprint was inferred.

| Region | Center (x,y) | Boundary polygon (x,y) | Confidence |
|---|---|---|---|
| Sundering Reach | (24,23) | (20,19)→(28,19)→(28,28)→(20,28) | HIGH |
| Ashgarden Vale | (25,31) | (21,28)→(30,28)→(30,35)→(21,35) | HIGH |
| Tollwood | (32,22) | (29,18)→(36,18)→(36,26)→(29,26) | HIGH |
| Pale Coast | (14,21) | (10,17)→(18,17)→(18,26)→(10,26) | HIGH |
| Caradril (city-state hinterland) | (34,35) | (31,32)→(37,32)→(37,38)→(31,38) | HIGH |
| Verdance Reaches | (42,42) | (38,38)→(48,38)→(48,48)→(38,48) | LOW |
| Glassmere League | (55,50) | (50,45)→(60,45)→(60,55)→(50,55) | LOW |
| Marrowdowns | (50,66) | (45,60)→(55,60)→(55,70)→(45,70) | LOW |
| Saltmere Reaches | (60,70) | (55,66)→(66,66)→(66,76)→(55,76) | LOW |
| Sallowmarch Protectorate | (58,84) | (53,80)→(63,80)→(63,88)→(53,88) | LOW |
| Hollow Gulf Ports | (66,90) | (60,86)→(72,86)→(72,94)→(60,94) | LOW |
| Wender Steppe | (46,16) | (40,12)→(55,12)→(55,22)→(40,22) | LOW |
| Karran Marches | (74,18) | (70,14)→(80,14)→(80,24)→(70,24) | LOW |
| Emberfell Theocracy / Ashfast | (80,62) | (76,56)→(86,56)→(86,68)→(76,68) | LOW |
| Concord Heartlands / Ruin'd Crown | (62,56) | (58,52)→(66,52)→(66,60)→(58,60) | LOW |
| Hethewald Free Holds | (72,40) | (66,34)→(78,34)→(78,46)→(66,46) | LOW |
| Sunmark | (44,80) | (38,75)→(50,75)→(50,85)→(38,85) | LOW |
| Highmark Passes (late frontier) | (30,8) | (26,7)→(44,7)→(44,11)→(26,11) | LOW |
| Cindern Waste (within Emberfell) | (84,66) | (80,62)→(90,62)→(90,72)→(80,72) | LOW |

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

## §16. Confidence Summary (geometry features)

| Confidence | Count (geometry features in this file) | Notes |
|---|---|---|
| HIGH | ~24 | NW cluster regions/water/routes/rivers; Pale Sea; Stillwater; Hollowmere basin; Mirewend; South/East/Pale Roads; Pale Coast Sea-Route |
| MEDIUM | ~16 | NW-adjacent coastline, Sunder Ocean, Calm Reach, Ammet, Highmark Spine W, Orchardmere lake, in-cluster fords/crossings |
| LOW | ~70 | All far-continent regions, rivers, ranges, terrain polygons, far routes, far lakes/seas, far bridges/passes |
| DERIVED | (subset of LOW) | Far-region boundary polygons inferred from centroid + adjacency; far river/range polylines drawn from endpoint pairs |

---

## §17. Unresolved Map Gaps

1. **Far-continent coastline** between the Hollow Gulf and the Wracking Straits is sketched at LOW confidence; exact capes/inlets are not canon-fixed. Drawn loosely is correct.
2. **Far river courses** (Glasswater mid-course, Hethe, Mardenflow) use endpoint-pair polylines; their meanders are illustrative, not canon.
3. **Greatspine/Sundering Wall exact crest line** is a NW–SE diagonal placeholder; the Crown Road's pass point (60,52) is DERIVED.
4. **Far-region internal geometry** (settlement spread within each far region) is light NPC-anchor only; deep internal maps are deferred (see far-region packets).
5. **Overseas landmasses** (Surren, Iron Skards, Sundered Isles) are off-grid edge-arrows only; not part of the Orrun render.

All gaps are **non-blocking** for player-safe and DM-only continent/region/city/settlement rendering.

## Related Files

- [`MAP_FEATURE_REGISTRY.md`](MAP_FEATURE_REGISTRY.md) · [`ROADS_RIVERS_AND_ROUTES_AUTHORITY.md`](ROADS_RIVERS_AND_ROUTES_AUTHORITY.md) · [`WATER_AND_SHORELINE_AUTHORITY.md`](WATER_AND_SHORELINE_AUTHORITY.md) · [`MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md`](MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md)
- [`FULL_WORLD_MAP_COORDINATES.md`](FULL_WORLD_MAP_COORDINATES.md) · [`WORLD_MAP_COORDINATES.md`](WORLD_MAP_COORDINATES.md) · [`PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md`](PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md)
- [`FULL_CONTINENT_SETTLEMENT_ANCHORS.md`](FULL_CONTINENT_SETTLEMENT_ANCHORS.md) · [`REGION_INDEX.md`](REGION_INDEX.md) · [`WORLD_MAP_LAYERS.md`](WORLD_MAP_LAYERS.md)
- [`../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
- region map packets: [`region_map_packets/`](region_map_packets/) · city packets: [`../06_settlements/city_map_packets/`](../06_settlements/city_map_packets/) · settlement packets: [`../06_settlements/settlement_map_packets/`](../06_settlements/settlement_map_packets/)
