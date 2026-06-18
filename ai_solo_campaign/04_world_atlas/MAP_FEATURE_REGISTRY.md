# MAP_FEATURE_REGISTRY.md — Single Registry of Every Map-Visible Feature

---
type: region
secrecy: mixed
status: static
region: Orrun
factions: []
level_range: 1-20
related: [CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md, FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ROADS_RIVERS_AND_ROUTES_AUTHORITY.md, WATER_AND_SHORELINE_AUTHORITY.md, MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md, ../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md]
tags: [type:map, secrecy:mixed, function:cartography, coordinates, map-packet, feature-registry, orrun, full-continent]
---

> **Secrecy classification:** Mixed. §DM-Only lists hidden subsurface features only to mark them `player-safe visibility: no`. Use to generate/audit maps; never hand directly to the player.

## AI Use

A single registry of **every map-visible feature** of Orrun, one row each, with feature ID, type, position, geometry type, visibility flags, label priority, icon, source, and confidence. Use it as the master index when assembling a render layer: filter by `player_safe_visibility = yes` for player maps, add the DM-only rows for DM maps. All coordinates are full-continent **render-grid** (X=0 west, X=100 east, Y=0 north, Y=100 south) from `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`.

> **Exploration-Determinism Pass (2026-06-18):** All §B settlements now have map packets at eagle-test floor depth (`../06_settlements/settlement_map_packets/SETTLEMENT_*_MAP.md` for the 40 settlement packets; `../06_settlements/city_map_packets/*_CITY_MAP.md` for the 4 city packets). Source references below point to the canonical settlement files; the map packets are the AI DM load targets for arrival/exploration scenes.

**Field key:**
- **player_safe_visibility:** `yes` / `no` / `label-only`
- **dm_only_visibility:** `yes` (only on DM maps) / `no`
- **label_priority:** 1 (always) … 5 (zoom-in only)
- **geometry:** point / line / polygon / area / route / hidden-layer

---

## §A. Regions

| ID | Label | Type | Region | Coords (x,y) | Geometry | Player-safe | DM-only | Priority | Icon | Source | Conf. | Notes |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| MF-001 | Sundering Reach | region | Sundering Reach | 24,23 | polygon | yes | no | 1 | region | SUNDERING_REACH.md | HIGH | Starting region; high detail |
| MF-002 | Ashgarden Vale | region | Ashgarden Vale | 25,31 | polygon | yes | no | 1 | region | ASHGARDEN_VALE.md | HIGH | Ring 1 S |
| MF-003 | Tollwood | region | Tollwood | 32,22 | polygon | yes | no | 1 | region | TOLLWOOD.md | HIGH | Ring 1 E |
| MF-004 | Pale Coast | region | Pale Coast | 14,21 | polygon | yes | no | 1 | region | PALE_COAST.md | HIGH | Ring 1 W |
| MF-005 | Caradril (city-state) | region/city | Caradril | 34,35 | point/polygon | yes | no | 1 | city | CARADRIL.md | HIGH | Only true city |
| MF-006 | The Verdance Reaches | region (placeholder) | Verdance Reaches | 42,42 | faint-area | yes | no | 3 | region | REGION_INDEX.md | LOW | Ring 2 |
| MF-007 | The Glassmere League | region (placeholder) | Glassmere League | 55,50 | faint-area | yes | no | 2 | region | REGION_INDEX.md | LOW | Central league |
| MF-008 | The Marrowdowns | region (placeholder) | Marrowdowns | 50,66 | faint-area | yes | no | 3 | region | REGION_INDEX.md | LOW | Chalk downs |
| MF-009 | The Saltmere Reaches | region (placeholder) | Saltmere Reaches | 60,70 | text-over-terrain | yes | no | 3 | region | REGION_INDEX.md | LOW | On land around the Saltmere |
| MF-010 | The Sallowmarch Protectorate | region (placeholder) | Sallowmarch | 58,84 | faint-area | yes | no | 3 | region | REGION_INDEX.md | LOW | Fever delta |
| MF-011 | The Hollow Gulf Ports | region (placeholder) | Hollow Gulf Ports | 66,90 | faint-area | yes | no | 3 | region | REGION_INDEX.md | LOW | Port city-states |
| MF-012 | The Wender Steppe | region (placeholder) | Wender Steppe | 46,16 | faint-area | yes | no | 3 | region | REGION_INDEX.md | LOW | One label only |
| MF-013 | The Karran Marches | region (placeholder) | Karran Marches | 74,18 | faint-area | yes | no | 3 | region | REGION_INDEX.md | LOW | NE frontier |
| MF-014 | The Emberfell Theocracy / Ashfast | region (placeholder) | Emberfell | 80,62 | faint-area | yes | no | 4 | region | REGION_INDEX.md | LOW | Volcanic theocracy |
| MF-015 | Concord Heartlands / Ruin'd Crown | region (fallen ruin) | Concord Heartlands | 62,56 | faint-area | yes | no | 3 | region | REGION_INDEX.md | LOW | Surface ruin, unexplained |
| MF-016 | The Hethewald Free Holds | region (placeholder) | Hethewald | 72,40 | faint-area | yes | no | 3 | region | REGION_INDEX.md | LOW | Forest free-holds |
| MF-017 | The Sunmark | region (placeholder) | Sunmark | 44,80 | faint-area | yes | no | 3 | region | REGION_INDEX.md | LOW | Sacred groves |
| MF-018 | The Highmark Passes | region (late frontier) | Highmark Passes | 30,8 | faint-area | yes | no | 4 | region | WORLD_MAP_AUTHORITY.md | LOW | Optional late frontier |

