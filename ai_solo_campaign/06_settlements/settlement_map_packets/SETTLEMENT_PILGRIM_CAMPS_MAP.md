# SETTLEMENT_PILGRIM_CAMPS_MAP.md — Settlement Map Packet

---
type: settlement
secrecy: mixed
status: static
region: Concord Heartlands
settlement: The Pilgrim Camps
level_range: 12-17
related: [../../04_world_atlas/region_map_packets/REGION_CONCORD_HEARTLANDS.md, ../../04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../../08_npcs/by_region/CONCORD_HEARTLANDS_NPCS.md, ../../09_quests/by_region/CONCORD_HEARTLANDS_QUESTS.md]
tags: [type:map, secrecy:mixed, function:cartography, settlement-map, map-packet, pilgrim-camps, concord-heartlands]
---

> **Secrecy classification:** Mixed. The Pilgrim Camps are a refugee-and-relic-seeker shanty-camp at the ruin's edge. Father Casian Ord's presence is M6-oblique. The ruin beyond is surface-only. Never hand directly to the player; render only the Player-Safe Layer.

## Settlement: The Pilgrim Camps (Concord Heartlands — refugee/relic-seeker shanty-camps)

- **Local grid:** 0–100 (X east, Y south); (0,0) = NW corner. A dispersed sprawl of camps and rough shelters around a central clearing; Father Ord's tent at the center; the ruin-edge visible to the E.
- **Full-continent position:** render-grid (63,58).
- **Population / scale:** ~300–600 shifting; a mix of refugees from collapsed Heartlands villages, relic-seekers, desperate pilgrims, and Remnant scholars. People arrive and leave constantly.
- **Water/road relationship:** in the Concord Heartlands, near the ruin's outer edge; **Crownmouth** is NW (60,54; days by road); the **Pilgrim Road** leads SW (toward the Saltmere approaches; weeks); the **Ruin-Road** leads E (immediately into D21 territory; dangerous).

## Layout / Notable Areas

| Area | Local | Notes |
|---|---|---|
| Father Ord's Tent | (45,40) | the camp's moral center; heretic-priest; the reliable social hub |
| The Salvage-Market | (60,50) | relic-trade and food-barter; informal and dangerous |
| The Remnant Scholars' Tents | (35,55) | Hollin Vane's expedition camp; more organized than the rest |
| The Refuge-Quarter | (25,65) | displaced families from fallen villages; the most desperate area |
| The Ruin-Road head | (80,50) | where the road into D21 begins; scouts and scavengers go in here |
| The Watch-Fire | (50,70) | the only shared light at night; communal safety point |

## Entrances / Exits

| Exit | Local edge | Leads to |
|---|---|---|
| Crownmouth Road (NW) | (0,35) | Crownmouth (60,54; days) |
| Pilgrim Road (SW) | (0,75) | Saltmere approaches / broader Orrun (weeks) |
| Ruin-Road (E) | (100,50) | D21 / the Ruin'd Crown (immediately dangerous) |

## Services

| Service | Where | Details |
|---|---|---|
| Rest | any open ground (free) | unsafe at night (theft risk); Father Ord's area is safer (DC 13 to earn a watched space) |
| Resupply | Salvage-Market (60,50) | salvage-food, rope, basic tools; prices are gouged; Persuasion DC 14 for fair treatment |
| Healing | Father Ord's Tent (45,40) | mundane healing; freely given; Ord treats everyone |
| Information | Father Ord's Tent or Watch-Fire | Ord (DC 14; knows more than he says; Insight DC 16); Remnant Scholars (DC 15; more structured knowledge) |
| Faction contact | Remnant Scholars' Tents | Hollin Vane (DC 17; Remnant inner access) / Father Ord (independent) |

## Law and Threat DCs

