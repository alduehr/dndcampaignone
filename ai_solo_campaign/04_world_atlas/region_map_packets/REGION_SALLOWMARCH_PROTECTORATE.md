# REGION_SALLOWMARCH_PROTECTORATE.md — Regional Map Packet

---
type: region
secrecy: mixed
status: static
region: Sallowmarch Protectorate
level_range: 10-14
related: [../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, ../FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../MAP_FEATURE_REGISTRY.md, ../../08_npcs/by_region/SALLOWMARCH_PROTECTORATE_NPCS.md, ../../09_quests/by_region/SALLOWMARCH_PROTECTORATE_QUESTS.md, ../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md, ../../10_dungeons_and_ruins/THE_SALLOWMARCH_DROWNED_STEPS.md]
tags: [type:map, secrecy:mixed, function:cartography, map-packet, region-map, sallowmarch]
---

> **Secrecy classification:** Mixed. The Drowned Steps are a peripheral pre-Concord / Concord sea-causeway echo — a far-south corroboration of the crisis's reach, NEVER the keystone, the machine, the Concord Deep, or the Hollow Court (NW only, vertical beneath Hollowmere). Never hand this file directly to the player; render only the Player-Safe Layer.

## Region: Sallowmarch Protectorate (MF-010)

- **Local grid:** 0–100, where **(0,0) = NW corner of the region frame, X = east, Y = south** (Y=0 top). (100,100) = SE.
- **Full-continent bounds this local grid maps to:** render-grid **X 53–63, Y 80–88** (centroid full (58,84)); from `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §10`.
- **Local↔full transform:** `local_X = (full_X - 53) / 10 * 100`; `local_Y = (full_Y - 80) / 8 * 100`. (Inverse: `full_X = 53 + local_X/100*10`; `full_Y = 80 + local_Y/100*8`.)
- **One-sentence identity:** A fever-ridden delta of rice, reed, and smuggling at the Mardenflow's mouth, held under the cold, tolerated rule of an absent southern crown — foreign occupation laid over a marsh-people who endure it, smuggle around it, and outlast it.

> **Level note:** the authored NPC/quest content sets this region at **Lvl 10–14** (a deep-south, fever-and-occupation region). The original build-brief suggested "7–11"; this packet follows the authored content (10–14) per predetermined-first and flags the discrepancy.

## Neighboring Regions

| Direction | Region |
|---|---|
| N | Marrowdowns (the Mardenflow flows down from there) |
| W | Sunmark |
| E | Hollow Gulf Ports |
| S | the Calm Reach / Hollow Gulf (delta coast, the Drowned Steps offshore) |

## Terrain Zones (local polygons)

| Zone | Type | Local centroid | Full-grid | Description |
|---|---|---|---|---|
| The Sallow Marches | deltaic wetland | (50,50) | (58,84) | The splayed Mardenflow delta; reed, mud, fever-mist; the region's defining wet country. |
| The Rice Sallows | flooded paddy-country | (20,75) | (55,86) | Worked rice-paddies; the paddy-folk's villages; the delta's food and labor. |
| The garrison shelf (Fenward) | drained delta-edge | (40,25) | (57,82) | The driest, most defensible ground; the crown's garrison-capital. |
| The Fever Channels | deep delta backwaters | (70,87.5) | (60,87) | Lethal, shifting backwaters the crown's boats can't follow; smuggler country. |
| The delta-edge / tidal flats | tidal mudflats | (10,95) | (53.5,87.6) | Where the delta meets the sea; the Drowned Steps lie offshore beyond. |

## Water Features

| Feature | Type | Local | Full-grid | Flow |
|---|---|---|---|---|
| The Mardenflow (delta) | river splaying to delta | enters NW, splays S | (52,64) source → (58,84) delta → (65,92) Hollow Gulf | tidal at the delta; floods seasonally |
| The Fever Channels | deep tidal backwaters | (70,87.5) | (60,87) | shifting; "some go strange" (Q_SP_002/006) |
| The Rice Sallows | flooded paddies | (20,75) | (55,86) | standing paddy-water, leech-and-fever |

## Roads / Routes (local polylines)

