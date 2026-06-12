# FULL_WORLD_MAP_COORDINATES.md — Full-Continent Normalized Grid

---
type: region
secrecy: mixed
status: static
region: Orrun
factions: []
level_range: 1-20
related: [FULL_WORLD_MAP_AUTHORITY.md, FULL_WORLD_MAP_LAYERS.md, FULL_WORLD_MAP_PROMPTS.md, WORLD_MAP_COORDINATES.md, WORLD_MAP_AUTHORITY.md]
tags: [type:map, secrecy:mixed, function:cartography, coordinates, grid, orrun, full-continent, vael]
---

## AI Use

A normalized **0–100 grid for the entire continent of Orrun** (plus Vael's placeholder landmasses), for placing far features and for whole-world spatial reasoning. **North = top (Y=0), south = bottom (Y=100); west = left (X=0), east = right (X=100).** This grid spans **all of Orrun**, unlike `WORLD_MAP_COORDINATES.md`, which is a ~3× zoom on the NW corner only.

**Confidence:** `high` = directly established by existing canon (campaign-cluster rows, re-anchored); `medium` = consistent inference / logical continental placement; `low` = placeholder, expansion will pin down. **DM-only rows are flagged; never render them on a player-facing map.**

---

## Grid Rescaling Note (campaign cluster → full continent)

The existing campaign-area grid (`WORLD_MAP_COORDINATES.md`, 0–100, NW-quarter only) is **embedded into this full-continent grid** in the **NW corner** by this linear transform:

```
full_X = 8 + (campaign_X * 0.32)      → campaign 0–100 maps to full 8–40 on X
full_Y = 8 + (campaign_Y * 0.34)      → campaign 0–100 maps to full 8–42 on Y
```

Spot-checks (campaign → full): Hollowmere (50,45) → **(24.0, 23.3)**; Caradril (82,80) → **(34.2, 35.2)**; Wrackmouth (14,44) → **(12.5, 23.0)**; Sunder Heights ruins (50,20) → **(24.0, 14.8)**; Highmark Spine (55,6) → **(25.6, 10.0)**. Campaign-cluster rows below carry their **full-grid** coordinates (rounded); their precise intra-cluster positions remain authoritative in `WORLD_MAP_COORDINATES.md`. The cluster occupies full-grid **X 8–40, Y 8–42** — the upper-left quarter. **No campaign travel time or description is changed by this; only the proportional frame is recorded.**

---

## Other Landmasses of Vael (placeholder)

| Feature | Type | X | Y | Confidence | Notes |
|---|---|---|---|---|---|
| Surren (continent) | landmass (off-map) | 12 | 118 | low | **Placeholder.** Across the ocean, far S/SW (off-grid south). Non-campaign. |
| The Iron Skards (isles) | island chain (off-map) | 60 | -10 | low | **Placeholder.** Cold volcanic isles far N, off the top edge. Non-campaign. |
| The Sundered Isles / Far Wrack | island chain | -8 | 70 | low | **Placeholder.** Far-W mid-ocean isles in the Pale Sea. Non-campaign. |

---

## Major Regions (continental centroids / labels)

| Feature | Type | X | Y | Confidence | Notes |
|---|---|---|---|---|---|
| Sundering Reach | region (campaign) | 24 | 23 | high | NW cluster center; starting region. |
| Ashgarden Vale | region (campaign) | 25 | 31 | high | NW cluster, S of Reach. |
| Tollwood | region (campaign) | 32 | 22 | high | NW cluster, E of Reach. |
| Pale Coast | region (campaign) | 14 | 21 | high | NW cluster, W of Reach. |
| Caradril (city-state) | region/city (campaign) | 34 | 35 | high | NW cluster SE corner; frontier-edge city. |
| The Verdance Reaches | region (Ring 2 placeholder) | 42 | 42 | low | SE of cluster, up the Verdance. |
| The Glassmere League | region (placeholder) | 55 | 50 | low | Central; river-city league on the Glasswater. |
| The Marrowdowns | region (placeholder) | 50 | 66 | low | S-central chalk downs. |
| The Sallowmarch Protectorate | region (placeholder) | 58 | 84 | low | S coast, the Mardenflow delta. |
| The Hollow Gulf Ports | region (placeholder) | 66 | 90 | low | S coast, around the Hollow Gulf. |
| The Wender Steppe | region (placeholder) | 46 | 16 | low | N-central grass-sea, beyond the Spine. |
| The Karran Marches | region (placeholder) | 74 | 18 | low | NE outlaw/mining frontier. |
| The Emberfell Theocracy / Ashfast | region (placeholder) | 80 | 62 | low | SE-central volcanic highlands. |
| The Saltmere Reaches | region (placeholder) | 60 | 70 | low | S-central inland salt sea. |
| The Concord Heartlands / Ruin'd Crown | region (fallen, placeholder) | 62 | 56 | low | Central-SE, astride the Greatspine; forbidden ruin. |
| The Hethewald Free Holds | region (placeholder) | 72 | 40 | low | E-central great forest. |
| The Sunmark | region (placeholder) | 44 | 80 | low | S warm forest & sacred groves. |
| The Highmark Passes | region (late frontier, placeholder) | 30 | 8 | low | Far N/NE barrier passes (cluster-edge & beyond). |
| The Concord Heartlands deep ruins | forbidden zone (placeholder) | 64 | 54 | low | Surface-Concord ruin core (NOT the underground keystone). |

## Bodies of Water

| Feature | Type | X | Y | Confidence | Notes |
|---|---|---|---|---|---|
| The Pale Sea | ocean | 4 | 30 | high | W/NW ocean, whole west coast. |
| The Sunder Ocean | ocean | 50 | 2 | medium | N ocean beyond the Highmark Spine. |
| The Calm Reach | warm sea | 82 | 92 | medium | SE/S warm sea; southern trade heart. |
| The Saltmere | inland salt sea | 60 | 70 | low | S-central brackish inland sea. |
| The Hollow Gulf | major bay | 66 | 92 | low | S-coast bay; Mardenflow delta mouth. |
| The Wracking Straits | strait | 2 | 64 | low | Far-W narrows toward open ocean. |
| The Stillwater | harbor-lake | 34 | 35 | high | Caradril's port-lake (campaign). |
| Hollowmere basin | flooded basin | 24 | 23 | high | NW cluster sink; the keystone (interior DM-only). |

## Rivers (course endpoints — draw as lines between)

| Feature | Type | X | Y | Confidence | Notes |
|---|---|---|---|---|---|
| Mirewend River (NW cluster) | river course pt | 24 | 23 | high | Reach river; tributary of the NW system. |
| Ammet River (NW cluster) | river course pt | 25 | 30 | medium | Vale river. |
| Verdance (Caradril/Stillwater) | river course pt | 34 | 35 | high | NW-quarter great river at Caradril. |
| Verdance (upland source, inland) | river course pt | 48 | 46 | medium | Rises in the interior toward the Glassmere country. |
| Verdance (sea-mouth) | river course pt | 15 | 32 | medium | Reaches the Pale Sea S of the Coast (campaign). |
| Glasswater (source, Greatspine) | river course pt | 58 | 40 | low | Rises in the central cordillera. |
| Glasswater (Glassmere League) | river course pt | 55 | 50 | low | The great river's middle trade-cities. |
| Glasswater (to the Hollow Gulf) | river course pt | 64 | 88 | low | Runs S to the southern sea. |
| Mardenflow (source, Marrowdowns) | river course pt | 52 | 64 | low | Rises in the southern downs. |
| Mardenflow (Sallow Marches delta) | river course pt | 58 | 86 | low | Splays into the southern delta. |
| Hethe (source, Karran Teeth) | river course pt | 74 | 22 | low | Rises in the NE range. |
| Hethe (to the Calm Reach) | river course pt | 80 | 50 | low | Runs E/SE through the Hethewood to the sea. |

## Mountain Ranges (range endpoints / spine points)

| Feature | Type | X | Y | Confidence | Notes |
|---|---|---|---|---|---|
| The Highmark Spine (W end) | mountain range | 26 | 10 | medium | Far-N wall over the campaign cluster. |
| The Highmark Spine (E end) | mountain range | 44 | 8 | low | Runs E along the N edge. |
| The Karran Teeth | mountain range | 74 | 16 | low | NE range; isolates the northeast. |
| The Greatspine / Sundering Wall (N end) | mountain range | 50 | 38 | low | Continental cordillera, NW–SE axis. |
| The Greatspine / Sundering Wall (S end) | mountain range | 70 | 64 | low | Splits the continent; passes control trade. |
| The Emberfells (volcanic) | volcanic highland | 80 | 60 | low | SE-central; active vents, obsidian. |
| The Ghostmark Range | low mountains | 58 | 72 | low | Rings the Saltmere; eroded, haunted. |

## Forests

| Feature | Type | X | Y | Confidence | Notes |
|---|---|---|---|---|---|
| The Tollwood | old-growth forest (campaign) | 32 | 22 | high | NW cluster, E. |
| The Hethewood | great eastern forest | 72 | 38 | low | E-central; Tollwood is its NW finger. |
| The Sunmark Wilds | warm forest | 44 | 80 | low | S sacred-grove forest. |
| The Ashen Reach Woods | volcanic woodland | 78 | 56 | low | Around the Emberfells. |

## Deserts / Badlands / Wetlands / Steppe

| Feature | Type | X | Y | Confidence | Notes |
|---|---|---|---|---|---|
| The Cindern Waste | ash badland | 84 | 66 | low | Emberfells' rain-shadow; buried works rumored. |
| The Bonepan Flats | salt badland | 56 | 74 | low | Around the Saltmere. |
| The Greyfens | fog marsh (campaign) | 22 | 25 | high | NW cluster wetland. |
| The Sallow Marches | deltaic wetland | 58 | 84 | low | S-coast delta; natural border. |
| The Mirewend Sinks | boglands | 28 | 40 | low | S of the cluster, before the land rises. |
| The Sunder Heights | highlands (campaign) | 24 | 15 | high | NW cluster N highlands. |
| The Wender Steppe | cold steppe | 46 | 16 | low | N-central grass-sea. |
| The Marrowdowns | chalk downs | 50 | 66 | low | S-central uplands. |

## Coastal Features / Islands / Unusual Terrain

| Feature | Type | X | Y | Confidence | Notes |
|---|---|---|---|---|---|
| The Skerries | offshore reefs (campaign) | 10 | 22 | medium | Off the Pale Coast; gated. |
| The Wracking Isles | island chain | 3 | 60 | low | Far-W storm isles in the Straits. |
| The Glass Coast | volcanic-glass coast | 86 | 74 | low | SE, Emberfells-to-Calm-Reach. |
| The Drowned Steps | submerged ruin-causeway | 54 | 90 | low | Off the S coast; pre-Concord; rumored. |

## Campaign Cluster Settlements (re-anchored into the full grid)

| Feature | Type | X | Y | Confidence | Notes |
|---|---|---|---|---|---|
| Hollowmere | town (start/hub) | 24 | 23 | high | NW cluster center; keystone town. |
| Kettle Bridge | town | 27 | 23 | high | E gateway (→ Tollwood). |
| Saltmargin | town | 20 | 22 | high | W gateway (→ Pale Coast). |
| Candlewick | village | 24 | 26 | high | S gateway (→ Vale). |
| Harrowgast | mining town | 25 | 17 | medium | N, Sunder Heights. |
| Orchardmere | town (Vale hub) | 25 | 32 | high | Vale hub. |
| Saint Veddow's Rest | town (pilgrimage) | 23 | 33 | medium | Vale hill-shrine. |
| Hartfell | town (Tollwood hub) | 33 | 22 | high | Tollwood hub. |
| Wrackmouth | town (Coast hub/port) | 12 | 23 | high | Coast port; sea-route start. |
| Cobble Strand | village | 13 | 20 | medium | Coast cove. |
| Caradril (city) | major city | 34 | 35 | high | NW cluster SE corner; the city. |

> Other campaign settlements (Reedford, Greywater Holm, the Ashwalk Rest, Tilbrook, Coldhearth, Tollstone Cross) cluster tightly around the above; for fine intra-cluster placement use `WORLD_MAP_COORDINATES.md`. They are not separately re-gridded at continental scale.

## Long-Distance Travel-Route Anchor Points

| Route | From (X,Y) | To (X,Y) | Confidence | Notes |
|---|---|---|---|---|
| The Verdance Road | Caradril (34,35) | Glassmere League (55,50) | low | Up-Verdance into settled Orrun (Ring 2). |
| The Glasswater Run | Glassmere (55,50) | Hollow Gulf Ports (66,90) | low | Down the great river to the S sea. |
| The Greatspine Passes (Crown Road) | Glassmere (55,50) | Concord Heartlands (62,56) → S | low | **Contested.** Through the cordillera. |
| The Salt Road | Pale Coast (14,21) | Saltmere Reaches (60,70) | low | Overland salt/relic caravan track. |
| The Hethe Tollway | Karran Marches (74,18) | Calm Reach coast (80,50) | low | Forest-river toll corridor. |
| The South Sea Lanes | Hollow Gulf (66,90) | Wracking Isles (3,60) → Surren | low | Open-ocean lanes. |
| The Pale Coast Sea-Route | Wrackmouth (12,23) | Caradril (34,35) → Hollow Gulf | high | Coastal water-route; extends S beyond cluster. |
| The Steppe Tracks | Wender Steppe (46,16) | central Orrun (55,40) | low | **Ungoverned** seasonal tracks. |

## DM-Only Subsurface / Endgame (NEVER render player-facing)

| Feature | Type | X | Y | Confidence | Notes |
|---|---|---|---|---|---|
| The Concord Deep | DM-only buried network | 24 | 24 | low | **DM-ONLY.** Subsurface; hub under the NW cluster basin. Not a surface label. |
| The Under-Shrine / Drowned Keystone | DM-only endgame | 24 | 23 | high | **DM-ONLY.** *Directly below* Hollowmere (same X,Y, deepest Z). Vertical, not lateral. |
| Concord node links (network) | DM-only edges | — | — | low | **DM-ONLY.** Lines from the basin to campaign-cluster nodes only; see `WORLD_MAP_LAYERS.md` Layer 7. |

---

## Coordinate Summary Counts

- **High confidence:** 22 (campaign-cluster rows + Pale Sea + Under-Shrine, re-anchored from established canon)
- **Medium confidence:** 16 (logical continental placement consistent with the NW-tilt axis and existing descriptions)
- **Low confidence:** 86 (placeholder continental regions, far rivers/ranges/forests, far routes, other landmasses, DM subsurface)
- **Total entries:** **124**
- **DM-only flagged rows:** 3 (the Concord Deep, the Under-Shrine/Keystone, the node-link edges)

## New Cartographic Assumptions (recorded)

1. **Dominant axis NW→SE:** cold-poor frontier NW, warm-rich settled SE. All placements honor this tilt.
2. **Campaign cluster = NW quarter** (X 8–40, Y 8–42), via the rescale transform above. Caradril is a frontier-edge city at continental scale, not a capital.
3. **The Greatspine cordillera (NW–SE) is the master divider;** its passes gate interior trade; the Concord Heartlands sit astride it.
4. **The endgame stays vertical** (under Hollowmere); no distant forbidden continent. Far ruins (Heartlands, Cindern, Saltmere, Drowned Steps) are surface/pre-Concord echoes, never the keystone.
5. **Volcanic region placed SE-central** (Emberfells/Ashfast), deliberately far from and unlike the cold NW.
6. **Variety over symmetry:** wetlands appear NW (Greyfens) and S (Sallow Marches); forests NW (Tollwood) and E/S (Hethewood/Sunmark); no single biome owns a compass direction.
7. **Other Vael landmasses** are off-grid placeholders (negative or >100 coords) and must never be drawn as part of Orrun proper.

## Duplicate-Prone Entries (render notes)

Several features in this file are referenced in more than one table here (and across `WORLD_MAP_COORDINATES.md`, `FULL_WORLD_MAP_AUTHORITY.md`, and `REGION_INDEX.md`) and could be accidentally rendered with more than one label. For each, the **single canonical player-safe map label lives in `PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md` §4. All other references in this file are aliases, context, or route anchors — not additional labels.**

- **Caradril** — appears as a city, a political region, the Stillwater settlement, and a route anchor (Verdance Road, Pale Coast Sea-Route). Render note: canonical player-safe label in PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md §4. All other references are aliases.
- **The Pale Sea** — water body plus coastline/route context. Render note: canonical player-safe label in PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md §4. All other references are aliases.
- **The Greatspine / Sundering Wall** — two range-endpoint rows (one range), two names, plus the Crown Road runs over it. Render note: canonical player-safe label in PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md §4. All other references are aliases.
- **The Glassmere League** — region row plus Glasswater river rows plus three route anchors. Render note: canonical player-safe label in PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md §4. All other references are aliases.
- **The Sunder Heights** — highlands row plus the "deep" placeholder sub-region plus a ruins sub-point. Render note: canonical player-safe label in PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md §4. All other references are aliases.
- **The Greyfens** — wetland row plus travel-hazard/route context. Render note: canonical player-safe label in PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md §4. All other references are aliases.
- **Hollowmere** — settlement row plus "Hollowmere basin" water row plus a Mirewend river course point (same X,Y). Render note: canonical player-safe label in PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md §4. All other references are aliases.
- **Saltmere / Saltmere Reaches** — inland-sea water row plus the region row (shared root, shared area; two DISTINCT labels). Render note: canonical player-safe labels in PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md §4. All other references are aliases.
- **Route-anchor settlements** (Wrackmouth, Caradril, and any settlement named in the Long-Distance Travel-Route Anchor Points table) — must not be re-labeled as separate route-point places. Render note: canonical player-safe label in PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md §4. All other references are aliases.

## Related Files

- [`PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md`](PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md) (player-safe render label authority)
- [`FULL_WORLD_MAP_AUTHORITY.md`](FULL_WORLD_MAP_AUTHORITY.md) · [`FULL_WORLD_MAP_LAYERS.md`](FULL_WORLD_MAP_LAYERS.md) · [`FULL_WORLD_MAP_PROMPTS.md`](FULL_WORLD_MAP_PROMPTS.md)
- [`WORLD_MAP_COORDINATES.md`](WORLD_MAP_COORDINATES.md) (campaign-area grid) · [`WORLD_MAP_AUTHORITY.md`](WORLD_MAP_AUTHORITY.md)