## §B. Cities and Settlements

| ID | Label | Type | Region | Coords | Geometry | Player-safe | DM-only | Priority | Icon | Source | Conf. |
|---|---|---|---|---|---|---|---|---|---|---|---|
| MF-101 | Caradril | city (major) | Caradril | 34,35 | point | yes | no | 1 | city | CARADRIL.md | HIGH |
| MF-102 | Hollowmere | town | Sundering Reach | 24,23 | point | yes | no | 1 | town | HOLLOWMERE.md | HIGH |
| MF-103 | Kettle Bridge | town | Sundering Reach | 27,23 | point | yes | no | 1 | town | KETTLE_BRIDGE.md | HIGH |
| MF-104 | Saltmargin | town | Sundering Reach | 20,22 | point | yes | no | 1 | town | SALTMARGIN.md | HIGH |
| MF-105 | Candlewick | village | Sundering Reach | 24,26 | point | yes | no | 2 | village | CANDLEWICK.md | HIGH |
| MF-106 | Greywater Holm | village | Sundering Reach | 22,26 | point | yes | no | 2 | village | GREYWATER_HOLM.md | MEDIUM |
| MF-107 | Harrowgast | mining town | Sundering Reach | 25,17 | point | yes | no | 1 | town | HARROWGAST.md | MEDIUM |
| MF-108 | Reedford | hamlet | Sundering Reach | 25,24 | point | yes | no | 3 | hamlet | REEDFORD.md | MEDIUM |
| MF-109 | The Ashwalk Rest | waystation | Sundering Reach | 24,25 | point | yes | no | 3 | waystation | THE_ASHWALK_REST.md | MEDIUM |
| MF-110 | Orchardmere | town | Ashgarden Vale | 25,32 | point | yes | no | 1 | town | ORCHARDMERE.md | HIGH |
| MF-111 | Saint Veddow's Rest | town | Ashgarden Vale | 23,33 | point | yes | no | 2 | town/shrine | SAINT_VEDDOWS_REST.md | MEDIUM |
| MF-112 | Tilbrook | village | Ashgarden Vale | 25,29 | point | yes | no | 3 | village | TILBROOK.md | MEDIUM |
| MF-113 | Hartfell | town | Tollwood | 33,22 | point | yes | no | 1 | town | HARTFELL.md | HIGH |
| MF-114 | Coldhearth | village | Tollwood | 34,20 | point | yes | no | 2 | village | COLDHEARTH.md | MEDIUM |
| MF-115 | Tollstone Cross | hamlet | Tollwood | 30,22 | point | yes | no | 3 | hamlet | TOLLSTONE_CROSS.md | MEDIUM |
| MF-116 | Wrackmouth | town/port | Pale Coast | 12,23 | point | yes | no | 1 | port | WRACKMOUTH.md | HIGH |
| MF-117 | Cobble Strand | village | Pale Coast | 13,20 | point | yes | no | 2 | village | COBBLE_STRAND.md | MEDIUM |
| MF-118 | Marrowfen Stair | town (hub) | Verdance Reaches | 41,41 | point | yes | no | 2 | town | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-119 | Lord's Wend | town | Verdance Reaches | 45,39 | point | yes | no | 4 | town | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-120 | Cresswater | river landing | Verdance Reaches | 39,45 | point | yes | no | 5 | landing | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-121 | Glassmere | city (major) | Glassmere League | 55,50 | point | yes | no | 1 | city | GLASSMERE_CITY_MAP.md | LOW |
| MF-122 | Sennfort | town | Glassmere League | 52,47 | point | yes | no | 4 | town | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-123 | Cairnwater | town | Glassmere League | 58,53 | point | yes | no | 4 | town | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-124 | Marrowmoot | town (hub) | Marrowdowns | 50,66 | point | yes | no | 2 | town | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-125 | Penmark Hold | town/manor | Marrowdowns | 47,63 | point | yes | no | 4 | town | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-126 | Wether | village | Marrowdowns | 53,68 | point | yes | no | 5 | village | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-127 | Fenward | town (hub) | Sallowmarch | 57,82 | point | yes | no | 2 | town | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-128 | Reedmouth | village | Sallowmarch | 60,85 | point | yes | no | 4 | village | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-129 | Calderport | city (major) | Hollow Gulf Ports | 65,89 | point | yes | no | 1 | port-city | CALDERPORT_CITY_MAP.md | LOW |
| MF-130 | Saltgate | town/port | Hollow Gulf Ports | 69,91 | point | yes | no | 3 | port | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-131 | The Winter-Camp at Cold Springs | seasonal camp (hub) | Wender Steppe | 45,16 | point | yes | no | 2 | camp | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-132 | Brask's Hold | fortress-town (hub) | Karran Marches | 73,17 | point | yes | no | 2 | fortress | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-133 | Karran-Gate | mining town | Karran Marches | 76,20 | point | yes | no | 4 | town | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-134 | Ashfast | city (major) | Emberfell | 80,62 | point | yes | no | 1 | temple-city | ASHFAST_CITY_MAP.md | LOW |
| MF-135 | Cinderhold | mining town | Emberfell | 83,65 | point | yes | no | 4 | town | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-136 | Brackhold | salt-clan hold (hub) | Saltmere Reaches | 57,68 | point | yes | no | 2 | hold | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-137 | Saltcairn | clan-town | Saltmere Reaches | 63,73 | point | yes | no | 4 | town | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-138 | Crownmouth | scavenger-town (hub) | Concord Heartlands | 60,54 | point | yes | no | 2 | fortified-town | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-139 | Hethemoot | free-hold (hub) | Hethewald | 71,39 | point | yes | no | 2 | town | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-140 | Greenward | grove-village | Hethewald | 68,43 | point | yes | no | 4 | village | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-141 | The Great Grove at Sunhollow | grove gathering (hub) | Sunmark | 44,80 | point | yes | no | 2 | grove | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |

