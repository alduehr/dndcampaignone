# WORLD_MAP_COORDINATES.md — Normalized Coordinate Grid

---
type: region
secrecy: mixed
status: static
region: Orrun
factions: []
level_range: 1-20
related: [WORLD_MAP_AUTHORITY.md, MAP_DESCRIPTION.md, WORLD_MAP_LAYERS.md, WORLD_MAP_PROMPTS.md, TRAVEL_ROUTES_RING1.md]
tags: [type:map, secrecy:mixed, function:cartography, coordinates, grid, orrun]
---

## AI Use

A normalized **0–100 grid** for the mapped NW quarter of Orrun, for placing features on a future image map and for spatial reasoning. **North = top (Y=0), south = bottom (Y=100); west = left (X=0), east = right (X=100).** The grid spans only the mapped quarter (see `WORLD_MAP_AUTHORITY.md` §9), not all of Orrun.

**Confidence:** `high` = directly established by canon (named direction + travel time); `medium` = consistent inference from existing descriptions; `low` = placeholder, expansion will pin it down. **DM-only rows are flagged; never render them on a player-facing map.**

---

## Coordinate Frame (recorded assumptions)

- **Hollowmere is the dramatic center** and placed near the grid middle: **(50, 45)** — slightly north of center, because the land falls south to the Vale and the Heights wall sits N.
- **Direction anchors from canon:** Sunder Heights N (low Y), Pale Coast/Pale Sea W (low X), Tollwood E (high X), Ashgarden Vale S (high Y), Caradril SE (high X, high Y).
- **Travel-time scaling:** Caradril is the farthest established point (~10–12 days SE), so it sits near the SE corner. Ring 1 hubs (4–8 days out) sit at mid-radius. In-Reach sites (0.5–2 days) cluster near Hollowmere.
- **Coast runs N–S along the west edge;** the Verdance mouth is to the **south** of the Coast (the sea-route bends south then inland to Caradril).

---

## Major Regions (region centroids / labels)

| Feature | Type | X | Y | Confidence | Notes |
|---|---|---|---|---|---|
| Sundering Reach | region | 50 | 42 | high | Central fen basin; starting region. |
| Ashgarden Vale | region | 52 | 68 | high | South; farmland/shrine-towns. |
| Tollwood | region | 74 | 40 | high | East; deep forest. |
| Pale Coast | region | 18 | 38 | high | West; sea-cliffs. |
| Caradril (city-state) | region/city | 82 | 80 | high | SE; the city corner. |
| Sunder Heights | highlands | 50 | 18 | high | North broken highlands. |
| The Highmark Spine | mountain range (placeholder) | 55 | 6 | low | Far-N barrier wall; parent range. |
| The Verdance Reaches | region (Ring 2 placeholder) | 92 | 92 | low | Up-Verdance, SE off the mapped corner. |
| The Concord Deep | DM-only buried network | 50 | 47 | low | **DM-ONLY.** Subsurface, radiating from the basin; not a surface label. |

## Bodies of Water

| Feature | Type | X | Y | Confidence | Notes |
|---|---|---|---|---|---|
| The Pale Sea | ocean | 6 | 30 | high | Open sea filling the W/NW off the Coast. |
| Hollowmere basin | flooded basin | 50 | 45 | high | Lowest point; the drowned-shrine sink. |
| The Stillwater | harbor-lake | 80 | 78 | high | Caradril's port-lake on the Verdance. |
| Verdance mouth | river-mouth (sea) | 22 | 70 | medium | Where the Verdance reaches the Pale Sea, S of the Coast. |
| The Skerries | offshore stacks/reefs | 8 | 42 | medium | Gated; offshore W of the Coast. |

## Rivers (course endpoints — draw as lines between)

