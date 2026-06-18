# GLASSMERE_CITY_MAP.md — City Map Packet

---
type: settlement
secrecy: mixed
status: static
region: Glassmere League
settlement: Glassmere
level_range: 9-13
related: [../../04_world_atlas/region_map_packets/REGION_GLASSMERE_LEAGUE.md, ../../04_world_atlas/CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, ../../04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md]
tags: [type:map, secrecy:mixed, function:cartography, city-map, map-packet, glassmere]
---

> **Secrecy classification:** Mixed. The Reliquary/Counting-Deep vault truths are DM-only (relic-trade/Script fragments), never the keystone. Never hand directly to the player.

## City: Glassmere — Local City Grid

- **Local grid:** 0–100 (X east, Y south).
- **Full-continent position:** render-grid (55,50). The greatest river-city on the Glasswater; the Glassmere League capital.
- **Canonical decision (justified from canon):** the name **"the Three Bridges"** implies multiple river-crossings, so Glassmere is a **two-bank city** straddling the Glasswater, joined by three bridges. The Floor (merchant-exchange), the Three Bridges (banking quarter), and the Reliquary (Remnant chapter-house) are named anchors; Lowwater is the poor riverside district.

## River Geometry

- **The Glasswater** runs **north-to-south** through the city: enters at local (50,5), flows to local (50,95). The city sits on **both banks** (W bank = X<50, E bank = X>50).

## District Positions

| District | Bank | Local centroid | Identity |
|---|---|---|---|
| The Three Bridges (banking quarter) | both (at the crossings) | (50,45) | banking; the league's money; the Counting-Deep below |
| The Floor (merchant exchange) | W bank | (35,40) | the commercial exchange-hall district |
| Civic quarter | W bank (upper) | (30,25) | the league council / civic halls |
| Remnant district (the Reliquary) | E bank | (62,35) | Concord Remnant great chapter-house |
| Lowwater (poor district) | E bank (riverside, low) | (60,65) | poor riverside district; old-songs node |
| Commercial/dock quarter | both (riverfront) | (50,60) | river-port, warehouses |

## The Three Bridges (positions)

| Bridge | Local | Notes |
|---|---|---|
| Upper Bridge | (50,30) | civic ↔ Remnant |
| Middle Bridge | (50,45) | the Floor ↔ banking quarter |
| Lower Bridge | (50,60) | dock quarter crossing |

## Docks / River-Port

- River-port and warehouse quays along both banks at local (45–55, 55–70) — the Glasswater Run's chief inland port.

## Main Road Exits

| Exit | Local edge | Leads to |
|---|---|---|
| NW road | (20,15) | the Verdance Reaches / Caradril (Verdance Road) |
| N road | (50,5) up-river | Sennfort (52,47) |
| S road / down-river | (50,95) | Cairnwater (58,53) and the Glasswater Run to the Hollow Gulf |
| SE road | (80,70) | the Concord Heartlands (Crown Road) |

## Named Landmark Positions

| Landmark | Local | Notes |
|---|---|---|
| The Floor (merchant exchange) | (35,40) | trade-floor |
| The Three Bridges (banking quarter) | (50,45) | banking |
| The Reliquary (Remnant chapter-house) | (62,35) | D28 site |
| Lowwater (district) | (60,65) | poor riverside |

## Dungeons / Adventure Sites

| Site | Local | Surface marker | Player-map |
|---|---|---|---|
| D28 Glassmere Reliquary Vaults | (62,35) | the Reliquary chapter-house | urban/visible |
| D29 Three Bridges Counting-Deep | (50,45) | the banking quarter | urban |

## Population and Scale

Glassmere is the greatest inland city on the continent — the League's capital, the hub of the Glasswater trade-axis. Population 45,000–65,000. Cosmopolitan, mercantile, confident. Visitors range from frontier settlers to Surren overseas merchants. Scale: larger than Caradril; feels like a whole world of banks, guilds, and civic halls. Wealth is visible; the Sill's equivalent (Lowwater) is poorer than Caradril's poor.