## §C. Rivers

| ID | Label | Type | Coords (label) | Geometry | Player-safe | DM-only | Priority | Icon | Source | Conf. |
|---|---|---|---|---|---|---|---|---|---|---|
| MF-201 | Verdance | river | 34,35 | line | yes | no | 1 | river | CARTOGRAPHY_AUTHORITY §7 | HIGH |
| MF-202 | Glasswater | river | 58,68 | line | yes | no | 2 | river | CARTOGRAPHY_AUTHORITY §7 | LOW |
| MF-203 | Mirewend | river | 24,22 | line | yes | no | 1 | river | CARTOGRAPHY_AUTHORITY §7 | HIGH |
| MF-204 | Ammet | river | 25,30 | line | yes | no | 2 | river | CARTOGRAPHY_AUTHORITY §7 | MEDIUM |
| MF-205 | Mardenflow | river | 55,76 | line | yes | no | 3 | river | CARTOGRAPHY_AUTHORITY §7 | LOW |
| MF-206 | Hethe | river | 78,40 | line | yes | no | 3 | river | CARTOGRAPHY_AUTHORITY §7 | LOW |

## §D. Lakes / Seas / Bays

| ID | Label | Type | Coords | Geometry | Player-safe | DM-only | Priority | Icon | Source | Conf. |
|---|---|---|---|---|---|---|---|---|---|---|
| MF-301 | The Pale Sea | ocean | 4,30 | area | yes | no | 1 | water | CARTOGRAPHY_AUTHORITY §5 | HIGH |
| MF-302 | The Sunder Ocean | ocean | 50,2 | area | yes | no | 1 | water | CARTOGRAPHY_AUTHORITY §5 | MEDIUM |
| MF-303 | The Calm Reach | warm sea | 82,92 | area | yes | no | 1 | water | CARTOGRAPHY_AUTHORITY §5 | MEDIUM |
| MF-304 | The Hollow Gulf | major bay | 66,92 | area | yes | no | 2 | water | CARTOGRAPHY_AUTHORITY §5 | LOW |
| MF-305 | The Wracking Straits | strait | 2,64 | area | yes | no | 4 | water | CARTOGRAPHY_AUTHORITY §5 | LOW |
| MF-306 | The Saltmere | inland salt sea | 60,70 | polygon | yes | no | 2 | water | CARTOGRAPHY_AUTHORITY §6 | LOW |
| MF-307 | The Stillwater | harbor-lake | 34,35 | polygon | yes | no | 2 | water | CARTOGRAPHY_AUTHORITY §6 | HIGH |
| MF-308 | Hollowmere basin | flooded basin | 24,23 | polygon | yes | no | 2 | water | CARTOGRAPHY_AUTHORITY §6 | HIGH |
| MF-309 | Orchardmere lake | lake | 25,32 | polygon | yes | no | 3 | water | CARTOGRAPHY_AUTHORITY §6 | MEDIUM |

