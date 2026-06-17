# ROADS_RIVERS_AND_ROUTES_AUTHORITY.md — Deterministic Route Geometry

---
type: region
secrecy: mixed
status: static
region: Orrun
factions: []
level_range: 1-20
related: [CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, MAP_FEATURE_REGISTRY.md, WATER_AND_SHORELINE_AUTHORITY.md, TRAVEL_ROUTES_RING1.md, MAP_DESCRIPTION.md, PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md, WORLD_MAP_LAYERS.md]
tags: [type:map, secrecy:mixed, function:cartography, route-geometry, coordinates, orrun, full-continent]
---

> **Secrecy classification:** Mixed. Route geometry is player-safe; the DM-only overlay rows (Concord-Deep node crossings) name hidden features only to mark them DM-only. Never hand directly to the player.

## AI Use

Deterministic geometry for every named road, river, and sea-lane of Orrun. All coordinates are full-continent **render-grid** (X=0 west, X=100 east, Y=0 north, Y=100 south). Each route is a single polyline through ordered waypoints with place-name labels. Use with `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md` (master geometry) and `TRAVEL_ROUTES_RING1.md` (day-counts and travel events). Route labels are placed **once** (see render manifest §5); a waypoint is not a place label unless it has its own feature entry.

**Direction convention:** rivers run **source → mouth**; roads/sea-lanes run **start → end** as listed.

---

## ROADS AND LAND ROUTES

### Verdance Road
- **Type:** road · **Direction:** Caradril → Glassmere · **Importance:** primary
- **Waypoints:** (34,35) Caradril → (40,40) Marrowfen Stair approach → (43,43) the Nine Locks → (55,50) Glassmere
- **Terrain crossed:** Verdance river-corridor; rises from the Stillwater into settled interior.
- **Bridges/fords/ferries:** the Nine Locks (43,43); Verdance-corridor landings near Cresswater (39,45).
- **Toll/gates:** Marrowfen Stair locks-tolls.
- **Hazards:** river floods; up-corridor lordlings' tolls; bandits past the Locks.
- **Nearby settlements:** Marrowfen Stair (41,41), Lord's Wend (45,39, ~+4 E), Cresswater (39,45, ~-2 SW).
- **Player-map visibility:** yes · **Confidence:** LOW (campaign-end HIGH at Caradril)
- **DM-only overlay:** the Nine Locks Sunken Stair (D34) is a flooded relay-vault beneath the Locks — surface route player-safe; the vault is a node-fragment (DM Layer 7).

### Glasswater Run
- **Type:** river/road corridor · **Direction:** Glassmere → Hollow Gulf Ports · **Importance:** primary
- **Waypoints:** (55,50) Glassmere → (60,66) Cairnwater reach → (64,84) Mardenflow confluence → (66,90) Calderport
- **Terrain crossed:** the Glasswater river-plain; the continent's main commercial artery; tolled.
- **Bridges/fords/ferries:** Glassmere's Three Bridges (55,50); delta ferries near the Hollow Gulf.
- **Toll/gates:** league tolls at Glassmere; port-tolls at Calderport.
- **Hazards:** river piracy; delta fever (S end); seasonal floods.
- **Nearby settlements:** Cairnwater (58,53), Brackhold (57,68, ~+W via Salt Road branch), Fenward (57,82).
- **Player-map visibility:** yes · **Confidence:** LOW

### Greatspine Crown Road (contested)
- **Type:** mountain pass road · **Direction:** Glassmere → Concord Heartlands → south · **Importance:** secondary (contested)
- **Waypoints:** (55,50) Glassmere → (60,52) Greatspine pass → (62,56) Concord Heartlands / Crownmouth → south
- **Terrain crossed:** the Greatspine cordillera; the master divider; through contested fallen-ruin country.
- **Bridges/fords/ferries:** mountain bridges (uncharted, LOW).
- **Toll/gates:** Crownmouth scavenger-tolls; warlord checkpoints.
- **Hazards:** mountain weather; bandits; the Heartlands ruins (D21); contested by far powers.
- **Nearby settlements:** Crownmouth (60,54), the Pilgrim Camps (63,58).
- **Player-map visibility:** yes (mark "contested") · **Confidence:** LOW
- **DM-only overlay:** the Old Concord Heartlands Ruin (D21) is surface-only; it is NOT the keystone (which is vertical beneath Hollowmere). Draw faint/unexplained.

