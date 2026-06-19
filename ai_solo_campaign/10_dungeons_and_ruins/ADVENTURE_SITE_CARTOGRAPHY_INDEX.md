# ADVENTURE_SITE_CARTOGRAPHY_INDEX.md — D01–D36 Coordinate Anchors

---
type: index
secrecy: mixed
status: static
region: Orrun
level_range: 1-20
related: [DUNGEON_INDEX.md, ../04_world_atlas/CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, ../04_world_atlas/MAP_FEATURE_REGISTRY.md, ../04_world_atlas/WORLD_MAP_COORDINATES.md, ../04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../04_world_atlas/WORLD_MAP_LAYERS.md]
tags: [index, type:dungeon, secrecy:mixed, function:cartography, coordinates, orrun]
---

> **Secrecy classification:** Mixed. **D23 (the Under-Shrine Approach) is DM-ONLY** — never place, label, name, or hint at it on any map shared with the player. Use this file to place adventure sites on DM maps and to place only the player-visible surface markers on player maps.

## AI Use

Coordinate anchors for every authored adventure site (D01–D36). For each site: full-continent **render-grid** coordinates (X=0 west, X=100 east, Y=0 north, Y=100 south), the region-packet local-grid position, nearest settlement + direction + travel time, terrain context, the **surface marker** (what the player sees above ground), and **player-map vs DM-map visibility**. Use with `DUNGEON_INDEX.md` (the master site table: type, level, danger, mystery/faction links).

**Visibility key:**
- **player-map:** `visible` (marked on player map) / `label-only` (named as a hazard landmark, not a node) / `hidden` (not shown until discovered) / `urban` (part of a city map only)
- **DM-map:** all sites are always visible on the DM map.

**Coordinate derivation:** Reach/Ring-1 site positions are taken from `WORLD_MAP_COORDINATES.md` (campaign grid) and transformed to the full-continent render grid via `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §15`; where a site only had a "near settlement X" description, the position is **DERIVED** from the settlement coordinate + a directional offset (noted). Far-continent sites sit within their region's settlement-anchor footprint.

> **Survey Certainty column (legacy Conf.):** HIGH/MEDIUM/LOW/DERIVED values in the tables below indicate geographic-placement certainty only — how precisely the site's position is known. This is NOT render-readiness. For render-confidence of any feature, use `MAP_FEATURE_REGISTRY.md` (four-status taxonomy: AUTHORITATIVE / DERIVED_CANON / NOT_MAP_AUTHORITATIVE / CARTOGRAPHY_BLOCKER). Legacy HIGH/MEDIUM/LOW values are geographic-certainty context; they do not affect map rendering.

---

## Sundering Reach (D01–D06, D18–D20, D23)

| Site | Name | Full-grid (x,y) | Region-packet local | Nearest settlement | Dir / time | Terrain | Surface marker | Player-map | DM-map | Icon | Survey Certainty |
|---|---|---|---|---|---|---|---|---|---|---|---|
| D01 | The Peat Chapel | 24,25 | REACH (48,52) | Hollowmere | S, ~0.5 day | fen wayside | half-sunk chapel stones | visible | yes | ruin | DERIVED |
| D02 | The Whispering Cairn | 25,24 | REACH (54,48) | Reedford/Hollowmere | E on road, ~1 day | roadside | standing archive-cairn | visible | yes | stone | DERIVED |
| D03 | The Sunken Tollhouse | 27,23 | REACH (60,44) | Kettle Bridge | at the broken arch | river crossing | drowned arch under the bridge | label-only | yes | ruin | MEDIUM |
| D04 | The Ledger Vault | 24,23 | REACH (50,45) | Hollowmere | in-town (Counting-House) | urban (town) | counting-house (heist interior) | urban | yes | building | HIGH |
| D05 | The Deep Adit | 25,17 | REACH (52,26) | Harrowgast | at the mine | mine-adit | mine entrance in the Heights | label-only | yes | mine | MEDIUM |
| D06 | The Barrow of Nine Doors | 21,26 | REACH (42,52) | Greywater Holm | SW in Greyfens, ~1 day | fen barrow | grass barrow-mound, nine doors | label-only | yes | ruin | DERIVED |
| D18 | The Concord Relay-Vault | 26,15 | REACH (55,22) | Harrowgast | N in Sunder Heights, ~1 day | highland | buried signal-cairn | hidden | yes | ruin | DERIVED |
| D19 | The Greyfens Deep | 21,26 | REACH (42,55) | Greywater Holm | into the deep fen | fen (multi-zone) | open fen (the terrain is the dungeon) | label-only | yes | marsh | MEDIUM |
| D20 | The Basin Keystone Approach | 24,23 | REACH (50,45) | Hollowmere | basin shore | basin shore/upper works | basin shore ruin (upper level only) | label-only ("deep basin — lethal") | yes | ruin | HIGH |
| **D23** | **The Under-Shrine Approach** | **24,23 (deepest Z)** | REACH (50,45, vertical) | Hollowmere | **straight down beneath the basin** | subsurface endgame | **NONE — DM-ONLY** | **hidden (NEVER)** | yes | (none) | DM-only |

