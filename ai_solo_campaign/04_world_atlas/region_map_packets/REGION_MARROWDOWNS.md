# REGION_MARROWDOWNS.md — Regional Map Packet

---
type: region
secrecy: mixed
status: static
region: Marrowdowns
level_range: 6-10
related: [../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, ../FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../MAP_FEATURE_REGISTRY.md, ../../08_npcs/by_region/MARROWDOWNS_NPCS.md, ../../09_quests/by_region/MARROWDOWNS_QUESTS.md, ../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md, ../../10_dungeons_and_ruins/THE_MARROWDOWNS_BARROW_COMPLEX.md]
tags: [type:map, secrecy:mixed, function:cartography, map-packet, region-map, marrowdowns]
---

> **Secrecy classification:** Mixed. The Barrow-Fields are **pre-Concord** (older than the Concord and its network), a resonant "older-fall" echo — NEVER the keystone, the machine, the Concord Deep, or the Hollow Court (NW only, vertical beneath Hollowmere). Never hand this file directly to the player; render only the Player-Safe Layer.

## Region: Marrowdowns (MF-008)

- **Local grid:** 0–100, where **(0,0) = NW corner of the region frame, X = east, Y = south** (Y=0 top). (100,100) = SE.
- **Full-continent bounds this local grid maps to:** render-grid **X 45–55, Y 60–70** (centroid full (50,66)); from `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §10`.
- **Local↔full transform:** `local_X = (full_X - 45) / 10 * 100`; `local_Y = (full_Y - 60) / 10 * 100`. (Inverse: `full_X = 45 + local_X/100*10`; `full_Y = 60 + local_Y/100*10`.)
- **One-sentence identity:** Settled chalk-down sheep-country and ancient barrow-fields — a gentler, orderly, custom-bound pastoral mid-continent of manorial holds and shire-moots, useful as a route south and a place of quiet old custom where the barrow-dead are "growing restless."

## Neighboring Regions

| Direction | Region |
|---|---|
| N | Glassmere League |
| E | Saltmere Reaches |
| S | Sunmark / Sallowmarch Protectorate (the route south) |
| W | (toward the Mirewend Sinks / inland transitions) |

## Terrain Zones (local polygons)

| Zone | Type | Local centroid | Full-grid | Description |
|---|---|---|---|---|
| The central downs | rolling chalk grassland | (50,50) | (50,65) | Open green sheep-walks; the shire's heart; Marrowmoot sits on the down-roads here. |
| The Barrow-Fields | ancient burial-downs | (70,40) | (52,64) | Pre-Concord barrow-mounds; sacred old ground "that must lie quiet"; now stirring. |
| The Penmark vale | manorial farmland | (20,30) | (47,63) | Hedged manor-fields and Penmark Hold; the gentry's orderly heart. |
| The wool-walks | high sheep-pasture | (80,80) | (53,68) | Upland fleece-country around Wether; the wool-wealth. |
| The Mardenflow head | spring-fed down-valley | (70,40) | (52,64) | The Mardenflow rises among the barrows and runs S to the delta. |

## Water Features

| Feature | Type | Local | Full-grid | Flow |
|---|---|---|---|---|
| The Mardenflow (source) | river headwaters | (70,40) | (52,64) | rises in the downs; runs S → Sallow Marches delta → Hollow Gulf |
| Down-springs & chalk-streams | seasonal streams | scattered | — | clear chalk-fed brooks feeding the sheep-walks |

## Roads / Routes (local polylines)

| Route | Local waypoints | Full-grid | Travel time | Notes |
|---|---|---|---|---|
| Salt Road | NW edge → (50,50) Marrowmoot → E edge | (37,54)→(50,66)→(60,70) Saltmere | Marrowmoot→Saltmere ~1 week | the cross-continent overland salt-and-wool route |
| The Road South | (50,50) Marrowmoot → (80,80) Wether → S edge | (50,66)→(53,68)→south to Sunmark/Sallowmarch | days south to the warm regions | the wool-drive route and the player's path onward (Q_MD_005) |
| Down-roads (shire lanes) | radiate from Marrowmoot to the holds | local | hours–1 day between holds | shire lanes patrolled by the horse-reeve |

## Bridges / Fords / Ferries / Locks

| Feature | Type | Local | Full-grid | Notes |
|---|---|---|---|---|
| Marrowmoot down-ford | stream ford | (50,50) | (50,66) | the shire-town crossing |
| Mardenflow head-ford | spring-stream ford | (70,40) | (52,64) | near the Barrow-Fields; where the southbound road begins to fall toward the delta |

## Settlements

| Settlement | Type | Local | Full-grid | Anchor source / file |
|---|---|---|---|---|
| Marrowmoot | town (shire-town hub) | (50,50) | (50,66) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (md.marrowmoot); NPC/quest hub |
| Penmark Hold | manor-town | (20,30) | (47,63) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (md.penmark_hold) |
| Wether | wool-trade village | (80,80) | (53,68) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (md.wether) |

> Light NPC-facing anchors, not deep-built gazetteers; internal micro-geography is improv-safe.

## Dungeons / Adventure Sites

| Site | Local | Full-grid | Surface marker | Player-map |
|---|---|---|---|---|
| D26 The Marrowdowns Barrow Complex | (70,40) | (52,64) | barrow-mounds on the downs (the Barrow-Fields) | label-only |

> **Authority note (resolved 2026-06-18, Cartography Determinism Cleanup):** the `ADVENTURE_SITE_CARTOGRAPHY_INDEX.md` master table (and `DUNGEON_INDEX.md`, `RUIN_INDEX.md`, `MAP_FEATURE_REGISTRY.md`, `CLUE_INDEX.md`) assign the Marrowdowns Barrow Complex **D26**; **D30** is the Sallowmarch Drowned Steps and **D33** is the Sunhollow Great Grove. An earlier packet edit incorrectly "corrected" this to D30 in the wrong direction; the master index is authoritative and this packet now uses **D26**.

