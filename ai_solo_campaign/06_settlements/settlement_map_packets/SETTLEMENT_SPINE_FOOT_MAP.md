# SETTLEMENT_SPINE_FOOT_MAP.md — Settlement Map Packet

---
type: settlement
secrecy: player-safe
status: static
region: Wender Steppe
settlement: The Spine-Foot Trade-Meet
level_range: 7-12
related: [../../04_world_atlas/region_map_packets/REGION_WENDER_STEPPE.md, ../../04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../../08_npcs/by_region/WENDER_STEPPE_NPCS.md, ../../09_quests/by_region/WENDER_STEPPE_QUESTS.md]
tags: [type:map, secrecy:player-safe, function:cartography, settlement-map, map-packet, spine-foot, wender-steppe]
---

> **Secrecy classification:** Player-safe. The Spine-Foot trade-meet is the seasonal gathering where the steppe clans and the settled world do business. Entirely player-safe. No apex content.

## Settlement: The Spine-Foot Trade-Meet (Wender Steppe — steppe/settled trade-meeting ground)

- **Local grid:** 0–100 (X east, Y south); (0,0) = NW corner. A large open-ground meeting-place where the Highmark Spine's S foothills meet the open steppe; seasonal permanent structures (felt-covers over stone frames) on the W side; open steppe E.
- **Full-continent position:** render-grid (50,20).
- **Population / scale:** seasonal; ~200–300 permanent (the meet's stewards and settled-world merchants); swells to 1,500+ during peak trade-season (the autumn-gathering).
- **Water/road relationship:** at the **Greatspine / Highmark foothills** S edge; the **Great Road** (settled-world trade track) leads S (into Orrun's interior; weeks); the **Steppe Track** leads N (to Cold Springs, 45,16; hours–day); seasonal markets run on a fixed calendar.

## Layout / Notable Areas

| Area | Local | Notes |
|---|---|---|
| The Stone Halls | (30,40) | permanent market structures; settled-world merchants operate here year-round |
| The Clan-Ground | (65,40) | where steppe clans pitch their trade-tents; open-side facing E |
| The Spine Road head | (25,70) | toward the settled world; Great Road S; most travelers arrive here |
| The Steppe Track head | (70,70) | toward the Cold Springs camp; Tamur Wend-Khar's approach |
| The Arbitration Tent | (50,50) | where trade disputes are settled; neutral ground |

## Entrances / Exits

| Exit | Local edge | Leads to |
|---|---|---|
| Great Road (S) | (30,100) | settled-world (Glassmere approaches; weeks) |
| Steppe Track (N) | (65,0) | Cold Springs (45,16; hours–day) |
| Highmark foothills (W) | (0,50) | Highmark Spine passes (weeks; extreme altitude) |
| Open steppe (E) | (100,50) | deep steppe / Borr's territory (days) |

## Services

| Service | Where | Details |
|---|---|---|
| Rest | Stone Halls (30,40; merchant lodges) | 2sp/night; safe within the meet's neutral-ground rules |
| Resupply | Stone Halls + Clan-Ground market | steppe goods (horses, furs, felt) + settled goods (metal, cloth, preserved food); the widest selection on the steppe |
| Healing | settled-world medic (Stone Halls) | mundane; 2gp; DC 13 |
| Information | Stone Halls or Arbitration Tent | settled merchants (DC 13); steppe-clan traders (DC 14); Borr's riders (Perception DC 16 to spot near the E edge) |
| Faction contact | Clan-Ground | steppe confederacy traders (Tamur-adjacent); Compact-affiliated settled merchants |

## Law and Threat DCs

- **Entering the trade-meet:** neutral ground; no toll; meet's rules (no unsheathed weapons, no clan-disputes) apply. Persuasion DC 13 to establish good-faith.
- **Breaking neutral-ground (fighting):** immediate mass response — 30+ merchants and clan-traders stop you; Persuasion DC 17 to explain; DC 12 to de-escalate before it becomes lethal.
- **Borr's riders near the E edge:** they technically don't enter the meet (neutral ground); but they watch; Perception DC 16 to spot a scout.

## Key NPC Links

| NPC | Role | Location | Notes |
|---|---|---|---|
| Clan-Speaker Tamur Wend-Khar | confederacy Speaker | visiting from Cold Springs (seasonal) | Persuasion DC 15 here (neutral context; slightly more accessible than at camp) |
| (Spine-Foot steward) | meet's senior merchant-representative | Stone Halls | secondary NPC; Persuasion DC 13; knows all the merchants' names |

## Quest Hooks

- **Q_WS_001 — The Confederacy's Crisis:** Tamur can also be approached at the Spine-Foot (less formal than Cold Springs; Persuasion DC 14 here for initial contact).
- **Q_WS_002 — Borr's Raids:** settled-world merchants at the Stone Halls have posted a bounty on Borr's raid-captains; this is where the contract is offered (L9+; DC 13 to find it).
- **Steppe supply-contract:** a Compact-affiliated merchant needs goods delivered to Cold Springs without Borr intercepting; a paid escort contract (L7+).

## Encounter / Treasure References

- Encounter: Borr's raiding parties (**Berserker-like**, AC 13, ~67 HP; on the open steppe approaches, not inside the meet); Highmark pass bandits (S approaches; Veteran-like, CR 3–6); see L7+ plains/trade lines.
- Treasure: `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` Tier 2 trade-meet rewards; steppe goods as trade-currency; Tamur's formal trade-gift (a fine steppe-horse or sky-iron tool).

## Related Files

- Region: [`../../04_world_atlas/region_map_packets/REGION_WENDER_STEPPE.md`](../../04_world_atlas/region_map_packets/REGION_WENDER_STEPPE.md)
- Camp: [`SETTLEMENT_COLD_SPRINGS_MAP.md`](SETTLEMENT_COLD_SPRINGS_MAP.md)
- NPCs: [`../../08_npcs/by_region/WENDER_STEPPE_NPCS.md`](../../08_npcs/by_region/WENDER_STEPPE_NPCS.md)
- Quests: [`../../09_quests/by_region/WENDER_STEPPE_QUESTS.md`](../../09_quests/by_region/WENDER_STEPPE_QUESTS.md)
