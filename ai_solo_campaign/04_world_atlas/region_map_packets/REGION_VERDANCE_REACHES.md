# REGION_VERDANCE_REACHES.md — Regional Map Packet

---
type: region
secrecy: mixed
status: static
region: Verdance Reaches
level_range: 8-12
related: [../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, ../FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../MAP_FEATURE_REGISTRY.md, ../../08_npcs/by_region/VERDANCE_REACHES_NPCS.md, ../../09_quests/by_region/VERDANCE_REACHES_QUESTS.md, ../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md, ../../10_dungeons_and_ruins/THE_NINE_LOCKS_SUNKEN_STAIR.md]
tags: [type:map, secrecy:mixed, function:cartography, map-packet, region-map, verdance-reaches]
---

> **Secrecy classification:** Mixed. The Nine Locks Sunken Stair is a minor Concord relay/water-node fragment that *points home* toward the NW keystone — it is NEVER the keystone, the machine, the Concord Deep, or the Hollow Court seat. Those stay vertical beneath Hollowmere (NW only). Never hand this file directly to the player; render only the Player-Safe Layer.

## Region: Verdance Reaches (MF-006)

- **Local grid:** 0–100, where **(0,0) = NW corner of the region frame, X = east, Y = south** (Y=0 top). (100,100) = SE.
- **Full-continent bounds this local grid maps to:** render-grid **X 38–48, Y 38–48** (centroid full (42,42)); from `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §10`.
- **Local↔full transform:** `local_X = (full_X - 38) / 10 * 100`; `local_Y = (full_Y - 38) / 10 * 100`. (Inverse: `full_X = 38 + local_X/100*10`; `full_Y = 38 + local_Y/100*10`.)
- **One-sentence identity:** The river-road corridor up the Verdance past Caradril — locks, wharves, and barge-villages where the cold frontier gives way to the older, richer, more settled inland Orrun, and where the death-rite crisis is *just beginning* to be noticed up-river.

## Neighboring Regions

| Direction | Region |
|---|---|
| NW (down-river) | Caradril (city-state hinterland) → the NW campaign cluster |
| SE (up-river) | Glassmere League |
| S | Marrowdowns |
| NE | (Greatspine foothills toward the Concord Heartlands, far) |

## Terrain Zones (local polygons)

| Zone | Type | Local centroid | Full-grid | Description |
|---|---|---|---|---|
| The Verdance corridor (river-bottom) | settled river valley | (45,45) | (42.5,42.5) | Tilled bottomland, wharves, lock-towns, willow-banks; the lived-in spine of the region. |
| The Stair shelf (up-river terraces) | terraced farmland | (30,30) | (41,41) | Stepped fields and orchards rising from the river around Marrowfen Stair; prosperous, lock-fed. |
| The Marrowfen edge (down-river fen) | wet meadow / sink-fen | (15,75) | (39.5,45.5) | Reedy half-bog where the corridor sheds toward the Mirewend Sinks and Marrowdowns; Cresswater sits on its dry margin. |
| The Wend uplands (NE bluffs) | low wooded bluffs | (75,12) | (45.5,39.2) | Drier hill-shoulders above Lord's Wend; vineyards, the lord's hunting-wood. |
| The drowned reaches (river ruins) | flooded old works | (52,52) | (43.2,43.2) | Stretches where old Concord causeways and lock-works lie half-sunk; barge hazards. |

## Water Features

| Feature | Type | Local | Full-grid | Flow |
|---|---|---|---|---|
| The Verdance (river) | navigable river | corridor diagonal | source (48,46)→Caradril (34,35) | flows NW (down to Caradril/Stillwater, then Pale Sea); barges climb SE to up-river |
| The Nine Locks pool | lock-staircase reach | (50,50) | (43,43) | the great staircase that lifts barges up the corridor's main fall |
| Marrowfen sink-water | sink-fen standing water | (15,75) | (39.5,45.5) | sluggish; drains S toward the Mirewend Sinks |
| Lock-chambers (drowned) | flooded Concord works | (52,52) | (43.2,43.2) | still, "wrong" water at the failing locks |

## Roads / Routes (local polylines)

