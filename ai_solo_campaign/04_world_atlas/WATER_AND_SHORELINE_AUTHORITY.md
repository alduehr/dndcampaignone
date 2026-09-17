# WATER_AND_SHORELINE_AUTHORITY.md — Deterministic Water Geometry

---
type: region
secrecy: mixed
status: static
region: Orrun
factions: []
level_range: 1-20
related: [CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, ROADS_RIVERS_AND_ROUTES_AUTHORITY.md, MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md, MAP_FEATURE_REGISTRY.md, PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md]
tags: [type:map, secrecy:mixed, function:cartography, water-geometry, coordinates, orrun, full-continent]
---

> **Secrecy classification:** Mixed. Water geometry is player-safe; the only DM-only note is that the Hollowmere basin's *interior/depth* (the drowned shrine/keystone) is never rendered. Never hand directly to the player.

## AI Use

Deterministic geometry for every water feature of Orrun: oceans, inland seas, bays, straits, harbor-lakes, lakes, rivers, wetlands, and key crossings. All coordinates are full-continent **render-grid** (X=0 west, X=100 east, Y=0 north, Y=100 south). Lakes/bays are polygons; rivers are polylines (full course geometry in `ROADS_RIVERS_AND_ROUTES_AUTHORITY.md`). Use to draw coastlines, fills, and crossing markers without guessing.

> **Confidence (Strict Cartography Determinism Cleanup, 2026-06-18):** every water body below has a committed polygon (seas/bays/lakes) or polyline (rivers/coastlines) — no endpoint-only or shapeless water remains. Per-feature render-confidence uses the four-status taxonomy in `MAP_FEATURE_REGISTRY.md`: the Pale Sea, Stillwater, Hollowmere basin, Orchardmere lake, and in-cluster crossings = **AUTHORITATIVE**; far seas/bays/inland-sea and far crossings (Sunder Ocean, Calm Reach, Hollow Gulf, Wracking Straits, Saltmere, Nine Locks, Three Bridges, Tollreach, Mardenflow ferries) = **DERIVED_CANON** (committed geometry; far-survey detail is placeholder context). The legacy HIGH/MEDIUM/LOW lines are geographic-certainty context only.

---

## OCEANS AND SEAS

### The Pale Sea
- **Type:** ocean · **Shore orientation:** water W, land E (the W coast of Orrun fronts it)
- **Geometry (W-margin fill):** polygon (0,5)→(10,5)→(10,60)→(0,60); label centroid (4,30)
- **Coastline (land edge, N→S):** (12,18)→(12,23) Wrackmouth→(14,28)→(15,32) Verdance mouth→(10,45)→(5,58)→(2,64) Wracking Straits
- **Adjacent settlements:** Wrackmouth (12,23, on shore), Cobble Strand (13,20, shingle cove).
- **Ports/docks:** Wrackmouth port (W side, 12,23); Verdance sea-mouth ferry (15,32).
- **Crossings:** none (open sea); the Pale Coast Sea-Route runs along it.
- **Navigability:** fully navigable, storm-battered · **Player-map visibility:** yes · **Confidence:** HIGH (NW) / MEDIUM (S)

### The Sunder Ocean
- **Type:** ocean · **Shore orientation:** water N, land S (tops the continent beyond the Highmark Spine)
- **Geometry (N-margin fill):** polygon (20,0)→(70,0)→(70,6)→(20,6); label centroid (50,2)
- **Coastline:** (20,6)→(35,5)→(50,4)→(65,5) (behind the Highmark Spine / Karran Teeth)
- **Adjacent settlements:** none authored (far cold-N frontier).
- **Navigability:** open, cold · **Player-map visibility:** yes · **Confidence:** MEDIUM

### The Calm Reach
- **Type:** warm sea · **Shore orientation:** water SE/S, land NW (the warm-rich SE corner)
- **Geometry (SE/S-margin fill):** polygon (70,85)→(95,85)→(95,98)→(70,98); label centroid (82,92)
- **Coastline:** (78,88) Glass Coast→(86,80)→(90,70)→(88,55) Hethe mouth
- **Adjacent settlements:** Calderport (65,89, opens into it via the Hollow Gulf), Saltgate (69,91).
- **Ports/docks:** Calderport (NW of the gulf), the Hethe mouth (88,55).
- **Navigability:** fully navigable; southern trade heart · **Player-map visibility:** yes · **Confidence:** MEDIUM

