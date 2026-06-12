# PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET.md
# Self-Contained Copy-Paste Prompt for External Image Generators

---
type: map
secrecy: player-safe
status: static
region: Orrun
factions: []
level_range: 1-20
related: [PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md, FULL_WORLD_MAP_PROMPTS.md, FULL_WORLD_MAP_AUTHORITY.md]
tags: [type:map, secrecy:player-safe, function:cartography, generation-packet, orrun, full-continent]
---

## Purpose

A **self-contained copy-paste prompt** for any external image generator that cannot read the campaign repository. Paste all sections from **A** through **K** into the image model.

All content is copied directly from `PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md` (the authoritative source). If the image model has access to the repository, use the manifest and `FULL_WORLD_MAP_PROMPTS.md` instead of this packet.

This file is **player-safe in its entirety**. It contains no DM-only geography.

> **If the image model has access to the repository:** Use `PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md` as the authoritative source and `FULL_WORLD_MAP_PROMPTS.md` Prompt 1 as the generation prompt instead of this packet.

---

## ——— COPY FROM HERE ———

---

## Section A — Style and Medium

Generate a **vintage fantasy cartographic map** with these properties:

- Hand-drawn feel, aged parchment or linen paper texture, subtle watercolor washes
- Ink linework with decorative compass rose (top-right), border, and legend
- **Palette gradient:** cold greys, peat-browns, and sea-greys in the northwest → greens and earth tones through the settled center → warm ochres, ash-greys, and obsidian-blacks in the volcanic southeast → warm blues in the southern sea
- Landscape orientation, ~3:2 or 16:10 aspect ratio, high resolution for continental label density
- Scale bar: "approx. 2–3 months' travel corner to corner"
- The **NW campaign frontier** is drawn directly on the main continent with somewhat higher local detail than the rest — crisp linework; far regions softer, "less-surveyed"

---

## Section B — Layout Rules

**CRITICAL — follow these layout rules exactly:**

1. This is a **single continuous map** of the full continent of **Orrun** (world of **Vael**). A large continent that tilts from a cold, broken northwest frontier to a warm, rich south and southeast.
2. **NO inset panels, NO mini-maps, NO overlay boxes, NO "you are here" callouts, NO inset map in any corner.** The NW campaign frontier (Sundering Reach, Ring 1 regions, Caradril) is shown directly on the main continent map — never boxed, never inset, never in a separate panel.
3. **Coordinate grid:** X = 0 is west, X = 100 is east, Y = 0 is north, Y = 100 is south. North is top, west is left. All feature positions in this packet use this 0–100 normalized grid.
4. The **NW campaign cluster** (Sundering Reach + Ring 1 + Caradril) occupies approximately **X 8–40, Y 8–42** — the upper-left quarter of the continent. It is the only high-detail zone; all other regions are drawn fainter and less detailed.

---

## Section C — Secrecy / Forbidden Content

**NEVER include any of the following, in any form:**

- The Concord Deep (a subsurface network) — no label, no area, no hint, no lines
- The Under-Shrine / Drowned Keystone (an endgame location beneath Hollowmere) — never shown, never labeled, never implied
- Any node-network lines, warming-node marks, dashed subterranean links, or relay glyphs
- The Hollow Court or any reference to surviving Custodians
- Any underground callout, depth annotation, or subsurface feature of any kind
- Any implication that the "far ruins" are a machine or a connected network — the ruined central country is drawn only as a distant, broken, unexplained surface ruin-country
- The endgame is **vertical** (straight down, beneath the NW cluster) — never a distant land; do not draw, label, or hint at it as a faraway place
- DM-only region annotations, secret travel routes, mystery-site markers, faction hidden-reach overlays

---

## Section D — Required Labels (must appear and be labeled)

Place each at or near the stated x,y position (0–100 grid: X=0 west, Y=0 north).

