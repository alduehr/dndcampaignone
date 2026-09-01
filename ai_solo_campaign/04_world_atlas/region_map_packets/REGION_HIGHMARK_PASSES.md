# REGION_HIGHMARK_PASSES.md — Regional Map Packet

---
type: region
secrecy: mixed
status: static
region: Highmark Passes
level_range: 12-16
related: [../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, ../FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../MAP_FEATURE_REGISTRY.md, ../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md, ../../10_dungeons_and_ruins/THE_HIGHMARK_FROZEN_WORKS.md]
tags: [type:map, secrecy:mixed, function:cartography, map-packet, region-map, highmark-passes]
---

> **Secrecy classification:** Mixed — D35 (the Highmark Frozen Works) is **DM-ONLY** and NEVER appears on a player map. The Highmark Spine's deep Concord works are the *oldest* Concord infrastructure; their existence proves the Concord's reach once extended to the campaign world's N limit, but they are NEVER the keystone or the machine. No NPC lives here permanently; no NPC file exists for this region. Optional late-frontier region; never required for main arc completion. Never hand this file directly to the player.

## Region: Highmark Passes (MF-018) — Optional Late Frontier

- **Local grid:** 0–100, where **(0,0) = NW corner of the region frame, X = east, Y = south** (Y=0 top). (100,100) = SE.
- **Full-continent bounds this local grid maps to:** render-grid **X 26–44, Y 7–11** (centroid full (35,9)); from `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §10`.
- **Local↔full transform:** `local_X = (full_X - 26) / 18 * 100`; `local_Y = (full_Y - 7) / 4 * 100`. (Inverse: `full_X = 26 + local_X/100*18`; `full_Y = 7 + local_Y/100*4`.)
- **One-sentence identity:** The campaign world's far-northern mountain barrier — a near-impassable spine of ice and ancient passes where the oldest Concord works lie frozen in the high passes, untouched since before the Quietfall.

> **Level note:** This is an **optional late-frontier region** for Level 12–16 characters. It has no permanent NPC population, no settlement anchors, and no dedicated NPC/quest file. The Highmark Spine is a geographic barrier, an exploration zone, and a source of late-arc lore at D35.

## Neighboring Regions

