# REGION_WENDER_STEPPE.md — Regional Map Packet

---
type: region
secrecy: mixed
status: static
region: Wender Steppe
level_range: 8-13
related: [../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, ../FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../MAP_FEATURE_REGISTRY.md, ../../08_npcs/by_region/WENDER_STEPPE_NPCS.md, ../../09_quests/by_region/WENDER_STEPPE_QUESTS.md, ../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md, ../../10_dungeons_and_ruins/THE_WENDER_SKY_STONES.md]
tags: [type:map, secrecy:mixed, function:cartography, map-packet, region-map, wender-steppe]
---

> **Secrecy classification:** Mixed. The Sky-Stones are an **independent steppe holy site, NOT Concord** — they "hum" by their own old nature and the seers perceive a "thinning sky" (an extremely-oblique cosmic far-echo of the Quiet Country thinning); they are NEVER a Concord node, the keystone, the machine, or the Hollow Court (NW only, vertical beneath Hollowmere). Render ONE region label. Never hand this file directly to the player; render only the Player-Safe Layer.

## Region: Wender Steppe (MF-012)

- **Local grid:** 0–100, where **(0,0) = NW corner of the region frame, X = east, Y = south** (Y=0 top). (100,100) = SE.
- **Full-continent bounds this local grid maps to:** render-grid **X 40–55, Y 12–22** (centroid full (46,16)); from `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §10`.
- **Local↔full transform:** `local_X = (full_X - 40) / 15 * 100`; `local_Y = (full_Y - 12) / 10 * 100`. (Inverse: `full_X = 40 + local_X/100*15`; `full_Y = 12 + local_Y/100*10`.)
- **One-sentence identity:** A cold open grass-sea ridden by free horse-clans the Concord never tamed — a people outside the Concord's whole history, to whom the death-rite crisis is a foreign "settled-folk's sickness" and a "thinning of the southern Sky" their seers read with dread but no understanding.

> **Level note:** the authored NPC/quest content sets this region at **Lvl 8–13**; this packet follows the authored content and flags that the original build-brief suggested "6–10."

## Neighboring Regions

