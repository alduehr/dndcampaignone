# REGION_HOLLOW_GULF_PORTS.md — Regional Map Packet

---
type: region
secrecy: mixed
status: static
region: Hollow Gulf Ports
level_range: 10-15
related: [../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, ../FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../MAP_FEATURE_REGISTRY.md, ../../08_npcs/by_region/HOLLOW_GULF_PORTS_NPCS.md, ../../09_quests/by_region/HOLLOW_GULF_PORTS_QUESTS.md, ../../06_settlements/city_map_packets/CALDERPORT_CITY_MAP.md, ../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md, ../../10_dungeons_and_ruins/THE_HOLLOW_GULF_WRECK_REEF.md]
tags: [type:map, secrecy:mixed, function:cartography, map-packet, region-map, hollow-gulf-ports]
---

> **Secrecy classification:** Mixed. The Wreck-Reef and the Drowned Steps (shared with Sallowmarch) hold only faint far-south relic-echoes — NEVER the keystone, the machine, the Concord Deep, or the Hollow Court (NW only, vertical beneath Hollowmere). Never hand this file directly to the player; render only the Player-Safe Layer.

## Region: Hollow Gulf Ports (MF-011)

- **Local grid:** 0–100, where **(0,0) = NW corner of the region frame, X = east, Y = south** (Y=0 top). (100,100) = SE.
- **Full-continent bounds this local grid maps to:** render-grid **X 60–72, Y 86–94** (centroid full (66,90)); from `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §10`.
- **Local↔full transform:** `local_X = (full_X - 60) / 12 * 100`; `local_Y = (full_Y - 86) / 8 * 100`. (Inverse: `full_X = 60 + local_X/100*12`; `full_Y = 86 + local_Y/100*8`.)
- **One-sentence identity:** A string of great warm-water southern port city-states ringing the Hollow Gulf — rival merchant ports, the gateway overseas to Surren and the wider world, and the campaign's most *normal* region, proof that most of the world neither knows nor cares about the frontier crisis.

## Neighboring Regions

| Direction | Region |
|---|---|
| W | Sallowmarch Protectorate (the delta) |
| N (up-river) | Glassmere League (via the Glasswater Run) |
| NE | Saltmere Reaches / Emberfell (far interior) |
| S | the Hollow Gulf / Calm Reach (open sea, overseas to Surren) |

## Terrain Zones (local polygons)

| Zone | Type | Local centroid | Full-grid | Description |
|---|---|---|---|---|
| The Hollow Gulf shore | warm crescent-harbor coast | (50,40) | (66,89) | The great bay; crescent harbors; a thousand ships; the warm mercantile heart. |
| Calderport harbor | major port-city ground | (42,38) | (65,89) | The greatest Gulf port; counting-house terraces over the harbor. |
| Saltgate headland | rival-port ground | (75,62) | (69,91) | The rival city-state on its own headland across the Gulf. |
| The Mardenmouth wharves | delta-mouth port-flats | (25,25) | (63,88) | Where the Mardenflow/Glasswater delta meets the Gulf; wharves, sea-shrines. |
| The open Gulf / Reach Lanes | open warm sea | (60,80) | (67,92) | The shipping lanes south, out to Surren and the overseas world. |

## Water Features

| Feature | Type | Local | Full-grid | Flow |
|---|---|---|---|---|
| The Hollow Gulf | major bay | (50,50) | (66,90) | warm bay; mouth opens S to the Calm Reach |
| The Glasswater/Mardenflow delta-mouth | river deltas → sea | (25,25) | (63,88) | the rivers' terminus; the Mardenmouth wharves |
| The Reach Lanes | open-sea shipping lanes | (60,90) | (67,92) | the sea-routes S to Surren and the Sundered Isles |

## Roads / Routes (local polylines)

| Route | Local waypoints | Full-grid | Travel time | Notes |
|---|---|---|---|---|
| Glasswater Run (in, from up-river) | NW edge → (42,38) Calderport | (55,50) Glassmere → (65,89) Calderport | Glassmere→Calderport ~3–4 weeks by river | the great commercial artery's terminus |
| South Sea Lanes (out, overseas) | (50,40) → S edge (edge-arrow "to Surren / overseas lands") | (66,90) → off-map S | weeks by sea to Surren | the door overseas (dashed edge-arrows) |
| The Reach Lanes (Gulf coastal) | Calderport ↔ Saltgate ↔ the Mardenmouth | (65,89)↔(69,91)↔(63,88) | hours–days by ship | the privateers' and ports' coastal sea-routes |
| Delta-road (W, to Sallowmarch) | (25,25) Mardenmouth → W edge | (63,88) → Sallowmarch delta | days into the fever-delta | the land/water link to the Protectorate |

