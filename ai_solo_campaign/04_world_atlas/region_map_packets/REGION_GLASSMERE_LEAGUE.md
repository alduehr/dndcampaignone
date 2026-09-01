# REGION_GLASSMERE_LEAGUE.md — Regional Map Packet

---
type: region
secrecy: mixed
status: static
region: Glassmere League
level_range: 9-13
related: [../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, ../FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../MAP_FEATURE_REGISTRY.md, ../../08_npcs/by_region/GLASSMERE_LEAGUE_NPCS.md, ../../09_quests/by_region/GLASSMERE_LEAGUE_QUESTS.md, ../../06_settlements/city_map_packets/GLASSMERE_CITY_MAP.md, ../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md, ../../10_dungeons_and_ruins/THE_GLASSMERE_RELIQUARY_VAULTS.md, ../../10_dungeons_and_ruins/THE_THREE_BRIDGES_COUNTING_DEEP.md]
tags: [type:map, secrecy:mixed, function:cartography, map-packet, region-map, glassmere-league]
---

> **Secrecy classification:** Mixed. The Reliquary Vaults and the Three Bridges Counting-Deep are urban Concord-relic / banking-vault sites — relic-trade and scholarly secrets, never the keystone, the machine, the Concord Deep, or the Hollow Court (NW only, vertical beneath Hollowmere). Never hand this file directly to the player; render only the Player-Safe Layer.

## Region: Glassmere League (MF-007)

- **Local grid:** 0–100, where **(0,0) = NW corner of the region frame, X = east, Y = south** (Y=0 top). (100,100) = SE.
- **Full-continent bounds this local grid maps to:** render-grid **X 50–60, Y 45–55** (centroid full (55,50)); from `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §10`.
- **Local↔full transform:** `local_X = (full_X - 50) / 10 * 100`; `local_Y = (full_Y - 45) / 10 * 100`. (Inverse: `full_X = 50 + local_X/100*10`; `full_Y = 45 + local_Y/100*10`.)
- **One-sentence identity:** A confederacy of free river-cities grown rich on the Glasswater — the Cinder Ledger's true heartland and the "real" urban Orrun, a city-world of banks, guilds, and old wealth that denies the frontier crisis by sheer prosperity.

## Neighboring Regions

| Direction | Region |
|---|---|
| NW (down-river) | Verdance Reaches → Caradril → NW cluster |
| S | Marrowdowns |
| SE (down the Glasswater) | toward Saltmere Reaches / Hollow Gulf (via the Glasswater Run) |
| NE | Greatspine foothills → Concord Heartlands (Crown Road, contested) |

## Terrain Zones (local polygons)

| Zone | Type | Local centroid | Full-grid | Description |
|---|---|---|---|---|
| The Glasswater valley | great river city-corridor | (50,50) | (55,50) | The continent's main commercial artery; Glassmere city straddles it; wharves, exchanges, banks. |
| The up-river league shelf | settled river-terraces | (20,20) | (52,47) | Prosperous tilled terraces and the smaller league-city of Sennfort. |
| The down-river league plain | river plain / orchards | (80,80) | (58,53) | Rich plain around Cairnwater, opening toward the Glasswater Run south. |
| The Glasswater canal-country | Concord-built canals | (55,55) | (55.5,50.5) | Old Concord canals and locks that feed the League's wealth (infrastructure, not mystery). |

## Water Features

| Feature | Type | Local | Full-grid | Flow |
|---|---|---|---|---|
| The Glasswater (river) | great navigable river | corridor NW→SE | source (58,40) Greatspine → Glassmere (55,50) → Hollow Gulf delta (64,88) | the main artery; flows SE to the Gulf |
| The Three Bridges reach | city river-crossings | (50,50) | (55,50) | the banking quarter's three great spans across the Glasswater |
| Concord canals | engineered waterways | (55,55) | (55.5,50.5) | feed the exchange-wharves; lock-fed |

## Roads / Routes (local polylines)