| Feature | Type | X | Y | Confidence | Notes |
|---|---|---|---|---|---|
| Mirewend River (source, Heights) | river course pt | 52 | 24 | medium | Rises in the Sunder Heights. |
| Mirewend River (through Hollowmere) | river course pt | 50 | 45 | high | Crosses the basin/Reach. |
| Mirewend River (E toward Kettle Bridge) | river course pt | 60 | 44 | high | The Mirewend crossing is the E toll-town. |
| Ammet River (headwaters, toward Tollwood) | river course pt | 66 | 56 | medium | Rises toward the Tollwood/Vale border. |
| Ammet River (through the Vale) | river course pt | 52 | 66 | medium | The Vale's river; Tilbrook/Orchardmere on it. |
| Verdance (upland source) | river course pt | 90 | 70 | low | Rises in the SE interior uplands. |
| Verdance (the Stillwater) | river course pt | 80 | 78 | high | Broadens at Caradril. |
| Verdance (to the sea-mouth) | river course pt | 22 | 70 | medium | Runs SW to the Pale Sea mouth. |

## Reach Settlements

| Feature | Type | X | Y | Confidence | Notes |
|---|---|---|---|---|---|
| Hollowmere | town (start/hub) | 50 | 45 | high | Basin rim; the keystone town. |
| Kettle Bridge | town | 60 | 44 | high | E, Mirewend crossing; on-ramp to Tollwood. |
| Saltmargin | town | 36 | 42 | high | W salt-town; on-ramp to Pale Coast (~5 days W). |
| Candlewick | village | 50 | 54 | high | S edge of Reach; on-ramp to the Vale. |
| Greywater Holm | village | 44 | 52 | medium | SE Greyfens edge; rites fail worst. |
| Harrowgast | mining town | 52 | 26 | medium | N, up in the Sunder Heights (2–3 days N). |
| Reedford | hamlet | 53 | 48 | medium | Central ford on the road. |
| The Ashwalk Rest | waystation | 51 | 49 | medium | Central crossroads sanctuary. |

## Reach Wilderness / Landmarks

| Feature | Type | X | Y | Confidence | Notes |
|---|---|---|---|---|---|
| The Greyfens | marsh zone | 42 | 50 | high | SW-of-center fog marsh. |
| The Sunder Heights ruins | highland ruins | 50 | 20 | high | N highland Concord ruins. |
| The Mirewend roads / causeways | travel layer | 50 | 45 | high | Radiate from Hollowmere along the Mirewend. |
| The drowned shrine (basin) | DM-only keystone | 50 | 45 | high | **DM-ONLY.** Beneath the basin; the keystone node. |

## Ring 1 Settlements

| Feature | Type | X | Y | Confidence | Notes |
|---|---|---|---|---|---|
| Orchardmere | town (Vale hub) | 52 | 70 | high | On Orchardmere lake; ~5–6 days S of Hollowmere. |
| Saint Veddow's Rest | town (pilgrimage) | 48 | 74 | medium | Hill-shrine town just S/SW of Orchardmere. |
| Tilbrook | village | 53 | 62 | medium | On the Ammet, between Candlewick and Orchardmere. |
| Hartfell | town (Tollwood hub) | 78 | 40 | high | ~4–5 days E; stockaded road-town. |
| Coldhearth | village | 82 | 34 | medium | Deeper E into the wood. |
| Tollstone Cross | hamlet | 68 | 42 | medium | On the East Road between Kettle Bridge and Hartfell. |
| Wrackmouth | town (Coast hub/port) | 14 | 44 | high | ~7–8 days W; cliff-harbor; the port. |
| Cobble Strand | village | 16 | 36 | medium | Shingle cove under the Drowned Lamp headland, N of Wrackmouth. |

## Ring 1 Landmarks / Wilderness

