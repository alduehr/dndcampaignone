# REGION_KARRAN_MARCHES.md — Regional Map Packet

---
type: region
secrecy: mixed
status: static
region: Karran Marches
level_range: 9-14
related: [../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, ../FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../MAP_FEATURE_REGISTRY.md, ../../08_npcs/by_region/KARRAN_MARCHES_NPCS.md, ../../09_quests/by_region/KARRAN_MARCHES_QUESTS.md, ../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md, ../../10_dungeons_and_ruins/THE_KARRAN_OLD_IRON_FORTS.md]
tags: [type:map, secrecy:mixed, function:cartography, map-packet, region-map, karran-marches]
---

> **Secrecy classification:** Mixed. The Old Iron forts are thin, peripheral Concord ruins — their stirring dead corroborate the crisis through a brutal mining-frontier lens but are NEVER the keystone, the Concord Deep, or the Hollow Court's seat. Never hand this file directly to the player; render only the Player-Safe Layer.

## Region: Karran Marches (MF-013)

- **Local grid:** 0–100, where **(0,0) = NW corner of the region frame, X = east, Y = south** (Y=0 top). (100,100) = SE.
- **Full-continent bounds this local grid maps to:** render-grid **X 70–80, Y 14–24** (centroid full (75,19)); from `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §10`.
- **Local↔full transform:** `local_X = (full_X - 70) / 10 * 100`; `local_Y = (full_Y - 14) / 10 * 100`. (Inverse: `full_X = 70 + local_X/100*10`; `full_Y = 14 + local_Y/100*10`.)
- **One-sentence identity:** A second, harsher frontier mirroring the Sundering Reach — cold stone, mines, petty-warlord holds, the rule of the strong, and peripheral Concord ruins whose stirring dead the warlords simply call "bad ground."

## Neighboring Regions