| Display Label | Type | x | y | Notes |
|---|---|---|---|---|
| Sundering Reach | region | 24 | 23 | Cluster center; high detail; starting region |
| Hollowmere | settlement (town) | 24 | 23 | Hub town on its dark flooded basin |
| Kettle Bridge | settlement (town) | 27 | 23 | E gateway toward Tollwood |
| Saltmargin | settlement (town) | 20 | 22 | W gateway toward Pale Coast |
| Candlewick | settlement (village) | 24 | 26 | S gateway toward Ashgarden Vale |
| Harrowgast | settlement (mining town) | 25 | 17 | N, up in the Sunder Heights |
| Ashgarden Vale | region | 25 | 31 | S of Reach; orchards/shrine-towns |
| Orchardmere | settlement (town) | 25 | 32 | Vale hub |
| Saint Veddow's Rest | settlement (town) | 23 | 33 | Vale pilgrimage hill-shrine town |
| Tollwood | region | 32 | 22 | E of Reach; deep old-growth forest |
| Hartfell | settlement (town) | 33 | 22 | Tollwood hub |
| Pale Coast | region | 14 | 21 | W of Reach; storm coast |
| Wrackmouth | settlement (town/port) | 12 | 23 | Coast hub/port |
| Caradril | city (major) | 34 | 35 | NW cluster SE corner; only true city; on the Verdance/Stillwater |
| The Highmark Spine | mountain range | 35 | 9 | Far-N barrier wall; runs W(26,10)→E(44,8) |
| The Sunder Heights | wilderness (highlands) | 24 | 15 | N highlands of the cluster |
| The Greyfens | wilderness (fog marsh) | 22 | 25 | Fog marsh SW of Hollowmere |
| The Pale Sea | ocean | 4 | 30 | W/NW ocean along the whole west coast |
| The Sunder Ocean | ocean | 50 | 2 | N ocean beyond the Highmark Spine |
| The Calm Reach | warm sea | 82 | 92 | SE/S warm sea |
| The Saltmere | inland salt sea | 60 | 70 | S-central brackish inland sea; render ON the water body |
| The Greatspine / Sundering Wall | mountain range | 60 | 51 | Continental cordillera NW–SE; one label (may show "/ Sundering Wall" as subtitle) |
| Concord Heartlands | region (fallen ruin) | 62 | 56 | Primary label. Optional subtitle italic: "the fallen Concord heart — ruins, contested." Draw as broken towers, UNEXPLAINED. |

---

## Section E — Standard Labels (include if space allows)

| Display Label | Type | x | y | Notes |
|---|---|---|---|---|
| Greywater Holm | settlement (village) | 22 | 26 | SE Greyfens edge |
| Reedford | settlement (hamlet) | 25 | 24 | Central ford |
| The Ashwalk Rest | settlement (waystation) | 24 | 25 | Crossroads waystation |
| Tilbrook | settlement (village) | 25 | 29 | On the Ammet |
| Coldhearth | settlement (village) | 34 | 20 | Deeper E in Tollwood |
| Tollstone Cross | settlement (hamlet) | 30 | 22 | On the East Road |
| Cobble Strand | settlement (village) | 13 | 20 | Coast shingle cove |
| The Stillwater | water (harbor-lake) | 34 | 35 | Caradril's port-lake; render adjacent to city label |
| The Verdance Reaches | region (placeholder) | 42 | 42 | SE of cluster; draw faint |
| The Glassmere League | region (placeholder) | 55 | 50 | Central river-city league; draw faint |
| The Marrowdowns | region (placeholder) | 50 | 66 | S-central chalk downs; draw faint |
| The Saltmere Reaches | region (placeholder) | 60 | 70 | S-central salt-clan country; render ON THE LAND surrounding the Saltmere, not on the water |
| The Sallowmarch Protectorate | region (placeholder) | 58 | 84 | S coast; draw faint |
| The Hollow Gulf Ports | region (placeholder) | 66 | 90 | S-coast port city-states; draw faint |
| The Wender Steppe | region (placeholder) | 46 | 16 | N-central steppe; draw faint. **ONE label only — never add "(steppe)" suffix.** |
| The Karran Marches | region (placeholder) | 74 | 18 | NE outlaw frontier; draw faint |
| The Hethewald Free Holds | region (placeholder) | 72 | 40 | E-central forest free-holds; draw faint |
| The Sunmark | region (placeholder) | 44 | 80 | S sacred-grove territory; draw faint |
| The Hollow Gulf | major bay | 66 | 92 | S-coast bay; render ON the water |
| The Karran Teeth | mountain range | 74 | 16 | NE range |
| The Emberfells | volcanic highland | 80 | 60 | SE-central; vents, obsidian. **Render this label before the Emberfell Theocracy label.** |