| Route | Local waypoints | Full-grid | Travel time | Notes |
|---|---|---|---|---|
| Verdance Road (in) | NW edge → (50,50) Glassmere | (43,43) Nine Locks → (55,50) Glassmere | from Caradril ~12–16 days | the corridor up from the frontier |
| Glasswater Run (out, S) | (50,50) Glassmere → (80,80) Cairnwater → SE edge | (55,50)→(58,53)→(60,66)→(66,90) Hollow Gulf | Glassmere→Hollow Gulf ~3–4 weeks by river | the great commercial run to the southern ports |
| Greatspine Crown Road (NE, contested) | (50,50) Glassmere → NE edge | (55,50)→(62,56) Concord Heartlands | days into the contested ruin-country | mark CONTESTED; toward the Heartlands |
| Salt Road (junction) | brushes S toward the Saltmere | (37,54)→(60,70) | — | the cross-continent salt route brushes the region's S |

## Bridges / Fords / Ferries / Locks

| Feature | Type | Local | Full-grid | Notes |
|---|---|---|---|---|
| The Three Bridges | three great city bridges + banking quarter | (50,50) | (55,50) | the banking district; D29 Counting-Deep vault beneath |
| Glasswater exchange-locks | Concord canal-locks | (55,55) | (55.5,50.5) | lift cargo to the wharf-canals |
| Sennfort river-bridge | league-city span | (20,20) | (52,47) | up-river crossing |
| Cairnwater landing | down-river wharf | (80,80) | (58,53) | head of the Glasswater Run south |

## Settlements

| Settlement | Type | Local | Full-grid | Anchor source / file |
|---|---|---|---|---|
| Glassmere | major city (league capital) | (50,50) | (55,50) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (gl.glassmere); NPC/quest hub; city packet `GLASSMERE_CITY_MAP.md` |
| Sennfort | smaller league-city (up-river) | (20,20) | (52,47) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (gl.sennfort) |
| Cairnwater | smaller league-city (down-river) | (80,80) | (58,53) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (gl.cairnwater) |

> Glassmere's internal districts (the Floor, the Three Bridges, the Reliquary, Lowwater) are **city locales within the single Glassmere marker** — not separate full-continent markers (per the anchor file Table 3). They appear on the Glassmere city map, not as continent markers.

## Dungeons / Adventure Sites

| Site | Local | Full-grid | Surface marker | Player-map |
|---|---|---|---|---|
| D28 The Glassmere Reliquary Vaults | (60,30) | (56,48) | the Reliquary chapter-house building | urban / visible (building) |
| D29 The Three Bridges Counting-Deep | (50,50) | (55,50) | the Three Bridges banking quarter | urban |

## Ruins / Wilderness Landmarks

| Landmark | Local | Full-grid | Notes |
|---|---|---|---|
| The Reliquary | (60,30) | (56,48) | Remnant grand chapter-house; greatest relic-collection on the continent (Q_GL_004) |
| The Floor | (50,50) | (55,50) | the famous merchant-exchange (Q_GL_001) |
| Lowwater | (40,70) | (54,52) | poor riverside district; old urban Mourners' presence (Q_GL_005/006) |
| Concord canal-works | (55,55) | (55.5,50.5) | old infrastructure; a "humming cabinet" relic surfaces here (Q_GL_007; M2-oblique) |

## Level Range And Solo Danger