### Salt Road
- **Type:** land caravan track · **Direction:** Pale Coast → Saltmere Reaches · **Importance:** secondary
- **Waypoints:** (14,21) Pale Coast/Wrackmouth → (28,40) Mirewend Sinks edge → (37,54) mid-continent → (50,66) Marrowdowns → (57,68) Brackhold → (60,70) Saltmere
- **Terrain crossed:** salt-marsh → boglands → mid-continent uplands → chalk downs → salt-clan country.
- **Bridges/fords/ferries:** Mirewend Sinks fords (LOW).
- **Toll/gates:** Marrowdowns shire-tolls; salt-clan holds.
- **Hazards:** long exposed track; fallen country; salt-clan raiders.
- **Nearby settlements:** Marrowmoot (50,66), Penmark Hold (47,63), Saltcairn (63,73).
- **Player-map visibility:** yes · **Confidence:** LOW

### Hethe Tollway
- **Type:** forest-river toll road · **Direction:** Karran Marches → Calm Reach coast · **Importance:** secondary
- **Waypoints:** (74,18) Karran-Gate → (75,37) Tollreach → (78,40) Hethemoot reach → (80,50) Calm Reach mouth
- **Terrain crossed:** the Hethewood; the Hethe river-corridor; outlaw-shadowed.
- **Bridges/fords/ferries:** Hethe fords; Tollreach river-toll (75,37).
- **Toll/gates:** Karran-Gate; Tollreach outlaw-tolls; Hethemoot.
- **Hazards:** forest outlaws; toll-lords; the Old Holds (D25, forbidden deep-wood).
- **Nearby settlements:** Hethemoot (71,39), Greenward (68,43), Karran-Gate (76,20).
- **Player-map visibility:** yes · **Confidence:** LOW

### South Road (in-cluster)
- **Type:** road (Concord causeway) · **Direction:** Candlewick → Orchardmere → Caradril · **Importance:** primary (campaign)
- **Waypoints:** (24,26) Candlewick → (25,29) Tilbrook → (25,32) Orchardmere → (33,33) southern downs → (34,35) Caradril
- **Terrain crossed:** fen → hedged Vale farmland → open sheep-downs → city hinterland.
- **Bridges/fords/ferries:** Ammet crossings at Tilbrook; Vale field-fords.
- **Toll/gates:** none major (patrolled by harvest-moot wardens).
- **Hazards:** low; down-barrows best left alone; rare Vale-leakage Remembrance.
- **Nearby settlements:** Tilbrook (25,29), Orchardmere (25,32), Saint Veddow's Rest (23,33, ~-2 SW).
- **Player-map visibility:** yes · **Confidence:** HIGH

### East Road (in-cluster)
- **Type:** road (Concord toll-causeway) · **Direction:** Kettle Bridge → Hartfell → Caradril · **Importance:** primary (campaign)
- **Waypoints:** (27,23) Kettle Bridge → (30,22) Tollstone Cross → (33,22) Hartfell → (34,28) forest-edge → (34,35) Caradril
- **Terrain crossed:** fen → old-growth Tollwood → thinning farmland near the city.
- **Bridges/fords/ferries:** Kettle Bridge (Mirewend crossing, 27,23); the Green Mile drowned stretch (30,22).
- **Toll/gates:** Tollstone Cross bandit-toll (30,22); the Greenward Toll-Station (31,22).
- **Hazards:** bandit-tolls; washed-out causeway; dire wolves; the deep wood off-road (gated).
- **Nearby settlements:** Tollstone Cross (30,22), Hartfell (33,22), Coldhearth (34,20, deeper E).
- **Player-map visibility:** yes · **Confidence:** HIGH