## §E. Mountain Ranges and Terrain Zones

| ID | Label | Type | Coords | Geometry | Player-safe | DM-only | Priority | Icon | Source | Conf. |
|---|---|---|---|---|---|---|---|---|---|---|
| MF-401 | The Highmark Spine | mountain-range | 35,9 | line | yes | no | 1 | mountains | MOUNTAINS_AUTHORITY | MEDIUM |
| MF-402 | The Sunder Heights | highlands | 24,15 | polygon | yes | no | 1 | hills | MOUNTAINS_AUTHORITY | HIGH |
| MF-403 | The Karran Teeth | mountain-range | 74,16 | line | yes | no | 3 | mountains | MOUNTAINS_AUTHORITY | LOW |
| MF-404 | The Greatspine / Sundering Wall | mountain-range | 60,51 | line | yes | no | 1 | mountains | MOUNTAINS_AUTHORITY | LOW |
| MF-405 | The Emberfells | volcanic highland | 80,60 | line | yes | no | 2 | volcano | MOUNTAINS_AUTHORITY | LOW |
| MF-406 | The Ghostmark Range | mountain-range | 58,72 | line | yes | no | 4 | mountains | MOUNTAINS_AUTHORITY | LOW |
| MF-407 | Tollwood | forest | 32,22 | polygon | yes | no | 1 | forest | MOUNTAINS_AUTHORITY | HIGH |
| MF-408 | The Hethewood | forest | 72,38 | polygon | yes | no | 3 | forest | MOUNTAINS_AUTHORITY | LOW |
| MF-409 | The Sunmark Wilds | forest | 44,80 | polygon | yes | no | 4 | forest | MOUNTAINS_AUTHORITY | LOW |
| MF-410 | The Greyfens | fog marsh | 22,25 | polygon | yes | no | 1 | marsh | MOUNTAINS_AUTHORITY | HIGH |
| MF-411 | The Mirewend Sinks | boglands | 28,40 | polygon | yes | no | 3 | marsh | MOUNTAINS_AUTHORITY | LOW |
| MF-412 | The Sallow Marches | wetland | 58,84 | polygon | yes | no | 4 | marsh | MOUNTAINS_AUTHORITY | LOW |
| MF-413 | The Cindern Waste | badland | 84,66 | polygon | yes | no | 4 | badland | MOUNTAINS_AUTHORITY | LOW |
| MF-414 | The Bonepan Flats | badland | 56,74 | polygon | yes | no | 4 | badland | MOUNTAINS_AUTHORITY | LOW |
| MF-415 | The Marrowdowns | chalk downs | 50,66 | polygon | yes | no | 3 | downs | MOUNTAINS_AUTHORITY | LOW |
| MF-416 | The Wender Steppe (terrain) | steppe | 46,16 | area-fill | label-only | no | 5 | steppe | MOUNTAINS_AUTHORITY | LOW |

