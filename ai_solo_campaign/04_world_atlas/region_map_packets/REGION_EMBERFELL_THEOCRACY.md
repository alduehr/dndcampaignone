# REGION_EMBERFELL_THEOCRACY.md — Regional Map Packet

---
type: region
secrecy: mixed
status: static
region: Emberfell Theocracy
level_range: 12-16
related: [../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, ../FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../MAP_FEATURE_REGISTRY.md, ../../06_settlements/city_map_packets/ASHFAST_CITY_MAP.md, ../../08_npcs/by_region/EMBERFELL_THEOCRACY_NPCS.md, ../../09_quests/by_region/EMBERFELL_THEOCRACY_QUESTS.md, ../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md, ../../10_dungeons_and_ruins/THE_EMBERFELL_CALDERA_DESCENT.md, ../../10_dungeons_and_ruins/THE_CINDERN_WASTE_BURIED_WORKS.md]
tags: [type:map, secrecy:mixed, function:cartography, map-packet, region-map, emberfell, ashfast, cindern-waste]
---

> **Secrecy classification:** Mixed. The Caldera Descent (D22) and the Cindern Waste Buried Works (D36) hold only far-south echoes of the crisis, never the keystone. The Emberfell fire-theocracy is a mirror of how the Concord corrupted rites — the fire-faith's harvest of the dead (pyres, ash-absorption) is a thematic echo of the main crisis, never the same machine. Ashfast's closed theocracy makes the DM-only layer especially important. Never hand this file directly to the player; render only the Player-Safe Layer.

## Region: Emberfell Theocracy / Ashfast (MF-014)

- **Local grid:** 0–100, where **(0,0) = NW corner of the region frame, X = east, Y = south** (Y=0 top). (100,100) = SE.
- **Full-continent bounds this local grid maps to:** render-grid **X 76–86, Y 56–68** (centroid full (81,62)); from `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §10`.
- **Local↔full transform:** `local_X = (full_X - 76) / 10 * 100`; `local_Y = (full_Y - 56) / 12 * 100`. (Inverse: `full_X = 76 + local_X/100*10`; `full_Y = 56 + local_Y/100*12`.)
- **One-sentence identity:** A closed volcanic fire-theocracy built on a pre-Concord faith that harvests the dead through fire — alien, self-sufficient, and sitting on top of the oldest pre-Concord ruins the campaign contains.

## Neighboring Regions