| Direction | Region |
|---|---|
| S (SE) | Wender Steppe (the steppe begins where the Spine's S foot opens) |
| S (SW) | the Sundering Reach cluster / the campaign's NW starting-area (the Spine's W foot) |
| E | Karran Marches (the Karran Teeth are the Spine's E spur) |
| N | the Sunder Ocean (beyond the Spine; off-grid) |
| W | the Iron Skards (beyond the Spine's W seaward end; off-grid) |

## Terrain Zones (local polygons)

| Zone | Type | Local centroid | Full-grid | Description |
|---|---|---|---|---|
| The Highmark Spine core | continental mountain barrier | (50,50) | (35,9) | The great ice-clad mountains; permanent snow, altitude, near-impassable except at the named passes. |
| The named passes | narrow high-altitude corridors | (33,50) | (32,9), (67,50) | The campaign's two confirmed passes: the High Pass (W) and the Iron Pass (E). |
| The Frozen Works zone | pre-Concord/Concord ruins (ice-locked) | (67,25) | (38,8) | Where D35 lies — a Concord relay-station frozen into a high-altitude ice-shelf. |
| The S approach foothills | highland transition (S face) | (50,85) | (35,10.4) | The S face's lower slopes; accessible from the Wender Steppe or the Sundering Reach cluster. |

## Water Features

| Feature | Type | Local | Full-grid | Flow |
|---|---|---|---|---|
| Highmark glaciers | permanent ice | (50,30) | (35,8.2) | Feed the Sunder Ocean (N) via melt; the Spine's dominant terrain |
| Highmark melt-streams | seasonal glacial melt (S face) | (50,80)→S edge | (35,10.2)→(35,11) | Flow S into the Wender Steppe's seasonal water-holes and the Sundering Reach cluster's rivers |

## Roads / Routes (local polylines)

| Route | Local waypoints | Full-grid | Travel time | Notes |
|---|---|---|---|---|
| The High Pass (W) | S foothills → (33,50) pass-crest → N face | (29,10.6)→(32,9)→(32,7) | weeks (seasonal only; spring/summer) | The western crossing; trade-route potential; the Iron Skards sea-approach on the N side |
| The Iron Pass (E) | S foothills → (67,50) pass-crest → N face | (38,10.6)→(38,9)→(38,7) | weeks (dangerous year-round) | The eastern crossing; near the Frozen Works; colder and more exposed |
| The Frozen Works approach | (67,50) Iron Pass → (67,25) D35 | (38,9)→(38,8) | days (extreme) | Not a road — a navigation challenge through ice and altitude |

## Bridges / Fords / Ferries / Locks

| Feature | Type | Local | Full-grid | Notes |
|---|---|---|---|---|
| Natural ice-bridges | seasonal crossings | scattered | — | Form in deep winter; collapse in spring; passage-windows are narrow |
| Pass waystation ruins | broken Concord rest-stations | (33,50), (67,50) | (32,9), (38,9) | Roofless; usable for short rest shelter; the Frozen Works is the intact version |

## Settlements

> **None.** The Highmark Passes have no permanent settlements and no settlement anchors. The region is a geographic barrier, an exploration zone, and an optional late-arc dungeon approach. The only structure is D35 (Frozen Works), which is DM-only.

## Dungeons / Adventure Sites

| Site | Local | Full-grid | Surface marker | Player-map |
|---|---|---|---|---|
| D35 The Highmark Frozen Works | (67,25) | (38,8) | ice-locked Concord relay-station (barely visible through the glacier) | **DM-ONLY — NEVER on player map** |

> D35 is the campaign's highest-altitude, most isolated Concord site — a relay-station frozen into the Highmark glaciers at the moment of the Quietfall. It is accessible only through the Iron Pass and extreme mountaineering. Its existence is **DM-only information** until a player actively seeks it (high-level arc, M6/M9 optional lore).

## Ruins / Wilderness Landmarks

| Landmark | Local | Full-grid | Notes |
|---|---|---|---|
| The Frozen Works (D35) | (67,25) | (38,8) | DM-ONLY; the oldest intact Concord station; frozen mid-operation; M6-optional deep lore |
| The Pass waystation ruins (High Pass) | (33,50) | (32,9) | roofless Concord rest-station; short-rest shelter; script carved in walls (DC 18 to read) |
| The Pass waystation ruins (Iron Pass) | (67,50) | (38,9) | same; closer to D35; the last mark before the glacier |
| The Sunder Heights signal relay | (15,70) | (28.7,9.8) | a relay-marker visible from the campaign-cluster's Sunder Heights; the faintest DM hint of the Highmark |

## Level Range And Solo Danger

- **Recommended level:** 12–16.
- **Expected solo danger:** Extreme throughout. The Highmark Passes are the campaign's most hostile environment. Cold, altitude, isolation, and disorientation are the primary killers. There are no allies, no safe rest-points except the ruined waystations, no vendors, and no rescue.
- **Lethal zones:** the entire region above the S foothills is potentially lethal (extreme cold, avalanche, altitude exhaustion, disorientation). The Frozen Works approach (D35) is extreme even for a fully prepared L16 character.
- **Telegraphing:** the Wender Steppe's seers name "the Spine" as the world's N limit; the Sunder Heights' signal relay (visible from the campaign cluster) points at the Highmark as a destination only for the truly determined. No NPC sends the player here; they must come themselves.

## Encounter And Hazard Mechanics

- **Encounter themes (stat references):** the Highmark has **no intelligent faction encounters** — the region is empty of humanoid power. Natural hazards only: extreme weather, wildlife (Ice-Bear / Remorhaz-like threats, CR 10–15, solitary, territorial), and the Frozen Works' preserved Concord-construct defenders at D35 (**Shield Guardian / Golem-like**, CR 10–14). Use `13_encounters_and_bestiary/` arctic/mountain encounter lines at high tier.
- **Environmental hazards:** extreme cold (Constitution DC 15 per hour without extreme-weather gear; DC 17 above the pass-crests; 3d6 cold damage on fail); altitude exhaustion (Constitution DC 14 each hour above the pass; exhaustion levels); avalanche (Dexterity DC 16 to avoid; 8d6 bludgeoning; telegraphed by unstable snow-pack); disorientation (Survival DC 17 to navigate in white-out; Survival DC 20 in blizzard); ice-shelf instability near D35 (Dexterity DC 16, 4d6 falling/cold).
- **Social DCs:** not applicable. No social encounters; no humanoid NPCs here. Any encounter is with the environment or the Frozen Works' preserved guardians.
- **Scaling:** L12 — the passes themselves, waystation-shelter runs. L16 — the Frozen Works approach and D35 interior (the oldest intact Concord station, frozen at the moment of the Quietfall).

## Local Labels (player map)

The Highmark Spine (mountain range fill, dominant; label "Highmark Spine"); the Highmark Passes (region label, ONE — smaller, below the range label); the High Pass (pass marker W); the Iron Pass (pass marker E); the Sunder Ocean (water, N edge; label on water). **D35 is NEVER on the player map.**

## Player-Safe Layer

- Visible: the great mountain barrier, the two named passes as the only crossings, the Sunder Ocean to the N. The region reads as the campaign world's N limit — impassable except by the determined, cold, and empty.
- The Concord's northern reach is implied by the waystation ruins (Script carved in the walls) but never stated outright on the player map.

## DM-Only Layer (NEVER on the player map)

- D35 (The Highmark Frozen Works) is the **oldest intact Concord infrastructure** — a relay-station frozen mid-operation at the Quietfall moment. Its preservation reveals what the Concord was doing at the moment of its collapse. This is **M6-optional deep lore**: a late-arc optional revelation that corroborates the campaign's hidden history.
- The Frozen Works contains a **Concord message, frozen in the sending** — instructions for the harvest-network that confirm the keystone's location (Hollowmere basin, NW). This is the most direct non-Hollowmere pointer to the endgame's vertical axis. ONLY reachable at late arc through extreme effort.
- No Hollow Court presence; the Court withdrew from the Spine at the Quietfall. The Works are empty of living agents.
- The Spine's N face and the Sunder Ocean beyond are **off-grid** and off-campaign. The Iron Skards are a distant placeholder, never built.

## Unresolved Map Gaps

- The pass-crests' exact positions and the glacier's extent are approximate; the Frozen Works is deterministic at local (67,25) / full (38,8).
- The Highmark's W extent (toward the Iron Skards) is off-grid.
- D35's interior layout is in `THE_HIGHMARK_FROZEN_WORKS.md`; this packet positions the approach.

## Related Files

- D-site: [`../../10_dungeons_and_ruins/THE_HIGHMARK_FROZEN_WORKS.md`](../../10_dungeons_and_ruins/THE_HIGHMARK_FROZEN_WORKS.md)
- Authority: [`../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`](../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md) · [`../FULL_CONTINENT_SETTLEMENT_ANCHORS.md`](../FULL_CONTINENT_SETTLEMENT_ANCHORS.md) · [`../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