| Route | Local waypoints | Full-grid | Travel time | Notes |
|---|---|---|---|---|
| The Mardenflow river-road | NW edge → (40,25) Fenward → S delta | (52,64)→(58,84)→(65,92) Gulf | days through fever-country | the spine; barge + tidal |
| Delta tracks & ferries | between Fenward, Reedmouth, the paddies | within frame | slow, fever-slowed | the only land-links; cut by flood |
| The Fever Channels (smuggler ways) | hidden, through (70,87.5) | (60,87) | only Heron Maddox's pilots run them | crown boats can't follow |
| The delta-road (out, to the dry interior) | (40,25) Fenward → NW edge | toward Marrowdowns | days north | the land-link to the dry uplands |

## Bridges / Fords / Ferries / Locks

| Feature | Type | Local | Full-grid | Notes |
|---|---|---|---|---|
| Fenward garrison-causeway | drained causeway / gate | (40,25) | (57,82) | the crown's defensible approach to the capital |
| Reedmouth channel-ferries | smuggler ferries | (70,62.5) | (60,85) | the smuggling-village's hidden crossings |
| Rice-paddy dykes | earthwork dykes | (20,75) | (55,86) | the paddy-folk's water-control; flood-prone |

## Settlements

| Settlement | Type | Local | Full-grid | Anchor source / file |
|---|---|---|---|---|
| Fenward | town (garrison-capital hub) | (40,25) | (57,82) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (sm.fenward); NPC/quest hub |
| Reedmouth | delta smuggling-village | (70,62.5) | (60,85) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (sm.reedmouth) |
| The Rice Sallows | paddy-country waterway node | (20,75) | (55,86) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (sm.rice_sallows) |

> The Fever Channels are a **diffuse non-rendered area-label** (terrain texture, no point marker — per the anchor file Table 3), not a settlement.

## Dungeons / Adventure Sites

| Site | Local | Full-grid | Surface marker | Player-map |
|---|---|---|---|---|
| D30 The Sallowmarch Drowned Steps | (10,125) offshore (off-frame S) | (54,90) | drowned causeway steps at low tide (offshore) | label-only ("drowned steps") |

