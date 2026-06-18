# SETTLEMENT_PENMARK_HOLD_MAP.md — Settlement Map Packet

---
type: settlement
secrecy: player-safe
status: static
region: Marrowdowns
settlement: Penmark Hold
level_range: 6-10
related: [../../04_world_atlas/region_map_packets/REGION_MARROWDOWNS.md, ../../04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../../08_npcs/by_region/MARROWDOWNS_NPCS.md, ../../09_quests/by_region/MARROWDOWNS_QUESTS.md]
tags: [type:map, secrecy:player-safe, function:cartography, settlement-map, map-packet, penmark-hold, marrowdowns]
---

> **Secrecy classification:** Player-safe. Penmark Hold is the Shire-Reeve's manor: landed gentry, chalk-downs law, the downs' formal legal authority. No apex content.

## Settlement: Penmark Hold (Marrowdowns — shire-reeve's manor-hold)

- **Local grid:** 0–100 (X east, Y south); (0,0) = NW corner. A fortified manor-hold on the chalk downs NW of Marrowmoot; the Hold itself dominates the ridge; village below.
- **Full-continent position:** render-grid (47,63).
- **Population / scale:** ~200–400; the Shire-Reeve's household plus a small farming-village; the downs' administrative center.
- **Water/road relationship:** the **Penmark Road** leads SE (to Marrowmoot, 50,66; half-day); chalk streams provide water; the **South Downs Track** leads W (toward Sallowmarch frontier; days).

## Layout / Notable Areas

| Area | Local | Notes |
|---|---|---|
| Penmark Manor | (40,30) | Shire-Reeve Aldous Penmark's fortified manor; law and records |
| The Manor Hall | (55,35) | Penmark's formal court and audience chamber |
| The Village Green | (50,65) | the farming-village below the ridge; modest market |
| The Stables | (70,45) | Horse-Reeve Edony Marrow's base; 15+ riding horses |
| The Warden Post | (30,60) | the circuit-warden's waystation; regional law enforcement hub |

## Entrances / Exits

| Exit | Local edge | Leads to |
|---|---|---|
| Penmark Road (SE) | (75,100) | Marrowmoot (50,66; half-day) |
| South Downs Track (W) | (0,50) | Sallowmarch frontier (days) |
| Barrow Road (NE) | (85,0) | Barrow-Fields / D26 approach (hours from the ridge; dangerous) |

## Services

| Service | Where | Details |
|---|---|---|
| Rest | Manor guesthouse (Penmark's hospitality) | free for Compact officials or shire business; 1sp for others |
| Resupply | Village Green market | limited; rations, horses, chalk-country goods |
| Healing | Village healer (standard) | mundane only; DC 13 to access |
| Information | Manor Hall | Penmark (DC 15); Horse-Reeve Edony (DC 14) |
| Faction contact | Manor Hall | shire law; Compact-affiliated; Horse-Reeve's patrol network |

## Law and Threat DCs

- **Entering Penmark Hold:** open to approach; Penmark's household greets visitors formally.
- **Requesting legal adjudication:** Shire-Reeve Penmark; Persuasion DC 14 (legitimate matter) or DC 16 (politically sensitive).
- **Violent act at the Hold:** manor guards (15 men-at-arms, **Guard-like**, AC 14) + the Horse-Reeve's mounted response.

## Key NPC Links

| NPC | Role | Location | Notes |
|---|---|---|---|
| Shire-Reeve Aldous Penmark | downs law; landed authority | Manor Hall (55,35) | Persuasion DC 15; circuit-travels to Marrowmoot |
| Horse-Reeve Edony Marrow | mounted lawkeeper | Stables (70,45) | Persuasion DC 14; can track across the downs; excellent scout |

## Quest Hooks

- **Q_MD_002 — The Moot's Truth:** Penmark is at the manor between circuit-stops; Senna Crale's request to break the political silence on the Barrow problem (L8; he resists).
- **The Barrow-Fields access warrant:** Penmark issues legal entry-permits to D26; earn his trust to get one (L6+; Persuasion DC 16 or prior service).
- **Horse-Reeve tracking contract:** Edony Marrow can track something (person, creature, object) anywhere in the downs; she charges in favors owed to the Shire (L6+).

## Encounter / Treasure References

- Encounter: manor guards (**Guard-like**, AC 14, 15 total); Horse-Reeve Edony mounted (**Cavalry-Scout-like**, AC 14, mounted); see L6+ plains lines.
- Treasure: `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` Tier 1–2 Shire-Reeve's legal pay (silver, land-right, access-warrant).

## Related Files

- Region: [`../../04_world_atlas/region_map_packets/REGION_MARROWDOWNS.md`](../../04_world_atlas/region_map_packets/REGION_MARROWDOWNS.md)
- Hub: [`SETTLEMENT_MARROWMOOT_MAP.md`](SETTLEMENT_MARROWMOOT_MAP.md)
- NPCs: [`../../08_npcs/by_region/MARROWDOWNS_NPCS.md`](../../08_npcs/by_region/MARROWDOWNS_NPCS.md)
- Quests: [`../../09_quests/by_region/MARROWDOWNS_QUESTS.md`](../../09_quests/by_region/MARROWDOWNS_QUESTS.md)
