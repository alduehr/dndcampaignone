# REGION_HETHEWALD_FREE_HOLDS.md — Regional Map Packet

---
type: region
secrecy: mixed
status: static
region: Hethewald Free Holds
level_range: 7-12
related: [../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, ../FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../MAP_FEATURE_REGISTRY.md, ../../08_npcs/by_region/HETHEWALD_FREE_HOLDS_NPCS.md, ../../09_quests/by_region/HETHEWALD_FREE_HOLDS_QUESTS.md, ../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md, ../../10_dungeons_and_ruins/THE_HETHEWALD_OLD_HOLDS.md]
tags: [type:map, secrecy:mixed, function:cartography, map-packet, region-map, hethewald]
---

> **Secrecy classification:** Mixed. The Old Holds are surface-Concord ruins, NOT the keystone, NOT the Concord Deep, NOT the Hollow Court's seat. The forest's "failing bargains" read as a pagan cousin of the campaign crisis but are never named as the harvest. Never hand this file directly to the player; render only the Player-Safe Layer.

## Region: Hethewald Free Holds (MF-016)

- **Local grid:** 0–100, where **(0,0) = NW corner of the region frame, X = east, Y = south** (Y=0 top). (100,100) = SE.
- **Full-continent bounds this local grid maps to:** render-grid **X 66–78, Y 34–46** (centroid full (72,40)); from `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §10`.
- **Local↔full transform:** `local_X = (full_X - 66) / 12 * 100`; `local_Y = (full_Y - 34) / 12 * 100`. (Inverse: `full_X = 66 + local_X/100*12`; `full_Y = 34 + local_Y/100*12`.)
- **One-sentence identity:** Tollwood writ large — a great dark forest of free-holds, river-tollers, and outlaws, where old pagan bargains with the wood are failing and deep Concord ruins fester in the forbidden interior.

## Neighboring Regions