> **Authority note (resolved 2026-06-18, Cartography Determinism Cleanup):** the `ADVENTURE_SITE_CARTOGRAPHY_INDEX.md` master table (and `DUNGEON_INDEX.md`, `RUIN_INDEX.md`, `MAP_FEATURE_REGISTRY.md`, `CLUE_INDEX.md`) assign the Sallowmarch Drowned Steps **D30** at full-grid (54,90); **D26** is the Marrowdowns Barrow Complex and **D33** is the Sunhollow Great Grove. An earlier packet edit incorrectly "corrected" this to D33 in the wrong direction; the master index is authoritative and this packet now uses **D30**. The site sits **offshore, south of the region frame** (full Y=90 > the frame's Y 80–88), so its local-Y projects below 100 — render it as an offshore tidal landmark below the delta coast.

## Ruins / Wilderness Landmarks

| Landmark | Local | Full-grid | Notes |
|---|---|---|---|
| The Drowned Steps | offshore S | (54,90) | submerged tidal causeway; a far-south "drowned ground" (Q_SP_006; M2/M5-oblique) |
| Deep-delta "drowned grounds" | (70,90) | (60,87.5) | half-sunken ruins the fen-witches warn against (Q_SP_006) |
| Delta water-shrines | scattered | — | Mother Sela Reed's fen-Mourner shrines to the drowned dead |

## Level Range And Solo Danger

- **Recommended level:** 10–14.
- **Expected solo danger:** Moderate–high. The delta itself is the danger: fever (Constitution saves), lethal shifting channels, and an armed (if fever-thinned) imperial garrison.
- **Lethal-at-low-level zones (telegraphed):** the **Fever Channels** and the deep "drowned grounds" / Drowned Steps are high-danger — telegraphed by the fen-witches' warnings ("drowned ground, best left"), shifting water, and the fever's grim toll. A solo PC should travel the Channels only with Heron Maddox's pilots.
- **Telegraphing:** the delta's lethality is foregrounded constantly (fever, leech-water, "bad water" hideouts); the garrison's response is cold but slow and fever-weakened, giving room to bargain or flee into the marsh.

## Encounter And Hazard Mechanics

- **Encounter themes (stat references):** crown soldiers / garrison (**Guard / Veteran-like**, AC 16, fever-weakened — see faction-capability profiles); delta smugglers (**Bandit / Scout-like**, AC 13–15; "Heron" Maddox is a **Scout/Assassin-like** ambusher, AC 15 ~48 HP); marsh predators (use `13_encounters_and_bestiary/` swamp lines); a rare "won't-go-down" Remembrance manifestation and drowned-dead at the deep ruins (scale **drowned-dead / Memory-Echo** profiles to L11–14, AC 11). Use `13_encounters_and_bestiary/SALLOWMARCH_ENCOUNTERS.md` and `13_encounters_and_bestiary/TRAVEL_ENCOUNTERS.md` for generic delta/swamp lines.
- **Environmental hazards:** marsh-fever (Constitution save DC 13–15 on prolonged exposure; Doll Fenn's craft mitigates); shifting Fever Channels (Survival DC 16–17 to navigate without a pilot); tidal/flood windows; raw relic exposure at the drowned grounds may inflict **Thin-touch** (Stage 3 condition).
- **Social/investigation DCs (typical):** Persuasion DC 16 (Vorr Sallow, the moots); Insight DC 16 (delta defiance); Medicine DC 16–17 (the "new sickness"); Investigation DC 17 (vanishing revenue). See the quest file for per-quest DCs.
- **Scaling:** L10 — a village dispute, a contained outbreak. L14 — an occupation flashpoint, a delta-wide plague, and the deep "drowned ground" at full danger.

## Local Labels (player map)

The Sallowmarch Protectorate (faint); the Sallow Marches (terrain); Fenward; Reedmouth; the Rice Sallows; the Mardenflow delta; the Drowned Steps (offshore, label-only). The Fever Channels appear only as terrain texture, not a marked place.

## Player-Safe Layer

- Visible: the three anchor settlements, the Mardenflow delta, the rice-paddy country, the garrison-capital, the Drowned Steps as an offshore submerged-ruin landmark.
- Telegraph the delta as **fever-dangerous and lawless-deep** ("the fen keeps its own"; "drowned ground, best left") and the occupation as a cold, resented imperial presence — without explaining any node, network, or depth.

## DM-Only Layer (NEVER on the player map)

- The Drowned Steps (D30) and the deep "drowned grounds" are **peripheral pre-Concord / Concord sea-works** (M2/M5-oblique) — far-south corroboration that the crisis reaches even here; NEVER the keystone, the machine, or the Concord Deep.
- The "new sickness" (the dead "not settling") is the crisis reaching the deep south, masked by the fever's death-familiarity (M5, far-south faintest) — Doll Fenn (medicine) and Sela Reed (rite) are the twin early-witnesses; never explain the mechanism.
- Mother Sela Reed carries the **old-songs network fragment** ("the grey hands took the dead"), fused with delta water-lore — M6-oblique folk-memory ONLY; no mechanism, no Court, no keystone.
- The distant southern crown (Vorr Sallow) is a world-scale foreign power; strategic/world content, not a map secret.
- No apex geometry exists here. The endgame is vertical beneath Hollowmere (NW only).

## Unresolved Map Gaps

- Delta channel geometry is **diffuse by design** (terrain texture, not point markers); the Fever Channels shift and are intentionally unmapped.
- The Drowned Steps' exact offshore position (full (54,90)) is LOW confidence; render below the delta coast.
- Internal layouts of Fenward/Reedmouth are improv-safe.

## Related Files

- NPCs: [`../../08_npcs/by_region/SALLOWMARCH_PROTECTORATE_NPCS.md`](../../08_npcs/by_region/SALLOWMARCH_PROTECTORATE_NPCS.md)
- Quests: [`../../09_quests/by_region/SALLOWMARCH_PROTECTORATE_QUESTS.md`](../../09_quests/by_region/SALLOWMARCH_PROTECTORATE_QUESTS.md)
- D-site: [`../../10_dungeons_and_ruins/THE_SALLOWMARCH_DROWNED_STEPS.md`](../../10_dungeons_and_ruins/THE_SALLOWMARCH_DROWNED_STEPS.md)
- Authority: [`../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`](../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md) · [`../FULL_CONTINENT_SETTLEMENT_ANCHORS.md`](../FULL_CONTINENT_SETTLEMENT_ANCHORS.md) · [`../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
