# SETTLEMENT_REEDMOUTH_MAP.md — Settlement Map Packet

---
type: settlement
secrecy: mixed
status: static
region: Sallowmarch Protectorate
settlement: Reedmouth
level_range: 10-14
related: [../../04_world_atlas/region_map_packets/REGION_SALLOWMARCH_PROTECTORATE.md, ../../04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../../08_npcs/by_region/SALLOWMARCH_PROTECTORATE_NPCS.md, ../../09_quests/by_region/SALLOWMARCH_PROTECTORATE_QUESTS.md]
tags: [type:map, secrecy:mixed, function:cartography, settlement-map, map-packet, reedmouth, sallowmarch]
---

> **Secrecy classification:** Mixed. Reedmouth is a smuggling-village in Heron Maddox's territory; Fen-Witch Sela Reed's Rice Sallows are nearby. The delta is genuinely dangerous. No apex content.

## Settlement: Reedmouth (Sallowmarch Protectorate — delta smuggling-village)

- **Local grid:** 0–100 (X east, Y south); (0,0) = NW corner. A raised-bank village in the delta; the river-mouth channels below; the Rice Sallows surrounding; Heron's dock built out over the water.
- **Full-continent position:** render-grid (60,85).
- **Population / scale:** ~300–500; a mixed community of fisherfolk, delta-workers, and Heron Maddox's smuggling network.
- **Water/road relationship:** in the **Mardenflow delta** channels; Fenward is upstream NW (57,82; hours by flat-barge); the **Rice Sallows** surround E/S; the **Fever Channels** are S/SE (dangerous swamp-water).

## Layout / Notable Areas

| Area | Local | Notes |
|---|---|---|
| Heron's Dock | (65,65) | Reed-Boss "Heron" Maddox's smuggling dock; flatboats, hidden cargo |
| The Delta Market | (50,50) | mixed delta goods; smuggled goods often here openly |
| The Rice Sallows edge | (25,70) | where the village thins into the flooded paddy-country; Sela Reed's meeting place |
| The Fever Channels approach | (70,85) | the dangerous waterway S; no casual approach; Heron's hidden route |
| The Raised House | (40,35) | the only two-story building; impromptu inn for those Heron approves |

## Entrances / Exits

| Exit | Local edge | Leads to |
|---|---|---|
| Upstream barge (NW) | (0,50) | Fenward (57,82; hours upstream) |
| Delta channel (S/SE) | (65,100) | Fever Channels (deep delta; days) |
| Rice Sallows path (E) | (100,65) | Rice Sallows and Fen-Witch Sela's territory (hours) |
| Coast approach (SW) | (0,85) | coast / Drowned Steps approach (hours–days) |

## Services

| Service | Where | Details |
|---|---|---|
| Rest | The Raised House (40,35) | Heron's approval required (Persuasion DC 15); safe if approved; 2sp |
| Resupply | Delta Market (50,50) | delta goods, some contraband, rations, rope, boats; Persuasion DC 13 to access full stock |
| Healing | Fen-Witch Sela (Rice Sallows edge, 25,70) | old-rite delta healing; mundane + 1st-level divine; DC 14 to approach respectfully |
| Information | Heron's Dock or Delta Market | Heron (DC 15); Delta Market gossip (DC 12) |
| Faction contact | Heron's Dock | Heron's smuggling network; Sela (old-faith; independent) |

## Law and Threat DCs

- **Entering Reedmouth:** no formal gate; but Heron's people note newcomers; Persuasion DC 14 to be treated as a welcome guest vs. a mark.
- **Accessing Heron's dock or hidden goods:** Persuasion DC 15 (Heron's trust needed first).
- **Approaching the Rice Sallows edge / Sela:** Persuasion DC 14 (respectful); Sela is not hostile to genuine need.
- **Garrison pursuit from Fenward:** Vorr Sallow rarely sends soldiers to Reedmouth (he doesn't want to know); but if they come: 20 soldiers (**Guard-like**, AC 14); Survival DC 16 by boat.

## Key NPC Links

| NPC | Role | Location | Notes |
|---|---|---|---|
| Reed-Boss "Heron" Maddox | delta smuggler-king | Heron's Dock (65,65) | Persuasion DC 15; bribable; turnable on principle |
| Fen-Witch Mother Sela Reed | old-faith grief-keeper | Rice Sallows edge (25,70) | Insight DC 16 for her oblique delta-lore |
| Rice-Moot Speaker Pell Sallows | village-speaker | Delta Market (periodic) | Persuasion DC 13; delta news |

## Quest Hooks

- **Q_SP_002 — Heron's Blocked Canal:** something in the Fever Channels S has blocked Heron's main smuggling route; he needs it cleared (L11+; Fever Channels = dangerous swamp encounter).
- **Fen-Witch's warning:** Sela has seen something in the Rice Sallows that she won't name to Fenward's garrison; she'll share with someone she trusts (L10; M2/M5-oblique delta-lore).
- **Drowned Steps approach:** Heron knows the coastal route to D30 (the Drowned Steps); he charges for the guide (L12+; Persuasion DC 15).

## Encounter / Treasure References

- Encounter: Heron's smugglers (**Bandit / Scout-like**, AC 12–13); delta hazards (giant crocodile equivalent, CR 5; Will-o'-wisp, CR 2, in the Fever Channels); Fever Channels undead (if D30 is active; **Drowned Dead / Ghoul-like**, CR 3–7); see L10+ swamp lines.
- Treasure: `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` Tier 2–3 delta smuggling rewards; Heron's pay (good coin, no questions); Sela's gift (delta-herb kit: 3 uses of Cure Wounds).

## Player-Safe Layer

Heron's dock, the delta market, the raised house (inn), the Rice Sallows edge with the fen-witch's presence. A delta smuggling-village where the official law is hours away and the real authority is a river-lord who charges by the ton.

## DM-Only Layer (NEVER on player map)

- The Drowned Steps (D30; off the coast S at 54,90) are pre-Concord ruins. Their occasional dead drifting up the Fever Channels are M2/M5-oblique; Sela's warning is about "the old steps giving back the wrong tide." NEVER the keystone.
- No apex geometry here.

## Related Files

- Region: [`../../04_world_atlas/region_map_packets/REGION_SALLOWMARCH_PROTECTORATE.md`](../../04_world_atlas/region_map_packets/REGION_SALLOWMARCH_PROTECTORATE.md)
- Hub: [`SETTLEMENT_FENWARD_MAP.md`](SETTLEMENT_FENWARD_MAP.md)
- NPCs: [`../../08_npcs/by_region/SALLOWMARCH_PROTECTORATE_NPCS.md`](../../08_npcs/by_region/SALLOWMARCH_PROTECTORATE_NPCS.md)
- Quests: [`../../09_quests/by_region/SALLOWMARCH_PROTECTORATE_QUESTS.md`](../../09_quests/by_region/SALLOWMARCH_PROTECTORATE_QUESTS.md)
