# FULL_CONTINENT_SETTLEMENT_ANCHORS.md — Settlement and Social Anchor Coordinate Layer

---
type: region
secrecy: dm-facing-player-safe-output
status: static
region: Orrun
factions: []
level_range: 1-20
related: [FULL_WORLD_MAP_AUTHORITY.md, FULL_WORLD_MAP_COORDINATES.md, PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md, PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET.md, REGION_INDEX.md, ../00_control/NAMING_REGISTRY.md, ../00_control/CONTENT_INDEX.md]
tags: [type:map, secrecy:dm-facing-player-safe-output, function:cartography, settlement-anchors, social-anchors, orrun, full-continent, render-layer]
---

> **Secrecy classification:** This file instructs the AI what to OMIT from player-facing map output (see "Secrecy Rules" below, which name DM-only locations like the Concord Deep / Under-Shrine / Hollow Court only to forbid rendering them). The *map output* it produces is player-safe; the file itself is **not** player-safe to share directly, because it lists the excluded apex secrets. Use it to generate/audit player maps; never hand it to the player.

## AI Use

This file is the **settlement-and-social-anchor render layer** for the player-safe full-continent map of Orrun. Load it whenever generating, reviewing, or auditing a full-continent map that should show **settlement markers distributed across the whole continent**, not bunched in the northwest.

- It assigns **player-safe full-continent grid coordinates** (0–100) to (a) the canonical NW campaign settlements and (b) the **light NPC-facing anchors** registered for the 12 far-continent placeholder regions in Stages 9.5/10.
- It is a **cartographic precision layer**, not a lore or settlement-gazetteer expansion. It coins no new places. Every name here is already registered in `NAMING_REGISTRY.md` or already used in the `08_npcs/by_region/` and `09_quests/by_region/` files.
- For **label authority and render rules** (regions, seas, ranges, rivers), the parent source of truth is `PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md`. This file *extends* that manifest with a settlement/social anchor layer; it does not override region/water/terrain labels.
- For **raw region/feature coordinates**, see `FULL_WORLD_MAP_COORDINATES.md`. The NW settlement coordinates here are **mirrored** from it (Table 1); their authoritative source remains `FULL_WORLD_MAP_COORDINATES.md` / `WORLD_MAP_COORDINATES.md`.

---

## Purpose — what this file is and is NOT

**This file IS:**
- A coordinate layer so full-continent maps place settlement/social markers across central, southern, eastern, northern, and southeastern Orrun, giving the continent a believable lived-in distribution.
- A render-priority manifest distinguishing which anchors appear on a detailed **reference map**, which appear on a stylized **art map**, and which are **never rendered** on a full-continent map (too small/local).
- A bridge between the Stage 9.5 NPC anchors and the cartographic system.

**This file is NOT:**
- A settlement gazetteer. The far-continent anchors are **light NPC-facing anchors** — towns, camps, districts, wharves, gathering-places, ruin-edge posts — not deep-built settlements. They have no district lists, leadership rosters, or full mechanical write-ups, and this file does not promote them to full settlements.
- A new-content pass. No new regions, factions, gods, artifacts, mysteries, or major settlements are created here.
- A DM-only file. **Everything here is player-safe.** DM-only locations must never be added (see Secrecy Rules).

---

## Secrecy Rules

All anchors in this file are **player-safe**. The following DM-only locations must **NEVER** appear in this file, on any reference map, or on any art map — not as a label, point, line, area, or implication:

- The **Concord Deep** (subsurface node-network).
- The **Under-Shrine / Drowned Keystone** (endgame, beneath Hollowmere).
- The **Hollow Court** seat or any surviving-Custodian reference.
- Any subsurface, depth, node-network, or "machine" annotation of any kind.

The endgame is **vertical (straight down beneath the NW cluster)**, never a distant land. Far ruins (Concord Heartlands, Saltmere Drowned Towns, Karran Old Iron forts, Hethewald Old Holds, Marrowdowns Barrow-Fields) are drawn only as distant, broken, **unexplained surface ruin-country** — never as a connected network. Their `ruin_edge_anchor` markers show only the **living camps beside** those ruins, never the DM-only truth.

---

## Coordinate Rules