---

## Section F — Optional Labels (small/faint if space allows; omit if crowded)

| Display Label | Type | x | y | Notes |
|---|---|---|---|---|
| The Emberfell Theocracy / The Ashfast | region (placeholder) | 80 | 62 | Optional italic below "The Emberfells." Omit if tight. |
| The Hethewood | forest | 72 | 38 | Optional italic adjacent to "The Hethewald Free Holds." Omit if tight. |
| The Sunmark Wilds | forest | 44 | 80 | Optional italic adjacent to "The Sunmark." Omit if tight. |
| The Sallow Marches | wetland | 58 | 84 | Optional italic adjacent to "The Sallowmarch Protectorate." Omit if tight. |
| The Cindern Waste | badland | 84 | 66 | Ash badland; faint ominous wash; no explanation |
| The Bonepan Flats | badland | 56 | 74 | Salt-pan badland around the Saltmere |
| The Mirewend Sinks | wetland | 28 | 40 | Boglands S of the NW cluster |
| The Ghostmark Range | mountain range | 58 | 72 | Low mountains ringing the Saltmere |
| The Wracking Straits | strait | 2 | 64 | Far-W narrows |
| to overseas lands (Surren) | edge annotation | — | S edge | South edge-arrow only; never drawn as part of Orrun |
| to overseas lands (Iron Skards) | edge annotation | — | N edge | North edge-arrow only |
| The Sundered Isles (Far Wrack) | edge annotation | — | W edge | Far-W edge note only |

---

## Section G — Duplicate Rules

Every feature below must appear **no more than once**. All other references to it (in route context, adjacency notes, or alternate names) are aliases — do not render them as additional labels.

- Render **Caradril** exactly once. Do not add a second label for: Caradril as a region, Caradril as a route anchor, or Caradril as the Stillwater gateway.
- Render **The Pale Sea** exactly once as a body label. One additional coastline repetition along the W coast is allowed only if the ocean area is large.
- Render **The Greatspine / Sundering Wall** exactly once (one range, one label).
- Render **The Glassmere League** exactly once. Do not add a second label from the Glasswater river-name root or from route-anchor mentions.
- Render **Hollowmere** exactly once. The Hollowmere basin is dark water beneath the town label — no separate basin label.
- Render **The Saltmere** exactly once ON the water body. Render **The Saltmere Reaches** exactly once ON the surrounding land. Do not stack these labels.
- Render **The Wender Steppe** exactly once. Do not add "The Wender Steppe (steppe)" or any terrain-type suffix as a second label.
- Render **Concord Heartlands** exactly once as the primary label. Never use "the fallen Concord heart" as the primary label.
- Render **The Emberfells** exactly once. The Emberfell Theocracy label is optional italic below — if rendered, it is a subtitle, not a second terrain label.
- Route-anchor settlements (Wrackmouth, Caradril, etc.) are named as route endpoints — do not render them as additional separate place labels.
- Every other feature listed in Sections D–F: render exactly once.

---

## Section H — Route and River Geometry

Draw each as a single polyline through its waypoints. Place the route label once near the stated label position. Route labels are NOT place labels — do not render a waypoint as a separate location.

**Routes:**

| Label | Type | Waypoints (x,y) | Label Position | Notes |
|---|---|---|---|---|
| Verdance Road | land route | (34,35) → (55,50) | around (44,43) | Up-Verdance into settled Orrun |
| Glasswater Run | river/road corridor | (55,50) → (66,90) | around (60,66) | Main commercial artery |
| Greatspine Crown Road *(contested)* | mountain pass | (55,50) → (62,56) → south | around (61,54) | Mark "contested"; through the cordillera |
| Salt Road | land route | (14,21) → (60,70) | around (37,54) | Overland salt/relic caravan track |
| Hethe Tollway | land route | (74,18) → (80,50) | around (77,34) | Forest-river toll corridor |
| Pale Coast Sea-Route | sea route | (12,23) → (34,35) → south | W coast / NW waters | Fast water-route along the west coast |
| South Sea Lanes | sea route | (66,90) → off-map | S sea | Dashed arrows + edge annotation "to overseas lands" |

