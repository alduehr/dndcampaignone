# SETTLEMENT_CINDERHOLD_MAP.md — Settlement Map Packet

---
type: settlement
secrecy: mixed
status: static
region: Emberfell Theocracy
settlement: Cinderhold
level_range: 12-16
related: [../../04_world_atlas/region_map_packets/REGION_EMBERFELL_THEOCRACY.md, ../../06_settlements/city_map_packets/ASHFAST_CITY_MAP.md, ../../04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../../08_npcs/by_region/EMBERFELL_THEOCRACY_NPCS.md, ../../09_quests/by_region/EMBERFELL_THEOCRACY_QUESTS.md]
tags: [type:map, secrecy:mixed, function:cartography, settlement-map, map-packet, cinderhold, emberfell]
---

> **Secrecy classification:** Mixed. The Cindern Waste Buried Works (D36) are ash-drowned Concord peripheral works — M5/M6-oblique fragment, never the keystone. Cinderhold is the theocracy's industrial arm: the warden-checkpoint is lighter here than at Ashfast, but the faith's law still governs. Never hand directly to the player.

## Settlement: Cinderhold (Emberfell Theocracy — volcanic mining town)

- **Local grid:** 0–100 (X east, Y south); (0,0) = NW corner. Industrial mining town on the volcanic slope below Ashfast; the Cinder Gate faces W toward Ashfast; mine-head E toward the caldera; Waste Track SE.
- **Full-continent position:** render-grid (83,65).
- **Population / scale:** ~700–1,000 miners, wardens, and their dependents; a working industrial town, not a faith-center.
- **Water/road relationship:** on the **Emberfells** volcanic slope; cold-spring water from the Ash Roads W (80,62 Ashfast) is piped down; the **Ash Roads** connect W to Ashfast; the **Cinder Road** runs E toward the mine-head; the **Waste Track** leads SE toward the Cindern Waste (warden-forbidden).

## Layout / Notable Areas

| Area | Local | Notes |
|---|---|---|
| The Cinder Gate | (20,35) | theocracy checkpoint; passes from Ashfast required; warden inspection |
| The Ore-Exchange | (50,35) | Doss Ashfast's trading house; obsidian, iron ore, ash-glass, volcanic tools |
| The Mine-Head | (75,40) | the active working face on the volcano side; warden-supervised |
| The Ash Roads Station | (40,65) | pilgrim-way waypost connecting to Ashfast W; the gossip hub |
| The Pyre-Post | (65,70) | small theocracy shrine; miners' pyres held here when someone dies underground |
| The Waste Track head | (85,80) | toward D36 and the Cindern Waste; warden-forbidden; visible but blocked |

## Entrances / Exits

| Exit | Local edge | Leads to |
|---|---|---|
| Cinder Road (W, to Ashfast) | (0,35) | Ashfast (80,62; 2-3 days via Ash Roads) |
| Mine-Head approach | (100,35) | the active caldera-side workings (warden-supervised access only) |
| Ash Roads (S approach) | (35,100) | the Ash Roads descent toward the W lowlands |
| Waste Track (SE, forbidden) | (100,80) | Cindern Waste / D36 (84,66; days; near-lethal without preparation) |

## Services