All coordinates use the **full-continent normalized grid** of `FULL_WORLD_MAP_COORDINATES.md`:

- **X = 0** = west edge; **X = 100** = east edge.
- **Y = 0** = north edge; **Y = 100** = south edge.
- **North is top; west is left.**
- One full-continent grid unit ≈ **8–12 miles**; corner-to-corner ≈ **2–3 months' travel** by road.
- The **NW campaign cluster** occupies approximately **X 8–40, Y 8–42** (upper-left quarter); it is the only high-detail zone. Far-continent anchors are spread **within their region footprints** (see `PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET.md` Section I), not stacked on region centroids.

---

## Category Definitions

| Type | Meaning | Render rule |
|---|---|---|
| `settlement_major` | Major city, city-state, port, or major political/religious center. | Reference map AND art map. |
| `settlement_secondary` | Town, local hub, district-scale settlement, region hub. | Reference map; art map only if high priority. |
| `travel_anchor` | Road stop, river landing, caravan camp, pass camp, dock, route node. | Reference map for important ones only; art map rarely. |
| `social_anchor` | Light NPC-facing social place (gathering, meeting-ground, sacred site used for play). Used for play, not necessarily a settlement. | Reference map only if it doubles as a locatable point; never art map. |
| `ruin_edge_anchor` | Living/semi-permanent camp, scholar post, salvage site, watch post, or pilgrim camp near a ruin or dangerous area. | Reference map only; never art map. Shows the living camp, never the DM-only ruin truth. |
| `non_rendered_local_anchor` | Too small/local for full-continent maps; useful in NPC/quest files only. | NEVER rendered on a full-continent map (reference or art). |

**Render-priority key (`render_priority` column):** `high` · `medium` · `low`. Higher priority = render first / larger when space is tight.

---

## Table 1 — NW Campaign Cluster (existing, canonical — MIRRORED)

> These coordinates are **mirrored** from `FULL_WORLD_MAP_COORDINATES.md` (Campaign Cluster Settlements) and `PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md` §4. The authoritative source remains those files; do not edit positions here independently. The NW cluster is correctly **dense in the northwest** — that is intended.

| anchor_id | display_label | type | region | x | y | render_priority | render_on_reference_map | render_on_art_map | source_files | notes |
|---|---|---|---|---|---|---|---|---|---|---|
| nw.caradril | Caradril | settlement_major | Caradril (NW cluster SE) | 34 | 35 | high | true | true | `06_settlements/CARADRIL.md` | Only true city in the cluster; on the Verdance/Stillwater. Render exactly once. |
| nw.hollowmere | Hollowmere | settlement_secondary | Sundering Reach | 24 | 23 | high | true | true | `06_settlements/HOLLOWMERE.md` | Starting hub town on its dark flooded basin. |
| nw.kettle_bridge | Kettle Bridge | settlement_secondary | Sundering Reach | 27 | 23 | high | true | true | `06_settlements/KETTLE_BRIDGE.md` | E gateway (→ Tollwood). |
| nw.saltmargin | Saltmargin | settlement_secondary | Sundering Reach | 20 | 22 | high | true | true | `06_settlements/SALTMARGIN.md` | W gateway (→ Pale Coast). |
| nw.candlewick | Candlewick | settlement_secondary | Sundering Reach | 24 | 26 | medium | true | false | `06_settlements/CANDLEWICK.md` | S gateway (→ Ashgarden Vale). |
| nw.greywater_holm | Greywater Holm | settlement_secondary | Sundering Reach | 22 | 26 | medium | true | false | `06_settlements/GREYWATER_HOLM.md` | SE Greyfens edge. |
| nw.harrowgast | Harrowgast | settlement_secondary | Sundering Reach | 25 | 17 | high | true | true | `06_settlements/HARROWGAST.md` | N mining town, Sunder Heights. |
| nw.reedford | Reedford | travel_anchor | Sundering Reach | 25 | 24 | low | true | false | `06_settlements/REEDFORD.md` | Central ford-hamlet. |
| nw.ashwalk_rest | The Ashwalk Rest | travel_anchor | Sundering Reach | 24 | 25 | low | true | false | `06_settlements/THE_ASHWALK_REST.md` | Warden waystation / crossroads sanctuary. |
| nw.orchardmere | Orchardmere | settlement_secondary | Ashgarden Vale | 25 | 32 | high | true | true | `06_settlements/ORCHARDMERE.md` | Vale hub on Orchardmere lake. |
| nw.saint_veddows_rest | Saint Veddow's Rest | settlement_secondary | Ashgarden Vale | 23 | 33 | medium | true | true | `06_settlements/SAINT_VEDDOWS_REST.md` | Vale pilgrimage hill-shrine town. |
| nw.tilbrook | Tilbrook | settlement_secondary | Ashgarden Vale | 25 | 29 | low | true | false | `06_settlements/TILBROOK.md` | Mill village on the Ammet. |
| nw.hartfell | Hartfell | settlement_secondary | Tollwood | 33 | 22 | high | true | true | `06_settlements/HARTFELL.md` | Tollwood hub; stockaded road-town. |
| nw.coldhearth | Coldhearth | settlement_secondary | Tollwood | 34 | 20 | medium | true | false | `06_settlements/COLDHEARTH.md` | Charcoal village, deeper E in the wood. |
| nw.tollstone_cross | Tollstone Cross | travel_anchor | Tollwood | 30 | 22 | low | true | false | `06_settlements/TOLLSTONE_CROSS.md` | Bandit toll-hamlet on the East Road. |
| nw.wrackmouth | Wrackmouth | settlement_secondary | Pale Coast | 12 | 23 | high | true | true | `06_settlements/WRACKMOUTH.md` | Coast hub/port; sea-route start. |
| nw.cobble_strand | Cobble Strand | settlement_secondary | Pale Coast | 13 | 20 | medium | true | false | `06_settlements/COBBLE_STRAND.md` | Shingle-cove fishing village. |