> **D23 is DM-ONLY.** It is vertical — directly below Hollowmere — never a lateral site. Never render, label, mark, or hint at it on any player map. Reach it only via the gated descent below D20.

## Ashgarden Vale (D07–D09)

| Site | Name | Full-grid | Local | Nearest settlement | Dir / time | Terrain | Surface marker | Player-map | DM-map | Icon | Survey Certainty |
|---|---|---|---|---|---|---|---|---|---|---|---|
| D07 | The Buried Cloister | 25,32 | VALE (50,40) | Orchardmere | orchard country, ~1 day | farmland ruin | sunken cloister walls in an orchard | visible | yes | ruin | DERIVED |
| D08 | The Pellow Grange | 27,31 | VALE (62,38) | Orchardmere | E, Ledger quarry, ~1 day | grange/quarry | grange manor + relic-quarry | visible | yes | building | DERIVED |
| D09 | Saint Veddow's Tomb | 23,33 | VALE (40,52) | Saint Veddow's Rest | beneath the pilgrimage hill | shrine-hill | pilgrimage shrine on the hill | visible (shrine) | yes | shrine | MEDIUM |

## Tollwood (D10–D12)

| Site | Name | Full-grid | Local | Nearest settlement | Dir / time | Terrain | Surface marker | Player-map | DM-map | Icon | Survey Certainty |
|---|---|---|---|---|---|---|---|---|---|---|---|
| D10 | The Greenward Toll-Station | 31,22 | TOLLWOOD (44,52) | Tollstone Cross | on the East Road | road-node | overgrown toll-station ruin | visible | yes | ruin | DERIVED |
| D11 | The Hanging Oaks | 33,21 | TOLLWOOD (56,44) | Hartfell | mid-deep wood, ~1 day | grove | old grove of hanged oaks | label-only | yes | grove | DERIVED |
| D12 | The Old Mast | 36,20 | TOLLWOOD (82,32) | Coldhearth | deep wood heart (gated) | deep forest | (gated) no clear marker — "deep wood, do not enter" | label-only ("deep wood — do not enter") | yes | hazard | MEDIUM |

## Pale Coast (D13–D15)

| Site | Name | Full-grid | Local | Nearest settlement | Dir / time | Terrain | Surface marker | Player-map | DM-map | Icon | Survey Certainty |
|---|---|---|---|---|---|---|---|---|---|---|---|
| D13 | The Wreckers' Caves | 11,21 | COAST (40,44) | Wrackmouth | wild coast, ~1 day | sea-caves | sea-cave mouths in the cliffs | label-only | yes | cave | DERIVED |
| D14 | The Drowned Lamp | 12,20 | COAST (44,40) | Cobble Strand | headland N of Wrackmouth | coastal headland | ruined lighthouse on the headland | label-only ("ruined lighthouse") | yes | tower | MEDIUM |
| D15 | The Skerry Shrine | 10,22 | COAST (32,46) | Wrackmouth | offshore (gated) | offshore reef | sea-stacks / wrecking reef offshore | label-only ("wrecking reef") | yes | hazard | MEDIUM |

## Caradril (D16–D17)

| Site | Name | Full-grid | Local | Nearest settlement | Dir / time | Terrain | Surface marker | Player-map | DM-map | Icon | Survey Certainty |
|---|---|---|---|---|---|---|---|---|---|---|---|
| D16 | The Sunken Wards Deep | 34,35 | CARADRIL city (S/below) | Caradril | beneath the city (Sealgate) | urban undercity | the Sealgate (sealed stair) | urban (city map; gate visible) | yes | gate | HIGH |
| D17 | The Caradril Ashmarket Undercroft | 34,35 | CARADRIL city (Ashmarket) | Caradril | beneath the Ashmarket | urban warren | Ashmarket cellars (interior) | urban | yes | building | HIGH |

## Far Continent — Stage 12 / 12.5 (D21–D22, D24–D36)

