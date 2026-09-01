# REGION_CONCORD_HEARTLANDS.md — Regional Map Packet

---
type: region
secrecy: mixed
status: static
region: Concord Heartlands
level_range: 13-17
related: [../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, ../FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../MAP_FEATURE_REGISTRY.md, ../../08_npcs/by_region/CONCORD_HEARTLANDS_NPCS.md, ../../09_quests/by_region/CONCORD_HEARTLANDS_QUESTS.md, ../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md, ../../10_dungeons_and_ruins/THE_OLD_CONCORD_HEARTLANDS_RUIN.md]
tags: [type:map, secrecy:mixed, function:cartography, map-packet, region-map, concord-heartlands, ruind-crown]
---

> **Secrecy classification:** Mixed — CRITICAL. This is the Concord's *surface* fallen-capital country. It is **NOT** the Concord Deep (the buried harvest-network), **NOT** the Under-Shrine / Drowned Keystone beneath Hollowmere, and **NOT** the Hollow Court's seat. The Heartlands corroborate the theme (Concord grandeur and fall) but are **NEVER** the live mechanism. The Crown's deepest secret is a *record of what the Concord did*, not the living machine. Hollin Vane is a dupe — never let him confirm the Court or keystone. The endgame is **vertical beneath Hollowmere, NW only.** Never hand this file directly to the player; render only the Player-Safe Layer.

## Region: Concord Heartlands / Ruin'd Crown (MF-015)

- **Local grid:** 0–100, where **(0,0) = NW corner of the region frame, X = east, Y = south** (Y=0 top). (100,100) = SE.
- **Full-continent bounds this local grid maps to:** render-grid **X 58–66, Y 52–60** (centroid full (62,56)); from `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §10`.
- **Local↔full transform:** `local_X = (full_X - 58) / 8 * 100`; `local_Y = (full_Y - 52) / 8 * 100`. (Inverse: `full_X = 58 + local_X/100*8`; `full_Y = 52 + local_Y/100*8`.)
- **One-sentence identity:** The shattered surface heart of the old Custodian Concord — an enormous contested ruin astride the Greatspine, where every faction scrambles for records and relics, and no one knows what the Concord *actually did*.

## Neighboring Regions