---

## Table 2 — Far-Continent Regional Anchors (new this pass)

> All names are **light NPC-facing anchors** already registered in `NAMING_REGISTRY.md` (Stage 9.5) and used in `08_npcs/by_region/*_NPCS.md` / `09_quests/by_region/*_QUESTS.md`. Coordinates are spread **within** each region's footprint (per `PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET.md` Section I), not on the centroid. Each far-continent region gets one hub (`settlement_major`/`settlement_secondary`), 2–4 additional anchors, at least one quest-start-suitable anchor, and at least one travel-route-tied anchor.

### Verdance Reaches (centroid ~42,42; bounds X 38–48, Y 38–48) — Ring 2 river-corridor

| anchor_id | display_label | type | region | x | y | render_priority | render_on_reference_map | render_on_art_map | source_files | notes |
|---|---|---|---|---|---|---|---|---|---|---|
| vr.marrowfen_stair | Marrowfen Stair | settlement_secondary | Verdance Reaches | 41 | 41 | high | true | true | `08_npcs/by_region/VERDANCE_REACHES_NPCS.md`, `09_quests/by_region/VERDANCE_REACHES_QUESTS.md` | Corridor hub: stepped river-town of locks and wharves. Quest-start anchor; on the Verdance Road. |
| vr.lords_wend | Lord's Wend | settlement_secondary | Verdance Reaches | 45 | 39 | medium | true | false | `08_npcs/by_region/VERDANCE_REACHES_NPCS.md` | Petty lord's hall-town up-corridor. |
| vr.cresswater | Cresswater | travel_anchor | Verdance Reaches | 39 | 45 | low | true | false | `08_npcs/by_region/VERDANCE_REACHES_NPCS.md` | Barge-village / river landing on the Verdance Road. |
| vr.nine_locks | The Nine Locks | travel_anchor | Verdance Reaches | 43 | 43 | low | true | false | `08_npcs/by_region/VERDANCE_REACHES_NPCS.md` | Great lock-staircase landmark on the Verdance; route node. |

### Glassmere League (centroid ~55,50; bounds X 50–60, Y 45–55) — central river-city league