## §F. Roads / Trade Routes / Sea-Lanes

| ID | Label | Type | Coords (label) | Geometry | Player-safe | DM-only | Priority | Icon | Source | Conf. |
|---|---|---|---|---|---|---|---|---|---|---|
| MF-501 | Verdance Road | trade-route (land) | 44,43 | route | yes | no | 2 | road | ROADS_AUTHORITY | LOW |
| MF-502 | Glasswater Run | trade-route (river/road) | 60,66 | route | yes | no | 2 | road | ROADS_AUTHORITY | LOW |
| MF-503 | Greatspine Crown Road (contested) | trade-route (pass) | 61,54 | route | yes | no | 3 | road | ROADS_AUTHORITY | LOW |
| MF-504 | Salt Road | trade-route (land) | 37,54 | route | yes | no | 3 | road | ROADS_AUTHORITY | LOW |
| MF-505 | Hethe Tollway | trade-route (land) | 77,34 | route | yes | no | 4 | road | ROADS_AUTHORITY | LOW |
| MF-506 | South Road | road (in-cluster) | 30,30 | route | yes | no | 2 | road | ROADS_AUTHORITY | HIGH |
| MF-507 | East Road | road (in-cluster) | 30,22 | route | yes | no | 2 | road | ROADS_AUTHORITY | HIGH |
| MF-508 | Pale Road | road (in-cluster) | 16,21 | route | yes | no | 2 | road | ROADS_AUTHORITY | HIGH |
| MF-509 | Pale Coast Sea-Route | sea-route | W coast | route | yes | no | 2 | sea-lane | ROADS_AUTHORITY | HIGH |
| MF-510 | South Sea Lanes | sea-route | S sea | route | yes | no | 4 | sea-lane | ROADS_AUTHORITY | LOW |

## §G. Bridges / Ferries / Fords / Locks / Passes / Toll Points / Ports