| Direction | Region |
|---|---|
| W | the Highmark Spine / Highmark Passes (cluster's far-N edge) |
| E | Karran Marches |
| S | the Greatspine's N end → central Orrun (the Spine-Foot trade-meet) |
| N | the Sunder Ocean (beyond the Spine) |

## Terrain Zones (local polygons)

| Zone | Type | Local centroid | Full-grid | Description |
|---|---|---|---|---|
| The long grass (open steppe) | cold grass-sea | (50,50) | (47.5,17) | The trackless heart; the migrating clans' country; deadly to the unguided. |
| The Cold Springs basin | watered winter-ground | (33,40) | (45,16) | Spring-fed wintering ground; the largest cold-season gathering. |
| The Sky-Stones rise | ancient shrine-upland | (13,20) | (42,14) | A low rise crowned by the independent steppe shrine-circle; the seers' vigil. |
| The Spine-Foot margin | steppe/settled border | (67,80) | (50,20) | Where the grass meets the Greatspine's foot; the neutral trade-meet. |
| The far steppe | deep ungoverned grass | (85,55) | (52.75,17.5) | Raider country; the Black Horse clan's range. |

## Water Features

| Feature | Type | Local | Full-grid | Flow |
|---|---|---|---|---|
| Cold Springs | spring-fed water-ground | (33,40) | (45,16) | the reliable winter-water; reason for the great gathering |
| Steppe water-holes | scattered seasonal wells | scattered | — | the survival-craft; dowsed by water-finders |

> The steppe has **no major river** within the frame; the Highmark Spine to the W and the Greatspine to the S shed seasonal melt into the grass.

## Roads / Routes (local polylines)

| Route | Local waypoints | Full-grid | Travel time | Notes |
|---|---|---|---|---|
| Steppe Tracks | (33,40) Cold Springs → (67,80) Spine-Foot → S edge | (45,16)→(50,20)→(55,40) central Orrun | weeks; ungoverned, seasonal | the only "roads" — migration and trade tracks |
| The Summer-Riding (migration) | the clan-host's seasonal circuit across the grass | shifts seasonally | the host moves with the grazing | not a fixed line — the clans themselves on the move |
| Spine-Foot trade-road (out, to settled) | (67,80) Spine-Foot → S edge | (50,20) → Greatspine foot | days to the settled lands | the bridge between two worlds (Q_WS_005) |

## Bridges / Fords / Ferries / Locks

| Feature | Type | Local | Full-grid | Notes |
|---|---|---|---|---|
| Spine-Foot trade-meet ground | neutral trade-ground | (67,80) | (50,20) | the one fixed meeting-place; guest-truce holds here |
| Steppe water-holes / fords | seasonal crossings | scattered | — | known only to clan water-finders and guides |

## Settlements

| Settlement | Type | Local | Full-grid | Anchor source / file |
|---|---|---|---|---|
| The Winter-Camp at Cold Springs | seasonal gathering-camp (hub) | (33,40) | (45,16) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (ws.cold_springs); NPC/quest hub |
| The Spine-Foot trade-meet | steppe/settled trade-ground | (67,80) | (50,20) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (ws.spine_foot) |

> These are **seasonal/mobile anchors**, not fixed towns; the clans migrate. The Summer-Riding is the clan-host on the move and has no fixed marker.

## Dungeons / Adventure Sites

| Site | Local | Full-grid | Surface marker | Player-map |
|---|---|---|---|---|
| D25 The Wender Sky-Stones | (13,20) | (42,14) | a standing-stone circle (independent steppe shrine, NON-Concord) | visible (standing stones) |

> **Authority note:** the build-brief cited "D25 Wender Sky-Stones (42,14)"; the `ADVENTURE_SITE_CARTOGRAPHY_INDEX.md` master table confirms **D32 The Wender Sky-Stones (42,14)** (D25 is the Hethewald Old Holds). This packet uses the authority index's **D32**. Flagged to the coordinating agent.

## Ruins / Wilderness Landmarks

| Landmark | Local | Full-grid | Notes |
|---|---|---|---|
| The Sky-Stones | (13,20) | (42,14) | ancient independent steppe shrine-circle; "hums strange" of late; the seers' vigil (Q_WS_003; oblique cosmic echo) |
| Lone clan-cairns | scattered | — | clan-riders' grave-cairns on the open grass (steppe death-custom; NO Concord) |

## Level Range And Solo Danger

- **Recommended level:** 8–13.
- **Expected solo danger:** Moderate–high, almost entirely environmental and martial. The open steppe itself is the killer (cold, distance, no water); mounted raiders are the martial threat.
- **Lethal-at-low-level zones (telegraphed):** the **trackless open grass** (death by exposure/thirst without a guide) and **Raid-Lord Borr's far-steppe range** (deadly mounted cavalry). Telegraphed by the universal warning that "the steppe kills the unguided" and by raiders' visible approach. Guest-law, once earned, makes the clans protectors.
- **Telegraphing:** the steppe's lethality is the central on-ramp lesson (Q_WS_001); a guide ("Cold" Esha-Mor) is the explicit safety valve; mounted raids are seen coming across open ground.

## Encounter And Hazard Mechanics

- **Encounter themes (stat references):** mounted clan-warriors and raiders (**Scout / Veteran / Berserker-like**, mounted; Clan-Speaker Tamur and Raid-Lord Borr are **Tier 1** chieftains, AC 15–16, ~80–90 HP, with mounted hosts); steppe predators (wolves/great cats — use `13_encounters_and_bestiary/` plains lines). Combat on open grass favors cavalry — a solo PC on foot is badly exposed; the clans' riders are the counter once allied.
- **Environmental hazards:** exposure/cold (Constitution save DC 13–15 on prolonged unguided travel); thirst/navigation on the trackless grass (Survival DC 16, far worse without a guide); the Sky-Stones "hum" (an eerie, non-mechanical effect — Insight/Religion DC 17 to read the omen; no Thin-touch, no Concord relic here).
- **Social DCs (typical):** Persuasion DC 16 (guest-law, the Speaker, Wind-Sai); Persuasion/Intimidation DC 18 (Raid-Lord Borr); Insight DC 16–17 (the feuds, the omen). See the quest file for per-quest DCs.
- **Scaling:** L8 — guest-law and the steppe-edge. L13 — a confederacy fracture, a mounted raid-war, and the deepening "thinning sky" vigil.

## Local Labels (player map)

The Wender Steppe (ONE region+terrain label — never a "(steppe)" suffix); the Winter-Camp at Cold Springs; the Spine-Foot trade-meet; the Sky-Stones; the Steppe Tracks. Mark the Sky-Stones as a standing-stone circle.

## Player-Safe Layer

- Visible: the seasonal winter-camp, the trade-meet, the standing-stone circle, the steppe tracks, one faint grass-green region fill.
- Frame the steppe as **free, foreign, and deadly to the unprepared** ("the long grass answers to no crown"; "the steppe kills the unguided"). The Sky-Stones are an ancient holy site that "hums strange," presented as steppe mystery, never as a Concord work.

## DM-Only Layer (NEVER on the player map)

- The Sky-Stones (D32) are an **independent steppe holy site, NOT Concord** — never a node, never the keystone. They "hum" by their own old nature.
- Wind-Singer Esha perceives the crisis as **"a thinning of the southern Sky, something pulling at the dead"** — an extremely-oblique, deniable far-echo of the **Quiet Country thinning** (the harvest's deepest consequence), reached through steppe-cosmology with no framework to name it. Keep EXTREMELY oblique; never name the harvest, the Quiet Country, or the Court.
- The steppe-clans are **outside the Concord's whole history** — no Concord ruins, no harvest, no rites here; the crisis is foreign to them. This is the campaign's deliberate "outside view."
- No apex geometry exists here. The endgame is vertical beneath Hollowmere (NW only).

## Unresolved Map Gaps

- The clans **migrate**: the Winter-Camp and Summer-Riding positions are illustrative cold-season/seasonal anchors, not fixed settlements; the Summer-Riding is intentionally a moving host with no marker.
- Water-holes and the far-steppe raider range are diffuse by design (the trackless grass is meant to be unmapped).
- The N edge against the Sunder Ocean and the W edge against the Highmark Spine are loosely bounded.

## Related Files

- NPCs: [`../../08_npcs/by_region/WENDER_STEPPE_NPCS.md`](../../08_npcs/by_region/WENDER_STEPPE_NPCS.md)
- Quests: [`../../09_quests/by_region/WENDER_STEPPE_QUESTS.md`](../../09_quests/by_region/WENDER_STEPPE_QUESTS.md)
- D-site: [`../../10_dungeons_and_ruins/THE_WENDER_SKY_STONES.md`](../../10_dungeons_and_ruins/THE_WENDER_SKY_STONES.md)
- Authority: [`../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`](../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md) · [`../FULL_CONTINENT_SETTLEMENT_ANCHORS.md`](../FULL_CONTINENT_SETTLEMENT_ANCHORS.md) · [`../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