| Direction | Region |
|---|---|
| N | Karran Marches (across the forest's NE edge) |
| NW | Wender Steppe (open steppe begins where the Hethewood thins, N) |
| W | open country toward the Greatspine / Verdance Reaches |
| SW | Concord Heartlands / Glassmere League approaches |
| S | Concord Heartlands (via the forest's S edge) |
| E | Karran Marches / the Karran Teeth |

## Terrain Zones (local polygons)

| Zone | Type | Local centroid | Full-grid | Description |
|---|---|---|---|---|
| The Hethewood heart | great dark forest | (50,50) | (72,40) | The campaign's largest forest; old-growth, pagan, barely mapped in the interior. |
| The Hethemoot clearing | great gathering free-hold | (42,42) | (71,39) | The only open ground for the full confederacy moot; ancient and politically contested. |
| The Greenward grove | sacred grove-village | (17,75) | (68,43) | The old-faith forest heart; Onn Greenward's seat; where the bargains are thinnest. |
| Tollreach river-cut | outlaw toll-hold on the Hethe | (75,25) | (75,37) | The Hethe river's toll-point; "Greenfinger" Maddoc's extortion ground. |
| The Old Holds (forbidden) | deep-forbidden Concord ruin-cluster | (67,83) | (74,44) | The interior ruins the free-holds forbid outsiders from entering; the dead stir; D25. |
| The forest edge (W) | thinning forest / transition | (10,30) | (67.2,37.6) | Where the Hethewood gives way to the Greatspine foothills and the road-country. |

## Water Features

| Feature | Type | Local | Full-grid | Flow |
|---|---|---|---|---|
| The Hethe | major river (running S) | (75,25)→S edge | (75,37)→(75,46) | Flows S to the Calm Reach; the region's main waterway; barge-navigable in the lower reaches |
| Greenward stream | spring-fed forest stream | (17,75) | (68,43) | Feeds the Greenward grove; sacred to the forest-faith |
| Forest-tarns | scattered peat-black pools | scattered | — | Navigation markers for guides; the dead stir near several |

## Roads / Routes (local polylines)

| Route | Local waypoints | Full-grid | Travel time | Notes |
|---|---|---|---|---|
| The Hold-Road (W edge entry) | W edge → (42,42) Hethemoot | (66,37.6)→(71,39) | 2–4 days | Main outsider entry; contested at the forest edge by Maddoc's tollers |
| The River-Road (Hethe, N–S) | N edge → (75,25) Tollreach → S edge | (75,34)→(75,37)→(75,46) | weeks end-to-end | Fast N–S route; Maddoc's toll blocks access without payment or bypass |
| Greenward Path | (42,42) Hethemoot → (17,75) Greenward | (71,39)→(68,43) | 2–3 days (guided only) | The faith-path; requires wood's-law welcome; unmarked to outsiders |
| Old Holds track (forbidden) | (42,42) Hethemoot → (67,83) Old Holds | (71,39)→(74,44) | 3–5 days (deep forest) | The free-holds try to keep it closed; the deep wood is hostile without a guide |

## Bridges / Fords / Ferries / Locks

| Feature | Type | Local | Full-grid | Notes |
|---|---|---|---|---|
| Tollreach river-crossing | extortion toll-bridge | (75,25) | (75,37) | Maddoc's force controls it; toll or fight; bypassable by deep-wood ford (Survival DC 16) |
| Hethemoot log-bridge | free-holds great-moot crossing | (42,42) | (71,39) | Open during moots; the confederacy's neutral ground |
| Greenward ford | sacred ford | (17,75) | (68,43) | Passable freely for those with wood's-law welcome |

## Settlements

| Settlement | Type | Local | Full-grid | Anchor source / file |
|---|---|---|---|---|
| Hethemoot | great gathering free-hold (hub) | (42,42) | (71,39) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (hfw.hethemoot); NPC/quest hub |
| Greenward | sacred grove-village | (17,75) | (68,43) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (hfw.greenward); NPC/quest hub |
| Tollreach | outlaw river-toll camp | (75,25) | (75,37) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (hfw.tollreach) |
| The Old Holds | deep-wood Concord ruin-cluster (D25 — NOT a live settlement) | (67,83) | (74,44) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (hfw.old_holds); D25 dungeon anchor |

> The Old Holds are a **forbidden ruin-cluster** in the deep forest — not a settlement. The free-holds kept outsiders away for a generation.

## Dungeons / Adventure Sites

| Site | Local | Full-grid | Surface marker | Player-map |
|---|---|---|---|---|
| D25 The Hethewald Old Holds | (67,83) | (74,44) | crumbling ruins visible through the canopy (broken towers, vine-choked gates) | visible (label "the Old Holds"; annotated "forbidden") |

## Ruins / Wilderness Landmarks

| Landmark | Local | Full-grid | Notes |
|---|---|---|---|
| The Old Holds (D25) | (67,83) | (74,44) | deep-wood Concord ruins; the dead stir; Q_HFH_004/007; M2/M5-oblique |
| The Mark-Trees | (42,30) | (71,37.6) | enormous old-growth oaks marking the inner wood's law-boundary; the real border |
| The Mast-Beast Range | (60,55) | (73.2,40.6) | the deep forest's apex-predator country; the wood's natural deterrent to deep travel |
| "Greenfinger" Maddoc's Toll-Gate | (75,25) | (75,37) | the extortion-bridge; visible, known, politically contested (Q_HFH_002) |

## Level Range And Solo Danger

- **Recommended level:** 7–12.
- **Expected solo danger:** Moderate on the Hold-Road and at Hethemoot (politics, social); high in the deep wood (predators, outlaws, failing bargains); extreme at the Old Holds (undead + Concord constructs at D25).
- **Lethal-at-low-level zones (telegraphed):** the **Mast-Beast range** (predators that stalk alone; telegraphed by stripped bones and the free-holds' avoidance), the **Old Holds** (gated behind Q_HFH_007 and Mab's explicit warnings), and **Maddoc's toll-fight** if attempted without preparation. All are telegraphed by the forest's own warning systems — the free-holds tell every outsider what to avoid.
- **Telegraphing:** the on-ramp is the wood's-law challenge (Q_HFH_001); earning welcome explicitly unlocks safe paths and names the dangerous ones; the Old Holds' interdiction is public, visible, and stated free-hold law.

## Encounter And Hazard Mechanics

- **Encounter themes (stat references):** free-hold warriors (**Tribal Warrior / Veteran-like**, AC 13–15, ~37–52 HP; the moot fields a substantial force); Maddoc's river-bandits (**Bandit / Spy-like**, AC 13–14, ~16–22 HP; motivated by profit, turnable); deep-forest predators (**Mast-Beast-like**: use Owlbear statistics as baseline, +1 CR, stealthy); Old Holds undead (**Skeleton / Wight / Revenant-like**, CR 4–11 scale by D25 depth). Use `13_encounters_and_bestiary/` forest and undead encounter lines.
- **Environmental hazards:** deep wood's disorientation (Survival DC 15 without a guide); Mast-Beast territory (Perception DC 14 for advance warning; Stealth DC 15 to avoid); Old Holds ruin-collapse (Dexterity DC 14, 3d6 bludgeoning); Thin-touch at D25 unshielded relics.
- **Social DCs (typical):** Persuasion DC 16 (Hold-Speaker Bram Hethe — wood's-law welcome); Persuasion DC 16 (Maddoc — toll negotiation, turnable); Insight DC 15 (Onn Greenward's bargain-failure knowledge); Persuasion DC 18 (the Moot's full vote — Q_HFH_006). Per-quest DCs in `HETHEWALD_FREE_HOLDS_QUESTS.md`.
- **Scaling:** L7 — wood's-law on-ramp and the river-toll (Q_HFH_001/002). L12 — the failing bargains at full depth, the Old Holds (D25), and the moot's vote on the confederacy's future (Q_MAJOR_027).

## Local Labels (player map)

The Hethewald Free Holds (region label, ONE); the Hethewood (forest fill); Hethemoot; Greenward; Tollreach; the Old Holds (ruin marker, "forbidden"); the Hethe (river, label on water); the Hold-Road; the River-Road; the Mast-Beast Range (terrain annotation).

## Player-Safe Layer

- Visible: the great dark forest, Hethemoot as the clearing-hub, the Greenward grove as a sacred sub-destination, Tollreach as the contested toll-bridge, the Old Holds as a visible but interdicted ruin. The region reads as Tollwood at continental scale — beautiful, ancient, politically complex, with a dangerous interior.
- The "failing bargains" are presented as a forest-religion concern (the groves are quiet, the old rites are weak) — never named as the campaign crisis.

## DM-Only Layer (NEVER on the player map)

- The Old Holds (D25) are **surface-Concord ruins** — their stirring dead and "wrong" resonance are M2/M5-oblique echoes of the crisis reaching the E forest, not the keystone.
- Forest-Mother Onn Greenward's failing bargains articulate the crisis as **"the old dead are not going where they go"** — a pagan rendering of the Quiet Country thinning; NEVER name the harvest or Hollow Court; keep it as forest-faith.
- No apex geometry here. The endgame is vertical beneath Hollowmere (NW only).

## Unresolved Map Gaps

- The Hethewood's interior track-network is intentionally unmapped; outsiders need guides.
- Individual free-hold villages are numerous but unnamed; they feed into Hethemoot.
- The Old Holds' interior complexity is covered in D25 (`THE_HETHEWALD_OLD_HOLDS.md`); this packet positions the site.

## Related Files

- NPCs: [`../../08_npcs/by_region/HETHEWALD_FREE_HOLDS_NPCS.md`](../../08_npcs/by_region/HETHEWALD_FREE_HOLDS_NPCS.md)
- Quests: [`../../09_quests/by_region/HETHEWALD_FREE_HOLDS_QUESTS.md`](../../09_quests/by_region/HETHEWALD_FREE_HOLDS_QUESTS.md)
- D-site: [`../../10_dungeons_and_ruins/THE_HETHEWALD_OLD_HOLDS.md`](../../10_dungeons_and_ruins/THE_HETHEWALD_OLD_HOLDS.md)
- Authority: [`../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`](../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md) · [`../FULL_CONTINENT_SETTLEMENT_ANCHORS.md`](../FULL_CONTINENT_SETTLEMENT_ANCHORS.md) · [`../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