| Route | Local waypoints | Full-grid | Travel time | Notes |
|---|---|---|---|---|
| Verdance Road (river-and-towpath corridor) | down-river edge → (30,30) Marrowfen Stair → (50,50) Nine Locks → (70,10) Lord's Wend approach → up-river SE edge | (34,35) Caradril → (41,41) Stair → (43,43) Locks → (55,50) Glassmere | Caradril→Glassmere ~12–16 days by road; ~2 weeks by barge if "the locks behave and the lord's paid" | the corridor; both a towpath road and the navigable river |
| The Verdance (barge route) | follows the river through (30,30)→(50,50) locks→SE | as river above | barge faster than road when water is good | Mossa Drenn's barge-trains run it |
| Cresswater branch-track | (50,50) Locks → (10,70) Cresswater | (43,43)→(39,45) | ~1 day | down-river fen landing; the free ferry crossing |
| Overland parallel road | runs the dry bluffs N of the river (Doss Frome's caravan road) | parallels Verdance Road, drier ground | slightly slower, toll-free of river-tolls | avoids the lock-tolls; favored by teamsters |

## Bridges / Fords / Ferries / Locks

| Feature | Type | Local | Full-grid | Notes |
|---|---|---|---|---|
| The Nine Locks | lock-staircase + toll | (50,50) | (43,43) | the corridor chokepoint; Lord Marrow taxes every barge that climbs; D34 vault beneath |
| Marrowfen Stair locks | stepped lock-town | (30,30) | (41,41) | the hub's own working locks and wharves; Ledger toll-house |
| Mab Cress's free ferry | small free ferry | (10,70) | (39,45) | at Cresswater; the poor's crossing the toll-lords want to tax (Q_VR_007) |
| Lord's Wend river-gate | toll/landing | (70,10) | (45,39) | Lord Marrow's hall-town landing |

## Settlements

| Settlement | Type | Local | Full-grid | Anchor source / file |
|---|---|---|---|---|
| Marrowfen Stair | town (corridor hub) | (30,30) | (41,41) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (vr.marrowfen_stair); NPC/quest hub |
| Lord's Wend | town (lord's hall-town) | (70,10) | (45,39) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (vr.lords_wend) |
| Cresswater | barge-village / river landing | (10,70) | (39,45) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (vr.cresswater) |

> These are **light NPC-facing anchors**, not deep-built gazetteers (per the anchor file). Local micro-geography within each is improv-safe.

## Dungeons / Adventure Sites

| Site | Local | Full-grid | Surface marker | Player-map |
|---|---|---|---|---|
| D34 The Nine Locks Sunken Stair | (50,50) | (43,43) | the Nine Locks lock-staircase (locks visible; sunken relay-vault stair beneath) | label-only (locks visible as a landmark) |

## Ruins / Wilderness Landmarks

| Landmark | Local | Full-grid | Notes |
|---|---|---|---|
| The drowned lock-chambers | (52,52) | (43.2,43.2) | "wrong" flooded Concord works at/near the Nine Locks (Q_VR_001 node-corroboration; M2 inland) |
| The bad-water stretches | scattered along the river | varies | river reaches where rites have failed and the dead "come up wrong" (Q_VR_004; M5 inland spread) |
| Lord Marrow's old hall-archive | (70,10) | (45,39) | pre-corridor records Hadwin Vael covets (Q_VR_001 reward) |

## Level Range And Solo Danger

