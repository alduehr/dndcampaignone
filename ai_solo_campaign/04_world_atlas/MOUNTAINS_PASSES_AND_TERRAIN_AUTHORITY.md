# MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md — Deterministic Terrain Geometry

---
type: region
secrecy: mixed
status: static
region: Orrun
factions: []
level_range: 1-20
related: [CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, WATER_AND_SHORELINE_AUTHORITY.md, ROADS_RIVERS_AND_ROUTES_AUTHORITY.md, MAP_FEATURE_REGISTRY.md, PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md]
tags: [type:map, secrecy:mixed, function:cartography, terrain-polygon, coordinates, orrun, full-continent]
---

> **Secrecy classification:** Mixed. Terrain geometry is player-safe; the only DM-only exclusion is that no Concord-Deep / node-network annotation may appear inside any terrain zone. Never hand directly to the player.

## AI Use

Deterministic geometry for every mountain range, highland, volcano, forest, wetland, steppe, badland, and downs of Orrun. All coordinates are full-continent **render-grid** (X=0 west, X=100 east, Y=0 north, Y=100 south). Ranges are polylines (spine); zones are polygons. Includes named passes and road crossings. Use to draw terrain fills and place terrain labels without guessing.

---

## MOUNTAIN RANGES (spine polylines)

### The Highmark Spine
- **Type:** mountain range (far-N barrier wall; parent of the Sunder Heights)
- **Spine polyline:** (26,10) W end → (35,9) → (44,8) E end
- **Key passes:** Highmark passes (~30,8 / ~40,8) — far-N frontier, optional late expansion.
- **Road crossings:** none authored (barrier); the passes are the only way N.
- **Adjacent settlements:** Harrowgast (25,17, below the W spine).
- **Terrain art:** a cold grey wall closing the top of the NW quarter; snow-capped.
- **Player-safe label:** "The Highmark Spine" · **Confidence:** MEDIUM (W) / LOW (E)

