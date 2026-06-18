# SETTLEMENT_KARRAN_GATE_MAP.md — Settlement Map Packet

---
type: settlement
secrecy: player-safe
status: static
region: Karran Marches
settlement: Karran-Gate
level_range: 9-14
related: [../../04_world_atlas/region_map_packets/REGION_KARRAN_MARCHES.md, ../../04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../../08_npcs/by_region/KARRAN_MARCHES_NPCS.md, ../../09_quests/by_region/KARRAN_MARCHES_QUESTS.md]
tags: [type:map, secrecy:player-safe, function:cartography, settlement-map, map-packet, karran-gate, karran-marches]
---

> **Secrecy classification:** Player-safe. Karran-Gate is the Marches' trade-and-mercenary town: an open market town (by frontier standards) where ore and hired steel change hands. No apex content.

## Settlement: Karran-Gate (Karran Marches — mining-and-mercenary town)

- **Local grid:** 0–100 (X east, Y south); (0,0) = NW corner. A sprawling mining-town in the Karran Teeth foothills; more open than Brask's Hold (no single warlord); the Iron Road runs through N–S.
- **Full-continent position:** render-grid (76,20).
- **Population / scale:** ~1,200–2,000; the Marches' largest trade-hub; multiple competing mercenary companies operate here.
- **Water/road relationship:** in the **Karran Teeth** foothills; a cold mountain river runs through (drinking water); the **Iron Road** leads N (to Brask's Hold, 73,17; days) and S (toward Glassmere approaches; weeks); the **Deep Cuts Road** leads W (to the Deep Cuts mines, 71,21; days).

## Layout / Notable Areas

| Area | Local | Notes |
|---|---|---|
| The Ore Exchange | (50,35) | Mully Karr's primary trading house; where metal is bought and sold |
| The Mercenary Row | (65,45) | competing mercenary company offices; bulletin boards; hiring |
| The Iron Road Gate (N) | (40,20) | toward Brask's Hold; loose inspection (Brask's territory starts here) |
| The Deep Cuts Road head | (25,60) | toward the mines; Karr's transport organization |
| The Rough House | (60,65) | the largest tavern-inn; 2sp/night; controlled violence; disputes settled here |
| The Compact Post | (35,75) | Reachward Compact way-station; records, permits, letters |

## Entrances / Exits

| Exit | Local edge | Leads to |
|---|---|---|
| Iron Road (N) | (40,0) | Brask's Hold (73,17; days) |
| Iron Road (S) | (50,100) | Glassmere approaches (weeks) |
| Deep Cuts Road (W) | (0,60) | Deep Cuts / D27 access road (71,21; days) |
| Old Forts track (NE) | (100,20) | Old Iron forts / D27 (78,15; weeks; dangerous) |

## Services

| Service | Where | Details |
|---|---|---|
| Rest | Rough House (60,65) | 2sp/night; safe by frontier standards; disputes arbitrated by the crowd |
| Resupply | Ore Exchange / Mercenary Row | weapons, armor, mining equipment, rations, horses; full frontier supply |
| Healing | Compact Post affiliated healer | mundane + 2nd-level; 3gp; DC 14 |
| Information | Ore Exchange or Rough House | Mully Karr (DC 16); Mercenary Row (DC 12 for local hiring gossip) |
| Faction contact | Ore Exchange | Mully Karr (Ledger-adjacent metals trade); Compact Post (records and permits) |

## Law and Threat DCs

- **Entering Karran-Gate:** loose; multiple companies share informal authority. No single gate-toll; expect to be sized up.
- **Hiring through Mercenary Row:** straightforward; rates posted; Persuasion DC 13 for discounts.
- **Starting a fight in the Rough House:** local mercenaries intervene fast (4–6 **Veteran-like**, AC 16, CR 3–5 each); escalation brings more.
- **Carrying Deep Cuts salvage (the wrong kind):** Mully's people notice; Persuasion DC 15 to explain before questions get uncomfortable.

## Key NPC Links

| NPC | Role | Location | Notes |
|---|---|---|---|
| Ore-Factor Mully Karr | metals-trader; information broker | Ore Exchange (50,35) | Persuasion DC 16; bribable with silver; anti-Brask sentiment |
| Reclaimer-Captain Wenna Stone | Remnant expedition-captain; turnable | Rough House (periodic; en route to Old Iron forts) | Persuasion DC 17; trusts demonstrated competence |

## Quest Hooks

- **Q_KM_001 — The Deep That Went Wrong:** Karran-Gate is where the first mine-mad survivors are brought; the on-ramp inciting event is first visible here before Brask's Hold confirms it (L9).
- **Q_KM_003 — Wenna Stone's Expedition:** Wenna hires out of Karran-Gate for the Old Iron forts push; she needs a companion with specific skills (L11+; leads to D27).
- **Mercenary Row contract:** short-term work available constantly (mine-guard, road-escort, Brask's border, Deep Cuts supply-run); DC 13 to qualify; 5–10gp/day (L9+).

## Encounter / Treasure References

- Encounter: rival mercenaries (**Veteran-like**, AC 16, CR 3–5; several companies in active competition); Deep Cuts mine hazards (mine-mad construct-echoes, CR 5–9; see `13_/`); Old Iron fort undead (D27; Wight / Animated Armor-like, CR 5–12).
- Treasure: `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` Tier 2–3 Marches mercenary rewards; Mully's ore-payment (refined iron, quality steel tools, silver); Wenna's Remnant seal (faction currency).

## Related Files

- Region: [`../../04_world_atlas/region_map_packets/REGION_KARRAN_MARCHES.md`](../../04_world_atlas/region_map_packets/REGION_KARRAN_MARCHES.md)
- Hold: [`SETTLEMENT_BRASKS_HOLD_MAP.md`](SETTLEMENT_BRASKS_HOLD_MAP.md)
- NPCs: [`../../08_npcs/by_region/KARRAN_MARCHES_NPCS.md`](../../08_npcs/by_region/KARRAN_MARCHES_NPCS.md)
- Quests: [`../../09_quests/by_region/KARRAN_MARCHES_QUESTS.md`](../../09_quests/by_region/KARRAN_MARCHES_QUESTS.md)
- D-site: [`../../10_dungeons_and_ruins/THE_KARRAN_OLD_IRON_FORTS.md`](../../10_dungeons_and_ruins/THE_KARRAN_OLD_IRON_FORTS.md)
