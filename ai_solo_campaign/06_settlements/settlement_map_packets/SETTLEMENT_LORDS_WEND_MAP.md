# SETTLEMENT_LORDS_WEND_MAP.md — Settlement Map Packet

---
type: settlement
secrecy: player-safe
status: static
region: Verdance Reaches
settlement: Lord's Wend
level_range: 8-12
related: [../../04_world_atlas/region_map_packets/REGION_VERDANCE_REACHES.md, ../../04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../../08_npcs/by_region/VERDANCE_REACHES_NPCS.md, ../../09_quests/by_region/VERDANCE_REACHES_QUESTS.md]
tags: [type:map, secrecy:player-safe, function:cartography, settlement-map, map-packet, lords-wend, verdance-reaches]
---

> **Secrecy classification:** Player-safe. Lord's Wend is a petty-lord's hall-town: rural, land-politics, Nine Locks administrative seat. No apex content.

## Settlement: Lord's Wend (Verdance Reaches — petty-lord hall-town)

- **Local grid:** 0–100 (X east, Y south); (0,0) = NW corner. Small fortified hall-town in the inland Verdance valley; the lord's hall NW; market square center; Nine Locks road N.
- **Full-continent position:** render-grid (60,45).
- **Population / scale:** ~300–500; a small hall-town serving the Nine Locks territory and inland farms.
- **Water/road relationship:** on a minor Verdance tributary; the **Nine Locks Road** leads N (to the Nine Locks landmark, D31); the **Interior Road** leads W (to Marrowfen Stair, 58,42) and E (toward the Heartlands passes).

## Layout / Notable Areas

| Area | Local | Notes |
|---|---|---|
| Lord Ennis Marrow's Hall | (25,30) | the petty-lord's manor; political authority for the Nine Locks territory |
| The Market Square | (55,50) | small inland market; farmstead goods, river-produce |
| The Nine Locks Road head | (50,20) | the road N toward D31; Lord Marrow controls access |
| The River Chapel | (70,60) | Three Thresholds shrine; Mourners' presence |
| The Wend Inn | (60,70) | rest and provisions; modest |

## Entrances / Exits

| Exit | Local edge | Leads to |
|---|---|---|
| Interior Road (W) | (0,50) | Marrowfen Stair (58,42; days) |
| Interior Road (E) | (100,50) | Heartlands passes (weeks) |
| Nine Locks Road (N) | (50,0) | Nine Locks / D31 (hours–days; Lord's permit needed) |
| Farmstead track (S) | (60,100) | inland Verdance farms (dead-end area) |

## Services

| Service | Where | Details |
|---|---|---|
| Rest | Wend Inn (60,70) | 1sp/night; modest but safe |
| Resupply | Market Square (55,50) | farmstead goods, rations, river-produce; no weapons or magic items |
| Healing | River Chapel (70,60) | mundane rites; the chapel keeper offers basic care |
| Information | Lord Marrow's Hall or Inn | Marrow (DC 15); Inn travelers (DC 12) |
| Faction contact | Lord Marrow's Hall | the petty-lord's court; Remnant indirect (Vael visits seasonally) |

## Law and Threat DCs

- **Entering Lord's Wend:** open; no gate fee. Lord Marrow's soldiers (10 men-at-arms) are present.
- **Requesting Nine Locks road access:** Lord Marrow's permit; Persuasion DC 16 or a fee (5gp).
- **Violent act in the Wend:** men-at-arms respond (**Guard / Veteran-like**, AC 14–16, 10 total).

## Key NPC Links

| NPC | Role | Location | Notes |
|---|---|---|---|
| Lord Ennis Marrow | petty-lord; Nine Locks administrator | Lord Marrow's Hall (25,30) | Persuasion DC 15; land-focused; suspicious of Ledger |
| Sub-Lector Hadwin Vael | Remnant scholar | visiting from Marrowfen Stair | periodic visit; carries Concord-Engineering maps |

## Quest Hooks

- **Q_VR_004 — The Nine Locks' Fee:** Lord Marrow has seized the Nine Locks in a toll-dispute with the Ledger; both sides want the player as courier-negotiator (L9).
- **Q_VR_005 — The Sunken Stair:** Vael (via Marrow's hall) hires the player to access D31; Marrow demands conditions (L10+; Nine Locks Sunken Stair).

## Encounter / Treasure References

- Encounter: men-at-arms (**Guard-like**, AC 14, 10 total); Heartlands road-bandits (E of Lord's Wend, CR 3–6); see L8+ encounter lines.
- Treasure: `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` Tier 2 inland-lord rewards; Lord Marrow's permit (access-token for D31).

## Related Files

- Region: [`../../04_world_atlas/region_map_packets/REGION_VERDANCE_REACHES.md`](../../04_world_atlas/region_map_packets/REGION_VERDANCE_REACHES.md)
- NPCs: [`../../08_npcs/by_region/VERDANCE_REACHES_NPCS.md`](../../08_npcs/by_region/VERDANCE_REACHES_NPCS.md)
- Quests: [`../../09_quests/by_region/VERDANCE_REACHES_QUESTS.md`](../../09_quests/by_region/VERDANCE_REACHES_QUESTS.md)
- D-site: [`../../10_dungeons_and_ruins/THE_NINE_LOCKS_SUNKEN_STAIR.md`](../../10_dungeons_and_ruins/THE_NINE_LOCKS_SUNKEN_STAIR.md)