### The Hollow Gulf
- **Type:** major bay · **Shore orientation:** water S, land N (the Mardenflow/Glasswater delta mouth)
- **Geometry:** polygon (60,88)→(72,88)→(72,96)→(60,96); label centroid (66,92)
- **Adjacent settlements:** Calderport (65,89, NW shore), Saltgate (69,91, NE shore), Reedmouth (60,85, W delta).
- **Ports/docks:** Calderport (NW), Saltgate (NE), the Mardenmouth wharves (63,88).
- **Crossings:** delta ferries.
- **Navigability:** navigable; tidal at the delta · **Player-map visibility:** yes · **Confidence:** LOW

### The Wracking Straits
- **Type:** strait · **Shore orientation:** water far-W; narrows between Orrun and the off-grid Sundered Isles
- **Geometry:** polygon (0,58)→(5,58)→(5,70)→(0,70); label centroid (2,64)
- **Adjacent settlements:** none.
- **Navigability:** dangerous (storm narrows) · **Player-map visibility:** yes (optional/faint) · **Confidence:** LOW

### The Saltmere
- **Type:** inland salt sea · **Shore orientation:** water at center; land on all sides (ringed by the Saltmere Reaches)
- **Geometry (polygon):** (56,67)→(64,67)→(66,71)→(62,75)→(56,73); label centroid (60,70) ON the water
- **Adjacent settlements:** Brackhold (57,68, NW shore, on land), Saltcairn (63,73, SE shore), the Drowned Towns (60,71, submerged ruins on the shoreline).
- **Ports/docks:** salt-clan landings (LOW).
- **Crossings:** none (saline, receding).
- **Navigability:** shallow/receding; brackish · **Player-map visibility:** yes (water label on water; the Saltmere Reaches label on surrounding land) · **Confidence:** LOW

---

## HARBOR-LAKES AND LAKES