**Rivers (polylines):**

| Label | Waypoints (x,y) | Label Position | Notes |
|---|---|---|---|
| Verdance | ~(48,46) → (34,35) → ~(15,32) | near (34,35) | NW-quarter great river; reaches the Pale Sea south of the Pale Coast. Label once. |
| Glasswater | (58,40) → (55,50) → (64,88) | near (58,68) | Continent's largest river; do not duplicate with Glassmere League label |
| Mardenflow | (52,64) → (58,84) → (66,92) | near (55,76) | Southern plains river; floods seasonally |
| Hethe | (74,22) → east → (80,50) | near (78,40) | Eastern trade river |
| Mirewend | (25,16) → (24,23) → NW drain | near (24,22) | NW cluster river; label once |
| Ammet | ~(25,30) → joins Verdance or coastal | near (25,30) | The Vale's river; label once |

---

## Section I — Region Footprints

Use these footprints for area-fills, tinted washes, and label placement. Positions are on the 0–100 grid.

| Display Label | center_x | center_y | approx_bounds | Adjacency |
|---|---|---|---|---|
| Sundering Reach | 24 | 23 | X 20–28, Y 19–28 | Center of NW cluster |
| Ashgarden Vale | 25 | 31 | X 21–30, Y 28–35 | S of Reach |
| Tollwood | 32 | 22 | X 29–36, Y 18–26 | E of Reach |
| Pale Coast | 14 | 21 | X 10–18, Y 17–26 | W of Reach |
| The Verdance Reaches | 42 | 42 | X 38–48, Y 38–48 | SE of Caradril |
| The Highmark Spine | 35 | 9 | X 26–44, Y 8–11 | Far-N wall over the cluster |
| The Sunder Heights | 24 | 15 | X 21–28, Y 12–18 | N highlands of cluster |
| The Greyfens | 22 | 25 | X 19–25, Y 23–28 | Fog marsh SW of Hollowmere |
| The Glassmere League | 55 | 50 | X 50–60, Y 45–55 | Central interior |
| The Marrowdowns | 50 | 66 | X 45–55, Y 60–70 | S-central uplands |
| The Saltmere Reaches | 60 | 70 | X 55–66, Y 66–76 | S-central, ringing the Saltmere sea |
| The Sallowmarch Protectorate | 58 | 84 | X 53–63, Y 80–88 | S coast delta |
| The Hollow Gulf Ports | 66 | 90 | X 60–72, Y 86–94 | S coast |
| The Wender Steppe | 46 | 16 | X 40–55, Y 12–22 | N-central beyond Greatspine |
| The Karran Marches | 74 | 18 | X 70–80, Y 14–24 | NE frontier |
| The Emberfells | 80 | 60 | X 76–86, Y 55–66 | SE-central volcanic |
| Concord Heartlands | 62 | 56 | X 58–66, Y 52–60 | Central-SE ruin-country |
| The Hethewald Free Holds | 72 | 40 | X 66–78, Y 34–46 | E-central forest |
| The Sunmark | 44 | 80 | X 38–50, Y 75–85 | S sacred-grove territory |
| The Pale Sea | 4 | 30 | X 0–10, Y 5–60 | W/NW ocean |
| The Sunder Ocean | 50 | 2 | X 20–70, Y 0–6 | N ocean |
| The Calm Reach | 82 | 92 | X 70–95, Y 85–98 | SE/S warm sea |
| The Hollow Gulf | 66 | 92 | X 60–72, Y 88–96 | S-coast bay |
| The Saltmere | 60 | 70 | X 55–66, Y 66–75 | S-central inland salt sea |
| The Greatspine / Sundering Wall | 60 | 51 | diagonal X 50–70, Y 38–64 | Continental cordillera NW–SE |
| The Karran Teeth | 74 | 16 | X 70–80, Y 12–22 | NE range |
| The Ghostmark Range | 58 | 72 | X 53–63, Y 68–76 | Low S-central mountains |
| The Hethewood | 72 | 38 | X 64–80, Y 32–46 | Great eastern forest |
| The Cindern Waste | 84 | 66 | X 80–90, Y 62–72 | Ash badland E of Emberfells |
| The Bonepan Flats | 56 | 74 | X 51–61, Y 70–78 | Salt-pan badland |
| The Sallow Marches | 58 | 84 | X 52–64, Y 80–90 | S-coast deltaic wetland |
| The Mirewend Sinks | 28 | 40 | X 24–34, Y 36–44 | Boglands S of NW cluster |

