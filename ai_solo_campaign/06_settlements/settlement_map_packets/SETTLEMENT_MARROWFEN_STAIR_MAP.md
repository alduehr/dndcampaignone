# SETTLEMENT_MARROWFEN_STAIR_MAP.md — Settlement Map Packet

---
type: settlement
secrecy: mixed
status: static
region: Verdance Reaches
settlement: Marrowfen Stair
level_range: 8-12
related: [../../04_world_atlas/region_map_packets/REGION_VERDANCE_REACHES.md, ../../04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../../08_npcs/by_region/VERDANCE_REACHES_NPCS.md, ../../09_quests/by_region/VERDANCE_REACHES_QUESTS.md]
tags: [type:map, secrecy:mixed, function:cartography, settlement-map, map-packet, marrowfen-stair, verdance-reaches]
---

> **Secrecy classification:** Mixed (reclassified 2026-07-11 — the file contains a DM-Only Layer section, so the whole file is not player-safe). Marrowfen Stair itself is an honest river-lock corridor-hub with no apex content; render the Player-Safe Layer freely, keep the DM-Only Layer back.

## Settlement: Marrowfen Stair (Verdance Reaches — river-lock corridor hub)

- **Local grid:** 0–100 (X east, Y south); (0,0) = NW corner. On the eastern bank of the Verdance, built around the lock-staircase; wharves S; Ledger offices N; ferry-road E.
- **Full-continent position:** render-grid (58,42).
- **Population / scale:** ~800–1,200 residents; the Verdance's largest working lock-town; goods flow through here from the Glassmere coast to the interior.
- **Water/road relationship:** on the **Verdance river** (major N–S river artery); the **lock-staircase** raises/lowers barges 12 meters here; the **Interior Road** leads E (to Lord's Wend, 60,45; and the Heartlands beyond); the **Verdance towpath** leads N (to Glassmere; weeks) and S (to Caradril; weeks).

## Layout / Notable Areas

| Area | Local | Notes |
|---|---|---|
| The Lock Gate (lower) | (30,65) | bottom of the staircase; barge-masters wait here; the busiest place |
| The Factor-General's Hall | (45,30) | Wessel Crane's Ledger directorate office; the commercial authority |
| The Wharves | (65,70) | lower river wharves; barge moorings; cargo warehouses |
| The Compact Checkpoint | (20,45) | Reachward Compact inspection post; permits checked |
| The Stair Inn | (55,45) | rest, provisions, river news; the social center |
| The Remnant Reading Room | (70,35) | Sub-Lector Hadwin Vael's small chapter; maps and records |

## Entrances / Exits

| Exit | Local edge | Leads to |
|---|---|---|
| Verdance towpath (N, upstream) | (30,0) | Glassmere (weeks by barge or towpath) |
| Verdance towpath (S, downstream) | (30,100) | Caradril (weeks by current) |
| Interior Road (E) | (100,50) | Lord's Wend (60,45; days); Heartlands passes (weeks) |
| Fen Track (W) | (0,60) | the Mirewend Sinks / Cresswater barge-village (55,46; days overland) |

## Services

| Service | Where | Details |
|---|---|---|
| Rest | Stair Inn (55,45) | 2sp/night; open to all; river-traffic news at the common table |
| Resupply | Wharves (65,70) | river cargo, rations, rope, tools, barge-equipment; standard market |
| Healing | Remnant Reading Room (visiting healer) | mundane; DC 15 to find when not publicized; Vael can direct |
| Information | Factor-General's Hall or Stair Inn | Crane (DC 16); Vael (DC 15); Inn travelers (DC 13) |
| Faction contact | Factor-General's Hall | Ledger directorate (Crane); Compact (checkpoint); Remnant (Vael) |

## Law and Threat DCs

- **Entering Marrowfen Stair:** Compact checkpoint; state purpose; Persuasion DC 13 (standard commercial reason) or DC 15 (unusual).
- **Requesting lock passage (barge):** Factor-General's permit needed; Persuasion DC 15 or Ledger membership.
- **Carrying relic salvage into the Stair:** Compact inspection; Persuasion DC 15 (declared) or DC 17 (undeclared and caught).
- **Violent act in the Stair:** Compact garrison (20 soldiers, **Guard-like**, AC 14) responds within 5 rounds.

## Key NPC Links

| NPC | Role | Location | Notes |
|---|---|---|---|
| Factor-General Wessel Crane | Ledger inland directorate head | Factor-General's Hall (45,30) | Persuasion DC 16; commercially minded; bribable with quality |
| Sub-Lector Hadwin Vael | Remnant inland chapter | Remnant Reading Room (70,35) | Persuasion DC 15; maps, records, Verdance route knowledge |
| River-Captain Mossa Drenn | independent barge-captain | Wharves (65,70; moored seasonally) | Persuasion DC 14; owns a barge; the safe water-route option |

## Quest Hooks

- **Q_VR_001 — The Lock Dispute:** the Ledger and the Compact are in a fee-dispute that is slowing barge traffic and costing river-merchants; Crane hires an outside arbitrator (L8).
- **Q_VR_003 — Mossa's Cargo:** River-Captain Drenn's barge has something in the hold that she won't declare at the Compact checkpoint; she needs discreet escorts (L9).
- **Vael's record-request:** Sub-Lector Vael wants old Concord lock-engineering records retrieved from the Nine Locks deeper site; a research expedition (L10+; see Nine Locks D31 / Q_VR_005).

## Encounter / Treasure References

- Encounter: Compact soldiers (**Guard-like**, AC 14); Ledger caravan-guards (**Guard / Bandit-like**); river bandits on the towpath (**Bandit / Scout-like**, CR 2–5); see `13_encounters_and_bestiary/` plains/river lines at L8+.
- Treasure: `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` Tier 2 (L6–11) river-trade rewards; Crane's commercial payment (gold, trade-goods, Ledger letters of credit); Vael's scholarly reward (old maps, Concord Script copies, healing herbs).

## Player-Safe Layer

The lock-staircase with its barge-traffic, the Factor-General's hall (Ledger's river presence), the Compact checkpoint, the wharves, the Stair Inn, the Remnant's small reading-room. A prosperous, watched, commercial river-junction.

## DM-Only Layer

None. All content here is player-safe. The Remnant's records at the reading room contain surface-level Concord engineering notes only — no apex content.

## Related Files

- Region: [`../../04_world_atlas/region_map_packets/REGION_VERDANCE_REACHES.md`](../../04_world_atlas/region_map_packets/REGION_VERDANCE_REACHES.md)
- NPCs: [`../../08_npcs/by_region/VERDANCE_REACHES_NPCS.md`](../../08_npcs/by_region/VERDANCE_REACHES_NPCS.md)
- Quests: [`../../09_quests/by_region/VERDANCE_REACHES_QUESTS.md`](../../09_quests/by_region/VERDANCE_REACHES_QUESTS.md)
- D-site nearby: [`../../10_dungeons_and_ruins/THE_NINE_LOCKS_SUNKEN_STAIR.md`](../../10_dungeons_and_ruins/THE_NINE_LOCKS_SUNKEN_STAIR.md)
