# SETTLEMENT_WETHER_MAP.md — Settlement Map Packet

---
type: settlement
secrecy: player-safe
status: static
region: Marrowdowns
settlement: Wether
level_range: 6-10
related: [../../04_world_atlas/region_map_packets/REGION_MARROWDOWNS.md, ../../04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../../08_npcs/by_region/MARROWDOWNS_NPCS.md, ../../09_quests/by_region/MARROWDOWNS_QUESTS.md]
tags: [type:map, secrecy:player-safe, function:cartography, settlement-map, map-packet, wether, marrowdowns]
---

> **Secrecy classification:** Player-safe. Wether is a small wool-trade village and travel anchor between Marrowmoot and the Barrow-Fields. Barrow-Master Doss Wether's home base. No apex content.

## Settlement: Wether (Marrowdowns — wool-trade village and barrow-guide base)

- **Local grid:** 0–100 (X east, Y south); (0,0) = NW corner. Small chalk-downs village astride the Barrow Road; Doss Wether's cottage is NE toward the Barrow approach.
- **Full-continent position:** render-grid (53,68).
- **Population / scale:** ~150–250; a small wool-village with a strong identity as "the last stop before the Barrows."
- **Water/road relationship:** the **Barrow Road** leads NE (to D26; hours); the **Marrowmoot Road** leads NW (to Marrowmoot, 50,66; half-day); the **Salt Road** passes through S (to Sallowmarch approaches).

## Layout / Notable Areas

| Area | Local | Notes |
|---|---|---|
| The Wool-Sheds | (60,40) | primary village economy; shearing and baling; Ledger buyer visits seasonally |
| The Barrow-Guide's Cottage | (70,25) | Doss Wether's home; his maps and ropes; the departure point for D26 runs |
| The Village Tap | (45,55) | the only tavern; basic rest and provisions |
| The Barrow Road head | (85,30) | where the chalk track becomes the "wrong ground" approach |

## Entrances / Exits

| Exit | Local edge | Leads to |
|---|---|---|
| Marrowmoot Road (NW) | (0,35) | Marrowmoot (50,66; half-day) |
| Barrow Road (NE) | (85,0) | Barrow-Fields / D26 (hours; warned as dangerous) |
| Salt Road (S) | (50,100) | Sallowmarch / Mardenflow frontier (days) |

## Services

| Service | Where | Details |
|---|---|---|
| Rest | Village Tap (45,55) | 1sp/night; basic; safe; Wether's maps on the wall |
| Resupply | Wool-Sheds (limited) | rations, rope, chalk-country provisions; no weapons |
| Healing | Village widow-healer | mundane; free for the genuinely injured |
| Information | Village Tap or Wether's Cottage | Doss Wether (DC 14); village (DC 12) |
| Faction contact | Wether's Cottage | independent (Wether's own network); Ledger buyer (seasonal) |

## Law and Threat DCs

- **Entering Wether:** completely open; no formal law here (circuit-visits from Penmark).
- **Asking about the Barrow-Fields:** willingly given (every village resident has a Barrow story); Doss shares freely if approached respectfully.
- **Going to the Barrows without Doss:** discouraged (strongly); no law against it; the wrong dead are the consequence.

## Key NPC Links

| NPC | Role | Location | Notes |
|---|---|---|---|
| Barrow-Master Doss Wether | barrow-guide; knows the wrong ground | Wether's Cottage (70,25) or Village Tap | Persuasion DC 14; requires coin for D26 runs; knows the moot's political stake |

## Quest Hooks

- **Q_MD_001 — The Barrow Problem:** Wether is the inciting-event vehicle; he returns white-faced and tells the Village Tap about what changed at D26 (L6; on-ramp).
- **D26 escort:** Wether offers to guide for 5gp; he knows exactly how far he will go and where the "wrong ground" starts (L6+; leads to `THE_MARROWDOWNS_BARROW_COMPLEX.md`).

## Encounter / Treasure References

- Encounter: Barrow undead (Wether warns: the wrong dead at D26 approach, **Barrow-Shade / Ghoul-like**, CR 2–5); see L6+ barrow lines.
- Treasure: Wether's guide fee; Barrow salvage is DM-managed (Thin-touch risk; use relic rules per `14_/`).

## Related Files

- Region: [`../../04_world_atlas/region_map_packets/REGION_MARROWDOWNS.md`](../../04_world_atlas/region_map_packets/REGION_MARROWDOWNS.md)
- Hub: [`SETTLEMENT_MARROWMOOT_MAP.md`](SETTLEMENT_MARROWMOOT_MAP.md)
- NPCs: [`../../08_npcs/by_region/MARROWDOWNS_NPCS.md`](../../08_npcs/by_region/MARROWDOWNS_NPCS.md)
- D-site: [`../../10_dungeons_and_ruins/THE_MARROWDOWNS_BARROW_COMPLEX.md`](../../10_dungeons_and_ruins/THE_MARROWDOWNS_BARROW_COMPLEX.md)