## Bridges / Fords / Ferries / Locks

| Feature | Type | Local | Full-grid | Notes |
|---|---|---|---|---|
| Calderport harbor-moles & quays | great stone harbor-works | (42,38) | (65,89) | the south's greatest harbor (see `CALDERPORT_CITY_MAP.md`) |
| Saltgate harbor | rival harbor-works | (75,62) | (69,91) | the second city's port |
| Mardenmouth wharf-ferries | delta-mouth ferries | (25,25) | (63,88) | link the wharves to the delta channels |
| Gulf-mouth lighthouse | great sea-light | (60,90) | (67,92) | marks the lanes out to open sea |

## Settlements

| Settlement | Type | Local | Full-grid | Anchor source / file |
|---|---|---|---|---|
| Calderport | major city (greatest Gulf port hub) | (42,38) | (65,89) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (hg.calderport); NPC/quest hub; city packet `CALDERPORT_CITY_MAP.md` |
| Saltgate | rival port city-state | (75,62) | (69,91) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (hg.saltgate) |
| The Mardenmouth | delta-mouth wharf-district / harbor node | (25,25) | (63,88) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (hg.mardenmouth) |

> The Foreign Quarter is a **district within Calderport** (overseas-traders' quarter — per the anchor file Table 3), not a separate marker; it appears on the Calderport city map.

## Dungeons / Adventure Sites

| Site | Local | Full-grid | Surface marker | Player-map |
|---|---|---|---|---|
| D31 The Hollow Gulf Wreck-Reef | (66.7,50) | (68,90) | wreck-reef / drowned harbour-quarter (offshore) | label-only ("wreck-reef") |

> The Drowned Steps (D33, full (54,90)) lie off the Sallowmarch delta just W of this region and are the **Q_HGP_007** salvage target shared with the Sallowmarch — see that region's packet; render once, on the delta coast.

## Ruins / Wilderness Landmarks

| Landmark | Local | Full-grid | Notes |
|---|---|---|---|
| The Wreck-Reef | (66.7,50) | (68,90) | offshore wreck-reef + drowned harbour-quarter; salvage and a faint relic-echo (D31; M2-oblique) |
| The Drowned Steps (shared) | off-frame W/S | (54,90) | submerged Concord sea-causeway off the delta (Q_HGP_007; M2/M5-oblique) |
| Mardenmouth sea-shrines | (25,25) | (63,88) | Tide-Mother Sera's wharf-shrines to the drowned (Q_HGP_006) |

## Level Range And Solo Danger

- **Recommended level:** 10–15.
- **Expected solo danger:** Low ashore (intrigue, trade, port-politics); high at sea (privateers, sea-battles, lethal dives).
- **Lethal-at-low-level zones (telegraphed):** the **open sea-lanes** (privateer raids, sea-battles with Roke Mallin's crew) and the **Wreck-Reef / Drowned Steps dives** are high-danger — telegraphed by sailors' dread ("won't dive past the third step"), the sea-Mourners' warnings, and the reef's wreck-strewn approach. Ashore, the ports are safe and cosmopolitan.
- **Telegraphing:** sea-danger is heavily signaled (the reef's wrecks, divers' refusals, Sera's warnings); the dive can be aborted at each "step," and ship-fights are escapable by speed/guile.

## Encounter And Hazard Mechanics

- **Encounter themes (stat references):** privateer/pirate crews and a Pirate-Captain-tier leader (Roke Mallin: **Pirate-Captain/Veteran-like**, AC 16 ~75 HP, with **Bandit/Veteran-like** crew); port-guards and dock-toughs (**Guard/Bandit-like**, AC 13–14); fever-thinned crown customs soldiers (**Guard/Veteran-like**); sea-drowned guardians / a stirring presence at the Wreck-Reef and Drowned Steps (scale drowned-dead profiles to L12–15, telegraphed). Use `13_encounters_and_bestiary/RANDOM_ENCOUNTERS.md` coastal/sea lines and the Pale Coast maritime profiles in `SUNDERING_REACH_ENCOUNTERS.md` scaled up.
- **Environmental hazards:** the dive (Vehicles(water)/Survival DC 16–17, Athletics DC 16; tidal windows constrain it); the reef's wreck-hazards; raw relic exposure at the deep ruins may inflict **Thin-touch** (Stage 3 condition); sailing-season/storm pressure on the lanes.
- **Social/investigation DCs (typical):** Persuasion DC 16–18 (Calder, Saltgate, Hadiz, Mallin); Insight DC 16–17 (Calder vs. Mallin, the double-agent); Deception DC 16–17 (port intrigue); History DC 18 (Surren lore — gated, oblique). See the quest file for per-quest DCs.
- **Scaling:** L10 — minor cargo/port favors. L15 — fleet-scale disputes, a deadly sea-battle, and the Drowned Steps' / Wreck-Reef's full danger; the overseas voyage to Surren opens.

## Local Labels (player map)

The Hollow Gulf Ports (faint region label); the Hollow Gulf (bay, on water); Calderport; Saltgate; the Mardenmouth; the Glasswater Run; the Reach Lanes; the South Sea Lanes (edge-arrow "to overseas lands / Surren"); the Wreck-Reef (offshore, label-only). On a Calderport city map: the Foreign Quarter.

## Player-Safe Layer

- Visible: the two port city-states + the Mardenmouth, the bay, the river terminus, the coastal and overseas sea-lanes, the lighthouse, the Wreck-Reef as a maritime hazard.
- The Gulf is openly warm, brash, and oblivious to the "northern ghost story." Sea-danger (the reef, the lanes) is telegraphed as ordinary maritime hazard.

## DM-Only Layer (NEVER on the player map)

- The Wreck-Reef (D31) and the Drowned Steps (D33, shared) hold only **faint far-south relic-echoes** (M2/M5-oblique) — far corroboration of the crisis's continental reach; NEVER the live machine, the keystone, or the Concord Deep.
- Tide-Mother Sera Mardenmouth is the **southernmost old-songs network anchor** and the Gulf's lone believer — she could carry the frontier warning to the maritime world via Roke Mallin (Q_MAJOR_010). Her "grey hands" fragment is M6-oblique folk-memory ONLY.
- Roke Mallin is the rare far-region NPC who *might believe* the frontier crisis — a late-game truth-bridge; keep his "north gone wrong" knowledge as vague sailor's-rumor.
- Foreign-Factor Hadiz carries the campaign's faintest, most optional **world-horizon** hint ("Surren has tales not unlike it") — keep EXTREMELY oblique; never develop; never pull focus from Hollowmere.
- No apex geometry exists here. The endgame is vertical beneath Hollowmere (NW only).

## Unresolved Map Gaps

- Harbor shapes are illustrative; Calderport's internal layout lives in `CALDERPORT_CITY_MAP.md`.
- Saltgate's exact relation to Calderport across the bay is LOW confidence (render across the Gulf to the E).
- The overseas lanes to Surren are edge-arrows only; Surren is off-grid.

## Related Files

- NPCs: [`../../08_npcs/by_region/HOLLOW_GULF_PORTS_NPCS.md`](../../08_npcs/by_region/HOLLOW_GULF_PORTS_NPCS.md)
- Quests: [`../../09_quests/by_region/HOLLOW_GULF_PORTS_QUESTS.md`](../../09_quests/by_region/HOLLOW_GULF_PORTS_QUESTS.md)
- City packet: [`../../06_settlements/city_map_packets/CALDERPORT_CITY_MAP.md`](../../06_settlements/city_map_packets/CALDERPORT_CITY_MAP.md)
- D-site: [`../../10_dungeons_and_ruins/THE_HOLLOW_GULF_WRECK_REEF.md`](../../10_dungeons_and_ruins/THE_HOLLOW_GULF_WRECK_REEF.md)
- Authority: [`../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`](../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md) · [`../FULL_CONTINENT_SETTLEMENT_ANCHORS.md`](../FULL_CONTINENT_SETTLEMENT_ANCHORS.md) · [`../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