### The Sunder Heights
- **Type:** broken highlands / old mined mountains (the Reach's name-source)
- **Zone polygon:** (21,18)→(28,13)→(28,18)→(21,21) (highland belt below the Highmark Spine)
- **Key passes:** old mine-adits and ridge-paths (Harrowgast workings).
- **Road crossings:** the Heights causeway (toward Harrowgast).
- **Adjacent settlements:** Harrowgast (25,17).
- **Terrain art:** broken grey ridges, ruined Concord works, cold.
- **Player-safe label:** "The Sunder Heights" · **Confidence:** HIGH
- **DM-only exclusion:** the Deep Adit (D05) and Concord Relay-Vault (D18) are node-fragments here — surface ruins only on player maps; no network annotation.

### The Karran Teeth
- **Type:** mountain range (NE; isolates the northeast)
- **Spine polyline:** (70,20) → (74,16) → (80,13)
- **Key passes:** Karran warlord passes (LOW).
- **Road crossings:** the Hethe Tollway head (Karran-Gate).
- **Adjacent settlements:** Brask's Hold (73,17), Karran-Gate (76,20).
- **Terrain art:** jagged isolated peaks, mine-scarred.
- **Player-safe label:** "The Karran Teeth" · **Confidence:** LOW

### The Greatspine / Sundering Wall
- **Type:** continental cordillera (the master divider; NW–SE axis)
- **Spine polyline:** (50,38) NW end → (58,48) → (62,56) → (70,64) SE end
- **Key passes:** the Greatspine passes (~60,52) — the Crown Road crosses here.
- **Road crossings:** Greatspine Crown Road (contested), at (60,52).
- **Adjacent settlements:** Crownmouth (60,54, astride the ruin), the Pilgrim Camps (63,58).
- **Terrain art:** a great diagonal range splitting the continent; passes gate interior trade.
- **Player-safe label:** "The Greatspine / Sundering Wall" (one label; "/ Sundering Wall" may be a subtitle) · **Confidence:** LOW

### The Emberfells
- **Type:** volcanic highland (vents, obsidian)
- **Spine polyline:** (76,57) → (80,60) → (84,64)
- **Key passes:** the Ash Roads (pilgrim-ways, 78,59).
- **Road crossings:** the Ash Roads through the highland.
- **Adjacent settlements:** Ashfast (80,62), Cinderhold (83,65).
- **Terrain art:** ash-grey/obsidian-black volcanic peaks; the Cindern Waste in the E rain-shadow.
- **Player-safe label:** "The Emberfells" (terrain label first; the Emberfell Theocracy label optional below) · **Confidence:** LOW

### The Ghostmark Range
- **Type:** low eroded mountains (ringing the Saltmere)
- **Spine polyline:** (53,70) → (58,72) → (63,74)
- **Adjacent settlements:** Saltcairn (63,73, range-edge).
- **Terrain art:** low, eroded, "haunted" hills around the inland salt sea.
- **Player-safe label:** "The Ghostmark Range" (optional/faint) · **Confidence:** LOW

---

## FORESTS (polygons)

### Tollwood
- **Polygon:** (29,18)→(36,18)→(36,26)→(29,26) · **Centroid:** (32,22)
- **Passes/crossings:** the East Road threads it; the deep wood off-road is gated.
- **Adjacent settlements:** Hartfell (33,22), Coldhearth (34,20), Tollstone Cross (30,22).
- **Terrain art:** deep old-growth; overgrown Concord toll-roads.
- **Player-safe label:** "Tollwood" · **DM-only exclusion:** the Old Mast (D12) deep heart — label-only "deep wood — do not enter"; no network annotation. · **Confidence:** HIGH

### The Hethewood
- **Polygon:** (64,32)→(80,32)→(80,46)→(64,46) · **Centroid:** (72,38)
- **Adjacent settlements:** Hethemoot (71,39), Greenward (68,43).
- **Terrain art:** great eastern forest (Tollwood is its NW finger).
- **Player-safe label:** "The Hethewood" (secondary to "The Hethewald Free Holds") · **Confidence:** LOW

### The Sunmark Wilds
- **Polygon:** (38,75)→(50,75)→(50,86)→(38,86) · **Centroid:** (44,80)
- **Adjacent settlements:** the Great Grove at Sunhollow (44,80), the Grove-Camps (40,77).
- **Terrain art:** warm sacred-grove forest.
- **Player-safe label:** "The Sunmark Wilds" (secondary to "The Sunmark") · **Confidence:** LOW

---

## WETLANDS (polygons)

| Zone | Polygon (x,y) | Centroid | Adjacent | Label | Conf. |
|---|---|---|---|---|---|
| The Greyfens | (19,23)→(25,23)→(25,28)→(19,28) | 22,25 | Greywater Holm (22,26), Hollowmere (24,23) | "The Greyfens" | HIGH |
| The Mirewend Sinks | (24,36)→(34,36)→(34,44)→(24,44) | 28,40 | (between cluster and rising mid-continent) | "The Mirewend Sinks" | LOW |
| The Sallow Marches | (52,80)→(64,80)→(64,90)→(52,90) | 58,84 | Fenward (57,82), Reedmouth (60,85) | "The Sallow Marches" (secondary to the Protectorate) | LOW |

---

## STEPPE / DOWNS / BADLANDS (polygons)

| Zone | Type | Polygon (x,y) | Centroid | Adjacent | Label | Conf. |
|---|---|---|---|---|---|---|
| The Wender Steppe | steppe | (40,12)→(55,12)→(55,22)→(40,22) | 46,16 | Cold Springs (45,16), the Sky-Stones (42,14) | "The Wender Steppe" (ONE label; no "(steppe)" suffix) | LOW |
| The Marrowdowns | chalk downs | (45,60)→(55,60)→(55,70)→(45,70) | 50,66 | Marrowmoot (50,66), Penmark Hold (47,63) | "The Marrowdowns" (region+terrain = one label) | LOW |
| The southern downs | open downs (in-cluster) | (33,32)→(42,32)→(42,36)→(33,36) | 37,34 | (Vale→Caradril approach) | (faint; the S approach) | MEDIUM |
| The Cindern Waste | ash badland | (80,62)→(90,62)→(90,72)→(80,72) | 84,66 | (Emberfells rain-shadow) | "The Cindern Waste" (faint, ominous, unexplained) | LOW |
| The Bonepan Flats | salt badland | (51,70)→(61,70)→(61,78)→(51,78) | 56,74 | (around the Saltmere) | "The Bonepan Flats" | LOW |

---

## NAMED PASSES (point markers)

| Pass | Coords | Range | Road | Conf. |
|---|---|---|---|---|
| Highmark passes (W) | 30,8 | Highmark Spine | far-N frontier | LOW |
| Highmark passes (E) | 40,8 | Highmark Spine | far-N frontier | LOW |
| Greatspine passes (Crown Road) | 60,52 | Greatspine | Crown Road (contested) | LOW |
| Karran passes | 74,16 | Karran Teeth | Hethe Tollway head | LOW |
| Ash Roads pass | 78,59 | Emberfells | Ash Roads (pilgrim) | LOW |
| Sunder Heights ridge-paths | 24,15 | Sunder Heights | Heights causeway | MEDIUM |

---

## Terrain Art Notes (what the map should show)

- **NW (cold frontier):** greys, peat-browns, fog-whites. Broken Sunder Heights ridges; the Highmark Spine wall; fog over the Greyfens and Hollowmere basin.
- **Center (settled):** greens and earth tones; river-plains (Glasswater/Verdance); chalk downs (Marrowdowns).
- **SE (warm/volcanic):** warm ochres → ash-greys → obsidian-blacks (Emberfells, Cindern Waste, Glass Coast).
- **S (warm):** warm forest (Sunmark Wilds), fever-delta greens (Sallow Marches), warm-blue southern sea (Calm Reach).
- **N-central (steppe):** faint grass-green wash (Wender Steppe) — terrain fill only, single region label.

## DM-Only Terrain Exclusions (NEVER on player maps)

No Concord-Deep, node-network, "machine," depth, or relay annotation may appear inside ANY terrain zone — not in the Sunder Heights, Tollwood deep, Greyfens, far ruins, or anywhere. Surface ruins inside terrain zones are drawn broken and unexplained. The endgame is vertical beneath Hollowmere, never inside a terrain zone on the map.

## Unresolved Terrain Gaps

1. Far-range crest lines (Greatspine, Karran Teeth, Emberfells) are endpoint-pair polylines, not surveyed ridgelines.
2. Far-zone polygons (Hethewood, Sunmark Wilds, Cindern Waste, Bonepan Flats, Marrowdowns, Wender Steppe) are loose rectangles around centroids; meant to be drawn soft/faint.
3. The Ghostmark Range and the southern downs are LOW/MEDIUM placeholders.

All gaps are non-blocking for player-safe and DM-only terrain rendering.

## Related Files

- [`CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`](CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md) · [`WATER_AND_SHORELINE_AUTHORITY.md`](WATER_AND_SHORELINE_AUTHORITY.md) · [`ROADS_RIVERS_AND_ROUTES_AUTHORITY.md`](ROADS_RIVERS_AND_ROUTES_AUTHORITY.md) · [`MAP_FEATURE_REGISTRY.md`](MAP_FEATURE_REGISTRY.md)