## Ruins / Wilderness Landmarks

| Landmark | Local | Full-grid | Notes |
|---|---|---|---|
| The Barrow-Fields | (70,40) | (52,64) | ancient pre-Concord burial-downs; "must lie quiet"; now stirring (Q_MD_001/002) |
| The deep barrow (the Barrow That Bites) | (72,42) | (52.2,64.2) | the oldest, most-stirring mound (Q_MD_002) |
| The moot-stone (Marrowmoot) | (50,50) | (50,66) | where the shire-moots gather (old law) |

## Level Range And Solo Danger

- **Recommended level:** 6–10.
- **Expected solo danger:** Low–moderate. Most of the region is orderly and safe (shire-law, hospitality). Danger concentrates in the Barrow-Fields and on the down-roads.
- **Lethal-at-low-level zones (telegraphed):** the **deep barrows** (Q_MD_002) hold waking barrow-dead and trap-laced mounds — moderate-to-high for a solo PC; telegraphed by shepherds' flocks refusing to graze, horses shying, and Senna Crale's warnings. Down-road banditry/rustling (Q_MD_005) is avoidable and the horse-reeve's troop backs the player.
- **Telegraphing:** the barrow-dread is heavily signaled (animal-omens, folk-songs, the shire's nervous talk) before any barrow fight; the open downs always allow retreat.

## Encounter And Hazard Mechanics

- **Encounter themes (stat references):** waking barrow-dead (**Skeleton / Zombie / Wight / Specter-like**, scaled L6–10 — slow, telegraphed; thinnable by barrow-custom rite; see `13_encounters_and_bestiary/` undead lines and the Reach's **Barrow-Wight/Barrow-Shade** profiles in `SUNDERING_REACH_ENCOUNTERS.md`); barrow-robbers and down-road bandits/rustlers (**Bandit / Scout-like**, AC 13); shire-constables and the horse-reeve's mounted troop (**Guard / Veteran-like**, allies). Use `13_encounters_and_bestiary/MARROWDOWNS_ENCOUNTERS.md` and `13_encounters_and_bestiary/TRAVEL_ENCOUNTERS.md` for generic downs/road lines.
- **Environmental hazards:** barrow-traps (Thieves' tools / Investigation DC 16; barrow-craft via Doss Wether mitigates); a deep barrow has a dread/air clock (no safe rest inside); a "wrong" pre-Concord relic may inflict **Thin-touch** on handling (Stage 3 condition).
- **Travel/social DCs (typical):** Survival DC 15 (down-roads); Investigation DC 16 (the stirring barrows, the relic side-trade); Religion DC 15 (barrow-custom); Persuasion DC 16 (Penmark, the gentry). See the quest file for per-quest DCs.
- **Scaling:** L6 — one stirring barrow, scattered rustlers. L10 — a barrow-field waking, the deepest mound, and an organized robber-and-rustler ring.

## Local Labels (player map)

The Marrowdowns (one label for region+terrain); Marrowmoot; Penmark Hold; Wether; the Mardenflow (source); the Salt Road; the Road South; the Barrow-Fields (label-only, "ancient barrows"). Mark barrow-mounds as broken pre-Concord ruins.

## Player-Safe Layer

- Visible: the three anchor settlements, the Salt Road and Road South, the Mardenflow source, the open downs, the Barrow-Fields as ancient mound-country.
- Telegraph the barrows as **old, sacred, and best left alone** ("the barrows must lie quiet"; "the dead have grown restless") without explaining any cause, network, or depth.

## DM-Only Layer (NEVER on the player map)

- The Barrow Complex (D26) is **pre-Concord** — its waking dead corroborate the *"older, wider fall"* theme; a resonant echo, NEVER the keystone, the machine, or the Concord Deep.
- Barrow-Master Doss Wether's robbing **worsens** the local stirring (an unwitting aggravator) — DM moral knot, not a map feature.
- Moot-Mother Senna Crale carries the **old-songs network fragment** ("the grey hands took the dead"), which she half-conflates with the older pre-Concord barrow-doom — M6-oblique folk-memory ONLY; no mechanism, no Court, no keystone.
- A "wrong" pre-Concord relic from a deep barrow is M2-oblique; never explain Remembrance/the harvest.
- No apex geometry exists here. The endgame is vertical beneath Hollowmere (NW only).

## Unresolved Map Gaps

- Exact barrow positions within the Barrow-Fields are illustrative (place mounds as play demands); the *fact* of pre-Concord barrows and their stirring is canon.
- Internal town/manor layouts are improv-safe.
- The S transition (the Road South to Sunmark/Sallowmarch) is loosely bounded at the region edge.

## Related Files

- NPCs: [`../../08_npcs/by_region/MARROWDOWNS_NPCS.md`](../../08_npcs/by_region/MARROWDOWNS_NPCS.md)
- Quests: [`../../09_quests/by_region/MARROWDOWNS_QUESTS.md`](../../09_quests/by_region/MARROWDOWNS_QUESTS.md)
- D-site: [`../../10_dungeons_and_ruins/THE_MARROWDOWNS_BARROW_COMPLEX.md`](../../10_dungeons_and_ruins/THE_MARROWDOWNS_BARROW_COMPLEX.md)
- Authority: [`../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`](../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md) · [`../FULL_CONTINENT_SETTLEMENT_ANCHORS.md`](../FULL_CONTINENT_SETTLEMENT_ANCHORS.md) · [`../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