- **Entering the Pilgrim Camps:** completely open; no law here. Watch for thieves (Perception DC 14 at night to notice someone rifling gear while sleeping).
- **Confronting a thief in the Salvage-Market:** quick dispute; 2–4 camp toughs (**Bandit-like**, AC 12); Father Ord can mediate (DC 13).
- **Moving toward the Ruin-Road head:** no one stops you — but Father Ord will offer advice (always with oblique significance; Insight DC 15 to sense what he knows and what he won't say).
- **Drawing weapons near the Remnant Scholars' Tents:** Vane's expedition-guards respond (6 soldiers, **Guard-like**, AC 14).

## Key NPC Links

| NPC | Role | Location | Notes |
|---|---|---|---|
| Father Casian Ord | heretic-priest; camp's moral anchor | Father Ord's Tent (45,40) | DC 14; Insight DC 16 to sense M6-oblique significance |
| Crown-Reclaimer Magister Hollin Vane | Remnant expedition-lord | Remnant Scholars' Tents (35,55) | DC 17; apex-adjacent dupe; never confirms keystone |
| "Old Crown" Mab | ruin-guide | Ruin-Road head (80,50; visiting) | DC 15; guides D21 from either Crownmouth or the Camps |

## Quest Hooks

- **Q_CH_001 — The Last Safe Town:** the Pilgrim Camps are the second social hub for this arc; Crownmouth and the Camps together frame the ruin's human cost (L13; see Crownmouth packet).
- **Q_CH_003 — Father Ord's Secret:** Ord is not what he claims; something he saw in the ruin early on changed him; the player can pursue this (L14+; M6-oblique; never names the keystone).
- **Refugee aid:** the Refuge-Quarter needs medicine and food; a short-term humanitarian mission that earns Ord's trust and unlocks his information-sharing (L12+; DC 13).

## Encounter / Treasure References

- Encounter: camp toughs (**Bandit-like**, AC 12); rival-expedition teams (Veteran-like, CR 5–8); Crown undead encountered approaching the Ruin-Road head (**Wight / Shadow-like**, CR 5–8; see D21); see L12+ undead and rival-faction lines.
- Treasure: `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` Tier 3 Heartlands salvage; Father Ord's gift (a hand-written letter of passage — unexpectedly effective; its significance is M6-oblique); Vane's expedition payment (gold, Remnant certification).

## Player-Safe Layer

The shanty-camp in the ruin's shadow; Father Ord's welcoming tent; the Salvage-Market; the Remnant scholars' organized corner; the Refuge-Quarter's quiet desperation; the Watch-Fire at night; the Ruin-Road head pointing into the dark.

## DM-Only Layer (NEVER on player map)

- Father Casian Ord saw something in the early D21 approach that he will not describe in full — he understood it as "the old empire's accounting of the dead" without comprehending the harvest. This is M6-oblique; he speaks in parables.
- The Camp's location (63,58) is NOT near the keystone — the ruin is a surface fallen-capital. The keystone is vertical beneath Hollowmere (NW only). No apex geometry here.

## Related Files

- Region: [`../../04_world_atlas/region_map_packets/REGION_CONCORD_HEARTLANDS.md`](../../04_world_atlas/region_map_packets/REGION_CONCORD_HEARTLANDS.md)
- Hub: [`SETTLEMENT_CROWNMOUTH_MAP.md`](SETTLEMENT_CROWNMOUTH_MAP.md)
- NPCs: [`../../08_npcs/by_region/CONCORD_HEARTLANDS_NPCS.md`](../../08_npcs/by_region/CONCORD_HEARTLANDS_NPCS.md)
- Quests: [`../../09_quests/by_region/CONCORD_HEARTLANDS_QUESTS.md`](../../09_quests/by_region/CONCORD_HEARTLANDS_QUESTS.md)
- D-site: [`../../10_dungeons_and_ruins/THE_OLD_CONCORD_HEARTLANDS_RUIN.md`](../../10_dungeons_and_ruins/THE_OLD_CONCORD_HEARTLANDS_RUIN.md)