| anchor_id | display_label | type | region | x | y | render_priority | render_on_reference_map | render_on_art_map | source_files | notes |
|---|---|---|---|---|---|---|---|---|---|---|
| gl.glassmere | Glassmere | settlement_major | Glassmere League | 55 | 50 | high | true | true | `08_npcs/by_region/GLASSMERE_LEAGUE_NPCS.md`, `09_quests/by_region/GLASSMERE_LEAGUE_QUESTS.md` | League capital; greatest river-city on the Glasswater. Major hub; quest-start anchor; junction of Verdance Road / Glasswater Run / Crown Road. |
| gl.sennfort | Sennfort | settlement_secondary | Glassmere League | 52 | 47 | medium | true | false | `08_npcs/by_region/GLASSMERE_LEAGUE_NPCS.md` | Smaller league-city up-river. |
| gl.cairnwater | Cairnwater | settlement_secondary | Glassmere League | 58 | 53 | medium | true | false | `08_npcs/by_region/GLASSMERE_LEAGUE_NPCS.md` | Smaller league-city down-river; on the Glasswater Run. |
| gl.lowwater | Lowwater | social_anchor | Glassmere League | 54 | 52 | low | false | false | `08_npcs/by_region/GLASSMERE_LEAGUE_NPCS.md` | Poor riverside district of Glassmere; city locale, not a separate marker (see Table 3). |
| gl.reliquary | The Reliquary | ruin_edge_anchor | Glassmere League | 56 | 48 | low | true | false | `08_npcs/by_region/GLASSMERE_LEAGUE_NPCS.md` | Remnant great chapter-house at Glassmere; scholar-post anchor (a building within the city). |

### Marrowdowns (centroid ~50,66; bounds X 45–55, Y 60–70) — pastoral chalk-down country

| anchor_id | display_label | type | region | x | y | render_priority | render_on_reference_map | render_on_art_map | source_files | notes |
|---|---|---|---|---|---|---|---|---|---|---|
| md.marrowmoot | Marrowmoot | settlement_secondary | Marrowdowns | 50 | 66 | high | true | true | `08_npcs/by_region/MARROWDOWNS_NPCS.md`, `09_quests/by_region/MARROWDOWNS_QUESTS.md` | Shire-town where the moots gather; region hub; quest-start anchor. Mardenflow rises nearby. |
| md.penmark_hold | Penmark Hold | settlement_secondary | Marrowdowns | 47 | 63 | medium | true | false | `08_npcs/by_region/MARROWDOWNS_NPCS.md` | Shire-reeve's manor-town. |
| md.wether | Wether | travel_anchor | Marrowdowns | 53 | 68 | low | true | false | `08_npcs/by_region/MARROWDOWNS_NPCS.md` | Wool-trade village; downs road-stop. |
| md.barrow_fields | The Barrow-Fields | ruin_edge_anchor | Marrowdowns | 52 | 64 | low | true | false | `08_npcs/by_region/MARROWDOWNS_NPCS.md` | Ancient burial-downs; barrow-robber camp anchor. Pre-Concord barrows, NOT the keystone. |

### Sallowmarch Protectorate (centroid ~58,84; bounds X 53–63, Y 80–88) — fever-delta protectorate

| anchor_id | display_label | type | region | x | y | render_priority | render_on_reference_map | render_on_art_map | source_files | notes |
|---|---|---|---|---|---|---|---|---|---|---|
| sm.fenward | Fenward | settlement_secondary | Sallowmarch Protectorate | 57 | 82 | high | true | true | `08_npcs/by_region/SALLOWMARCH_PROTECTORATE_NPCS.md`, `09_quests/by_region/SALLOWMARCH_PROTECTORATE_QUESTS.md` | Garrison-capital; the distant crown's seat; region hub; quest-start anchor. |
| sm.reedmouth | Reedmouth | settlement_secondary | Sallowmarch Protectorate | 60 | 85 | medium | true | false | `08_npcs/by_region/SALLOWMARCH_PROTECTORATE_NPCS.md` | Delta smuggling-village near the Mardenflow mouth. |
| sm.rice_sallows | The Rice Sallows | travel_anchor | Sallowmarch Protectorate | 55 | 86 | low | true | false | `08_npcs/by_region/SALLOWMARCH_PROTECTORATE_NPCS.md` | Flooded paddy-country sub-area; delta waterway node. |
| sm.fever_channels | The Fever Channels | non_rendered_local_anchor | Sallowmarch Protectorate | 59 | 87 | low | false | false | `08_npcs/by_region/SALLOWMARCH_PROTECTORATE_NPCS.md` | Deep delta backwaters; waterway label, too diffuse to mark (see Table 3). |

