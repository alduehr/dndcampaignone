# PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md — Authoritative Player-Safe Render Manifest

---
type: region
secrecy: player-safe
status: static
region: Orrun
factions: []
level_range: 1-20
related: [FULL_WORLD_MAP_AUTHORITY.md, FULL_WORLD_MAP_COORDINATES.md, FULL_WORLD_MAP_PROMPTS.md, FULL_WORLD_MAP_LAYERS.md, WORLD_MAP_COORDINATES.md, WORLD_MAP_PROMPTS.md, REGION_INDEX.md, ../00_control/NAMING_REGISTRY.md]
tags: [type:map, secrecy:player-safe, function:cartography, render-manifest, orrun, full-continent, label-authority]
---

## AI Use

This is the **single authoritative player-safe render manifest** for generating the full-continent map of Orrun (world of Vael). It is the **source of truth for all image-generation prompts**. **No image prompt may introduce a label that is not in this manifest.** Load it whenever generating, reviewing, or auditing any player-facing full-continent map.

- For **label authority** (what may appear, where, and how often), use this file.
- For **prose geography and lore**, see `FULL_WORLD_MAP_AUTHORITY.md`.
- For **raw coordinates**, see `FULL_WORLD_MAP_COORDINATES.md` (this manifest's positions are derived from it; positions are unchanged).
- For **layer secrecy rules**, see `FULL_WORLD_MAP_LAYERS.md`.
- For the **campaign-area zoom**, see `WORLD_MAP_COORDINATES.md` / `WORLD_MAP_PROMPTS.md`.

This file is **player-safe in its entirety**. It contains no DM-only geography. Section 2 lists what must be kept off any rendered map.

---

## Section 1 — Grid Reference

All coordinates in this manifest use the **full-continent normalized grid** of `FULL_WORLD_MAP_COORDINATES.md`.

- **X = 0** is the **west edge**; **X = 100** is the **east edge**.
- **Y = 0** is the **north edge**; **Y = 100** is the **south edge**.
- **North is top; west is left** (south is bottom, east is right).
- All coordinates are **normalized 0–100 on both axes**.
- One full-continent grid unit ≈ **8–12 miles**; corner-to-corner ≈ **2–3 months' travel** by road.
- The **NW campaign cluster** (Sundering Reach + Ring 1 [Ashgarden Vale, Tollwood, Pale Coast] + Caradril) occupies approximately **X 8–40, Y 8–42** in the full-continent grid — the upper-left quarter. It is the only **high-detail** zone; everything else is drawn faint/placeholder.
- The campaign-area grid (`WORLD_MAP_COORDINATES.md`) is a **~3× zoom** on this NW corner; do not mix the two grids. This manifest uses the **full-continent grid only**.

---

## Section 2 — Player-Safe Secrecy Reminder

The following must **NEVER** appear on a player-safe map — not as a label, line, mark, callout, depth annotation, inset, or implication:

- **The Concord Deep** (the subsurface network) — no label, no area, no hint.
- **The Under-Shrine / Drowned Keystone** (endgame, beneath Hollowmere) — never shown, never labeled, never implied.
- **Any node-network lines or warming-node marks** — no dashed subterranean links, no flame-marks, no relay glyphs.
- **The Hollow Court or any reference to surviving Custodians.**
- **Any underground callout, depth annotation, or subsurface feature** of any kind.
- **Any implication that the "far ruins" are a machine or a connected network.** The Concord Heartlands and other far ruins are drawn only as a distant, broken, **unexplained** surface ruin-country.
- The endgame is **VERTICAL** (straight down, beneath the NW cluster), **never a distant land** — do not draw, label, or hint at it as a faraway place.
- **DM-only region annotations, secret travel routes, and mystery-site markers** (the M-coded clue sites and any faction "hidden reach" overlays).

If any of the above would be produced by a prompt, the prompt is wrong; fix the prompt, regenerate, or remove the element with inpainting.

---

## Section 3 — Render Rules

1. **One feature, one canonical label.** Every feature in this manifest has exactly one canonical label entry (Section 4). All other references in any file — prose, route anchors, adjacency notes, region context, descriptive mentions — are **aliases**, not additional labels.
2. **No duplicate labels.** If a feature appears in multiple source tables (the coordinates file, the authority file, a route table, the region index), render **only** the single canonical manifest entry from Section 4. Allowed repetition (e.g., sea-lane text along a coast) is stated explicitly per-feature in the `duplicate_rule` column.
3. **No invented major labels.** Do not generate labels for regions, seas, mountains, rivers, cities, or routes that do **not** appear in this manifest or are not registered in `NAMING_REGISTRY.md`. If a feature is unnamed in the source files, leave it unnamed.
4. **No alias labels as places.** Route anchors, region-context mentions, and descriptive references are **not** separate place labels on the map. A feature gets a place label only if it has its own canonical entry in Section 4.

---

## Section 4 — Canonical Feature Table

Column key:
- **label_priority:** `required` (must appear and be labeled) · `standard` (include if space) · `optional` (faint/small if space) · `omit` (never on a player map).
- **render_as:** `point` · `area-fill` · `line` · `text-over-water` · `text-over-terrain` · `icon+label` · `faint-area` · `boundary-line` · `edge-annotation`.
- **duplicate_rule:** `render exactly once; all other references are aliases` unless an explicit repetition rule is given.

Positions are full-continent grid values from `FULL_WORLD_MAP_COORDINATES.md` (unchanged). Settlements marked "tight-cluster (NW)" sit inside the X 8–40 / Y 8–42 detail zone; their fine intra-cluster placement lives in `WORLD_MAP_COORDINATES.md`.

### NW Campaign Cluster (high detail)

| feature_id | display_label | type | x | y | label_priority | render_as | notes | duplicate_rule |
|---|---|---|---|---|---|---|---|---|
| region.sundering_reach | Sundering Reach | region | 24 | 23 | required | area-fill | Cluster center; starting region (high detail). | render exactly once; all other references are aliases |
| settlement.hollowmere | Hollowmere | settlement (town) | 24 | 23 | required | icon+label | Keystone hub town on its dark flooded basin. Basin shown as dark water (no depth/subsurface). | render exactly once; all other references are aliases |
| settlement.kettle_bridge | Kettle Bridge | settlement (town) | 27 | 23 | required | icon+label | E gateway (→ Tollwood); tight-cluster (NW). | render exactly once; all other references are aliases |
| settlement.saltmargin | Saltmargin | settlement (town) | 20 | 22 | required | icon+label | W gateway (→ Pale Coast); tight-cluster (NW). | render exactly once; all other references are aliases |
| settlement.candlewick | Candlewick | settlement (village) | 24 | 26 | required | icon+label | S gateway (→ Vale); tight-cluster (NW). | render exactly once; all other references are aliases |
| settlement.greywater_holm | Greywater Holm | settlement (village) | 22 | 26 | standard | icon+label | SE Greyfens edge; tight-cluster (NW). | render exactly once; all other references are aliases |
| settlement.harrowgast | Harrowgast | settlement (mining town) | 25 | 17 | required | icon+label | N, Sunder Heights. | render exactly once; all other references are aliases |
| settlement.reedford | Reedford | settlement (hamlet) | 25 | 24 | standard | icon+label | Central ford; tight-cluster (NW). | render exactly once; all other references are aliases |
| settlement.ashwalk_rest | The Ashwalk Rest | settlement (waystation) | 24 | 25 | standard | icon+label | Central crossroads sanctuary; tight-cluster (NW). | render exactly once; all other references are aliases |
| region.ashgarden_vale | Ashgarden Vale | region | 25 | 31 | required | area-fill | NW cluster, S of Reach; orchards/shrine-towns. | render exactly once; all other references are aliases |
| settlement.orchardmere | Orchardmere | settlement (town) | 25 | 32 | required | icon+label | Vale hub on Orchardmere lake. | render exactly once; all other references are aliases |
| settlement.saint_veddows_rest | Saint Veddow's Rest | settlement (town) | 23 | 33 | required | icon+label | Vale pilgrimage hill-shrine town. | render exactly once; all other references are aliases |
| settlement.tilbrook | Tilbrook | settlement (village) | 25 | 29 | standard | icon+label | On the Ammet; tight-cluster (NW). | render exactly once; all other references are aliases |
| region.tollwood | Tollwood | region | 32 | 22 | required | area-fill | NW cluster, E of Reach; deep old-growth forest. | render exactly once; all other references are aliases |
| settlement.hartfell | Hartfell | settlement (town) | 33 | 22 | required | icon+label | Tollwood hub; stockaded road-town. | render exactly once; all other references are aliases |
| settlement.coldhearth | Coldhearth | settlement (village) | 34 | 20 | standard | icon+label | Deeper E in the wood; tight-cluster (NW). | render exactly once; all other references are aliases |
| settlement.tollstone_cross | Tollstone Cross | settlement (hamlet) | 30 | 22 | standard | icon+label | On the East Road; tight-cluster (NW). | render exactly once; all other references are aliases |
| region.pale_coast | Pale Coast | region | 14 | 21 | required | area-fill | NW cluster, W of Reach; storm coast. | render exactly once; all other references are aliases |
| settlement.wrackmouth | Wrackmouth | settlement (town/port) | 12 | 23 | required | icon+label | Coast hub/port; sea-route start. | render exactly once; all other references are aliases |
| settlement.cobble_strand | Cobble Strand | settlement (village) | 13 | 20 | standard | icon+label | Coast shingle cove. | render exactly once; all other references are aliases |
| city.caradril | Caradril | city (major) | 34 | 35 | required | icon+label | NW cluster SE corner; the only true city; on the Verdance/Stillwater. Frontier-edge city-state, not a capital. | render exactly once; all other references are aliases (city, political region, route anchor, and Stillwater-settlement mentions are the SAME label) |
| water.stillwater | The Stillwater | water (harbor-lake) | 34 | 35 | standard | text-over-water | Caradril's port-lake on the Verdance. Render adjacent to Caradril; do not duplicate the Caradril label. | render exactly once; all other references are aliases |

### Ring 2 / Near Placeholders

| feature_id | display_label | type | x | y | label_priority | render_as | notes | duplicate_rule |
|---|---|---|---|---|---|---|---|---|
| region.verdance_reaches | The Verdance Reaches | region (placeholder) | 42 | 42 | standard | faint-area | SE of cluster, up the Verdance; first step into the wider continent. Draw faint. | render exactly once; all other references are aliases |
| range.highmark_spine | The Highmark Spine | mountain range | 26–44 | 8–10 | required | line | Far-N barrier wall over the cluster; runs W (26,10) to E (44,8). Parent range of the Sunder Heights. | render exactly once; all other references are aliases |
| wilderness.sunder_heights | The Sunder Heights | wilderness (highlands) | 24 | 15 | required | text-over-terrain | NW cluster N highlands, below the Highmark Spine. | render exactly once; all other references are aliases |
| wilderness.greyfens | The Greyfens | wilderness (fog marsh) | 22 | 25 | required | text-over-terrain | NW cluster wetland, SW of Hollowmere. | render exactly once; all other references are aliases |

### Full-Continent Regions (faint / placeholder)

| feature_id | display_label | type | x | y | label_priority | render_as | notes | duplicate_rule |
|---|---|---|---|---|---|---|---|---|
| region.glassmere_league | The Glassmere League | region (placeholder) | 55 | 50 | standard | faint-area | Central river-city league on the Glasswater. Draw faint, label only. | render exactly once; all other references are aliases (shares root with the Glasswater river — keep both full names) |
| region.marrowdowns | The Marrowdowns | region (placeholder) | 50 | 66 | standard | faint-area | S-central chalk downs. Region and terrain share this position/label; render once. | render exactly once; the chalk-downs terrain and the region are the SAME label — render once |
| region.saltmere_reaches | The Saltmere Reaches | region (placeholder) | 60 | 70 | standard | text-over-terrain | S-central salt-clan country, ringing the Saltmere inland sea. **Render on the surrounding land, not on the water body.** water.saltmere label goes on the water. Do not stack these labels. | render exactly once on the surrounding land; do not place this label on the water body |
| region.sallowmarch_protectorate | The Sallowmarch Protectorate | region (placeholder) | 58 | 84 | standard | faint-area | S coast, Mardenflow delta. Political label has priority over terrain.sallow_marches text label. If both appear, political label is larger/first; terrain label is smaller italic below or adjacent. Never at the same position. | render exactly once; if space is tight, omit terrain.sallow_marches text label and keep this one |
| region.hollow_gulf_ports | The Hollow Gulf Ports | region (placeholder) | 66 | 90 | standard | faint-area | S-coast rival port city-states around the Hollow Gulf. Distinct from water.hollow_gulf. | render exactly once; all other references are aliases |
| region.wender_steppe | The Wender Steppe | region (placeholder) | 46 | 16 | standard | faint-area | N-central nomadic confederacy on the steppe. **This is the single visible Wender Steppe label.** Do not render "The Wender Steppe (steppe)" or any terrain-type suffix as a separate label. terrain.wender_steppe_terrain uses faint-area fill only (no text). | render exactly once; this is the one visible Wender Steppe label — terrain.wender_steppe_terrain must not add a second text label |
| region.karran_marches | The Karran Marches | region (placeholder) | 74 | 18 | standard | faint-area | NE outlaw/warlord frontier in the Karran Teeth. Distinct from range.karran_teeth. | render exactly once; all other references are aliases |
| region.emberfell_theocracy | The Emberfell Theocracy / The Ashfast | region (placeholder) | 80 | 62 | optional | faint-area | SE-central volcanic theocracy. Two names = one region. **Range.emberfells is the terrain label (standard priority); this political label is secondary.** Render below or adjacent to the range label; never stack on the same line. | render exactly once; two names are aliases of one region; if space is tight, omit this label and let range.emberfells stand alone |
| region.concord_heartlands | Concord Heartlands | region (placeholder; fallen ruin) | 62 | 56 | standard | faint-area | Central-SE distant ruin-country, astride the Greatspine. Subtitle (optional italic below): "the fallen Concord heart — ruins, contested." Draw as broken towers, UNEXPLAINED. Surface ruin only — never a network/machine. No DM-only annotations. | render exactly once; subtitle is optional italic; never render only the subtitle as the primary label |
| region.hethewald_free_holds | The Hethewald Free Holds | region (placeholder) | 72 | 40 | standard | faint-area | E-central forest free-holds in the Hethewood. Political label has priority over terrain.hethewood text label. If both appear, political label is first; terrain label is smaller italic adjacent. Never stacked at the same position. | render exactly once; if space is tight, omit terrain.hethewood text label and keep this one |
| region.sunmark | The Sunmark | region (placeholder) | 44 | 80 | standard | faint-area | S warm sacred-grove territory. Political label has priority over terrain.sunmark_wilds text label. If both appear, political label is first; terrain label is smaller italic adjacent. Never stacked at the same position. | render exactly once; if space is tight, omit terrain.sunmark_wilds text label and keep this one |

### Bodies of Water

| feature_id | display_label | type | x | y | label_priority | render_as | notes | duplicate_rule |
|---|---|---|---|---|---|---|---|---|
| water.pale_sea | The Pale Sea | ocean | 4 | 30 | required | text-over-water | W/NW ocean along the whole west coast. | render once as a body label; coastline-edge repetition of the sea name along the W coast is allowed if the ocean is large, but only one primary label |
| water.sunder_ocean | The Sunder Ocean | ocean | 50 | 2 | required | text-over-water | N ocean beyond the Highmark Spine. | render once as a body label; one primary label only |
| water.calm_reach | The Calm Reach | warm sea | 82 | 92 | required | text-over-water | SE/S warm sea; southern trade heart. | render once as a body label; one primary label only |
| water.hollow_gulf | The Hollow Gulf | major bay | 66 | 92 | standard | text-over-water | S-coast bay; Mardenflow delta mouth. Distinct from region.hollow_gulf_ports. | render exactly once; all other references are aliases |
| water.saltmere | The Saltmere | inland salt sea | 60 | 70 | required | text-over-water | S-central brackish inland sea. **Render on the water body itself.** Distinct from region.saltmere_reaches (which is rendered on the surrounding land). Do not stack these labels. | render exactly once on the water body; region.saltmere_reaches label goes on the surrounding land, not on the water |
| water.wracking_straits | The Wracking Straits | strait | 2 | 64 | optional | text-over-water | Far-W narrows toward the open ocean. | render exactly once; all other references are aliases |

### Mountain Ranges

| feature_id | display_label | type | x | y | label_priority | render_as | notes | duplicate_rule |
|---|---|---|---|---|---|---|---|---|
| range.greatspine | The Greatspine / Sundering Wall | mountain range | 50–70 | 38–64 | required | line | Continental cordillera, NW (50,38) to SE (70,64); the master divider. Two names = one range. | render exactly once; the two names are aliases of one range — render one label (may show "/ Sundering Wall" as subtitle) |
| range.karran_teeth | The Karran Teeth | mountain range | 74 | 16 | standard | line | NE range; isolates the northeast. Distinct from region.karran_marches. | render exactly once; all other references are aliases |
| range.ghostmark_range | The Ghostmark Range | mountain range | 58 | 72 | optional | line | Low eroded mountains ringing the Saltmere. | render exactly once; all other references are aliases |
| range.emberfells | The Emberfells | volcanic highland | 80 | 60 | standard | line | SE-central volcanic highlands; vents, obsidian. Distinct from region.emberfell_theocracy. | render exactly once; all other references are aliases |

### Forests / Terrain

| feature_id | display_label | type | x | y | label_priority | render_as | notes | duplicate_rule |
|---|---|---|---|---|---|---|---|---|
| terrain.hethewood | The Hethewood | forest | 72 | 38 | optional | text-over-terrain | Great eastern forest; the Tollwood is its NW finger. **region.hethewald_free_holds is the primary label for this footprint.** Render as smaller italic adjacent to the political label, not stacked on it. Omit if space is tight. | render exactly once; secondary to region.hethewald_free_holds; never stack at the same position |
| terrain.sunmark_wilds | The Sunmark Wilds | forest | 44 | 80 | optional | text-over-terrain | S warm sacred-grove forest. **region.sunmark is the primary label for this footprint.** Render as smaller italic adjacent to the political label, not stacked on it. Omit if space is tight. | render exactly once; secondary to region.sunmark; never stack at the same position |
| terrain.cindern_waste | The Cindern Waste | badland | 84 | 66 | optional | text-over-terrain | Ash badland in the Emberfells' rain-shadow. Draw with a faint ominous wash; no explanation. | render exactly once; all other references are aliases |
| terrain.bonepan_flats | The Bonepan Flats | badland | 56 | 74 | optional | text-over-terrain | Salt-pan badland around the Saltmere. | render exactly once; all other references are aliases |
| terrain.sallow_marches | The Sallow Marches | wetland | 58 | 84 | optional | text-over-terrain | S-coast deltaic wetland. **region.sallowmarch_protectorate is the primary label for this footprint.** Render as smaller italic adjacent, not stacked. Omit if space is tight. | render exactly once; secondary to region.sallowmarch_protectorate; never stack at the same position |
| terrain.wender_steppe_terrain | (no text label) | steppe (terrain) | 46 | 16 | omit | faint-area | The physical cold grass-sea. **Do NOT render a text label for this terrain.** region.wender_steppe is the single visible Wender Steppe label. This entry exists for visual fill styling only (faint grass-green wash). | render as visual fill only; no text label; do not render "The Wender Steppe (steppe)" or any steppe-type suffix |
| terrain.mirewend_sinks | The Mirewend Sinks | wetland (boglands) | 28 | 40 | optional | text-over-terrain | Boglands S of the cluster, before the land rises. | render exactly once; all other references are aliases |

### Overseas Placeholder (off-grid; edge annotation only)

| feature_id | display_label | type | x | y | label_priority | render_as | notes | duplicate_rule |
|---|---|---|---|---|---|---|---|---|
| overseas.surren | to overseas lands (Surren) | landmass (off-map) | 12 | 118 | optional | edge-annotation | Off-grid far S/SW. Render only as a south edge-arrow "to overseas lands"; never draw as part of Orrun. | render exactly once as an edge-arrow only |
| overseas.iron_skards | to overseas lands (Iron Skards) | island chain (off-map) | 60 | -10 | optional | edge-annotation | Off-grid far N. Render only as a north edge-arrow "to overseas lands"; never draw as part of Orrun. | render exactly once as an edge-arrow only |
| overseas.sundered_isles | The Sundered Isles (Far Wrack) | island chain (off-map) | -8 | 70 | optional | edge-annotation | Off-grid far W mid-ocean. Render only as a far-W edge note; never draw as part of Orrun. | render exactly once as an edge note only |

---

## Section 5 — Route and River Geometry Table

Routes and rivers use **feature_id anchors** from Section 4, not prose. Draw each as a single polyline through its waypoints; place its label **once** near the stated label position. Route/river labels are **not** place labels — do not render a waypoint anchor as a separate location unless it has its own Section 4 entry.

| route_id | display_label | type | waypoint_sequence | label_position | notes |
|---|---|---|---|---|---|
| route.verdance_road | Verdance Road | land route | `city.caradril` (34,35) → `region.glassmere_league` (55,50) | around (44,43) | Up-Verdance into settled Orrun; the player's first step into the wider continent. |
| route.glasswater_run | Glasswater Run | river/road corridor | `region.glassmere_league` (55,50) → `region.hollow_gulf_ports` (66,90) | around (60,66) | The continent's main commercial artery; tolled. |
| route.greatspine_crown_road | Greatspine Crown Road *(contested)* | mountain pass route | `region.glassmere_league` (55,50) → `region.concord_heartlands` (62,56) → south | around (61,54) | Mark "contested." Through the central cordillera. |
| route.salt_road | Salt Road | land route | `region.pale_coast` (14,21) → `region.saltmere_reaches` (60,70) | around (37,54) | Overland salt/relic caravan track; passes fallen country. |
| route.hethe_tollway | Hethe Tollway | land route | `region.karran_marches` (74,18) → `water.calm_reach` (80,50 coast) | around (77,34) | Forest-river toll corridor; outlaw-shadowed. |
| route.pale_coast_sea_route | Pale Coast Sea-Route | sea route | `settlement.wrackmouth` (12,23) → `city.caradril` (34,35) → south | west coast / NW waters | The campaign's fast water-route; continues S past the cluster. |
| route.south_sea_lanes | South Sea Lanes | sea route | `water.hollow_gulf` (66,90) → off-map overseas | southern sea | Render as dashed arrows with edge annotation "to overseas lands." |
| river.verdance | Verdance | river | interior/upland source ~(48,46) → city.caradril/water.stillwater (34,35) → Pale Sea mouth ~(15,32) | label near (34,35) or along mid-course | NW-quarter great river at Caradril; reaches the Pale Sea south of the Pale Coast. Label once. |
| river.glasswater | Glasswater | river | central highlands (Greatspine source 58,40) → `region.glassmere_league` (55,50) → delta at `water.calm_reach` (to Hollow Gulf 64,88) | mid-course near (58,68) | The continent's largest river. Label once; do not duplicate with the Glassmere League label. |
| river.mardenflow | Mardenflow | river | south-central source (Marrowdowns 52,64) → `terrain.sallow_marches` (58,84) → `water.hollow_gulf` (66,92) | mid-course near (55,76) | Drains the southern plains; floods seasonally. |
| river.hethe | Hethe | river | `terrain.hethewood` (Karran Teeth source 74,22) → east → `water.calm_reach` (80,50) | mid-course near (78,40) | Eastern trade river; contested for tolls. |
| river.mirewend | Mirewend | river | `wilderness.greyfens` (22,25 / Heights source ~25,16) → `settlement.hollowmere` (24,23) → `water.stillwater`/coastal drain (NW system) | near (24,22) | NW cluster river; tributary of the NW-quarter system. Label once. |
| river.ammet | Ammet | river | `region.ashgarden_vale` internal (~25,30) → joins the Verdance or drains coastally (NW system) | near (25,30) | The Vale's river; Tilbrook/Orchardmere on it. Label once. |

---

## Section 6 — Region Footprint Guidance

`approx_bounds` is a rough X-span / Y-span for the area-fill or terrain label; far placeholders should be loose and faint. Every Section 4 feature_id is listed.

| feature_id | center_x | center_y | approx_bounds | adjacency_notes |
|---|---|---|---|---|
| region.sundering_reach | 24 | 23 | X 20–28, Y 19–28 | Center of NW cluster; Sunder Heights/Highmark Spine N, Ashgarden Vale S, Tollwood E, Pale Coast W, Caradril SE. |
| settlement.hollowmere | 24 | 23 | point | Reach center, on its basin; Kettle Bridge just E, Saltmargin just W, Candlewick just S. |
| settlement.kettle_bridge | 27 | 23 | point | E gateway of the Reach toward Tollwood; on the Mirewend. |
| settlement.saltmargin | 20 | 22 | point | W gateway of the Reach toward the Pale Coast. |
| settlement.candlewick | 24 | 26 | point | S gateway of the Reach toward Ashgarden Vale. |
| settlement.greywater_holm | 22 | 26 | point | SE Greyfens edge, S of Hollowmere. |
| settlement.harrowgast | 25 | 17 | point | N of Hollowmere, up in the Sunder Heights, below the Highmark Spine. |
| settlement.reedford | 25 | 24 | point | Central ford between Hollowmere and the Vale road. |
| settlement.ashwalk_rest | 24 | 25 | point | Central crossroads waystation just S of Hollowmere. |
| region.ashgarden_vale | 25 | 31 | X 21–30, Y 28–35 | S of the Reach; N of the Marrowdowns/Mirewend Sinks; W of Tollwood; E of the Pale Coast. |
| settlement.orchardmere | 25 | 32 | point | Vale hub on its lake; Saint Veddow's Rest just SW, Tilbrook just N. |
| settlement.saint_veddows_rest | 23 | 33 | point | Vale pilgrimage town SW of Orchardmere. |
| settlement.tilbrook | 25 | 29 | point | On the Ammet, between Candlewick and Orchardmere. |
| region.tollwood | 32 | 22 | X 29–36, Y 18–26 | E of the Reach; NW finger of the Hethewood; N of Caradril's approach; Kettle Bridge is its W gateway. |
| settlement.hartfell | 33 | 22 | point | Tollwood hub; Coldhearth deeper E, Tollstone Cross W toward Kettle Bridge. |
| settlement.coldhearth | 34 | 20 | point | Deeper E into the wood from Hartfell. |
| settlement.tollstone_cross | 30 | 22 | point | On the East Road between Kettle Bridge and Hartfell. |
| region.pale_coast | 14 | 21 | X 10–18, Y 17–26 | W of the Reach, along the Pale Sea; Saltmargin is the inland gateway; Sunder Heights NE. |
| settlement.wrackmouth | 12 | 23 | point | Coast hub/port; start of the Pale Coast Sea-Route; Cobble Strand just N. |
| settlement.cobble_strand | 13 | 20 | point | Coast shingle cove N of Wrackmouth. |
| city.caradril | 34 | 35 | point (city) | SE corner of the cluster, on the Verdance/Stillwater; the cluster's gate to the wider continent; Verdance Reaches lie SE up-river. |
| water.stillwater | 34 | 35 | small area at Caradril | Caradril's port-lake; render adjacent to the city, not as a separate town. |
| region.verdance_reaches | 42 | 42 | X 38–48, Y 38–48 | SE of Caradril, up the Verdance; between the cluster and the Glassmere League. |
| range.highmark_spine | 35 | 9 | X 26–44, Y 8–11 | Far-N wall over the whole cluster; parent of the Sunder Heights; runs W–E along the top of the NW quarter. |
| wilderness.sunder_heights | 24 | 15 | X 21–28, Y 12–18 | N highlands of the cluster, between Harrowgast and the Highmark Spine. |
| wilderness.greyfens | 22 | 25 | X 19–25, Y 23–28 | Fog marsh SW of Hollowmere; W edge of the Reach toward the Coast. |
| region.glassmere_league | 55 | 50 | X 50–60, Y 45–55 | Central interior on the Glasswater; SE of the Verdance Reaches; N of the Marrowdowns; W of the Hethewald Holds. |
| region.marrowdowns | 50 | 66 | X 45–55, Y 60–70 | S-central uplands; S of the Glassmere League; N of the Saltmere/Sallow Marches; Mardenflow rises here. |
| region.saltmere_reaches | 60 | 70 | X 55–66, Y 66–76 | S-central, ringing the Saltmere inland sea; Ghostmark Range and Bonepan Flats nearby; E of the Marrowdowns. |
| region.sallowmarch_protectorate | 58 | 84 | X 53–63, Y 80–88 | S coast, the Mardenflow delta/Sallow Marches; W of the Hollow Gulf Ports. |
| region.hollow_gulf_ports | 66 | 90 | X 60–72, Y 86–94 | S coast, around the Hollow Gulf; gateway to the South Sea Lanes; E of the Sallowmarch Protectorate. |
| region.wender_steppe | 46 | 16 | X 40–55, Y 12–22 | N-central grass-sea, beyond the Greatspine's N end; E of the Highmark Spine; W of the Karran Marches. |
| region.karran_marches | 74 | 18 | X 70–80, Y 14–24 | NE outlaw frontier in the Karran Teeth; E of the Wender Steppe; N of the Hethewald Holds. |
| region.emberfell_theocracy | 80 | 62 | X 76–86, Y 56–68 | SE-central volcanic theocracy in/around the Emberfells; Ashen Reach Woods and Cindern Waste nearby; near the Glass Coast. |
| region.concord_heartlands | 62 | 56 | X 58–66, Y 52–60 | Central-SE distant ruin-country astride the Greatspine; SE of the Glassmere League; on the Crown Road. Draw faint/broken, unexplained. |
| region.hethewald_free_holds | 72 | 40 | X 66–78, Y 34–46 | E-central forest free-holds in the Hethewood; along the Hethe; S of the Karran Marches; E of the Glassmere League. |
| region.sunmark | 44 | 80 | X 38–50, Y 75–85 | S warm sacred-grove territory; W of the Sallowmarch delta; S of the Marrowdowns. |
| water.pale_sea | 4 | 30 | W margin, X 0–10, Y 5–60 | W/NW ocean along the whole west coast; the Pale Coast fronts it; Wracking Straits to its far SW. |
| water.sunder_ocean | 50 | 2 | N margin, X 20–70, Y 0–6 | N ocean beyond the Highmark Spine; tops the continent. |
| water.calm_reach | 82 | 92 | SE/S margin, X 70–95, Y 85–98 | SE/S warm sea; the Hethe and Glasswater drain to it; the Hollow Gulf opens into it. |
| water.hollow_gulf | 66 | 92 | X 60–72, Y 88–96 | S-coast bay at the Mardenflow delta; ringed by the Hollow Gulf Ports. |
| water.saltmere | 60 | 70 | X 55–66, Y 66–75 | S-central inland salt sea; Ghostmark Range and Bonepan Flats around it; the Saltmere Reaches hold its shores. |
| water.wracking_straits | 2 | 64 | far W margin, X 0–5, Y 58–70 | Far-W narrows between Orrun and the off-map Sundered Isles. |
| range.greatspine | 60 | 51 | diagonal X 50–70, Y 38–64 | Continental cordillera NW–SE; the master divider; Concord Heartlands sit astride it; the Crown Road crosses it. |
| range.karran_teeth | 74 | 16 | X 70–80, Y 12–22 | NE range; the Karran Marches lie within it; the Hethe rises here. |
| range.ghostmark_range | 58 | 72 | X 53–63, Y 68–76 | Low eroded mountains ringing the Saltmere, S-central. |
| range.emberfells | 80 | 60 | X 76–86, Y 55–66 | SE-central volcanic highlands; the Emberfell Theocracy holds them; Cindern Waste in the rain-shadow E. |
| terrain.hethewood | 72 | 38 | X 64–80, Y 32–46 | Great eastern forest; the Tollwood is its NW finger; the Hethewald Holds occupy it; the Hethe runs through. |
| terrain.sunmark_wilds | 44 | 80 | X 38–50, Y 75–86 | S warm forest; the Sunmark territory occupies it; W of the Sallow Marches. |
| terrain.cindern_waste | 84 | 66 | X 80–90, Y 62–72 | Ash badland E of the Emberfells, in their rain-shadow; SE interior. |
| terrain.bonepan_flats | 56 | 74 | X 51–61, Y 70–78 | Salt-pan badland around the Saltmere; S-central. |
| terrain.sallow_marches | 58 | 84 | X 52–64, Y 80–90 | S-coast deltaic wetland at the Mardenflow mouth; the Sallowmarch Protectorate holds it. |
| terrain.wender_steppe_terrain | 46 | 16 | X 40–55, Y 12–22 | The physical N-central grass-sea co-located with the Wender Steppe region; beyond the Greatspine. |
| terrain.mirewend_sinks | 28 | 40 | X 24–34, Y 36–44 | Boglands S of the NW cluster, between the Reach/Vale and the rising mid-continent. |
| overseas.surren | 12 | 118 | off-grid S edge | Off-map far S/SW; edge-arrow only. |
| overseas.iron_skards | 60 | -10 | off-grid N edge | Off-map far N; edge-arrow only. |
| overseas.sundered_isles | -8 | 70 | off-grid far-W | Off-map far-W mid-ocean in the Pale Sea/Wracking Straits; edge note only. |

---

## Section 7 — Duplicate-Prone Entry Audit

Each entry below is referenced in **multiple source tables** and could be rendered twice. For each: the source tables that reference it, the canonical render location (Section 4), and the standard render note.

**Standard render note (applies to every entry):** "This feature has one canonical player-safe map label in `PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md` §4. All other references are aliases, context, route anchors, or descriptive mentions — not additional labels."

| Feature | Referenced in | Canonical entry (Section 4) | Why it is duplicate-prone |
|---|---|---|---|
| Caradril | FULL_WORLD_MAP_COORDINATES.md (Major Regions row + Campaign Cluster Settlements row + Verdance Road/Glasswater route anchors), WORLD_MAP_COORDINATES.md, FULL_WORLD_MAP_AUTHORITY.md §6, REGION_INDEX.md | `city.caradril` | Appears as a city, a political region, a Stillwater settlement, AND a route anchor on multiple routes. All are the SAME single label. |
| The Pale Sea | FULL_WORLD_MAP_COORDINATES.md (Bodies of Water), FULL_WORLD_MAP_AUTHORITY.md §4, WORLD_MAP_COORDINATES.md, Pale Coast Sea-Route context | `water.pale_sea` | A water body, plus coastline/route context text along the whole W coast. One primary label; coastline repetition is bounded (see §4 duplicate_rule). |
| Greatspine / Sundering Wall | FULL_WORLD_MAP_COORDINATES.md (two range endpoint rows: N end + S end), FULL_WORLD_MAP_AUTHORITY.md §5, Crown Road route name | `range.greatspine` | Two endpoint rows (one range), two names (Greatspine / Sundering Wall), AND a route ("Crown Road") run along/over it. One range label only. |
| The Glassmere League | FULL_WORLD_MAP_COORDINATES.md (Major Regions + Glasswater river rows), FULL_WORLD_MAP_AUTHORITY.md §6, Verdance Road/Glasswater Run/Crown Road anchors, REGION_INDEX.md | `region.glassmere_league` | The region shares a root with the Glasswater river and is a waypoint anchor on three routes. Region label and river label are distinct; render each once; do not add anchor labels. |
| Sunder Heights | FULL_WORLD_MAP_COORDINATES.md (Highlands/Steppe row), WORLD_MAP_COORDINATES.md (highlands + ruins rows), FULL_WORLD_MAP_AUTHORITY.md §5, REGION_INDEX.md (placeholder sub-region) | `wilderness.sunder_heights` | Listed as geographic highlands, as a "deep" placeholder sub-region, and contains a ruins sub-point. One wilderness label. |
| The Greyfens | FULL_WORLD_MAP_COORDINATES.md (Wetlands), WORLD_MAP_COORDINATES.md (marsh zone), travel-hazard context | `wilderness.greyfens` | A wilderness zone that is also referenced as a travel hazard and route context. One wilderness label. |
| Hollowmere | FULL_WORLD_MAP_COORDINATES.md (Campaign Cluster Settlements + Hollowmere basin water row + Mirewend river pt), WORLD_MAP_COORDINATES.md, REGION_INDEX.md | `settlement.hollowmere` | The settlement, the "Hollowmere basin" water feature, and a river course point share the (24,23) position. Render the town label once; the basin is dark water under it (no separate town-name repeat, no depth). |
| Saltmere / Saltmere Reaches | FULL_WORLD_MAP_COORDINATES.md (Bodies of Water row "The Saltmere" + Major Regions row "The Saltmere Reaches"), FULL_WORLD_MAP_AUTHORITY.md §4/§6, Salt Road anchor, REGION_INDEX.md | water: `water.saltmere`; region: `region.saltmere_reaches` | The inland sea and the political region share a name root and a position. Two DISTINCT labels (one water, one region); render each once; do not stack or duplicate. |
| Route-anchor settlements (Wrackmouth, Caradril, etc.) | FULL_WORLD_MAP_COORDINATES.md (Long-Distance Travel-Route Anchor Points), Section 5 here | their own §4 entries (`settlement.wrackmouth`, `city.caradril`, …) | Settlements named as route endpoints (e.g., Wrackmouth on the Pale Coast Sea-Route; Caradril on Verdance Road) must NOT be re-labeled as separate route-point places. The settlement's single §4 label is the only label. |

### Co-Located Terrain/Region Pair Resolutions

The following pairs share a footprint. Each has a **resolved priority rule** — follow it exactly:

| Pair | Resolution |
|---|---|
| `region.wender_steppe` vs `terrain.wender_steppe_terrain` | **One label only: "The Wender Steppe."** terrain.wender_steppe_terrain = visual fill (faint-area), no text label. Never render "The Wender Steppe (steppe)" or any terrain-type suffix. |
| `region.hethewald_free_holds` vs `terrain.hethewood` | Political label first (standard). Terrain label optional italic adjacent if space allows. Never stacked at the same position. If tight, omit terrain. |
| `region.sunmark` vs `terrain.sunmark_wilds` | Political label first (standard). Terrain label optional italic adjacent if space allows. Never stacked at the same position. If tight, omit terrain. |
| `region.sallowmarch_protectorate` vs `terrain.sallow_marches` | Political label first (standard). Terrain label optional italic adjacent if space allows. Never stacked. If tight, omit terrain. |
| `region.emberfell_theocracy` vs `range.emberfells` | Terrain/range label first (standard: "The Emberfells"). Political label optional italic below if space allows. If tight, omit political label. |
| `region.saltmere_reaches` vs `water.saltmere` | **Two distinct labels, distinct positions.** water.saltmere = on the water body (required). region.saltmere_reaches = on the surrounding land (standard). Never stack. |
| `region.hollow_gulf_ports` vs `water.hollow_gulf` | Region label on the land; bay label on the water. Distinct positions. |
| `region.karran_marches` vs `range.karran_teeth` | Range label first (line/terrain). Region label faint-area adjacent. |
| `region.marrowdowns` | Region and chalk-downs terrain are the SAME label — render once only as "The Marrowdowns." |
| `region.concord_heartlands` | Primary label: "Concord Heartlands." Optional subtitle italic: "the fallen Concord heart — ruins, contested." Never render only the subtitle as the primary label. |

---

## Section 8 — Post-Generation Audit Checklist

**Player-Safe Full Map Audit — run after generating any player-safe map:**

1. Is there no inset map, mini-map, callout map, or overlay panel? (The NW campaign frontier is shown directly on the main map, not boxed.)
2. Are all labels player-safe? (No DM-only content.)
3. Are there no DM-only labels? (No Concord Deep, Under-Shrine, node network, Hollow Court, warming nodes, or underground callouts.)
4. Are there no invented major regions, seas, mountain ranges, rivers, or cities not in this manifest?
5. Are the major seas named correctly: Pale Sea (W), Sunder Ocean (N), Calm Reach (SE/S), Hollow Gulf (S coast)?
6. Is the NW campaign cluster (Sundering Reach, Ring 1 regions, Caradril) in the far northwest quadrant?
7. Does the map preserve the cold/grey NW-to-warm/ochre SE gradient?
8. Are far placeholder regions rendered softer and less detailed than the NW campaign cluster?
9. Are all `label_priority: required` features from Section 4 present and labeled?
10. Does every `duplicate_rule: render exactly once` feature appear exactly once?
11. Are any labels duplicated outside their allowed duplicate rule?
12. Are any route anchors accidentally rendered as separate place labels?
13. Are any aliases rendered as separate place labels?
14. Are any labels misspelled relative to the `display_label` column in Section 4?
15. Is every label's position and adjacency consistent with Section 5 (routes) and Section 6 (footprints)?

---

## Section 9 — Image Model Warning

- Image models may **ignore coordinates** unless the prompt is generated **directly from this manifest**.
- **Recommended workflow:** when generating the player-safe map, **copy** the required-label table (Section 4, `label_priority: required` rows), the duplicate rules, the route geometry (Section 5), and the region footprint notes (Section 6) **directly into the image prompt** — do not paraphrase or summarize.
- The manifest sections are **designed to be copy-pasted into an image generation prompt verbatim.**
- If a model generates an **unlisted label**, treat it as an **error**; regenerate or use inpainting to remove the label.

---

## Related Files

- [`FULL_WORLD_MAP_AUTHORITY.md`](FULL_WORLD_MAP_AUTHORITY.md) · [`FULL_WORLD_MAP_COORDINATES.md`](FULL_WORLD_MAP_COORDINATES.md) · [`FULL_WORLD_MAP_PROMPTS.md`](FULL_WORLD_MAP_PROMPTS.md) · [`FULL_WORLD_MAP_LAYERS.md`](FULL_WORLD_MAP_LAYERS.md)
- [`WORLD_MAP_COORDINATES.md`](WORLD_MAP_COORDINATES.md) · [`WORLD_MAP_PROMPTS.md`](WORLD_MAP_PROMPTS.md) · [`REGION_INDEX.md`](REGION_INDEX.md)
- [`../00_control/NAMING_REGISTRY.md`](../00_control/NAMING_REGISTRY.md)