| Direction | Region |
|---|---|
| N | Karran Marches (across the Karran Teeth SE approach) |
| NW | Hethewald Free Holds |
| W | Concord Heartlands / Saltmere Reaches (across the Cindern Waste margin) |
| SW | Hollow Gulf Ports (across the Glass Coast) |
| S | the Calm Reach / Glass Coast (warm open sea) |
| E | the Cindern Waste / Glass Coast (off-grid; the campaign's SE limit) |

## Terrain Zones (local polygons)

| Zone | Type | Local centroid | Full-grid | Description |
|---|---|---|---|---|
| The Emberfells caldera highland | volcanic highland | (50,40) | (81,60.8) | The volcanic rise; the active caldera; lava-vent country; the D22 site. |
| Ashfast terrace | fortress-temple-city ground | (40,50) | (80,62) | The defensible terrace below the caldera where the theocracy's capital sits. |
| The Cindern Waste | ash badland (SE) | (80,83) | (84,66) | The rain-shadow ash desert downwind of the caldera; the D36 site lies buried here. |
| The Ash Roads country | pilgrim-road highland | (20,25) | (78,58.5) | The highland approach to Ashfast via the pilgrim-ways; shrines and warden-posts. |
| The Glass Coast margin | volcanic-glass coastal strip | (60,95) | (82,67.2) | Where the Emberfells meet the Calm Reach; obsidian beaches, hot springs. |

## Water Features

| Feature | Type | Local | Full-grid | Flow |
|---|---|---|---|---|
| Caldera hot springs | volcanic hot-water seeps | (50,35) | (81,60.2) | Near the caldera; hot, sulfurous; sacred to the pyre-faith |
| Ash Roads cold springs | highland springs (W side) | (20,25) | (78,58.5) | The pilgrim-road's only reliable water; tended by the Ash Roads wardens |
| Glass Coast tidal pools | obsidian-rimmed pools | (60,95) | (82,67.2) | Hot and mineral-rich; local fishing and swimming only for the initiated |

## Roads / Routes (local polylines)

| Route | Local waypoints | Full-grid | Travel time | Notes |
|---|---|---|---|---|
| The Ash Roads (W approach, main pilgrim-way) | W edge → (20,25) Ash Roads approach → (40,50) Ashfast Pilgrim Gate | (76,58.5)→(78,58.5)→(80,62) | weeks from lowlands | The only sanctioned approach; warden-posts every day; the Q_ET_001 route |
| Cinder Road (E, to Cinderhold) | (40,50) Ashfast → (70,75) Cinderhold | (80,62)→(83,65) | 2–3 days | The industrial road; obsidian and ore |
| Glass Coast Road (S) | (40,50) Ashfast → S edge | (80,62)→(80,68) Glass Coast | days–weeks | the southern exit; leads to Glass Coast harbors and overseas |
| Cindern Waste Track (E) | (70,75) Cinderhold → (80,83) Waste edge | (83,65)→(84,66) | days (dangerous) | the approach to D36; warden-forbidden; lethal without water and protection |

## Bridges / Fords / Ferries / Locks

| Feature | Type | Local | Full-grid | Notes |
|---|---|---|---|---|
| Ashfast Pilgrim Gate | fortress gate (warden-controlled) | (30,55) | (79,62.6) | The entry to the closed theocracy; Q_ET_001 passage required |
| Cinder Gate | secondary fortress gate | (55,50) | (81.5,62) | Faces Cinderhold; controlled by pyre-soldiers |
| Caldera rim-path | narrow warden-patrol ledge | (50,30) | (81,59.6) | Patrolled; access requires safe-conduct; one wrong step = caldera |

## Settlements

| Settlement | Type | Local | Full-grid | Anchor source / file |
|---|---|---|---|---|
| Ashfast | fortress-temple-city (theocracy capital) | (40,50) | (80,62) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (ef.ashfast); city packet `ASHFAST_CITY_MAP.md`; NPC/quest hub |
| Cinderhold | volcanic mining town | (70,75) | (83,65) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (ef.cinderhold) |
| The Ash Roads (approach area) | pilgrim-road warden-post string | (20,25) | (78,58.5) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (ef.ash_roads); route label; warden-posts only |

> Ashfast's full district layout, services, law/threat DCs, and NPC links are in `ASHFAST_CITY_MAP.md`.

## Dungeons / Adventure Sites

| Site | Local | Full-grid | Surface marker | Player-map |
|---|---|---|---|---|
| D22 Emberfell Caldera Descent | (50,42) | (81,61) | active caldera rim (NE; visible volcano) | visible (volcano symbol) |
| D36 Cindern Waste Buried Works | (80,83) | (84,66) | ash-buried rubble mound in the Waste (barely visible) | label only ("buried works"; warden-forbidden) |

## Ruins / Wilderness Landmarks

| Landmark | Local | Full-grid | Notes |
|---|---|---|---|
| The Emberfells Caldera (D22) | (50,42) | (81,61) | active volcano; the theocracy's sacred fire-source; D22 goes down through the lava-tube system |
| The Cindern Waste Buried Works (D36) | (80,83) | (84,66) | ash-drowned Concord-era works buried in the Waste; Q_ET_006/007; M2-oblique |
| The Pyre Grounds | (55,47) | (81.5,61.6) | Ashfast's ritual fire-ground; visible from the Ash Roads; where the dead are publicly pyred |
| The Bone-Arch | (25,30) | (78.5,59.6) | a natural volcanic-rock arch spanning the Ash Roads; a traditional shrine-point |

## Level Range And Solo Danger

- **Recommended level:** 12–16.
- **Expected solo danger:** Extreme within Ashfast (social/political danger — a wrong word here is fatal); high on the Ash Roads (warden patrols, volcanic hazards); extreme at the Caldera (D22, lava-vent traps, theocracy defenders); extreme in the Cindern Waste (D36, ash-exposure, warden-forbidden).
- **Lethal-at-low-level zones (telegraphed):** the **Caldera** (D22; approach requires theocracy safe-conduct; the caldera itself is lethal terrain), the **Cindern Waste** (ash-exposure; warden patrols shoot first), and **any religious offense in Ashfast** (the Pyre-Warden's response is overwhelming). All heavily telegraphed: the wardens name the rules, the pyre-soldiers are visible everywhere, and the closed-theocracy architecture says "you are watched."
- **Telegraphing:** the Q_ET_001 Ash Roads passage is the mandatory on-ramp; the warden-post gauntlet teaches the rules before the city is reached; the caldera's danger is visible and the theocracy explicitly forbids approach without a guide.

## Encounter And Hazard Mechanics

- **Encounter themes (stat references):** see `ASHFAST_CITY_MAP.md` for the city-specific encounter/threat table. Regional: Ash Roads warden-patrols (**Guard / Veteran-like**, AC 15–16; fire-weapons); pyre-soldiers (**Cultist / Veteran-like**, AC 15–16, ~44–52 HP; fight-to-the-death); volcanic hazards (lava-vent; falling ash). Pyre-Warden Sef Embren (**Inquisitor / Veteran-Priest-like**, AC 18, ~85 HP) is the boss-class regional enforcer. Use `13_encounters_and_bestiary/` fire-themed lines at L12+.
- **Environmental hazards:** ash-fall visibility (Perception penalties −2 during ash-fall); caldera proximity (Constitution DC 14, heat exhaustion; near the active vents DC 17); Cindern Waste dehydration (as Bonepan Flats, but also ash-lung — Constitution DC 15 per day); lava-vent traps (Dexterity DC 15, 3d10 fire); Thin-touch at D22/D36 relic depths.
- **Social DCs (typical):** see `ASHFAST_CITY_MAP.md`. Regional: Persuasion DC 17 (Sef Embren — Ash Roads passage); Persuasion DC 18 (Vole Cindra — theocracy access); Insight DC 17 (Mira Cindra's double-speak). Per-quest DCs in `EMBERFELL_THEOCRACY_QUESTS.md`.
- **Scaling:** L12 — Ash Roads passage and Ashfast entry (Q_ET_001). L16 — Caldera Descent (D22), the Cindern Waste Buried Works (D36), and the theocracy's hidden pre-Concord record.

## Local Labels (player map)

The Emberfell Theocracy (region label, ONE); the Emberfells (volcanic highland fill); Ashfast; Cinderhold; the Caldera (volcano symbol); the Cindern Waste (ash-badland fill, SE); the Ash Roads (route label, W approach); the Cinder Road (route, E); the Glass Coast Road (route, S); the Cindern Waste Buried Works (label "buried works"; forbidden annotation).

## Player-Safe Layer

- Visible: the fortress-temple-city on its volcanic terrace, the active caldera above it, the ash-badland SE, the pilgrim-road approach, Cinderhold as the industrial town. The region reads as an alien, closed, fire-faith theocracy — self-sufficient, intimidating, and sitting on a volcano.
- The fire-faith's pyring of the dead is presented as the local death-rite — the player can find it familiar-but-wrong (a rite that "works" in its own terms but differently than the Mourners' faith).

## DM-Only Layer (NEVER on the player map)

- D22 (Caldera Descent) holds an **M3/M5 echo** — pre-Concord fire-rite ruins beneath the caldera that corroborate the crisis's SE reach; NEVER the keystone or the machine.
- D36 (Cindern Waste Buried Works) holds **M2-oblique Concord-peripheral records** — scattered ash-drowned Concord supply-works; the theocracy has no idea they are there; they hum faintly.
- The theocracy's fire-faith is a **thematic mirror** of the campaign crisis: the fire-faith also "harvests" the dead (through pyres and ash-absorption) but does so with consent and visible rites. This is the "corrupted mirror" of what the Concord became; the contrast is never stated explicitly.
- Ash-Hierophant Vole Cindra is a **thematic mirror of the Hollow Court** — he rules through control of death-rites and fears what happens if the "old works" (D22) stir. He is not connected to the Court; the mirror is thematic only.
- Volcanic hazard zones, lava-tube access beneath the caldera (D22 approach), and ash-fall risk bands (SE): DM annotations, not player-map features.
- No apex geometry here. The endgame is vertical beneath Hollowmere (NW only).

## Unresolved Map Gaps

- Ashfast's internal district and building layout is in `ASHFAST_CITY_MAP.md`; this packet positions the city and the region.
- The caldera's active lava-flows shift year to year; D22 is position-deterministic, but the surface approach changes seasonally.
- The Cindern Waste's western and southern margins are approximate; the D36 site's exact burial depth is revealed by exploration.

## Related Files

- City packet: [`../../06_settlements/city_map_packets/ASHFAST_CITY_MAP.md`](../../06_settlements/city_map_packets/ASHFAST_CITY_MAP.md)
- NPCs: [`../../08_npcs/by_region/EMBERFELL_THEOCRACY_NPCS.md`](../../08_npcs/by_region/EMBERFELL_THEOCRACY_NPCS.md)
- Quests: [`../../09_quests/by_region/EMBERFELL_THEOCRACY_QUESTS.md`](../../09_quests/by_region/EMBERFELL_THEOCRACY_QUESTS.md)
- D-sites: [`../../10_dungeons_and_ruins/THE_EMBERFELL_CALDERA_DESCENT.md`](../../10_dungeons_and_ruins/THE_EMBERFELL_CALDERA_DESCENT.md) · [`../../10_dungeons_and_ruins/THE_CINDERN_WASTE_BURIED_WORKS.md`](../../10_dungeons_and_ruins/THE_CINDERN_WASTE_BURIED_WORKS.md)
- Authority: [`../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`](../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md) · [`../FULL_CONTINENT_SETTLEMENT_ANCHORS.md`](../FULL_CONTINENT_SETTLEMENT_ANCHORS.md) · [`../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