- **Recommended level:** 8–12 (Ring 2; the player's first true step into the wider continent).
- **Expected solo danger:** Low–moderate overall. The corridor is *settled* — most danger is social/political (debt-vises, Ledger–League pressure, toll-lords) rather than monstrous.
- **Lethal-at-low-level zones (telegraphed):** the drowned lock-chambers and bad-water stretches host **waking Concord node-manifestations** (telegraphed by humming works, "wrong" still water, failed rites, fish leaving). A solo PC under ~L8 should not enter a manifesting chamber. River-pirate ambushes (Eel Maddox) are toll-not-murder by nature and avoidable.
- **Telegraphing:** locals warn off "bad water"; lockmasters speak of works "going wrong"; Mourners' rites visibly slip. No node fight is unsignaled.

## Encounter And Hazard Mechanics

- **Encounter themes (stat references):** river-pirate crews (**Bandit/Scout-like**, AC 13) and a leader (**Veteran-like**); Ledger enforcers/auditors and a noble household guard (**Guard-like**, with a **Veteran-like** captain — see `FACTION_TURN_RULES.md` and `13_encounters_and_bestiary/` faction-capability profiles); waking node-manifestations at drowned works (scale a **Memory-Echo Haunt / drowned-dead** profile from `SUNDERING_REACH_ENCOUNTERS.md` up to L8–12). Use `13_encounters_and_bestiary/VERDANCE_REACHES_ENCOUNTERS.md` and `13_encounters_and_bestiary/TRAVEL_ENCOUNTERS.md` for generic river-corridor lines.
- **Environmental hazards:** "wrong" still water near a manifesting node — exposure to raw Remembrance works may inflict **Thin-touch** (Stage 3 custom condition; disadvantage on Death saves until a true rite / shrine long-rest). Flood/strong-current stretches: Athletics/Vehicles(water) DC 15 to navigate; failed lock-passage DC 15 (Survival/Vehicles).
- **Investigation/social DCs (typical):** Investigation DC 16 (the works' wrongness, true debt-books); Persuasion/Insight DC 16–17 (Marrow, Crane, creditors); History/Arcana DC 17 (Concord works — oblique). See the quest file for per-quest DCs.
- **Scaling:** L8 — a single contained node, debt-politics. L11–12 — an active corridor-wide barge crisis and a Ledger–League proxy conflict over the locks.

## Local Labels (player map)

The Verdance Reaches; Marrowfen Stair; Lord's Wend; Cresswater; the Verdance (river); the Verdance Road; the Nine Locks; the Marrowfen edge (fen); the free ferry crossing. Mark the Nine Locks as a visible landmark and label nearby drowned-works stretches only as hazard ("old works — bad water").

## Player-Safe Layer

- Visible: the three anchor settlements, the Verdance and its corridor road, the Nine Locks as a landmark, the free ferry crossing, the Marrowfen fen-edge, the up-river / down-river framing.
- Telegraph the drowned lock-chambers and "bad-water" stretches as **dangerous and unexplained** ("the works have gone wrong"; "bad water — the dead come up wrong") without naming any node, network, or depth.

## DM-Only Layer (NEVER on the player map)

- The Nine Locks Sunken Stair (D34) is a **minor Concord water/relay-node fragment** whose stirrings *corroborate that the crisis is spreading up-river* (M2/M5 inland). It POINTS toward the NW keystone; it is **never** the keystone, the machine, the Concord Deep, or the Hollow Court.
- The "bad water" is the maritime/freshwater harvest-leak reaching inland — kept oblique (M5/M6); never explain the mechanism here.
- Factor-General Crane's quiet **divestment** of down-river relic positions (he may abandon the Reach) is DM strategic content, not a map feature.
- No apex geometry exists in this region. The endgame is vertical beneath Hollowmere (NW only).

## Unresolved Map Gaps

- Internal micro-geography of each anchor town (street layouts) is improv-safe; only the corridor spine, three anchors, and the locks are fixed.
- Exact courses of the "bad-water" stretches are illustrative (place along the river as play demands); the *fact* of the up-river spread is canon.
- The NE upland bluffs and the S transition to the Marrowdowns/Mirewend Sinks are loosely bounded.

## Related Files

- NPCs: [`../../08_npcs/by_region/VERDANCE_REACHES_NPCS.md`](../../08_npcs/by_region/VERDANCE_REACHES_NPCS.md)
- Quests: [`../../09_quests/by_region/VERDANCE_REACHES_QUESTS.md`](../../09_quests/by_region/VERDANCE_REACHES_QUESTS.md)
- D-site: [`../../10_dungeons_and_ruins/THE_NINE_LOCKS_SUNKEN_STAIR.md`](../../10_dungeons_and_ruins/THE_NINE_LOCKS_SUNKEN_STAIR.md)
- Authority: [`../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`](../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md) · [`../FULL_CONTINENT_SETTLEMENT_ANCHORS.md`](../FULL_CONTINENT_SETTLEMENT_ANCHORS.md) · [`../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
