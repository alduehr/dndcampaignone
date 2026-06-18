# REGION_SUNMARK.md — Regional Map Packet

---
type: region
secrecy: mixed
status: static
region: Sunmark
level_range: 8-13
related: [../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, ../FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../MAP_FEATURE_REGISTRY.md, ../../08_npcs/by_region/SUNMARK_NPCS.md, ../../09_quests/by_region/SUNMARK_QUESTS.md, ../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md, ../../10_dungeons_and_ruins/THE_SUNHOLLOW_GREAT_GROVE.md]
tags: [type:map, secrecy:mixed, function:cartography, map-packet, region-map, sunmark]
---

> **Secrecy classification:** Mixed. The Sunmark's living old faith is the campaign's hopeful contrast — a death-rite that *works*, because it was never touched by the Concord. Keep the groves' working EXTREMELY oblique; never explain it as the antithesis of the harvest or connect it to the keystone. The groves are NOT Concord, never a Concord node. No NPC here knows the apex truth. Never hand this file directly to the player; render only the Player-Safe Layer.

## Region: Sunmark (MF-017)

- **Local grid:** 0–100, where **(0,0) = NW corner of the region frame, X = east, Y = south** (Y=0 top). (100,100) = SE.
- **Full-continent bounds this local grid maps to:** render-grid **X 38–50, Y 75–85** (centroid full (44,80)); from `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §10`.
- **Local↔full transform:** `local_X = (full_X - 38) / 12 * 100`; `local_Y = (full_Y - 75) / 10 * 100`. (Inverse: `full_X = 38 + local_X/100*12`; `full_Y = 75 + local_Y/100*10`.)
- **One-sentence identity:** A warm southern land of sacred groves and grove-keeper tribes with a *living* old nature-faith — the campaign's most peaceful region, and a quiet proof that proper rites for the dead are still possible somewhere.

## Neighboring Regions