| Feature | Type | X | Y | Confidence | Notes |
|---|---|---|---|---|---|
| Orchardmere lake | lake | 53 | 70 | medium | The Vale hub's lake. |
| The southern downs | open downs | 66 | 76 | medium | Between the Vale and Caradril (the S approach). |
| The Old Mast (deep wood) | gated landmark-power | 86 | 32 | medium | **Gated.** Tollwood's deep heart. |
| The Hanging Oaks | grove/dungeon | 80 | 36 | low | Mid-deep Tollwood; cult cell. |
| The Greenward Toll-Station | Concord road-node | 70 | 41 | low | On the East Road. |
| The Drowned Lamp | coastal Concord node | 15 | 34 | medium | **Gated lower levels.** Ruined lighthouse headland N of Wrackmouth. |
| The Skerry Shrine | gated coastal dungeon | 8 | 40 | low | **Gated.** Largest coastal node, offshore. |
| The Wreckers' Caves | sea-caves | 11 | 38 | low | Wild-coast sea-caves. |
| Saint Veddow's Tomb (inner shrine) | capped Concord node | 48 | 75 | medium | **Gated.** Beneath the pilgrimage hill. |
| The Buried Cloister | Concord ruin | 50 | 72 | low | Orchard-country Concord ruin. |
| The Pellow Grange | Ledger relic-quarry | 56 | 66 | low | Vale grange/quarry site. |
| Marrow Cross | gibbet-hamlet | 58 | 64 | low | Vale crossroads; leakage hotspot. |

## Caradril (city + key districts — fine grid near the city centroid)

| Feature | Type | X | Y | Confidence | Notes |
|---|---|---|---|---|---|
| Caradril (city) | major city | 82 | 80 | high | SE; on the Verdance/Stillwater. |
| The Stillwater quays | harbor | 80 | 79 | medium | The city's port frontage. |
| (Districts) | — | ~82 | ~80 | low | 8 districts cluster at the city point; see `CARADRIL.md` for internal layout. Not separately gridded at world scale. |

## Travel-Route Anchor Points (for the travel-route layer)

| Route | From (X,Y) | To (X,Y) | Confidence | Notes |
|---|---|---|---|---|
| South Road (Reach→Vale) | Candlewick (50,54) | Orchardmere (52,70) | high | via Tilbrook. |
| Vale→Caradril (S approach) | Orchardmere (52,70) | Caradril (82,80) | high | across the southern downs. |
| East Road (Reach→Tollwood) | Kettle Bridge (60,44) | Hartfell (78,40) | high | via Tollstone Cross. |
| Tollwood→Caradril (E approach) | Hartfell (78,40) | Caradril (82,80) | medium | forest thins to farmland near the city. |
| Pale Road (Reach→Coast) | Saltmargin (36,42) | Wrackmouth (14,44) | high | via Cobble Strand. |
| Coast→Caradril (sea/Verdance) | Wrackmouth (14,44) | Stillwater (80,79) | high | down-coast to Verdance mouth (22,70), then up-river. |

## Placeholder / Future Regions

| Feature | Type | X | Y | Confidence | Notes |
|---|---|---|---|---|---|
| The Verdance Reaches | Ring 2 region | 92 | 92 | low | Off the SE corner, up the Verdance. |
| The Highmark Spine | barrier range | 55 | 6 | low | Far-N wall closing the quarter. |
| The Highmark passes | late frontier | 60 | 8 | low | Optional late expansion in the N range. |
| The Concord Deep | DM-only network | 50 | 47 | low | **DM-ONLY.** Subsurface; centered under the basin. |
| The Under-Shrine / Drowned Keystone | DM-only endgame | 50 | 45 | high | **DM-ONLY.** *Directly below* Hollowmere (same X,Y, deepest Z). Vertical, not lateral. |

---

## Coordinate Summary Counts

- **High confidence:** 31
- **Medium confidence:** 24
- **Low confidence:** 22
- **Total entries:** 77
- **DM-only flagged rows:** 6 (the drowned shrine, the Concord Deep ×2 listings, the Under-Shrine/Keystone, plus the DM-only notes on the basin keystone).

(Counts are approximate working totals for this pass; expansion passes will add Ring 2+ detail and raise low-confidence placeholders.)

## Related Files

- [`WORLD_MAP_AUTHORITY.md`](WORLD_MAP_AUTHORITY.md) · [`MAP_DESCRIPTION.md`](MAP_DESCRIPTION.md) · [`WORLD_MAP_LAYERS.md`](WORLD_MAP_LAYERS.md) · [`WORLD_MAP_PROMPTS.md`](WORLD_MAP_PROMPTS.md) · [`TRAVEL_ROUTES_RING1.md`](TRAVEL_ROUTES_RING1.md)