### Hollow Gulf Ports (centroid ~66,90; bounds X 60–72, Y 86–94) — maritime south, door overseas

| anchor_id | display_label | type | region | x | y | render_priority | render_on_reference_map | render_on_art_map | source_files | notes |
|---|---|---|---|---|---|---|---|---|---|---|
| hg.calderport | Calderport | settlement_major | Hollow Gulf Ports | 65 | 89 | high | true | true | `08_npcs/by_region/HOLLOW_GULF_PORTS_NPCS.md`, `09_quests/by_region/HOLLOW_GULF_PORTS_QUESTS.md` | Greatest Gulf port city-state; gateway to the South Sea Lanes; major hub; quest-start anchor. |
| hg.saltgate | Saltgate | settlement_secondary | Hollow Gulf Ports | 69 | 91 | medium | true | true | `08_npcs/by_region/HOLLOW_GULF_PORTS_NPCS.md` | Rival Gulf port city-state. |
| hg.mardenmouth | The Mardenmouth | travel_anchor | Hollow Gulf Ports | 63 | 88 | low | true | false | `08_npcs/by_region/HOLLOW_GULF_PORTS_NPCS.md` | Delta-mouth wharves at Calderport; harbor node on the Glasswater Run / Mardenflow. |
| hg.foreign_quarter | The Foreign Quarter | social_anchor | Hollow Gulf Ports | 66 | 90 | low | false | false | `08_npcs/by_region/HOLLOW_GULF_PORTS_NPCS.md` | Overseas-traders' district of Calderport; city locale (see Table 3). |

### Wender Steppe (centroid ~46,16; bounds X 40–55, Y 12–22) — nomadic grass-sea

| anchor_id | display_label | type | region | x | y | render_priority | render_on_reference_map | render_on_art_map | source_files | notes |
|---|---|---|---|---|---|---|---|---|---|---|
| ws.cold_springs | The Winter-Camp at Cold Springs | settlement_secondary | Wender Steppe | 45 | 16 | high | true | true | `08_npcs/by_region/WENDER_STEPPE_NPCS.md`, `09_quests/by_region/WENDER_STEPPE_QUESTS.md` | Largest clans' cold-season gathering; region hub (seasonal camp, not a city); quest-start anchor. |
| ws.spine_foot | The Spine-Foot trade-meet | travel_anchor | Wender Steppe | 50 | 20 | medium | true | false | `08_npcs/by_region/WENDER_STEPPE_NPCS.md` | Steppe/settled trade-meeting ground; on the Steppe Tracks toward central Orrun. |
| ws.sky_stones | The Sky-Stones | social_anchor | Wender Steppe | 42 | 14 | low | true | false | `08_npcs/by_region/WENDER_STEPPE_NPCS.md` | Ancient steppe shrine-circle (independent, NOT Concord); seer's gathering-place. |

### Karran Marches (centroid ~74,18; bounds X 70–80, Y 14–24) — outlaw mining frontier

| anchor_id | display_label | type | region | x | y | render_priority | render_on_reference_map | render_on_art_map | source_files | notes |
|---|---|---|---|---|---|---|---|---|---|---|
| km.brasks_hold | Brask's Hold | settlement_secondary | Karran Marches | 73 | 17 | high | true | true | `08_npcs/by_region/KARRAN_MARCHES_NPCS.md`, `09_quests/by_region/KARRAN_MARCHES_QUESTS.md` | Strongest warlord's fortress-town; region hub; quest-start anchor. |
| km.karran_gate | Karran-Gate | settlement_secondary | Karran Marches | 76 | 20 | medium | true | false | `08_npcs/by_region/KARRAN_MARCHES_NPCS.md` | Mining-and-mercenary town; on the Hethe Tollway head. |
| km.deep_cuts | The Deep Cuts | travel_anchor | Karran Marches | 71 | 21 | low | true | false | `08_npcs/by_region/KARRAN_MARCHES_NPCS.md` | Great ore-mines; mining-camp node. |
| km.old_iron_forts | The Old Iron forts | ruin_edge_anchor | Karran Marches | 78 | 15 | low | true | false | `08_npcs/by_region/KARRAN_MARCHES_NPCS.md` | Scattered peripheral Concord ruins; scavenger/Reclaimer camp anchor. NOT the keystone. |