| Direction | Region |
|---|---|
| N | Marrowdowns (chalk-downs; the Ghostmark Range's SW foot) |
| NE | Sallowmarch Protectorate (the delta coast; NE edge of the Sunmark Wilds) |
| E | Hollow Gulf Ports (the Gulf coast begins E of the Sunmark Wilds) |
| W | the Sunmark Wilds extend to the western coast (beyond the frame; no named region) |
| S | the Calm Reach (warm open sea) |

## Terrain Zones (local polygons)

| Zone | Type | Local centroid | Full-grid | Description |
|---|---|---|---|---|
| The Sunmark Wilds (grove-heart) | warm sacred forest | (50,50) | (44,80) | The living old-faith groves; warm, lush, ancient. The heart of the campaign's hopeful contrast. |
| The Great Grove at Sunhollow | sacred grove-gathering heart | (50,50) | (44,80) | The grove-tribes' holy gathering-place; the D33 site; the faith's living center. |
| The Grove-Camps | dispersed grove-tribe settlements | (17,20) | (40,77) | The grove-keeper villages scattered through the wilds; the faith's daily life. |
| The Green Roads | pilgrimage-and-trade paths | (83,80) | (48,83) | The sacred walking-paths between groves; the route system of a living faith. |
| The coast-edge | warm SE coast | (75,90) | (47,84) | Where the Sunmark Wilds meet the Calm Reach; the southernmost groves. |

## Water Features

| Feature | Type | Local | Full-grid | Flow |
|---|---|---|---|---|
| Grove-springs | sacred spring-fed pools | scattered | — | Each major grove has a spring; sacred; travelers welcome to drink |
| Coast streams | warm seasonal streams | (75,80)→S edge | (47,83)→coast | Flow S to the Calm Reach |
| The Sunhollow Pool | sacred central pool (D33) | (50,50) | (44,80) | The faith's holiest water; where the dead are "properly sent"; D33 site |

## Roads / Routes (local polylines)

| Route | Local waypoints | Full-grid | Travel time | Notes |
|---|---|---|---|---|
| The Green Roads (main pilgrim-way) | (17,20) Grove-Camps → (50,50) Sunhollow → (83,80) Green Roads E | (40,77)→(44,80)→(48,83) | days (walking) | The living-faith route-system; safe for respectful travelers; marked by carved stones |
| The N Road (to Marrowdowns) | (50,50) Sunhollow → N edge | (44,80)→(44,75) Marrowdowns S | days–weeks | the route to the chalk-downs and the wider world |
| Coast track (E, to Gulf) | (83,80) → E edge | (48,83)→(50,84) Hollow Gulf W | days along the warm coast | the sea-route into the Gulf ports' world |

## Bridges / Fords / Ferries / Locks

| Feature | Type | Local | Full-grid | Notes |
|---|---|---|---|---|
| Sunhollow grove-ford | sacred crossing | (50,50) | (44,80) | The ford at the Great Grove; ceremonially important; not physically remarkable |
| Coast-landing | natural beach-landing | (75,90) | (47,84) | small-boat landing for coast-travellers arriving from the Gulf |

## Settlements

| Settlement | Type | Local | Full-grid | Anchor source / file |
|---|---|---|---|---|
| The Great Grove at Sunhollow | sacred gathering-place (hub; D33 anchor) | (50,50) | (44,80) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (su.sunhollow); NPC/quest hub; D33 |
| The Grove-Camps | dispersed grove-tribe settlements | (17,20) | (40,77) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (su.grove_camps); NPC/quest hub |
| The Green Roads | pilgrimage-and-trade route system (NOT a single settlement) | (83,80) | (48,83) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (su.green_roads); route label |

> The Great Grove at Sunhollow is a **sacred gathering-place and grove-heart**, not a town. The Grove-Camps are the region's actual daily-life settlements, dispersed through the wilds.

## Dungeons / Adventure Sites

| Site | Local | Full-grid | Surface marker | Player-map |
|---|---|---|---|---|
| D33 The Sunhollow Great Grove | (50,50) | (44,80) | the living grove-heart (sacred pool, ancient trees) | visible (label "the Great Grove at Sunhollow") |

> D33 is a **living sacred site**, not a Concord ruin. The grove works — its rites actually settle the dead. This is the campaign's hopeful contrast. Never connect it to the Concord harvest mechanism.

## Ruins / Wilderness Landmarks

| Landmark | Local | Full-grid | Notes |
|---|---|---|---|
| The Great Grove at Sunhollow (D33) | (50,50) | (44,80) | living old-faith grove-heart; working death-rites; Q_SUN_003/Q_SUN_007; oblique hopeful hint |
| The Oldest Grove | (20,30) | (40.4,78) | a specific ancient-tree cluster that pre-dates everything; Grove-Keeper Sael Sunmark's tending place |
| The Green Road Cairns | (83,80) | (48,83) | carved-stone route-markers throughout the Green Roads; the faith's map in stone |
| Cinder Ledger's Logging Camp | (70,30) | (46.4,78) | the contested site from Q_SUN_001; only present if the Ledger has moved in |

## Level Range And Solo Danger

- **Recommended level:** 8–13.
- **Expected solo danger:** Low to moderate throughout. The Sunmark is the campaign's safest far-region. The grove-tribes are peaceful and welcoming to respectful visitors. The only significant danger is from **outsider-brought conflict** (Ledger cutters, Ledger trade-lords, a crisis the player imported) and the oblique "far root-ache" of the crisis.
- **Lethal-at-low-level zones (telegraphed):** the **coast waters** (open-sea weather if the player attempts to sail without a guide) and **direct conflict with the full grove-tribes** (the tribes are peaceful but field significant numbers if driven to defense). Both are telegraphed clearly; the default is safety.
- **Telegraphing:** the grove-tribes' welcome is the default experience; threats are imported from outside; any violence against the groves provokes a clock (Q_SUN_007).

## Encounter And Hazard Mechanics

- **Encounter themes (stat references):** grove-keeper warriors (if the groves are threatened: **Tribal Warrior / Druid-like**, AC 13–15, ~22–37 HP; significant numbers; fight defensively); Ledger cutters and their guards (**Guard / Bandit-like**, AC 13–14); Sun-Singer Doll's grove-sight (not combat, but a presence that subtly unsettles those who come with ill-intent). Use `13_encounters_and_bestiary/` forest encounter lines.
- **Environmental hazards:** deep Sunmark Wilds (not hostile like the Hethewood — but pathless without a grove-keeper guide; Survival DC 13 to navigate; the wilds are warm and lush, not dangerous); coast-weather if sailing (Athletics/Vehicles DC 14).
- **Social DCs (typical):** Persuasion DC 16 (Plains-Factor Doss Sunward — logging negotiation); Persuasion DC 15 (Grove-Keeper Sael Sunmark — trust); Insight DC 15 (the grove-faith's significance); Persuasion DC 17 (the full grove-tribes — defense pact). Per-quest DCs in `SUNMARK_QUESTS.md`.
- **Scaling:** L8 — environmental defense and the Ledger logging-threat (Q_SUN_001). L13 — a grove clock at full depth, the Sunhollow Pool's significance, and the faintest oblique "root-ache" hint.

## Local Labels (player map)

The Sunmark (region label, ONE); the Sunmark Wilds (forest fill, warm green); the Great Grove at Sunhollow; the Grove-Camps; the Green Roads (route label); the Calm Reach (water, S edge); the N Road (route, N to Marrowdowns); the Coast Track (route, E to the Gulf).

## Player-Safe Layer

- Visible: the warm grove-forest, the Great Grove at Sunhollow as the central holy site, the Grove-Camps as the dispersed villages, the Green Roads as the living faith's route system, the warm coast S. The region reads as the campaign's most hopeful place — a people who still know how to properly tend the dead, because they were never inside the Concord's reach.
- Nothing here points to the Hollow Court or the keystone. The faith's working is presented as beautiful fact, not mechanism.

## DM-Only Layer (NEVER on the player map)

- D33 (The Sunhollow Great Grove) is a **living faith site** — the grove's rites actually settle the dead, because this faith was never compromised by the Concord's harvest. This is the campaign's strongest oblique hint of the "just" endgame path (restoring proper rites rather than destroying the harvest). Keep EXTREMELY oblique; never explain the mechanism; never connect to the keystone.
- Sun-Singer Doll perceives a **"far root-ache" in the southern sky** — an extremely-oblique, deniable far-echo of the Quiet Country thinning, felt through grove-cosmology with no framework to name it. Keep as mystical sensitivity only.
- The groves are **NOT Concord and never connect to the Concord harvest network**. Their working is precisely because they are *outside* the Concord's system.
- No apex geometry here. The endgame is vertical beneath Hollowmere (NW only).

## Unresolved Map Gaps

- The Grove-Camps are dispersed — their positions are illustrative anchors, not a definitive settlement map.
- The Sunmark Wilds extend W beyond the frame to the coast; that western coast is off-grid.
- The Sunhollow Pool's exact grove layout is revealed at D33.

## Related Files

- NPCs: [`../../08_npcs/by_region/SUNMARK_NPCS.md`](../../08_npcs/by_region/SUNMARK_NPCS.md)
- Quests: [`../../09_quests/by_region/SUNMARK_QUESTS.md`](../../09_quests/by_region/SUNMARK_QUESTS.md)
- D-site: [`../../10_dungeons_and_ruins/THE_SUNHOLLOW_GREAT_GROVE.md`](../../10_dungeons_and_ruins/THE_SUNHOLLOW_GREAT_GROVE.md)
- Authority: [`../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`](../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md) · [`../FULL_CONTINENT_SETTLEMENT_ANCHORS.md`](../FULL_CONTINENT_SETTLEMENT_ANCHORS.md) · [`../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