| Direction | Region |
|---|---|
| W | Wender Steppe (the steppe begins where the Karran Teeth's W foot opens) |
| SW | Hethewald Free Holds (the forest begins S of the Karran Teeth) |
| S | Hethewald Free Holds |
| SE | Emberfell Theocracy (across the Karran Teeth's SE approach) |
| N / NE | the Karran Teeth (mountain barrier) / Sunder Ocean (off-grid) |
| E | off-grid (beyond the Karran Teeth; the campaign's NE limit) |

## Terrain Zones (local polygons)

| Zone | Type | Local centroid | Full-grid | Description |
|---|---|---|---|---|
| Brask's Hold territory | petty-warlord frontier hold | (30,30) | (73,17) | The largest fortress-hold in the Marches; "Iron" Brask's domain; cold stone and iron discipline. |
| Karran-Gate environs | mining-and-mercenary hub | (60,60) | (76,20) | The closest thing to a neutral town; ore-factor Mully Karr's ground. |
| The Deep Cuts | great ore-mine complex | (10,70) | (71,21) | The richest mines in the Marches; also where the ground "went wrong" (Q_KM_001). |
| The Old Iron forts | scattered peripheral Concord ruins | (80,10) | (78,15) | The NE fringe's crumbling Concord road-forts; the source of the "old iron" problem. |
| The Karran Teeth | mountain barrier (N/NE) | (60,10) | (76,15) | The great NE range; cold, sheer, barely passable; marks the campaign's NE limit. |

## Water Features

| Feature | Type | Local | Full-grid | Flow |
|---|---|---|---|---|
| Karran mountain streams | cold fast streams (Teeth melt) | scattered (N edge) | — | Flow S toward the Hethewood; too small for navigation; useful for fresh water |
| Mine-sump drainage | seep-water from the Deep Cuts | (10,70) | (71,21) | The brine-tainted mine drainage; "tasted wrong" before the ground went wrong |

## Roads / Routes (local polylines)

| Route | Local waypoints | Full-grid | Travel time | Notes |
|---|---|---|---|---|
| The Iron Road (S–N, main) | S edge → (60,60) Karran-Gate → (30,30) Brask's Hold | (75,24)→(76,20)→(73,17) | weeks end-to-end | The Marches' main route; toll-demanded by Brask; partially paved Concord stone |
| Deep Cuts Access Road | (60,60) Karran-Gate → (10,70) Deep Cuts | (76,20)→(71,21) | days | Brask's controlled mining-road; no passage without his permit |
| Old Forts Track (NE) | (30,30) Brask's Hold → (80,10) Old Iron forts | (73,17)→(78,15) | weeks (dangerous) | Concord-era road remnants; partially passable; the dead increase as you approach the forts |
| Teeth Pass (N, out) | (50,0) N edge → off-grid | (75,14) | weeks (near impassable) | The campaign's NE limit; extreme cold and altitude; the Sunder Ocean is beyond |

## Bridges / Fords / Ferries / Locks

| Feature | Type | Local | Full-grid | Notes |
|---|---|---|---|---|
| Brask's Hold gate | fortified hold gate | (30,30) | (73,17) | Toll demanded for road transit; Brask personally inspects outsiders of note |
| Karran-Gate's toll-post | commercial toll-point | (60,60) | (76,20) | The ore-factor's toll; market prices for information; bribable |
| Mountain fords | rocky stream-crossings | scattered (N) | — | Cold and fast in spring; the only water-crossings in the Teeth approach |

## Settlements

| Settlement | Type | Local | Full-grid | Anchor source / file |
|---|---|---|---|---|
| Brask's Hold | petty-warlord fortress-town (hub) | (30,30) | (73,17) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (km.braskshold); NPC/quest hub |
| Karran-Gate | mining-and-mercenary town | (60,60) | (76,20) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (km.karrangate) |
| The Deep Cuts | great ore-mine complex (D27 anchor, NOT a true settlement) | (10,70) | (71,21) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (km.deep_cuts); D27 dungeon anchor |
| The Old Iron forts | scattered Concord ruin-forts (NOT a live settlement) | (80,10) | (78,15) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (km.old_iron_forts); D27 site; ruin-cluster |

> The Deep Cuts and the Old Iron forts are **operational/ruin-cluster anchors**, not settlements with permanent populations.

## Dungeons / Adventure Sites

| Site | Local | Full-grid | Surface marker | Player-map |
|---|---|---|---|---|
| D27 The Karran Old Iron Forts | (80,10) | (78,15) | crumbling Concord road-forts (broken walls, old iron gates visible) | visible (label "the Old Iron forts") |

> The Deep Cuts mine complex also feeds D27 — its "gone-wrong" deep gallery cuts into the Old Iron fort system. See `THE_KARRAN_OLD_IRON_FORTS.md`.

## Ruins / Wilderness Landmarks

| Landmark | Local | Full-grid | Notes |
|---|---|---|---|
| The Old Iron forts (D27) | (80,10) | (78,15) | peripheral Concord road-forts; the dead stir; Q_KM_001/005; M2/M5-oblique |
| The Karran-Gate relic-dump | (60,60) | (76,20) | a pile of "old iron" salvage Mully Karr sells; thin-touch risk to buyers |
| The Spine-Watch Tower | (50,10) | (75,15) | a half-standing Concord watch-tower above the Karran-Gate; scouts the Teeth passes |
| "Cold" Coll's Warning-Post | (10,65) | (71,20.5) | a marker-post left by a mine-mad digger; readable with a Language or Insight DC 17 |

## Level Range And Solo Danger

- **Recommended level:** 9–14.
- **Expected solo danger:** High throughout. The Karran Marches has no safe ground except behind Brask's or Karran-Gate's walls; the frontier is actively hostile. Every NPC here has a price and no sentimental attachments.
- **Lethal-at-low-level zones (telegraphed):** the **Deep Cuts' "gone-wrong" gallery** (D27 depth; stirring dead, Thin-touch risk; telegraphed by Brask's sealed door and the diggers' shaking hands), the **Old Iron forts** (active undead + Concord constructs; telegraphed by the forts' reputation and the Spine-Watch Tower scout's report), and **Brask's Hold without his permission** (armed force response). All are telegraphed explicitly by the warlord's own self-interested warnings.
- **Telegraphing:** Karran-Gate is the commercial on-ramp (Q_KM_001); Brask explicitly tells outsiders what is safe (his road, his rules); the mine's danger is described by shaking, changed diggers before the player commits.

## Encounter And Hazard Mechanics

- **Encounter themes (stat references):** warlord soldiers (**Guard / Veteran / Champion-like**, AC 14–16, ~44–84 HP; heavily armed frontier troops); mine-workers and mercenaries (**Scout / Bandit-like**, AC 12–13; motivated by coin); Old Iron fort undead and constructs (**Wight / Revenant / Animated Armor-like**, CR 5–12 scale by D27 depth). Warlord "Iron" Brask is **Tier 1** (Champion/Veteran stat profile, AC 18, ~104 HP, paired weapons, heavy armor). Use `13_encounters_and_bestiary/` plains/undead/construct lines at L9+.
- **Environmental hazards:** Karran winter (Constitution DC 13–15, exhaustion; the Teeth approach is extreme cold); Thin-touch from "old iron" relic contact at the mine/forts (the Stage 3 condition); mine collapse (Dexterity DC 14, 3d6–4d6 bludgeoning); the "mine-mad" condition from prolonged Thin-touch exposure (narrative: the digger comes back wrong; mechanically escalating Thin-touch).
- **Social DCs (typical):** Persuasion DC 16 ("Iron" Brask — employment/access); Persuasion DC 16 (Mully Karr — ore-trade/information); Persuasion DC 17 (Wenna Stone — Remnant turnable; her trust is earned through competence); Insight DC 16 (Brask's real fear: the ground going wrong under him). Per-quest DCs in `KARRAN_MARCHES_QUESTS.md`.
- **Scaling:** L9 — mine-clearance on-ramp (Q_KM_001). L14 — the Old Iron forts at full depth (D27), the Remnant expedition (Wenna Stone), and the "old iron" spreading into the warlord-holds' water.

## Local Labels (player map)

The Karran Marches (region label, ONE); the Karran Teeth (mountain range feature); Brask's Hold; Karran-Gate; the Deep Cuts (mine label); the Old Iron forts (ruin marker); the Iron Road; the Deep Cuts Road; the Old Forts Track (route, NE); the Teeth Pass (route, N; label "near impassable").

## Player-Safe Layer

- Visible: the great mountain barrier, the warlord fortress-town, the mining hub, the mine complex, the crumbling Concord forts. The region reads as a harsh northern frontier — the rule of the strong, iron discipline, and "bad ground" that nobody wants to talk about too closely.
- The "old iron" problem is presented as a frontier hazard (bad mine ground, dead walking) — never as the campaign's central crisis.

## DM-Only Layer (NEVER on the player map)

- The Old Iron forts (D27) are **peripheral Concord ruins** — their stirring dead and "old iron" hum are M2/M5-oblique echoes of the harvest's NE reach; NEVER the keystone, NEVER the machine. The Karran warlords frame it as "bad ground" and that framing is accurate at their level of knowledge.
- Wenna Stone (Remnant Reclaimer-Captain) is **turnable** — the only NPC here who might connect the "old iron" to the Concord properly; she knows it is Concord-origin but not why it is stirring. She is apex-adjacent the hard way (expedition-soldier, not scholar).
- No apex geometry here. The endgame is vertical beneath Hollowmere (NW only).

## Unresolved Map Gaps

- The Karran Teeth's interior passes are approximate; individual passes are not individually named.
- The Old Iron forts' site-layout is covered in D27 (`THE_KARRAN_OLD_IRON_FORTS.md`); this packet positions the cluster.
- The region beyond the Karran Teeth (N/NE) is off-grid and intentionally blank.

## Related Files

- NPCs: [`../../08_npcs/by_region/KARRAN_MARCHES_NPCS.md`](../../08_npcs/by_region/KARRAN_MARCHES_NPCS.md)
- Quests: [`../../09_quests/by_region/KARRAN_MARCHES_QUESTS.md`](../../09_quests/by_region/KARRAN_MARCHES_QUESTS.md)
- D-site: [`../../10_dungeons_and_ruins/THE_KARRAN_OLD_IRON_FORTS.md`](../../10_dungeons_and_ruins/THE_KARRAN_OLD_IRON_FORTS.md)
- Authority: [`../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`](../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md) · [`../FULL_CONTINENT_SETTLEMENT_ANCHORS.md`](../FULL_CONTINENT_SETTLEMENT_ANCHORS.md) · [`../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