### Pale Road (in-cluster)
- **Type:** road (coast road) · **Direction:** Saltmargin → Cobble Strand → Wrackmouth · **Importance:** primary (campaign)
- **Waypoints:** (20,22) Saltmargin → (13,20) Cobble Strand → (12,23) Wrackmouth
- **Terrain crossed:** salt-marsh → sea-cliffs and shingle coves.
- **Bridges/fords/ferries:** salt-pan causeways.
- **Toll/gates:** none major.
- **Hazards:** cliff-falls; sea-fog; the drowned-tide; wreckers off the wild coast.
- **Nearby settlements:** Cobble Strand (13,20), Wrackmouth (12,23).
- **Player-map visibility:** yes · **Confidence:** HIGH

---

## SEA-LANE ROUTES

### Pale Coast Sea-Route
- **Type:** sea-lane · **Direction:** Wrackmouth → Verdance mouth → up-Verdance → Caradril (continues S) · **Importance:** primary (fastest/safest campaign route)
- **Waypoints:** (12,23) Wrackmouth → (14,28) coast → (15,32) Verdance mouth → (24,33) up-river → (34,35) Stillwater/Caradril
- **Terrain crossed:** open Pale Sea, then the broad Verdance into the Stillwater.
- **Crossings/transfers:** Verdance mouth sea→river ferry/transfer (15,32).
- **Hazards:** storms; tides; wreckers off the wild coast. **Gated:** do not route a low-level boat near the Skerries (~10,22).
- **Nearby settlements:** Wrackmouth (12,23), Cobble Strand (13,20), Caradril (34,35).
- **Player-map visibility:** yes · **Confidence:** HIGH

### South Sea Lanes
- **Type:** sea-lane · **Direction:** Hollow Gulf → off-map overseas · **Importance:** primary (continental gateway overseas)
- **Waypoints:** (66,90) Hollow Gulf → off-map S edge (edge-arrow "to overseas lands")
- **Terrain crossed:** open S sea (the Calm Reach toward open ocean).
- **Hazards:** open-ocean storms; privateers (Hollow Gulf Ports).
- **Nearby settlements:** Calderport (65,89), Saltgate (69,91).
- **Player-map visibility:** yes (dashed arrows) · **Confidence:** LOW

---

## RIVERS (source → mouth)

### Mirewend River
- **Type:** river · **Direction:** Sunder Heights source → NW-system drain · **Importance:** regional (campaign artery)
- **Waypoints:** (25,16) Sunder Heights source → (24,23) Hollowmere basin → (24,28) → (28,40) Mirewend Sinks drain
- **Terrain crossed:** the Reach fens; slow, peat-dark; floods in autumn.
- **Crossings:** Kettle Bridge (27,23, via tributary reach E); Reedford ford (25,24); the Drowned Mile (26,24).
- **Nearby settlements:** Hollowmere (24,23), Kettle Bridge (27,23), Reedford (25,24).
- **Navigability:** shallow/seasonal · **Player-map visibility:** yes · **Confidence:** HIGH
- **DM-only overlay:** the basin (24,23) is the keystone; the Sunken Tollhouse (D03) sits at the Kettle Bridge crossing as a tapped node (DM Layer 7).

### Ammet River
- **Type:** river · **Direction:** Vale headwaters → joins Verdance / coastal drain · **Importance:** regional
- **Waypoints:** (28,28) headwaters (toward Tollwood) → (25,30) Tilbrook → (25,32) Orchardmere → drains to the NW system
- **Terrain crossed:** the Ashgarden Vale's farmland.
- **Crossings:** Tilbrook mill-fords (25,29).
- **Nearby settlements:** Tilbrook (25,29), Orchardmere (25,32).
- **Navigability:** shallow · **Player-map visibility:** yes · **Confidence:** MEDIUM

### Verdance River
- **Type:** river · **Direction:** interior upland source → Pale Sea mouth · **Importance:** primary (NW-quarter great river)
- **Waypoints:** (48,46) interior source → (40,40) → (34,35) Caradril/Stillwater → (24,33) → (15,32) Pale Sea mouth
- **Terrain crossed:** interior → the Stillwater harbor-lake → coastal plain to the sea.
- **Crossings:** Caradril river-bridges (34,35); the Nine Locks up-corridor (43,43).
- **Nearby settlements:** Caradril (34,35), Marrowfen Stair (41,41).
- **Navigability:** fully navigable (Stillwater → mouth) · **Player-map visibility:** yes · **Confidence:** HIGH (cluster) / MEDIUM (upper)