| ID | Label | Type | Coords | Geometry | Player-safe | DM-only | Priority | Icon | Source | Conf. |
|---|---|---|---|---|---|---|---|---|---|---|
| MF-601 | Kettle Bridge crossing | bridge/toll | 27,23 | point | yes | no | 2 | bridge | KETTLE_BRIDGE.md | HIGH |
| MF-602 | Reedford ford | ford | 25,24 | point | yes | no | 3 | ford | REEDFORD.md | MEDIUM |
| MF-603 | Sashe's Crossing | ford | 22,25 | point | yes | no | 4 | ford | GREYFENS_SITES.md | MEDIUM |
| MF-604 | The Drowned Mile | flooded causeway | 26,24 | point | yes | no | 4 | ford | MIREWEND_AND_ROADS_SITES.md | MEDIUM |
| MF-605 | The Green Mile | washed-out causeway | 30,22 | point | yes | no | 4 | ford | TOLLWOOD_SITES.md | MEDIUM |
| MF-606 | Tollstone Cross toll | road toll | 30,22 | point | yes | no | 3 | toll | TOLLSTONE_CROSS.md | MEDIUM |
| MF-607 | The Greenward Toll-Station | road-node toll | 31,22 | point | yes | no | 4 | toll | THE_GREENWARD_TOLL_STATION.md | LOW |
| MF-608 | Verdance mouth ferry | ferry (sea→river) | 15,32 | point | yes | no | 3 | ferry | TRAVEL_ROUTES_RING1.md | MEDIUM |
| MF-609 | Caradril river-bridges (×2) | city bridges | 34,35 | point | yes | no | 3 | bridge | CARADRIL_CITY_MAP.md | HIGH |
| MF-610 | The Nine Locks | lock-staircase | 43,43 | point | yes | no | 4 | lock | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-611 | The Three Bridges (Glassmere) | city bridges | 55,50 | point | yes | no | 4 | bridge | GLASSMERE_CITY_MAP.md | LOW |
| MF-612 | Tollreach | river toll-camp | 75,37 | point | yes | no | 4 | toll | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |
| MF-613 | Highmark passes | mountain passes | 35,8 | point | yes | no | 4 | pass | WORLD_MAP_AUTHORITY.md | LOW |
| MF-614 | Greatspine passes | mountain passes | 60,52 | point | yes | no | 4 | pass | ROADS_AUTHORITY | LOW |
| MF-615 | Wrackmouth port | port | 12,23 | point | yes | no | 2 | port | WRACKMOUTH.md | HIGH |
| MF-616 | Stillwater quays | port | 34,35 | point | yes | no | 3 | port | CARADRIL.md | HIGH |
| MF-617 | The Mardenmouth wharves | harbor node | 63,88 | point | yes | no | 4 | port | FULL_CONTINENT_SETTLEMENT_ANCHORS.md | LOW |

## §H. Adventure Sites (player-visible surface markers only)

Full coordinate detail in `ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`. Only sites with a **visible surface marker** appear on player maps (as labeled hazard landmarks, never nodes). Hidden/underground/urban-internal sites are DM-map only.

| ID | Label (site_id) | Type | Region | Coords | Player-safe | DM-only | Priority | Icon | Conf. |
|---|---|---|---|---|---|---|---|---|---|
| MF-701 | The Old Mast (D12) | gated landmark | Tollwood | 36,20 | label-only ("deep wood — do not enter") | yes | 4 | hazard | MEDIUM |
| MF-702 | The Skerries / Skerry Shrine (D15) | offshore reef | Pale Coast | 10,22 | label-only ("wrecking reef") | yes | 4 | hazard | MEDIUM |
| MF-703 | The Drowned Lamp (D14) | ruined lighthouse | Pale Coast | 12,20 | label-only ("ruined lighthouse") | yes | 4 | ruin | MEDIUM |
| MF-704 | Saint Veddow's Tomb (D09) | pilgrimage shrine-hill | Ashgarden Vale | 23,33 | yes (shrine) | yes | 3 | shrine | MEDIUM |
| MF-705 | The Barrow of Nine Doors (D06) | pre-Concord barrow | Sundering Reach | 21,26 | label-only ("old barrow") | yes | 4 | ruin | MEDIUM |
| MF-706 | The Concord Heartlands Ruin (D21) | far surface ruin | Concord Heartlands | 62,56 | yes (broken ruin, unexplained) | yes | 3 | ruin | LOW |
| MF-707 | The Sky-Stones (D32) | standing-stone circle | Wender Steppe | 42,14 | yes (standing stones) | yes | 4 | shrine | LOW |
| MF-708 | The Drowned Steps (D30) | submerged causeway | Sallowmarch | 54,90 | label-only ("drowned steps") | yes | 4 | ruin | LOW |

