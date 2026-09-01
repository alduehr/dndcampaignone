# REGION_SUNDERING_REACH.md — Regional Map Packet

---
type: region
secrecy: mixed
status: static
region: Sundering Reach
level_range: 1-8
related: [../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, ../MAP_FEATURE_REGISTRY.md, ../../05_regions/SUNDERING_REACH.md, ../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md, ../WORLD_MAP_COORDINATES.md]
tags: [type:map, secrecy:mixed, function:cartography, map-packet, region-map, sundering-reach]
---

> **Secrecy classification:** Mixed. The DM-only layer (the keystone/Under-Shrine/Concord Deep) must NEVER appear on a Sundering Reach player-safe map. Never hand directly to the player.

## Region: Sundering Reach (MF-001)

- **Local grid:** 0–100, where (0,0) = NW corner of the region frame, (100,100) = SE; X east, Y south.
- **Full-continent bounds this local grid maps to:** render-grid **X 19–28, Y 13–28** (the NW campaign cluster's center). Local (50,50) ≈ full (24,23) Hollowmere.
- **Local↔campaign grid:** this packet's local grid is a re-frame of the campaign grid in `WORLD_MAP_COORDINATES.md` (where Hollowmere = 50,45); positions below cite campaign-grid coords as the fine-placement authority.

## Neighboring Regions

| Direction | Region |
|---|---|
| N | Sunder Heights highlands → the Highmark Spine (far N) |
| S | Ashgarden Vale |
| E | Tollwood |
| W | Pale Coast |
| SE | Caradril (via the Vale/Tollwood approaches) |

## Terrain Zones (local polygons)

| Zone | Type | Local centroid | Campaign-grid | Notes |
|---|---|---|---|---|
| Hollowmere basin | flooded basin | (50,50) | (50,45) | Dark central water; lowest point. Render dark, unexplained. |
| The Greyfens | fog marsh | (35,55) | (42,50) | SW-of-center; most dangerous wetland. |
| The Sunder Heights | broken highlands | (52,18) | (50,20) | N highland Concord ruins/mines. |
| The Mirewend Sinks (S edge) | boglands | (50,90) | (50,60+) | S transition toward the Vale. |
| Firm holms / farmland | dry ground | scattered | — | Villages sit on these. |

## Water Features

| Feature | Type | Local | Campaign-grid | Flow |
|---|---|---|---|---|
| Hollowmere basin | basin | (50,50) | (50,45) | drainage sink (everything tilts in) |
| Mirewend River | river | (50,50) through | (50,45) | Heights source (52,24) → basin → E to Kettle Bridge (60,44) → S drain |
| Greyfens standing water | fen | (35,55) | (42,50) | stagnant, fog-bound |

## Roads / Routes (local polylines)

| Route | Local waypoints | Campaign-grid | Notes |
|---|---|---|---|
| In-Reach Concord roads | radiate from (50,50) | from (50,45) | safe-ish causeways; 0.5–2 days between sites |
| South Road (→ Vale) | (50,50)→(50,70) Candlewick | (50,45)→(50,54) | S gateway |
| East Road (→ Tollwood) | (50,50)→(62,46) Kettle Bridge | (50,45)→(60,44) | E gateway |
| Pale Road (→ Coast) | (50,50)→(34,44) Saltmargin | (50,45)→(36,42) | W gateway |

## Bridges / Fords / Ferries

| Feature | Local | Campaign-grid | Notes |
|---|---|---|---|
| Kettle Bridge (Mirewend crossing) | (62,46) | (60,44) | toll-town bridge |
| Reedford ford | (54,50) | (53,48) | central road ford |
| Sashe's Crossing | (40,52) | (44,52) | Greyfens guide-ford |
| The Drowned Mile | (52,50) | (51,49) | flooded causeway stretch |

## Settlements

| Settlement | Type | Local | Campaign-grid | File |
|---|---|---|---|---|
| Hollowmere | town (hub) | (50,50) | (50,45) | HOLLOWMERE.md |
| Kettle Bridge | town | (62,46) | (60,44) | KETTLE_BRIDGE.md |
| Saltmargin | town | (34,44) | (36,42) | SALTMARGIN.md |
| Candlewick | village | (50,70) | (50,54) | CANDLEWICK.md |
| Greywater Holm | village | (40,58) | (44,52) | GREYWATER_HOLM.md |
| Harrowgast | mining town | (52,26) | (52,26) | HARROWGAST.md |
| Reedford | hamlet | (54,52) | (53,48) | REEDFORD.md |
| The Ashwalk Rest | waystation | (51,53) | (51,49) | THE_ASHWALK_REST.md |

## Dungeons / Adventure Sites

| Site | Local | Campaign-grid | Surface marker | Player-map |
|---|---|---|---|---|
| D01 Peat Chapel | (48,55) | (48,52) | half-sunk chapel | visible |
| D02 Whispering Cairn | (54,48) | (54,48) | archive-cairn | visible |
| D03 Sunken Tollhouse | (62,46) | (60,44) | drowned arch under Kettle Bridge | label-only |
| D04 Ledger Vault | (50,50) | (50,45) | counting-house (urban heist) | urban |
| D05 Deep Adit | (52,28) | (52,26) | mine-adit (Harrowgast) | label-only |
| D06 Barrow of Nine Doors | (40,58) | (42,52) | grass barrow-mound | label-only |
| D18 Concord Relay-Vault | (55,22) | (55,22) | buried signal-cairn (Heights) | hidden |
| D19 Greyfens Deep | (35,58) | (42,55) | open deep fen | label-only |
| D20 Basin Keystone Approach | (50,50) | (50,45) | basin shore upper ruin | label-only ("deep basin — lethal") |

## Ruins / Landmarks

| Landmark | Local | Campaign-grid | Notes |
|---|---|---|---|
| The Surfacing Ruin (basin) | (50,48) | (50,45) | M2 site; basin shore |
| The Star-Stones (relay markers) | along roads | varies | standing stones (relay truth DM-only) |
| The Sundered Ridge / Roofless Hall | (52,16) | (50,20) | Heights ruins |
| The Drift-Line | (38,54) | (42,50) | Greyfens M5 field-proof |

## Local Labels (player map)

Sundering Reach; Hollowmere; Kettle Bridge; Saltmargin; Candlewick; Greywater Holm; Harrowgast; Reedford; The Ashwalk Rest; Hollowmere basin (dark water); the Greyfens; the Sunder Heights; the Mirewend; the South/East/Pale Roads.

## Player-Safe Layer

- Visible: all 8 settlements, the basin (dark water, unexplained), the Greyfens, the Sunder Heights, the Mirewend, the three roads, and the visible/label-only adventure-site markers above.
- Telegraph the deep basin as **dangerous/lethal** ("deep basin — do not enter") without naming any node or depth.

## DM-Only Layer (NEVER on the player map)

- The **drowned shrine / Under-Shrine / Drowned Keystone** beneath the basin (vertical, deepest Z) — D23.
- The **Concord Deep** subsurface network hub under the basin.
- The **Hollow Court** seat beneath the basin.
- The **node-network links** (basin ↔ Sunken Tollhouse ↔ Deep Adit ↔ Relay-Vault ↔ Star-Stones relays).
- Gravecaller cell at the Drowned Blind (Greyfens).

## Unresolved Map Gaps

- Exact fen-island ("holm") positions are illustrative; villages sit on dry ground, precise micro-geography is improv-safe.
- The Mirewend Sinks S-edge transition to the Vale is loosely bounded.

## Related Files

- [`../../05_regions/SUNDERING_REACH.md`](../../05_regions/SUNDERING_REACH.md) · [`../WORLD_MAP_COORDINATES.md`](../WORLD_MAP_COORDINATES.md) (fine campaign-grid placement) · [`../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