### The Stillwater
- **Type:** harbor-lake · **Shore orientation:** Caradril on the W/N shore; the Verdance feeds it from the W and drains it
- **Geometry (polygon):** (33,34)→(35,33)→(36,35)→(35,37)→(33,36); label centroid (34,35)
- **Adjacent settlements:** Caradril (34,35, W/N shore — the city wraps the lake's inland end).
- **Ports/docks:** the Stillwater quays / Counting-Quays (E/lake frontage of Caradril).
- **Crossings:** Caradril's river-bridges cross the Verdance, not the lake.
- **Navigability:** fully navigable (the campaign's grand water-arrival) · **Player-map visibility:** yes · **Confidence:** HIGH

### Hollowmere basin
- **Type:** flooded basin (harbor-lake-scale dark water) · **Shore orientation:** Hollowmere rings the rim; the lowest drainage point of the cluster
- **Geometry (polygon):** (23,22)→(25,22)→(25,24)→(23,24); label centroid (24,23)
- **Adjacent settlements:** Hollowmere (24,23, rings the basin).
- **Ports/docks:** stilt-house plank landings (no true port).
- **Crossings:** plank walkways over the boggy edges.
- **Navigability:** shallow, fog-bound; the deep basin is endgame-tier (off-limits early).
- **Player-map visibility:** yes — render as **dark water**, ominous but unexplained.
- **DM-only:** the basin's **interior/depth** is the drowned shrine / Under-Shrine / keystone — **never render depth, structure, or any subsurface annotation.** The "broken grey shapes" under the surface may be drawn as vague dark forms, never labeled.
- **Confidence:** HIGH (position/rim)

### Orchardmere lake
- **Type:** lake · **Shore orientation:** Orchardmere on its shore; fed by the Ammet
- **Geometry (polygon):** (24,31)→(26,31)→(26,33)→(24,33); label centroid (25,32)
- **Adjacent settlements:** Orchardmere (25,32, on shore).
- **Navigability:** small, calm · **Player-map visibility:** yes · **Confidence:** MEDIUM

---

## RIVERS (summary — full course geometry in ROADS_RIVERS_AND_ROUTES_AUTHORITY.md)

| River | Source (x,y) → Mouth (x,y) | Navigability | Key crossings (x,y) | Visibility | Survey Certainty |
|---|---|---|---|---|---|
| Verdance | (48,46) → Pale Sea mouth (15,32) | fully navigable Stillwater→mouth | Caradril bridges (34,35); Nine Locks (43,43) | yes | HIGH/MED |
| Glasswater | (58,40) → Hollow Gulf delta (64,88) | fully navigable mid-down | Three Bridges, Glassmere (55,50) | yes | LOW |
| Mirewend | (25,16) → Mirewend Sinks (28,40) | shallow/seasonal | Kettle Bridge (27,23); Reedford ford (25,24) | yes | HIGH |
| Ammet | (28,28) → NW drain | shallow | Tilbrook fords (25,29) | yes | MED |
| Mardenflow | (52,64) → Hollow Gulf (66,92) | seasonal/tidal delta | delta ferries | yes | LOW |
| Hethe | (74,22) → Calm Reach (80,50) | navigable mid-course | Tollreach toll (75,37) | yes | LOW |

---

## WETLANDS / FLOODED AREAS (water-character zones; terrain polygons in MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md)

| Wetland | Type | Polygon (x,y) | Water character | Visibility | Survey Certainty |
|---|---|---|---|---|---|
| The Greyfens | fog marsh | (19,23)→(25,23)→(25,28)→(19,28) | standing fen-water, fog; Sashe's Crossing (22,25) | yes | HIGH |
| The Mirewend Sinks | boglands | (24,36)→(34,36)→(34,44)→(24,44) | sinking bog, slow drains | yes | LOW |
| The Sallow Marches | deltaic wetland | (52,80)→(64,80)→(64,90)→(52,90) | tidal fever-delta; the Rice Sallows, Fever Channels | yes | LOW |
| The Drowned Steps | submerged causeway | offshore (54,90) | tidal, submerged pre-Concord ruin | label-only ("drowned steps") | LOW |

---

## KEY CROSSINGS (bridges / ferries / fords across water)

| Crossing | Type | Coords | Water | Side/notes | Survey Certainty |
|---|---|---|---|---|---|
| Kettle Bridge | bridge | 27,23 | Mirewend (E reach) | toll-town on the crossing | HIGH |
| Reedford | ford | 25,24 | Mirewend | central road ford-hamlet | MED |
| Sashe's Crossing | guide-ford | 22,25 | Greyfens | fen crossing; needs a guide | MED |
| Tilbrook fords | ford/mill | 25,29 | Ammet | Vale mill village | MED |
| Verdance mouth ferry | sea→river | 15,32 | Verdance/Pale Sea | the Pale Coast Sea-Route transfer | MED |
| Caradril river-bridges (×2) + ferry | bridges/ferry | 34,35 | Verdance | N/S bank crossings (see CARADRIL_CITY_MAP) | HIGH |
| The Nine Locks | lock-staircase | 43,43 | Verdance | Verdance Road up-corridor | LOW |
| The Three Bridges | city bridges | 55,50 | Glasswater | Glassmere's banking quarter | LOW |
| Tollreach | river toll | 75,37 | Hethe | outlaw toll-camp | LOW |
| Mardenflow delta ferries | ferry | ~58,86 | Mardenflow delta | Sallowmarch | LOW |

## Water Gaps (four-status classification)

All water geometry is committed; the items below are DERIVED_CANON (committed for mapping with placeholder far-survey context) or NOT_MAP_AUTHORITATIVE (off-grid, non-blocking).

1. **Far-continent coastline** (Hollow Gulf → Wracking Straits) — **DERIVED_CANON**: committed coastline waypoints in `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §4`; frontier inlet detail is placeholder context.
2. **Far river meanders** (Glasswater, Mardenflow, Hethe) — **DERIVED_CANON**: committed source→waypoint→mouth polylines (3+ intermediate waypoints each, passing through named settlements); micro-meanders are illustrative context.
3. **The Saltmere shoreline** — **DERIVED_CANON**: committed polygon (centroid 60,70); the receding waterline and the Drowned Towns' shifting edge are seasonal flavor, drawn at the committed polygon.
4. **Off-grid overseas waters** (beyond the Wracking Straits / South Sea Lanes) — **NOT_MAP_AUTHORITATIVE**: edge-annotations only.

All items are non-blocking for player-safe and DM-only water rendering. **CARTOGRAPHY_BLOCKER count: 0.**

## Related Files

- [`CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`](CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md) · [`ROADS_RIVERS_AND_ROUTES_AUTHORITY.md`](ROADS_RIVERS_AND_ROUTES_AUTHORITY.md) (full river geometry) · [`MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md`](MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md) · [`MAP_FEATURE_REGISTRY.md`](MAP_FEATURE_REGISTRY.md)