- **Recommended level:** 9–13.
- **Expected solo danger:** Low. This is a *city-world* — danger is intrigue, finance, espionage, and faction-war, not monsters. Most quests have no required fight.
- **Lethal-at-low-level zones (telegraphed):** none of the wilderness kind. The dangers are political (the Ledger's serene reach; the Glass Ear selling the player out; Reliquary wards), and a single "humming"/manifesting relic (Q_GL_007) is telegraphed and containable. A blown counting-house infiltration or sealed-vault attempt draws **Guard/Spy-like** security, not lethal ambush.
- **Telegraphing:** crossing the Ledger, the bank, or the Reliquary is signaled by escalating institutional pressure (credit frozen, agents tailing, wards raised), giving the solo PC room to retreat or change tack.

## Encounter And Hazard Mechanics

- **Encounter themes (stat references):** League/Ledger bank-guards and agents (**Guard-like** AC 14–16, **Spy-like** AC 12 cut-outs; a **Veteran-like** enforcer-captain at L13 — cf. the Mauld Tallow type in `08_npcs/by_region/STAGE_9_MAJOR_NPCS.md` and faction-capability profiles); hired toughs in Lowwater (**Thug/Guard-like**); a minor Remembrance-manifestation from a waking relic (scale a **Memory-Echo Haunt** from `SUNDERING_REACH_ENCOUNTERS.md` to L10–13, AC 12). Use `13_encounters_and_bestiary/GLASSMERE_LEAGUE_ENCOUNTERS.md` and `13_encounters_and_bestiary/TRAVEL_ENCOUNTERS.md` for generic urban/terrain lines.
- **Environmental/social hazards:** Reliquary wards (Arcana/Abjuration interaction, DC 18 to bypass safely); a "humming" raw Remembrance relic may inflict **Thin-touch** on prolonged handling (Stage 3 condition). Counting-house/vault security: Stealth DC 16–18.
- **Investigation/social DCs (typical):** Persuasion/Insight DC 15–18 (Glass, Holt, Mareth Senn); Investigation DC 17–18 (Ledger paper-trail, relic provenance); Deception DC 16–17 (the Ear's bargains). See the quest file for per-quest DCs.
- **Scaling:** L9 — pure social intrigue. L13 — the bank-war and Remnant schism become actionable continental levers; security and stakes escalate.

## Local Labels (player map)

The Glassmere League; Glassmere; Sennfort; Cairnwater; the Glasswater (river); the Verdance Road; the Glasswater Run; the Crown Road (mark contested). On a Glassmere city map: the Floor, the Three Bridges, the Reliquary, Lowwater. Mark the Reliquary as a notable building.

## Player-Safe Layer

- Visible: the three league-cities, the Glasswater and its routes, the Reliquary as a notable chapter-house, the bridges and canals, the up-river/down-river framing.
- The League is openly prosperous and skeptical of "down-river superstition." Nothing here is telegraphed as supernaturally dangerous except a single eerie "humming" relic in a private cabinet (Q_GL_007), framed as "old, strange, waking."

## DM-Only Layer (NEVER on the player map)

- The Reliquary Vaults (D28) hold the continent's greatest relic-collection and a **sealed-vault fragment** Mareth Senn fears (M6-oblique scholarly window) — deep history/language, never the live mechanism.
- The Three Bridges Counting-Deep (D29) is a banking-vault dungeon (Ledger heartland wealth); relic-trade and finance, not apex truth.
- A "humming cabinet" relic (Q_GL_007) is a **raw Remembrance relic reactivating** like every node, far up the chain (M2 continental corroboration) — never explain Remembrance/the harvest to the player.
- Mother Wenna Lowwater carries the **old-songs network fragment** ("the grey hands took the dead") — M6-oblique folk-memory ONLY; no mechanism, no Court, no keystone.
- The Ledger's true continental scale and the Holt-bank counterweight are strategic content (Q_MAJOR_004), not map features.
- No apex geometry exists here. The endgame is vertical beneath Hollowmere (NW only).

## Unresolved Map Gaps

- Glassmere's internal street/district geometry lives in the city packet (`GLASSMERE_CITY_MAP.md`); the Floor/Three Bridges/Reliquary/Lowwater are placed here only as in-city locales, not surveyed region coordinates.
- Sennfort and Cairnwater are named-in-passing league-cities, not deep-built; their internal layouts are improv-safe.
- The Glasswater's mid-course meanders (toward the Gulf) are illustrative beyond the region edge.

## Related Files

- NPCs: [`../../08_npcs/by_region/GLASSMERE_LEAGUE_NPCS.md`](../../08_npcs/by_region/GLASSMERE_LEAGUE_NPCS.md)
- Quests: [`../../09_quests/by_region/GLASSMERE_LEAGUE_QUESTS.md`](../../09_quests/by_region/GLASSMERE_LEAGUE_QUESTS.md)
- City packet: [`../../06_settlements/city_map_packets/GLASSMERE_CITY_MAP.md`](../../06_settlements/city_map_packets/GLASSMERE_CITY_MAP.md)
- D-sites: [`../../10_dungeons_and_ruins/THE_GLASSMERE_RELIQUARY_VAULTS.md`](../../10_dungeons_and_ruins/THE_GLASSMERE_RELIQUARY_VAULTS.md) · [`../../10_dungeons_and_ruins/THE_THREE_BRIDGES_COUNTING_DEEP.md`](../../10_dungeons_and_ruins/THE_THREE_BRIDGES_COUNTING_DEEP.md)
- Authority: [`../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`](../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md) · [`../FULL_CONTINENT_SETTLEMENT_ANCHORS.md`](../FULL_CONTINENT_SETTLEMENT_ANCHORS.md) · [`../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