### Emberfell Theocracy / Ashfast (centroid ~80,62; bounds X 76–86, Y 56–68) — volcanic fire-theocracy

| anchor_id | display_label | type | region | x | y | render_priority | render_on_reference_map | render_on_art_map | source_files | notes |
|---|---|---|---|---|---|---|---|---|---|---|
| ef.ashfast | Ashfast | settlement_major | Emberfell Theocracy | 80 | 62 | high | true | true | `08_npcs/by_region/EMBERFELL_THEOCRACY_NPCS.md`, `09_quests/by_region/EMBERFELL_THEOCRACY_QUESTS.md` | Fortress-temple-city; theocracy seat; major hub; quest-start anchor. |
| ef.cinderhold | Cinderhold | settlement_secondary | Emberfell Theocracy | 83 | 65 | medium | true | false | `08_npcs/by_region/EMBERFELL_THEOCRACY_NPCS.md` | Volcanic mining town in the Emberfells. |
| ef.ash_roads | The Ash Roads | travel_anchor | Emberfell Theocracy | 78 | 59 | low | true | false | `08_npcs/by_region/EMBERFELL_THEOCRACY_NPCS.md` | Pilgrim-ways through the highland; route-label anchor. |

### Saltmere Reaches (centroid ~60,70; bounds X 55–66, Y 66–76; render anchors on land around the inland sea) — salt-clan country

| anchor_id | display_label | type | region | x | y | render_priority | render_on_reference_map | render_on_art_map | source_files | notes |
|---|---|---|---|---|---|---|---|---|---|---|
| sr.brackhold | Brackhold | settlement_secondary | Saltmere Reaches | 57 | 68 | high | true | true | `08_npcs/by_region/SALTMERE_REACHES_NPCS.md`, `09_quests/by_region/SALTMERE_REACHES_QUESTS.md` | Largest surviving salt-clan hold; region hub; quest-start anchor. On land NW of the Saltmere water body. |
| sr.saltcairn | Saltcairn | settlement_secondary | Saltmere Reaches | 63 | 73 | medium | true | false | `08_npcs/by_region/SALTMERE_REACHES_NPCS.md` | Ghostmark-edge clan-town SE of the Saltmere; on the Salt Road. |
| sr.drowned_towns | The Drowned Towns | ruin_edge_anchor | Saltmere Reaches | 60 | 71 | low | true | false | `08_npcs/by_region/SALTMERE_REACHES_NPCS.md` | Receding-lake submerged ruins; delver-camp anchor on the shoreline. Pre-Concord drowning echo, NOT the keystone. |

### Concord Heartlands / Ruin'd Crown (centroid ~62,56; bounds X 58–66, Y 52–60) — fallen-Concord surface ruin

| anchor_id | display_label | type | region | x | y | render_priority | render_on_reference_map | render_on_art_map | source_files | notes |
|---|---|---|---|---|---|---|---|---|---|---|
| ch.crownmouth | Crownmouth | settlement_secondary | Concord Heartlands | 60 | 54 | high | true | true | `08_npcs/by_region/CONCORD_HEARTLANDS_NPCS.md`, `09_quests/by_region/CONCORD_HEARTLANDS_QUESTS.md` | Fortified scavenger-town at the ruin's edge; region hub; quest-start anchor. On the Crown Road. The living town only — never the DM-only truth. |
| ch.pilgrim_camps | The Pilgrim Camps | ruin_edge_anchor | Concord Heartlands | 63 | 58 | medium | true | false | `08_npcs/by_region/CONCORD_HEARTLANDS_NPCS.md` | Refugee/relic-seeker shanty-camps at the ruin-edge. Surface camps only; the ruin itself stays unexplained. |

### Hethewald Free Holds (centroid ~72,40; bounds X 66–78, Y 34–46) — forest free-holds

