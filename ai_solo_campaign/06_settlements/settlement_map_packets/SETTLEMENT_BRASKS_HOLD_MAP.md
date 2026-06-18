# SETTLEMENT_BRASKS_HOLD_MAP.md — Settlement Map Packet

---
type: settlement
secrecy: mixed
status: static
region: Karran Marches
settlement: Brask's Hold
level_range: 9-14
related: [../../04_world_atlas/region_map_packets/REGION_KARRAN_MARCHES.md, ../../04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../../08_npcs/by_region/KARRAN_MARCHES_NPCS.md, ../../09_quests/by_region/KARRAN_MARCHES_QUESTS.md]
tags: [type:map, secrecy:mixed, function:cartography, settlement-map, map-packet, brasks-hold, karran-marches]
---

> **Secrecy classification:** Mixed. The Old Iron forts (D27) are peripheral Concord ruins — their "bad ground" is M2/M5-oblique, never the keystone. Brask's Hold reads as an honest frontier warlord-town: iron law, coin economy, no sentiment. Never hand directly to the player.

## Settlement: Brask's Hold (Karran Marches — warlord fortress-town)

- **Local grid:** 0–100 (X east, Y south); (0,0) = NW corner. Compact fortress on a mountain-shoulder; mine road SE; Teeth ridge N.
- **Full-continent position:** render-grid (73,17).
- **Population / scale:** ~500–800 residents; mostly soldiers, mine-supervisors, and their dependents; a compact frontier fortress-hold.
- **Water/road relationship:** high on the **Karran Teeth** shoulder; cold mountain streams nearby (fresh water only); the **Iron Road** runs S (to Karran-Gate, 76,20) and N (to the Old Iron forts / Teeth Pass).

## Layout / Notable Areas

| Area | Local | Notes |
|---|---|---|
| The Hold Gate | (20,35) | iron-reinforced; Brask's soldiers inspect all entrants; toll collected |
| The Warlord's Hall | (45,30) | Iron Brask's command seat and audience chamber |
| The Mercenary Barracks | (65,25) | 50+ hired fighters always present; market for employment |
| The Ore-Yards | (50,60) | mine output staged and auctioned here; information hub |
| The Market Row | (35,75) | weapons, tools, cold-weather gear, rations; no luxuries, no magic items |
| The Mine Road head | (80,65) | the controlled gate to the Iron Road S and the Deep Cuts access road |

## Entrances / Exits

| Exit | Local edge | Leads to |
|---|---|---|
| Iron Road (S) | (75,100) | Karran-Gate (76,20; days via mountain track) |
| Old Forts Track (NE) | (100,20) | Old Iron forts / D27 (78,15; weeks; dangerous) |
| Teeth Pass (N) | (45,0) | Sunder Ocean / off-grid (near-impassable) |
| Deep Cuts Road (from Mine Road head) | (95,65) | Deep Cuts (71,21; days via mining road) |

## Services

| Service | Where | Details |
|---|---|---|
| Rest | Mercenary Barracks-adjacent inn (65,40) | 2sp/night; monitored; shared sleeping; no frills |
| Resupply | Market Row (35,75) | weapons, tools, cold-weather gear, rations; no magic items |
| Healing | Market Row (one ex-Remnant medic) | mundane healing only (Cure Wounds); charges 5sp/session |
| Information | Ore-Yards or Hold Gate | Mully Karr (visiting; DC 16); Brask's gate-guards (DC 14) |
| Faction contact | Warlord's Hall | Brask (Persuasion DC 16 for audience); Wenna Stone (periodic; DC 17) |

## Law and Threat DCs