## Services

| Category | Location | Details |
|---|---|---|
| **Rest (mid)** | The Gilded Lock (local 37,43; merchant quarter) | Innkeep Marrec Stair; 2–4 sp/night; busy, neutral ground for traders and agents alike |
| **Rest (poor)** | Lowwater poor-house (local 58,63) | Almoner Sera Frome; charity-rate; rough |
| **Resupply** | The Floor (local 35,40) | General goods, equipment, reagents; near-any trade good at city prices |
| **Resupply (specialist)** | Commercial/dock quarter (local 50,60) | Rare imports, southern goods, Surren trade items; premium prices |
| **Healing** | Three Thresholds grand temple (local 30,35) | Hierarch Mother Ysolde Glass; standard temple healing rites; 5–50 gp |
| **Healing (folk)** | Mother Wenna Lowwater (local 60,65) | Mourners' folk-rites; free for the poor; no combat healing |
| **Information** | The Glass Ear (via Cut-out "the Quiet Man"; city-wide) | Any secret for the right price; initial contact DC 15 Persuasion or Investigation |
| **Information** | The Floor + Lowwater (general) | Market gossip free; Mourner lore free for respectful visitors |
| **Faction (Remnant)** | The Reliquary (local 62,35); Mareth Senn | Script translation, Concord lore, archive access (gated) |
| **Faction (Ledger)** | Three Bridges (local 50,45); Heartland-Provost Iss Vyre | Banking, credit, trade-charters — Ledger terms |
| **Faction (League civic)** | Civic quarter (local 30,25); Oren Glass, Esh Cairn | League introductions, trade-charters, diplomatic backing |
| **Faction (Holt's bank)** | Three Bridges (local 50,45); Sefwy Holt | Anti-Ledger patronage; credit; high entry bar (DC 17 approach) |
| **City-watch** | Citywide; Watch-Captain Brun Sennfort | Professional but underfunded; bribable at lower ranks |

## Law and Threat

| Situation | DCs / Response |
|---|---|
| Petty crime (pickpocket, brawl) | Watch patrol (Guard-like, AC 14, ~22 HP each); response time 1d6 minutes; bribery DC 12 |
| Serious crime (theft from a chartered firm, assault on a banker) | Watch-Captain Sennfort (Veteran-like, AC 15, ~52 HP); 2–4 guards; bribery DC 17; fine or expulsion |
| Major crime (Ledger vault, civic archive) | League civic-guard (full force); Heartland-Provost Iss Vyre's agents; bribery DC 22+; imprisonment |
| Social leverage (League officials) | DC 15–18 Persuasion (Oren Glass circle); DC 17 Insight to detect Glass's real aims |
| Brokering with Holt | DC 17 Persuasion approach; DC 19 for material backing |
| The Glass Ear (major secret) | DC 20+ Investigation/Persuasion; price always intelligence in return |
| Rest safety | Safe in merchant quarter and civic quarter; Lowwater: DC 14 Perception for nighttime trouble; river-docks: DC 13 |

## Key NPC Links

| NPC | Location | Role in city | Link |
|---|---|---|---|
| League-Factor Oren Glass (GL-M1) | Civic quarter / the Floor | League envoy; the face of League power | `GLASSMERE_LEAGUE_NPCS.md` |
| Banker-Magistra Sefwy Holt (GL-M2) | Three Bridges | Anti-Ledger bank magnate | `GLASSMERE_LEAGUE_NPCS.md` |
| "the Glass Ear" (GL-M3) | Citywide via cut-outs | Continental information-broker | `GLASSMERE_LEAGUE_NPCS.md` |
| Reliquary-Lector Mareth Senn (GL-M4) | The Reliquary | Remnant grand chapter head | `GLASSMERE_LEAGUE_NPCS.md` |
| Mother Wenna Lowwater (GL-M5) | Lowwater (local 60,65) | Mourner eldest; old-songs node | `GLASSMERE_LEAGUE_NPCS.md` |
| Floor-Magister Doss Glass | The Floor (local 35,40) | Exchange presider | `GLASSMERE_LEAGUE_NPCS.md` |
| Civic-Magistra Esh Cairn | Civic quarter | Reform politician | `GLASSMERE_LEAGUE_NPCS.md` |
| Watch-Captain Brun Sennfort | Citywide | City-watch commander | `GLASSMERE_LEAGUE_NPCS.md` |
| Innkeep Marrec Stair | The Gilded Lock (37,43) | Neutral hub innkeeper | `GLASSMERE_LEAGUE_NPCS.md` |

## Quest Hooks (3)

1. **Q_GL_001 — The League's Overture** (Lvl 9–11): League-Factor Oren Glass offers the player a commission as courier for a League trade-overture to Caradril — but its fine print has Ledger fingerprints and a reform councilor is warning it be stopped. (`09_quests/by_region/GLASSMERE_LEAGUE_QUESTS.md`)

2. **Q_GL_002 — The Bank and the Ledger** (Lvl 10–12): Banker-Magistra Sefwy Holt wants proof of Cinder Ledger malfeasance. A frontier player carrying M3 evidence already holds the key — but allying with Holt trades one monopolist for another. (`09_quests/by_region/GLASSMERE_LEAGUE_QUESTS.md`)

3. **Q_GL_003 — The Face of the Ear** (Lvl 10–13): The Glass Ear has a secret the player needs. Finding and meeting the actual broker — not just the cut-outs — requires navigating the city's entire intelligence web. (`09_quests/by_region/GLASSMERE_LEAGUE_QUESTS.md`)

## Encounter and Treasure References

- **Urban social encounters:** city-league tier social scenes; `13_encounters_and_bestiary/CARADRIL_SOCIAL_ENCOUNTERS.md` (adapt for larger city)
- **Criminal/underworld:** "Carp" Maddox's Lowwater rackets; the Glass Ear's cut-outs (Spy-like, AC 12, ~22 HP)
- **Ledger confrontation:** Heartland-Provost Iss Vyre commands Guard/Veteran-like bank-guards (AC 14–16, ~40–52 HP)
- **Dungeon refs:** D28 Glassmere Reliquary Vaults; D29 Three Bridges Counting-Deep — `10_dungeons_and_ruins/`
- **Treasure:** `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` Tier 3 (Lvl 9–13); the Floor and the Reliquary are sources of Concord relics and Remembrance items (gated M3/M5/M6); Holt's bank-backing as a material reward; League trade-charters as income-class rewards

## Player-Safe Layer

The two banks; the Glasswater; the three bridges; the districts; the river-port; the road exits; the Floor, the Reliquary, and the Three Bridges as visible buildings/quarters.

## DM-Only Layer

The Reliquary Vaults (D28) and the Three Bridges Counting-Deep (D29) hold relic-trade/Script fragments (M2/M3/M5) — surface/echo, never the live machine or keystone.

## Unresolved Map Gaps

District boundaries and exact street geometry are illustrative; the city is positioned and services/NPCs are deterministic. Individual building interiors (beyond the named landmarks) are not mapped.

## Related Files

- [`../../04_world_atlas/region_map_packets/REGION_GLASSMERE_LEAGUE.md`](../../04_world_atlas/region_map_packets/REGION_GLASSMERE_LEAGUE.md)
- [`../../08_npcs/by_region/GLASSMERE_LEAGUE_NPCS.md`](../../08_npcs/by_region/GLASSMERE_LEAGUE_NPCS.md)
- [`../../09_quests/by_region/GLASSMERE_LEAGUE_QUESTS.md`](../../09_quests/by_region/GLASSMERE_LEAGUE_QUESTS.md)
- [`../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
- [`../../14_treasure_and_artifacts/REWARDS_BY_LEVEL.md`](../../14_treasure_and_artifacts/REWARDS_BY_LEVEL.md)