---

## Section J — Overlapping Terrain/Region Label Rules

Follow these rules exactly to avoid stacking or doubling labels:

1. **The Wender Steppe:** render ONE label only: "The Wender Steppe." Apply faint grass-green visual fill to the steppe terrain. Do NOT render "The Wender Steppe (steppe)" or any terrain-type suffix as a separate label.
2. **The Hethewald Free Holds / The Hethewood:** render "The Hethewald Free Holds" as the primary label. If space allows, render "The Hethewood" as smaller italic adjacent to it — never stacked at the same position. If tight, omit "The Hethewood."
3. **The Sunmark / The Sunmark Wilds:** render "The Sunmark" as the primary label. If space allows, render "The Sunmark Wilds" as smaller italic adjacent — never stacked. If tight, omit "The Sunmark Wilds."
4. **The Sallowmarch Protectorate / The Sallow Marches:** render "The Sallowmarch Protectorate" as the primary label. If space allows, render "The Sallow Marches" as smaller italic adjacent — never stacked. If tight, omit "The Sallow Marches."
5. **The Emberfells / The Emberfell Theocracy:** render "The Emberfells" as the terrain label (standard). If space allows, render "The Emberfell Theocracy / The Ashfast" as smaller italic below — never stacked. If tight, omit the theocracy label.
6. **The Saltmere / The Saltmere Reaches:** these are TWO distinct labels at distinct positions. "The Saltmere" goes ON the water body. "The Saltmere Reaches" goes ON the surrounding land. Never stack or place both on the water.
7. **Concord Heartlands:** primary label is "Concord Heartlands." The subtitle "the fallen Concord heart — ruins, contested" is optional italic below. Never use only the subtitle as the primary label.
8. **The Marrowdowns:** region and terrain are the SAME label — render once only.

---

## Section K — Post-Generation Audit Checklist

Run this checklist after generating the map. Any "No" is an error — fix or regenerate.

1. Is this a single continuous map with NO inset, NO mini-map, NO overlay box, NO "you are here" panel?
2. Is the NW campaign frontier (Sundering Reach, Ring 1, Caradril) shown directly on the main map at somewhat higher local detail?
3. Are ALL labels player-safe? (No Concord Deep, Under-Shrine, Hollow Court, node-network, underground callouts, or depth annotations?)
4. Are there no invented regions, seas, mountains, rivers, or cities not in Sections D–F above?
5. Are the major seas correctly placed: Pale Sea (W coast), Sunder Ocean (N), Calm Reach (SE/S), Hollow Gulf (S coast)?
6. Is the NW campaign cluster in the far northwest quadrant (upper-left area)?
7. Does the color gradient run cold-grey NW → warm-ochre SE?
8. Are far placeholder regions rendered softer and less detailed than the NW cluster?
9. Are all **Required Labels** (Section D) present on the map?
10. Does every feature appear exactly once (no duplicates)?
11. Is "The Wender Steppe" rendered as ONE label only (no "(steppe)" suffix)?
12. Is "Concord Heartlands" the primary label (not "the fallen Concord heart")?
13. Is "The Saltmere" on the water and "The Saltmere Reaches" on the surrounding land (not stacked)?
14. Are all route/river labels placed once only (not duplicated at each waypoint)?
15. Are all label spellings correct relative to Sections D–F (check proper names carefully)?

---

## ——— END COPY ———

---

## Related Files (repo use)

- [`PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md`](PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md) — authoritative repo source; this packet is derived from it
- [`FULL_WORLD_MAP_PROMPTS.md`](FULL_WORLD_MAP_PROMPTS.md) — repo-aware generation prompts (Prompt 1 for full continent; Prompt 5 for campaign-area standalone zoom)
- [`FULL_WORLD_MAP_AUTHORITY.md`](FULL_WORLD_MAP_AUTHORITY.md) — prose geography and lore
- [`FULL_WORLD_MAP_COORDINATES.md`](FULL_WORLD_MAP_COORDINATES.md) — raw 0–100 grid coordinates