### Glasswater River
- **Type:** river · **Direction:** Greatspine source → Hollow Gulf delta · **Importance:** primary (continent's largest river)
- **Waypoints:** (58,40) Greatspine source → (55,50) Glassmere → (60,66) → (64,88) Hollow Gulf delta
- **Terrain crossed:** central highlands → river-city plain → southern delta.
- **Crossings:** the Three Bridges at Glassmere (55,50).
- **Nearby settlements:** Glassmere (55,50), Sennfort (52,47), Cairnwater (58,53).
- **Navigability:** fully navigable (mid-course down) · **Player-map visibility:** yes · **Confidence:** LOW

### Mardenflow River
- **Type:** river · **Direction:** Marrowdowns source → Sallow Marches delta → Hollow Gulf · **Importance:** regional
- **Waypoints:** (52,64) Marrowdowns source → (55,76) → (58,84) Sallow Marches delta → (66,92) Hollow Gulf
- **Terrain crossed:** chalk downs → deltaic wetland; floods seasonally.
- **Crossings:** delta ferries (LOW).
- **Nearby settlements:** Marrowmoot (50,66), Fenward (57,82), Reedmouth (60,85).
- **Navigability:** seasonal/tidal (delta) · **Player-map visibility:** yes · **Confidence:** LOW

### Hethe River
- **Type:** river · **Direction:** Karran Teeth source → Calm Reach mouth · **Importance:** regional (toll-contested)
- **Waypoints:** (74,22) Karran Teeth source → (76,32) → (78,40) → (80,50) Calm Reach mouth
- **Terrain crossed:** the Hethewood; eastern trade corridor.
- **Crossings:** Tollreach river-toll (75,37).
- **Nearby settlements:** Hethemoot (71,39), Greenward (68,43).
- **Navigability:** navigable mid-course · **Player-map visibility:** yes · **Confidence:** LOW

---

## DM-Only Route Overlays (NEVER on player maps)

The surface roads the player walks secretly follow the **Concord-Deep node-network arteries** (DM Layer 2/7). Render these only on DM maps:

| Surface route | Hidden node crossing | DM note |
|---|---|---|
| East Road @ Kettle Bridge (27,23) | Sunken Tollhouse (D03) node | tapped relay; surface route player-safe |
| Mirewend @ Hollowmere (24,23) | the keystone basin / Under-Shrine (vertical) | NEVER surface; endgame |
| South Road @ Saint Veddow's (23,33) | Saint Veddow's Tomb (D09) node | capped node beneath the shrine-hill |
| Pale Coast Sea-Route @ headland (12,20) | Drowned Lamp (D14) / Skerry Shrine (D15) nodes | coastal nodes; surface = "ruined lighthouse"/"wrecking reef" only |
| Verdance Road @ the Nine Locks (43,43) | Nine Locks Sunken Stair (D34) | flooded relay-vault; surface route player-safe |
| In Caradril @ Sealgate (34,35) | Sunken Wards (D16) node | dormant cousin-node beneath the city |

The endgame is **vertical, straight down beneath Hollowmere** — never a lateral route. Do not draw node-links on any player map.

## Related Files

- [`CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`](CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md) · [`WATER_AND_SHORELINE_AUTHORITY.md`](WATER_AND_SHORELINE_AUTHORITY.md) · [`MAP_FEATURE_REGISTRY.md`](MAP_FEATURE_REGISTRY.md)
- [`TRAVEL_ROUTES_RING1.md`](TRAVEL_ROUTES_RING1.md) (day-counts/events) · [`MAP_DESCRIPTION.md`](MAP_DESCRIPTION.md) · [`WORLD_MAP_LAYERS.md`](WORLD_MAP_LAYERS.md) (DM Layers 2/7)