| Direction | Region |
|---|---|
| N / NW | Glassmere League (across the Greatspine's N slopes; Crown Road) |
| W | Marrowdowns (chalk-downs; Greatspine W foot) |
| SW | Saltmere Reaches (across the Ghostmark foothills) |
| E | Hethewald Free Holds (across the Greatspine's E flank) |
| SE | Emberfell Theocracy (across the Cindern margins) |

## Terrain Zones (local polygons)

| Zone | Type | Local centroid | Full-grid | Description |
|---|---|---|---|---|
| The Ruin'd Crown | vast surface-ruin complex | (50,50) | (62,56) | The shattered Concord capital — collapsed halls, broken roads, crumbling towers; the D21 site. |
| The Greatspine ridge | continental cordillera | (30,30) | (60.4,54.4) | The backbone of Orrun running NW–SE; passes, altitude, cold winds. |
| The Crownmouth margin | safe ruin-edge ground | (25,25) | (60,54) | The only defended ground at the Crown's edge; Crownmouth's perimeter. |
| The Pilgrim wastelands | refugee/relic-seeker scrubland | (63,75) | (63,58) | The open scrubland where the Pilgrim Camps squat at the ruin's S fringe. |
| The Crown's deep interior | completely unsafe ruin-heart | (70,40) | (63.6,55.2) | Where the halls still stand, the dead still walk, and the records still burn. |

## Water Features

| Feature | Type | Local | Full-grid | Flow |
|---|---|---|---|---|
| Greatspine melt-streams | seasonal mountain streams | (30,30)→(50,60) | (60.4,54.4)→(62,56.8) | Flow W (to Glassmere) and E (to Hethewald); no major river within the ruin |
| Crown cisterns | broken Concord waterworks | (50,50) | (62,56) | Dry or fouled; water is a tactical concern inside the ruin |

## Roads / Routes (local polylines)

| Route | Local waypoints | Full-grid | Travel time | Notes |
|---|---|---|---|---|
| The Crown Road (W, to Glassmere) | W edge → (25,25) Crownmouth → (50,50) ruin edge | (58,54)→(60,54)→(62,56) | Glassmere→Crownmouth ~2–3 weeks | Main approach; well-traveled to Crownmouth, then abandoned |
| The Greatspine Passes (N, to Glassmere) | (30,30) pass-top → N edge | (60.4,54.4)→(60.4,52) | days (high altitude) | Faster N route; dangerous altitude; contested |
| Pilgrim Road (S, to Saltmere) | (63,75) camps → S edge | (63,58)→(63,60) Saltmere N | days | Faction-contested; pilgrim-and-scavenger route |
| Eastern Track (E, to Hethewald) | (50,50) → E edge | (62,56)→(66,56) | weeks (dangerous) | Poorly mapped; most travelers don't attempt it alone |

## Bridges / Fords / Ferries / Locks

| Feature | Type | Local | Full-grid | Notes |
|---|---|---|---|---|
| Crownmouth defense-gate | fortified town gate | (25,25) | (60,54) | The only defended crossing into the safe zone; Lyssa Crownmouth's ward |
| Crown Road ford | seasonal stream-ford | (15,28) | (59.2,54.2) | Broken Concord bridge abutments still visible; main road ford |

## Settlements

| Settlement | Type | Local | Full-grid | Anchor source / file |
|---|---|---|---|---|
| Crownmouth | fortified scavenger-town (only safe ground) | (25,25) | (60,54) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (ch.crownmouth); NPC/quest hub |
| The Pilgrim Camps | refugee/relic-seeker shanty-camps | (63,75) | (63,58) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (ch.pilgrim_camps); NPC/quest hub |

> Crownmouth is the **only functioning settlement** in this region. The Pilgrim Camps are temporary, sprawling, and dangerous.

## Dungeons / Adventure Sites

| Site | Local | Full-grid | Surface marker | Player-map |
|---|---|---|---|---|
| D21 The Old Concord Heartlands Ruin (Ruin'd Crown) | (50,50) | (62,56) | collapsed Concord halls, broken towers (surface-visible) | visible (label "the Ruin'd Crown") |

> **CRITICAL:** D21 is a *surface ruin* — the shattered ground-level Concord capital. It is NOT the Concord Deep, NOT the keystone, NOT the Under-Shrine. Hollin Vane's deepest find is a *record* of the harvest, not the machine.

## Ruins / Wilderness Landmarks

| Landmark | Local | Full-grid | Notes |
|---|---|---|---|
| The Ruin'd Crown (D21) | (50,50) | (62,56) | shattered Concord capital; factional scramble; M2/M5/M6-oblique records only |
| The Concord Spire-stump | (55,35) | (62.4,54.8) | a single enormous broken tower; landmark visible for miles; dangerous interior |
| The Sealed Road-Hall | (40,55) | (61.2,56.4) | a Concord relay-hall still structurally intact; last seen sealed; Q_CH_003 |
| "Old Crown" Mab's Waypoint | (30,20) | (60.4,53.6) | the deep-ruin guide's staging-camp; the only reliable interior base |

## Level Range And Solo Danger

- **Recommended level:** 13–17. **This is a late-game destination only.**
- **Expected solo danger:** High to extreme throughout. Crownmouth itself: dangerous (politics, scavenging feuds). Ruin proper: high-danger. Deep Crown interior: extreme.
- **Lethal-at-low-level zones (telegraphed):** the **Crown's deep interior** (CR 13–17+ undead and constructs, unstable structures, ancient traps) and the **Greatspine passes** (altitude, cold, territorial disputes). Telegraphed by Crownmouth's town-legends ("no one comes back from the deep"), "Old Crown" Mab's explicit refusals, and visible scavenger-dead from the safe perimeter.
- **Telegraphing:** Crownmouth is the mandatory on-ramp (Q_CH_001); the ruin's danger is constant and stated (Lyssa Crownmouth names threat zones); going deeper requires a guide, preparation, and faction trust.

## Encounter And Hazard Mechanics

- **Encounter themes (stat references):** Crown undead guardians (**Wight / Wraith / Revenant / Death Knight-like**, CR 8–17, scale by D21 depth); construct remnants (**Animated Armor / Shield Guardian / Golem-like**, CR 7–14, Concord-made); rival faction expeditions (**Veteran / Champion-like**, AC 16–18, ~84–104 HP; Remnant, Ledger, Emberfell agents); Pilgrim Camps scavengers (**Scout / Bandit-like**, AC 12–13). Use `13_encounters_and_bestiary/` undead and construct lines at Tier 3–4.
- **Environmental hazards:** structural collapse (Dexterity DC 14–16, 4d6–6d6 bludgeoning; telegraphed by cracking stone); altitude cold in the Greatspine (Constitution DC 13–15, exhaustion risk); cursed-relic exposure (Thin-touch at depth, DC 17 concentration saves); Crown-side political danger (attacking a Remnant expedition brings retaliation).
- **Social DCs (typical):** Persuasion DC 17 (Warden Lyssa Crownmouth — trust/defense); Persuasion DC 17 (Hollin Vane — Remnant access); Insight DC 18 (Hollin Vane's dupe-status — he believes everything he found is the full truth); Persuasion DC 16 (Father Casian Ord — Pilgrim Camps). Per-quest DCs in `CONCORD_HEARTLANDS_QUESTS.md`.
- **Scaling:** L13 — Crownmouth defense and near-ruin access (Q_CH_001). L17 — deep Crown interior, the Sealed Road-Hall, and the record-vaults that confirm what the Concord did (never the living machine; the machine is elsewhere).

## Local Labels (player map)

The Concord Heartlands (region label, ONE); the Ruin'd Crown (ruin cluster, dominant label); Crownmouth; the Pilgrim Camps; the Greatspine (mountain range feature); the Crown Road (route label, W to Glassmere); the Greatspine Passes (route, N); Pilgrim Road (route, S).

## Player-Safe Layer

- Visible: the enormous ruin-complex, Crownmouth at its edge, the Pilgrim Camps at the S fringe, the Greatspine cutting through, factional expeditions everywhere. The region reads as the campaign's most grandly ruined setting — the Concord at its height, now smashed and contested.
- The ruin is presented as the Concord's surface seat — its fall explains why the world is as it is. Nothing here points to the *nature* of the harvest or the Hollow Court.

## DM-Only Layer (NEVER on the player map)

- D21's deepest record-vault holds a **partial history of the harvest** — what the Concord did, in the Concord's own Script. This is **M6-adjacent lore**, not M9. It confirms the harvest happened; it does not confirm the Hollow Court survived or where the machine is.
- Hollin Vane is an **apex-adjacent dupe** — he believes the records he found are the truth of everything. He has never read the keystone's location. He cannot; it is vertical beneath Hollowmere, not here.
- The Heartlands contain **no surviving Hollow Court presence** — the Court abandoned the surface capital at the Quietfall. The ruin's emptiness of the Court is itself a clue for a thorough player.
- No apex geometry here. The endgame is vertical beneath Hollowmere (NW only).

## Unresolved Map Gaps

- The Ruin'd Crown's internal district-layout is in D21 (`THE_OLD_CONCORD_HEARTLANDS_RUIN.md`); this packet positions the complex.
- The Greatspine's exact elevation and individual pass positions are approximate.
- The Pilgrim Camps' exact position shifts as factions claim and abandon sections.

## Related Files

- NPCs: [`../../08_npcs/by_region/CONCORD_HEARTLANDS_NPCS.md`](../../08_npcs/by_region/CONCORD_HEARTLANDS_NPCS.md)
- Quests: [`../../09_quests/by_region/CONCORD_HEARTLANDS_QUESTS.md`](../../09_quests/by_region/CONCORD_HEARTLANDS_QUESTS.md)
- D-site: [`../../10_dungeons_and_ruins/THE_OLD_CONCORD_HEARTLANDS_RUIN.md`](../../10_dungeons_and_ruins/THE_OLD_CONCORD_HEARTLANDS_RUIN.md)
- Authority: [`../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`](../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md) · [`../FULL_CONTINENT_SETTLEMENT_ANCHORS.md`](../FULL_CONTINENT_SETTLEMENT_ANCHORS.md) · [`../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