> Other D-sites (D01–D05, D07–D08, D10–D11, D13, D16–D20, D22, D24–D29, D31, D33–D36) are hidden / underground / urban-internal and appear only on DM maps. See `ADVENTURE_SITE_CARTOGRAPHY_INDEX.md` for every site's full visibility flag.

## §I. Major Landmarks / Shrines / Towers / Gates / Markets (player-visible)

| ID | Label | Type | Region | Coords | Player-safe | DM-only | Priority | Icon | Conf. |
|---|---|---|---|---|---|---|---|---|---|
| MF-801 | The Tide-Bell (Wrackmouth Mourners' shrine) | shrine | Pale Coast | 12,23 | yes | no | 4 | shrine | MEDIUM |
| MF-802 | The Old Circle (Orchardmere grave-garden) | landmark | Ashgarden Vale | 25,32 | yes | no | 4 | shrine | MEDIUM |
| MF-803 | The Star-Stones (road relay-markers) | landmark | Sundering Reach | varies | yes (standing stones) | yes (relay truth DM-only) | 5 | stone | MEDIUM |
| MF-804 | The Sealgate (Caradril) | gate (sealed stair) | Caradril | 34,35 | yes (sealed door) | yes (Sunken Wards) | 4 | gate | HIGH |
| MF-805 | Threshold Cathedral (Highmourn) | temple | Caradril | 34,35 | yes | no | 3 | temple | HIGH |
| MF-806 | The Reliquary (Glassmere) | scholar chapter-house | Glassmere League | 56,48 | yes | no | 4 | building | LOW |

## §DM-Only. Hidden Subsurface / Endgame Features (NEVER on player maps)

| ID | Label | Type | Region | Coords | Geometry | Player-safe | DM-only | Source | Conf. |
|---|---|---|---|---|---|---|---|---|---|
| MF-901 | The Concord Deep | subsurface node-network | Orrun (subsurface) | 24,24 | hidden-layer | **no** | yes | WORLD_MAP_LAYERS.md L7 | LOW |
| MF-902 | The Under-Shrine / Drowned Keystone | endgame (vertical, beneath Hollowmere) | Sundering Reach (subsurface) | 24,23 (deepest Z) | hidden-layer | **no** | yes | WORLD_MAP_AUTHORITY.md §8 | HIGH (position) |
| MF-903 | Hollow Court seat | apex faction seat | beneath the basin | 24,23 | hidden-layer | **no** | yes | HOLLOW_COURT.md | LOW |
| MF-904 | Node-network links | DM-only edges | NW cluster | — | hidden-layer | **no** | yes | WORLD_MAP_LAYERS.md L2 | LOW |
| MF-905 | The Under-Shrine Approach (D23) | endgame dungeon | Sundering Reach (subsurface) | 24,23 | hidden-layer | **no** | yes | THE_UNDER_SHRINE_APPROACH.md | DM-only |

---

## Registry Counts

- Regions: 18 · Cities/settlements: 41 · Rivers: 6 · Lakes/seas/bays: 9 · Mountains/terrain: 16 · Routes/sea-lanes: 10 · Bridges/ferries/fords/passes/ports: 17 · Adventure-site surface markers: 8 · Landmarks/shrines/gates: 6 · DM-only hidden: 5
- **Total registered features: ~136**
- **DM-only (player_safe = no): 5** (all in §DM-Only)

## Related Files

- [`CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`](CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md) (master geometry) · [`PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md`](PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md) (label authority)
- [`ROADS_RIVERS_AND_ROUTES_AUTHORITY.md`](ROADS_RIVERS_AND_ROUTES_AUTHORITY.md) · [`WATER_AND_SHORELINE_AUTHORITY.md`](WATER_AND_SHORELINE_AUTHORITY.md) · [`MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md`](MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md)
- [`FULL_CONTINENT_SETTLEMENT_ANCHORS.md`](FULL_CONTINENT_SETTLEMENT_ANCHORS.md) · [`../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