| Site | Name | Full-grid | Region | Nearest anchor | Dir / time | Terrain | Surface marker | Player-map | DM-map | Icon | Survey Certainty |
|---|---|---|---|---|---|---|---|---|---|---|---|
| D21 | The Old Concord Heartlands Ruin | 62,56 | Concord Heartlands | Crownmouth (60,54) | E, ~1 day | fallen ruin-country | broken towers (unexplained) | visible (broken ruin) | yes | ruin | LOW |
| D22 | The Emberfell Caldera Descent | 81,61 | Emberfell | Ashfast (80,62) | into the caldera | volcanic | active caldera rim | visible (volcano) | yes | volcano | LOW |
| D24 | The Saltmere Deep Towns | 60,71 | Saltmere Reaches | the Drowned Towns (60,71) | on the receding shore | drowned ruin | submerged town roofs at the waterline | label-only | yes | ruin | LOW |
| D25 | The Hethewald Old Holds | 74,44 | Hethewald | the Old Holds (74,44) | deep wood (forbidden) | deep forest | forbidden deep-wood ruin | label-only | yes | hazard | LOW |
| D26 | The Marrowdowns Barrow Complex | 52,64 | Marrowdowns | the Barrow-Fields (52,64) | barrow-downs | chalk downs | barrow-mounds on the downs | label-only | yes | ruin | LOW |
| D27 | The Karran Old Iron Forts | 78,15 | Karran Marches | the Old Iron forts (78,15) | scattered ridge forts | mountain | ruined iron-grey forts | visible (ruin) | yes | ruin | LOW |
| D28 | The Glassmere Reliquary Vaults | 56,48 | Glassmere League | the Reliquary (56,48) | within Glassmere | urban (chapter-house) | the Reliquary building | urban/visible | yes | building | LOW |
| D29 | The Three Bridges Counting-Deep | 55,50 | Glassmere League | Glassmere (55,50) | banking quarter | urban (bank vault) | the Three Bridges quarter | urban | yes | building | LOW |
| D30 | The Sallowmarch Drowned Steps | 54,90 | Sallowmarch | the Rice Sallows (55,86) | offshore tidal | submerged causeway | drowned causeway steps at low tide | label-only ("drowned steps") | yes | ruin | LOW |
| D31 | The Hollow Gulf Wreck-Reef | 68,90 | Hollow Gulf Ports | Calderport (65,89) | offshore reef | sea-reef | wreck-reef / drowned harbour-quarter | label-only ("wreck-reef") | yes | hazard | LOW |
| D32 | The Wender Sky-Stones | 42,14 | Wender Steppe | the Sky-Stones (42,14) | steppe shrine-circle | steppe | standing-stone circle | visible (standing stones) | yes | shrine | LOW |
| D33 | The Sunhollow Great Grove | 44,80 | Sunmark | the Great Grove (44,80) | sacred grove | warm forest | great living grove | visible (grove) | yes | grove | LOW |
| D34 | The Nine Locks Sunken Stair | 43,43 | Verdance Reaches | the Nine Locks (43,43) | beneath the locks | river-corridor | the Nine Locks lock-staircase | label-only (locks visible) | yes | lock | LOW |
| D35 | The Highmark Frozen Works | 38,8 | Highmark Passes | (far-N passes) | ice-locked station | mountain (ice) | ice-locked Concord works | hidden | yes | ruin | LOW |
| D36 | The Cindern Waste Buried Works | 84,66 | Emberfell (Cindern) | Cinderhold (83,65) | ash-drowned | ash badland | ash-buried works (faint mounds) | hidden | yes | ruin | LOW |

---

## Visibility Summary

- **Player-map visible (full marker):** D01, D02, D04(urban), D07, D08, D09, D10, D16(urban gate), D17(urban), D21, D22, D27, D28, D32, D33.
- **Player-map label-only (hazard landmark, never a node):** D03, D05, D06, D11, D12, D13, D14, D15, D19, D20, D24, D25, D26, D30, D31, D34.
- **Player-map hidden (not shown until discovered):** D18, D35, D36.
- **DM-ONLY (NEVER on player maps):** **D23 (Under-Shrine Approach).**
- **All 36 sites are coordinate-anchored** to the full-continent render grid and to a region-packet local grid (Reach/Ring-1 HIGH–DERIVED; far LOW within region footprints).

## Related Files

- [`DUNGEON_INDEX.md`](DUNGEON_INDEX.md) (master site table: type/level/danger/mystery/faction) · [`../04_world_atlas/CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`](../04_world_atlas/CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md) · [`../04_world_atlas/MAP_FEATURE_REGISTRY.md`](../04_world_atlas/MAP_FEATURE_REGISTRY.md)
- [`../04_world_atlas/WORLD_MAP_COORDINATES.md`](../04_world_atlas/WORLD_MAP_COORDINATES.md) (campaign-grid landmark positions) · [`../04_world_atlas/WORLD_MAP_LAYERS.md`](../04_world_atlas/WORLD_MAP_LAYERS.md) (DM Layers 2/7 — node-network; do not surface)