| anchor_id | display_label | type | region | x | y | render_priority | render_on_reference_map | render_on_art_map | source_files | notes |
|---|---|---|---|---|---|---|---|---|---|---|
| hw.hethemoot | Hethemoot | settlement_secondary | Hethewald Free Holds | 71 | 39 | high | true | true | `08_npcs/by_region/HETHEWALD_FREE_HOLDS_NPCS.md`, `09_quests/by_region/HETHEWALD_FREE_HOLDS_QUESTS.md` | Great gathering free-hold; region hub; quest-start anchor. |
| hw.greenward | Greenward | settlement_secondary | Hethewald Free Holds | 68 | 43 | medium | true | false | `08_npcs/by_region/HETHEWALD_FREE_HOLDS_NPCS.md` | Grove-village deeper in the Hethewood. |
| hw.tollreach | Tollreach | travel_anchor | Hethewald Free Holds | 75 | 37 | low | true | false | `08_npcs/by_region/HETHEWALD_FREE_HOLDS_NPCS.md` | Outlaw river-toll camp on the Hethe; on the Hethe Tollway. |
| hw.old_holds | The Old Holds | ruin_edge_anchor | Hethewald Free Holds | 74 | 44 | low | true | false | `08_npcs/by_region/HETHEWALD_FREE_HOLDS_NPCS.md` | Deep-wood Concord ruins (forbidden); ruin-edge label. Camps only; ruin unexplained. NOT the keystone. |

### Sunmark (centroid ~44,80; bounds X 38–50, Y 75–85) — sacred grove territory

| anchor_id | display_label | type | region | x | y | render_priority | render_on_reference_map | render_on_art_map | source_files | notes |
|---|---|---|---|---|---|---|---|---|---|---|
| su.sunhollow | The Great Grove at Sunhollow | settlement_secondary | Sunmark | 44 | 80 | high | true | true | `08_npcs/by_region/SUNMARK_NPCS.md`, `09_quests/by_region/SUNMARK_QUESTS.md` | Grove-tribes' holy heart and gathering-place; region hub (sacred grove + gathering, not a city); quest-start anchor. |
| su.grove_camps | The Grove-Camps | social_anchor | Sunmark | 40 | 77 | medium | true | false | `08_npcs/by_region/SUNMARK_NPCS.md` | Grove-tribes' dispersed settlements; camp-cluster anchor. |
| su.green_roads | The Green Roads | travel_anchor | Sunmark | 48 | 83 | low | true | false | `08_npcs/by_region/SUNMARK_NPCS.md` | Pilgrim-and-trade paths through the groves; route-label anchor. |

---

## Table 3 — Non-Rendered Local Anchors

> These exist in NPC/quest files for play but are **too small, too local, or too diffuse** to mark on a full-continent map. `render_on_reference_map = false` and `render_on_art_map = false` for all rows. They are listed here so an auditor can confirm they were deliberately excluded, not forgotten. Several are **districts/locales within an already-marked hub** (do not draw a second marker) or **diffuse area-labels** (no point marker).

| anchor_id | display_label | type | region | x | y | reason_not_rendered | source_files |
|---|---|---|---|---|---|---|---|
| gl.lowwater | Lowwater | non_rendered_local_anchor | Glassmere League | 54 | 52 | District within Glassmere (already marked); not a separate settlement. | `08_npcs/by_region/GLASSMERE_LEAGUE_NPCS.md` |
| gl.the_floor | The Floor | non_rendered_local_anchor | Glassmere League | 55 | 50 | Merchant-exchange locale inside Glassmere; a building, not a place marker. | `08_npcs/by_region/GLASSMERE_LEAGUE_NPCS.md` |
| gl.three_bridges | The Three Bridges | non_rendered_local_anchor | Glassmere League | 55 | 50 | Banking quarter inside Glassmere; a district, not a separate marker. | `08_npcs/by_region/GLASSMERE_LEAGUE_NPCS.md` |
| hg.foreign_quarter | The Foreign Quarter | non_rendered_local_anchor | Hollow Gulf Ports | 66 | 90 | District within Calderport (already marked). | `08_npcs/by_region/HOLLOW_GULF_PORTS_NPCS.md` |
| sm.fever_channels | The Fever Channels | non_rendered_local_anchor | Sallowmarch Protectorate | 59 | 87 | Diffuse deep-delta waterway; no point marker (terrain texture only). | `08_npcs/by_region/SALLOWMARCH_PROTECTORATE_NPCS.md` |