| Service | Where | Details |
|---|---|---|
| Rest | miner's lodges near the Ore-Exchange (50,50) | 2sp/night; monitored by theocracy wardens; safe for pass-holders |
| Resupply | Ore-Exchange (50,35) | obsidian, ash-glass, volcanic tools, mining equipment, standard rations |
| Healing | Pyre-Post shrine-healer (65,70) | mundane healing only (Cure Wounds); DC 14 to access (requires respectful engagement with the faith's forms) |
| Information | Ore-Exchange or Ash Roads Station | Doss Ashfast (DC 16); Ash Roads pilgrims (DC 12 for rumors from Ashfast) |
| Faction contact | Cinder Gate or Ore-Exchange | theocracy wardens (theocracy law); Doss Ashfast (industrial arm) |

## Law and Threat DCs

- **Entering through the Cinder Gate:** passes from Ashfast preferred; Persuasion DC 15 (plausible work purpose) or DC 17 (no pass, no obvious religious purpose). Ashfast passes provide immediate entry.
- **Religious offense (disrespecting the pyres or shrine):** wardens respond — 20 pyre-soldiers (**Cultist / Guard-like**, AC 15–16, ~22–44 HP); Persuasion DC 17 to walk it back; failure means detention.
- **Attempting to enter the Waste Track:** immediately stopped; Persuasion DC 18 or turned back; "the waste takes the careless" is the standard dismissal.
- **Accessing the Mine-Head without Doss's permit:** warden challenge; Persuasion DC 16 or turn back.
- **Violent act in Cinderhold:** warden response and possible Pyre-Warden Sef Embren deployment (patrol from Ashfast); Sef is **Inquisitor/Veteran-Priest-like**, AC 18, ~85 HP.

## Key NPC Links

| NPC | Role | Location | Notes |
|---|---|---|---|
| Cinder-Master Doss Ashfast | volcanic mining-lord; industrial authority | Ore-Exchange (50,35) | Persuasion DC 16; coin motivates him more than faith |
| Pyre-Warden Sef Embren | theocracy enforcer; Ashfast-based patrol | Cinder Gate (periodic patrol from Ashfast) | Persuasion DC 17 to negotiate access; fights-to-the-death if threatened |
| Ash-Hierophant Vole Cindra | theocracy ruler | NOT at Cinderhold; based at Ashfast — see `ASHFAST_CITY_MAP.md` | all significant theocracy access routes through Ashfast first |

## Quest Hooks

- **Q_ET_001 — The Ash Roads:** Cinderhold is the mandatory Ash Roads waypost en route to Ashfast; this is where travelers get their first theocracy inspection and their first clear view of the caldera (L12; mandatory on-ramp).
- **Q_ET_004 — The Mine Going Wrong:** Doss is losing miners to something in the deep gallery near the caldera edge; he wants outside investigators who won't trigger a theocracy internal-crisis (L13+).
- **Cindern Waste investigation:** Doss knows about the Waste Track and will tell a trusted outsider what the wardens say about D36 — "old ash-works that hum wrong"; approaching D36 is a late-arc mission (L14+; Waste Track is the access).

## Encounter / Treasure References

- Encounter: theocracy wardens (**Guard / Veteran-like**, AC 15–16); pyre-soldiers (**Cultist-like**, AC 15); Pyre-Warden Sef Embren (**Inquisitor-like**, AC 18, ~85 HP); volcanic mine hazards (lava-vent seep, Dexterity DC 15, 3d10 fire; ash-fall visibility penalty); see `13_encounters_and_bestiary/` fire-themed lines at L12+.
- Treasure: `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` Tier 3 (L11–16) volcanic resources; Doss's reward (obsidian-grade tools, rare ash-glass, gold); theocracy passage-permit (opens Ashfast Pilgrim Gate without a full entry check).

## Player-Safe Layer

The warden gate, the ore-exchange, the mine-head with its caldera-view, the ash-roads station with its pilgrims, the pyre-post shrine, and the forbidden waste-track head with its ominous blocked sign. The town reads as industrial, watched, and practical — the faith's presence is real but less visible here than at Ashfast; what's visible is ash-glass and obsidian, not theology.

## DM-Only Layer (NEVER on the player map)

- The Cindern Waste Buried Works (D36) are **ash-drowned Concord peripheral supply-works** — the theocracy has no idea they are there; they hum faintly under the Waste. M2-oblique Concord-peripheral records only; NEVER the keystone.
- Cinder-Master Doss Ashfast is not a Hollow Court agent; he is an industrial opportunist who doesn't ask cosmological questions.
- Volcanic hazard zones and D36's burial depth are DM annotations, not player-map features.
- No apex geometry here. The endgame is vertical beneath Hollowmere (NW only).

## Unresolved Map Gaps

- Ashfast's full district layout, services, and NPC links are in `ASHFAST_CITY_MAP.md`; Cinderhold is a subsidiary industrial town, not a secondary city.
- D36's burial depth and interior are in `THE_CINDERN_WASTE_BURIED_WORKS.md`; this packet positions the surface access.

## Related Files

- Region: [`../../04_world_atlas/region_map_packets/REGION_EMBERFELL_THEOCRACY.md`](../../04_world_atlas/region_map_packets/REGION_EMBERFELL_THEOCRACY.md)
- City: [`../../06_settlements/city_map_packets/ASHFAST_CITY_MAP.md`](../../06_settlements/city_map_packets/ASHFAST_CITY_MAP.md)
- NPCs: [`../../08_npcs/by_region/EMBERFELL_THEOCRACY_NPCS.md`](../../08_npcs/by_region/EMBERFELL_THEOCRACY_NPCS.md)
- Quests: [`../../09_quests/by_region/EMBERFELL_THEOCRACY_QUESTS.md`](../../09_quests/by_region/EMBERFELL_THEOCRACY_QUESTS.md)
- D-site: [`../../10_dungeons_and_ruins/THE_CINDERN_WASTE_BURIED_WORKS.md`](../../10_dungeons_and_ruins/THE_CINDERN_WASTE_BURIED_WORKS.md)