- **Entering the Hold:** mandatory gate challenge — state purpose; Persuasion DC 14 (routine business) or DC 16 (requesting audience with Brask himself).
- **Moving toward the Mine Road head without authorization:** soldiers stop you; Persuasion DC 15 or turn back (Brask's road rules are non-negotiable).
- **Entering the Deep Cuts without Brask's permit:** DC 17 Persuasion or outright blocked; bribery DC 14 (risky if Brask finds out).
- **Violent act within walls:** immediate overwhelming response — Brask himself (**Champion/Veteran-like**, AC 18, ~104 HP) plus 30+ soldiers; Survival DC 17 to escape the hold walls.
- **Challenging Brask's authority publicly:** social consequence (expelled from hold; all future DCs +3 until status repaired).

## Key NPC Links

| NPC | Role | Location | Notes |
|---|---|---|---|
| Warlord "Iron" Brask | hold-lord; Tier 1 combat profile | Warlord's Hall (45,30) | Persuasion DC 16; respects demonstrated competence |
| Ore-Factor Mully Karr | metals-trader; information broker | Ore-Yards (50,60; visiting from Karran-Gate) | Persuasion DC 16; bribable with silver |
| Reclaimer-Captain Wenna Stone | Remnant expedition-captain; turnable | periodic visits to Warlord's Hall | Persuasion DC 17; trusts competence over affiliation |

## Quest Hooks

- **Q_KM_001 — The Deep That Went Wrong:** first hook arrives at the Ore-Yards when shaking miners come up wrong from the Deep Cuts gallery; the "mine-mad" condition is visible before the player commits (L9).
- **Q_KM_002 — Scout the Old Iron Forts:** Brask wants the forts assessed (the dead stir; his road-patrols are returning changed); he hires outside observers (L10+; access to D27 approach).
- **Employment contract:** the Mercenary Barracks posts work on the board daily — road-escort, mine-guard, Teeth-pass scouting (DC 14 Persuasion to qualify; 5gp/day starting rate).

## Encounter / Treasure References

- Encounter: warlord soldiers (**Guard / Veteran-like**, AC 14–16, ~22–65 HP); mercenaries (**Veteran-like**); Old Iron fort undead/constructs at D27 (**Wight / Animated Armor-like**, CR 5–12); see `13_encounters_and_bestiary/` plains, undead, construct lines at L9+.
- Treasure: `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` Tier 2–3 (L9–16) ore-yard salvage; Brask's reward (gold, iron, passage-permit); "old iron" salvage from D27 (Remembrance-adjacent relics — Thin-touch risk; use relic rules).

## Player-Safe Layer

The fortress gate, the warlord's hall, the mercenary barracks, the ore-yards, the market row, the mine road head. The town reads as iron-law frontier: no sentiment, everything costs silver, the warlord sees all. The Old Iron forts are mentioned as "bad ground NE" — the mine-mad condition is visible but not explained.

## DM-Only Layer (NEVER on the player map)

- The Old Iron forts (D27) are **peripheral Concord road-forts** — their stirring dead and "old iron" hum are M2/M5-oblique echoes of the harvest's NE reach. NEVER the keystone, NEVER the machine.
- Brask knows the ground went wrong before he sealed the Deep Cuts gallery; his real fear is that the "bad ground" spreads to his water supply. He is not aware of the Concord connection.
- No apex geometry here. The endgame is vertical beneath Hollowmere (NW only).

## Unresolved Map Gaps

- The fortress's internal room-layout is not deep-built; the notable-areas grid is sufficient for eagle-test arrival.
- The Iron Road's exact condition between here and Karran-Gate depends on Brask's current politics.

## Related Files

- Region: [`../../04_world_atlas/region_map_packets/REGION_KARRAN_MARCHES.md`](../../04_world_atlas/region_map_packets/REGION_KARRAN_MARCHES.md)
- NPCs: [`../../08_npcs/by_region/KARRAN_MARCHES_NPCS.md`](../../08_npcs/by_region/KARRAN_MARCHES_NPCS.md)
- Quests: [`../../09_quests/by_region/KARRAN_MARCHES_QUESTS.md`](../../09_quests/by_region/KARRAN_MARCHES_QUESTS.md)
- D-site: [`../../10_dungeons_and_ruins/THE_KARRAN_OLD_IRON_FORTS.md`](../../10_dungeons_and_ruins/THE_KARRAN_OLD_IRON_FORTS.md)