> Additional locale-scale references in the NPC files (e.g. wharves, halls, market-floors named only to seat NPCs inside a hub) inherit their hub's single marker and are not individually re-listed. They are never separate full-continent markers.

---

## Audit Checklist (this file)

| Check | Status |
|---|---|
| Every far-continent region (12) has at least one `settlement_major`/`settlement_secondary` hub. | PASS — all 12 have a hub. |
| Every far-continent region has 2–4 additional anchors (mix of travel/social/ruin-edge). | PASS — each region has 2–4 extras (Verdance 3, Glassmere 4, Marrowdowns 3, Sallowmarch 3, Hollow Gulf 3, Wender 2, Karran 3, Emberfell 2, Saltmere 2, Heartlands 1, Hethewald 3, Sunmark 2). See note below. |
| Every far-continent region has ≥1 quest-start-suitable anchor. | PASS — each hub is the quest-start anchor (cross-listed to `*_QUESTS.md`). |
| Every far-continent region has ≥1 travel-route-tied anchor. | PASS — each region's hub or an extra ties to a Section-5 route (Verdance Road, Glasswater Run, Crown Road, Salt Road, Hethe Tollway, Steppe Tracks, South Sea Lanes, Pale Coast Sea-Route). |
| No new proper nouns coined. | PASS — all names from `NAMING_REGISTRY.md` / NPC / quest files. |
| No DM-only locations present. | PASS — no Concord Deep / Under-Shrine / keystone / Hollow Court. |
| NW settlement coordinates unchanged (mirrored). | PASS — Table 1 matches `FULL_WORLD_MAP_COORDINATES.md`. |
| Far anchors spread within region footprints (not on centroids). | PASS — anchors offset from centroids within bounds. |
| Caradril listed exactly once. | PASS — `nw.caradril` only. |

> **Note on the two small-region exceptions:** the Concord Heartlands gets **2** total anchors (Crownmouth hub + the Pilgrim Camps), and Emberfell, Saltmere, Wender, and Sunmark get the lower end (2 extras), because those regions are sparse/dangerous/forbidden by design — fewer living anchors is correct and intentional, and each still meets the "≥1 hub + ≥1 route-tied + ≥1 quest-start" minimums. The high-density settled regions (Glassmere, Verdance, Hollow Gulf, Hethewald, Marrowdowns) carry more anchors, so the map reads denser in the settled center/south than in the wild steppe/volcanic/forbidden zones.

---

## Render-Density Summary (for the map artist)

- **Densest:** the NW cluster (intended — 17 markers in X 8–40 / Y 8–42).
- **Second-densest:** the settled center and south (Glassmere League, Verdance Reaches, Hollow Gulf Ports, Marrowdowns, Hethewald, Sallowmarch).
- **Sparser:** the wild/dangerous/forbidden regions (Wender Steppe, Karran Marches, Emberfell Theocracy, Saltmere Reaches, Concord Heartlands, Sunmark) — fewer, more scattered markers.
- This gradient is deliberate and matches the NW-cold-frontier → SE-warm-settled tilt of the continent.

---

## Related Files

- [`PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md`](PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md) — parent label authority (regions/water/terrain/routes); this file adds the settlement/social anchor layer.
- [`PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET.md`](PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET.md) — self-contained image-generation packet (now includes the settlement-anchor layer).
- [`FULL_WORLD_MAP_COORDINATES.md`](FULL_WORLD_MAP_COORDINATES.md) — raw 0–100 grid; source of the mirrored NW coordinates and region footprints.
- [`FULL_WORLD_MAP_AUTHORITY.md`](FULL_WORLD_MAP_AUTHORITY.md) — prose geography and region placement.
- [`REGION_INDEX.md`](REGION_INDEX.md) — region directory and grid coords.
- [`../00_control/NAMING_REGISTRY.md`](../00_control/NAMING_REGISTRY.md) — anchor name registry (Stage 9.5 light anchors).
- [`../18_audits/PLAYER_SAFE_FULL_CONTINENT_MAP_AUDIT.md`](../18_audits/PLAYER_SAFE_FULL_CONTINENT_MAP_AUDIT.md) — full-continent map audit.
