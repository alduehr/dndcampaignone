# WORLD_MAP_AUTHORITY.md — Master Cartographic Reference

---
type: region
secrecy: mixed
status: static
region: Orrun
factions: []
level_range: 1-20
related: [MAP_DESCRIPTION.md, WORLD_OVERVIEW.md, WORLD_MAP_COORDINATES.md, WORLD_MAP_LAYERS.md, WORLD_MAP_PROMPTS.md, TRAVEL_ROUTES_RING1.md, REGION_INDEX.md, ../03_canon/CANON.md, ../03_canon/DM_ONLY_CANON.md]
tags: [type:map, secrecy:mixed, function:cartography, world, orrun, authority]
---

## AI Use

This is the **single cartographic source of truth** for Vael/Orrun. Load it when:
- Placing any new location relative to existing ones.
- Answering a player's "where is X relative to Y" or "what lies beyond" question.
- Generating or commissioning a world/region map (use with `WORLD_MAP_COORDINATES.md`, `WORLD_MAP_LAYERS.md`, `WORLD_MAP_PROMPTS.md`).
- Confirming travel-time/distance plausibility (use with `MAP_DESCRIPTION.md` and `TRAVEL_ROUTES_RING1.md`).

**This file does not override established travel times or region descriptions.** It records the spatial frame those facts already imply, and adds map-authoritative *placeholders* for not-yet-authored midgame/late/endgame regions so the AI DM never invents major geography on the fly. Keep DM-only geography (forbidden zones, hidden node-network, endgame placements) out of player-facing narration.

---

## 1. Authoritative World Shape

- **World:** **Vael.** **Continent of play:** **Orrun.** The campaign occupies the **northwestern quarter of Orrun** for Acts 1–4 and never requires the rest of the continent to be mapped in detail.
- **Outline (NW quarter):** a cold, wet **shelf of land between mountains and sea** — high broken country in the north, a low ruin-strewn fen basin at the center, farmland rising to the south, deep forest to the east, and an open sea edge to the west. The land tilts and drains toward the central basin (the keystone).
- **Size feel:** the mapped play-area is roughly **a 12–14 day overland span corner to corner** (Hollowmere → Caradril ≈ 10–12 days SE is the longest established run). At Orrun-continental scale this NW quarter is a **frontier corner**, not the heartland. The rest of Orrun (south, east-interior, far north) exists but is **off-map and largely DM-only / future**.
- **Orientation convention:** **north at top, west at left** (standard). All coordinates in `WORLD_MAP_COORDINATES.md` follow this.

## 2. Major Landmasses and Bodies of Water

- **The cold sea (the Pale Sea — new name, see §10):** the open western/northwestern ocean against which the Pale Coast stands. Storm-battered, fish-rich, the source of the frontier's drowned dead and its rite-salt.
- **The Verdance (river):** Orrun's major river in this quarter; rises in the southern/eastern uplands, runs southeast, widens into the **Stillwater** (Caradril's inland harbor-lake), and reaches the sea south of the mapped area. The Pale Coast's water-route to Caradril runs **down the coast to the Verdance mouth, then up the Verdance to the Stillwater.**
- **The Mirewend (river):** the Sundering Reach's slow, peat-dark artery; drains the central fen basin; floods in autumn.
- **The Ammet (river):** the Ashgarden Vale's river; its headwaters rise toward the Tollwood; flows through the Vale's farmland.
- **The Hollowmere basin:** a wide flooded hollow at the dead-center of the Reach over the great drowned Concord shrine — the **lowest point and drainage sink** of the mapped land; everything tilts toward it.
- **The Stillwater:** Caradril's harbor-lake, where the Verdance broadens.
- **The Skerries:** offshore sea-stacks and reefs west of the Pale Coast (gated, dangerous).

## 3. Major Geographic Features

| Feature | Type | Position | Notes |
|---|---|---|---|
| The Sunder Heights | Broken highlands / old mountains | N of the Reach | The mined Concord ridges; the Reach's name-source; cold, ruined. |
| The Tollwood | Deep old-growth forest | E of the Reach | Concord toll-roads; the gated deep "Old Mast." |
| The Greyfens | Fog-bound marsh | within/SW of the Reach | The most dangerous Reach wetland. |
| The Ashgarden Vale | Rolling farmland / low green hills | S of the Reach | Orchards, shrine-towns; the gentle south. |
| The Pale Coast | Sea-cliffs, shingle coves, salt-pans | W of the Reach | The western sea edge. |
| The Pale Sea | Open ocean | W/NW | The cold sea. |
| The southern downs | Open sheep-downs | S, between the Vale and Caradril | The southern approach to Caradril. |
| **The Highmark Spine** (new) | Continental mountain wall | N/NE, beyond the Sunder Heights | The Heights' parent range; the wall that closes the mapped quarter to the north. **Placeholder — barrier, not yet a play-region.** |

## 4. Major Political / Cultural Regions

**Currently authored (playable now):**
1. **Sundering Reach** (center) — starting region. Lvl 1–6/8.
2. **Ashgarden Vale** (south) — Ring 1. Lvl 1–6.
3. **Tollwood** (east) — Ring 1. Lvl 2–7.
4. **Pale Coast** (west) — Ring 1. Lvl 2–7.
5. **Caradril** (southeast) — first major city / city-state. Mid-game hub, Lvl ~5–12.

**Named map-authoritative placeholders (NOT yet authored; do not deep-detail):** see §6–§8.

## 5. Placement of the Established Play-Area

```
                       THE HIGHMARK SPINE (far N) — barrier range
                                  |
                          SUNDER HEIGHTS (N)
                                  |
   PALE SEA (W) — PALE COAST (W) — SUNDERING REACH — TOLLWOOD (E)
        |             \           [Hollowmere basin]      \
        |              \                |                   \
        |               \        ASHGARDEN VALE (S)          \
   (Verdance mouth, S) ___\____________|____ southern downs ___\
                            \           |                       CARADRIL (SE)
                             \___ sea + Verdance river route ___/
```

- **Hollowmere** sits at the **dead center** of the mapped quarter, on the basin — the spatial and dramatic keystone. Everything radiates from it.
- **The three Ring 1 regions** form a fan around the Reach: Vale (S), Tollwood (E), Coast (W). All three overland roads, plus the Coast's sea-route, **funnel southeast to Caradril.**
- **Caradril** is the mapped quarter's southeast corner and its only true city.

## 6. Likely Midgame Region Placement (Levels 5–12)

Midgame play is **anchored at Caradril** (already authored) and ranges across the Ring 1 regions and the deeper Reach. The next outward expansion ("Ring 2") will sit **beyond Caradril and along the Verdance**, deeper into settled Orrun. Map-authoritative placeholders:

| Placeholder | Position | 1-sentence identity | Level | Secrecy | Expansion note |
|---|---|---|---|---|---|
| **The Verdance Reaches** (new) | SE/S, up the Verdance beyond Caradril toward Orrun's interior | The river-road into richer, older, more settled Orrun — the trade and political world Caradril plugs into. | 8–12 | player-safe (placeholder) | Ring 2 hub-corridor; detail when the player commits past Caradril. |
| **The Sunder Heights (deep)** | N, beyond Harrowgast | The high broken Concord mines proper — colder, older ruins and a secondary-node belt. | 6–10 | mixed | Already partly authored (Reach wilderness); deepen as a midgame ruin-frontier. |
| **The Tollwood deep (the Old Mast)** | E, forest heart | The gated pre-Concord woodland power, opened only mid/late. | 6–10+ | mixed (gated) | Authored as a gated landmark-power; do NOT escalate into a new central mystery. |

## 7. Likely Late-Game Region Placement (Levels 13–16)

Late-game converges back toward the **keystone (Hollowmere)** and the Concord's continental truth. Placeholders:

| Placeholder | Position | 1-sentence identity | Level | Secrecy | Expansion note |
|---|---|---|---|---|---|
| **The Concord Deep / the buried network** (new) | DM-only; *under* the mapped land, radiating from the Hollowmere basin | The drowned shrine-network beneath Orrun — the harvest machine's true continental shape, reached through the keystone. | 13–16 | **DM-only** | The "map beneath the map"; see `WORLD_MAP_LAYERS.md` Layer 7. Never a surface region. |
| **The Highmark Spine passes** (new) | N/NE barrier range | The far cold passes where the oldest Concord works and the most isolated survivors lie; an optional late frontier. | 12–16 | mixed | Optional late expansion; barrier/frontier, not required by the arc. |

## 8. Likely Endgame / Forbidden Region Placement (Levels 17–20)

| Placeholder | Position | 1-sentence identity | Level | Secrecy | Expansion note |
|---|---|---|---|---|---|
| **The Under-Shrine / the Drowned Keystone** | DM-only; the deepest level **beneath the Hollowmere basin** | The dormant heart of the harvest where the Hollow Court sleeps — the campaign's final place. | 17–20 | **DM-only / forbidden** | The endgame "region" is **vertical, not lateral** — straight down through the keystone, not across the map. Telegraphed as lethal at all low levels. Built in Stage 12/15. **Never named to the player as the Court's seat.** |
| **The Quiet Country** (afterlife) | Cosmological, not geographic | The finite afterlife the harvest drained; reachable only by death/late-arc rite. | 17–20 | **DM-only** | A cosmological "place," not a map region. Do not render on any spatial map. |

**Endgame cartographic decision (recorded):** the campaign's apex is **not** a distant forbidden continent — it is **directly below the starting town.** The "forbidden region" is therefore placed at the **center-and-down** of the map (the basin), not at a far edge. This preserves the authored arc, which keeps the climax under Hollowmere.

## 9. Map Scale Assumptions

- **Travel-to-distance (overland, fair autumn weather, on Concord road):** ~**15–20 miles/day on foot**, ~**20–25 miles/day by cart**. Off-road in fen/forest **halves** that and adds hazard. (These are working conversions for map-drawing only; the canonical unit of travel is the **established day-count**, not miles — always defer to `MAP_DESCRIPTION.md` and `TRAVEL_ROUTES_RING1.md` day-counts.)
- **Anchor distances (canon, do not contradict):** Hollowmere → Caradril ~10–12 days SE; Hollowmere → Orchardmere (Vale hub) ~5–6 days S; Hollowmere → Hartfell (Tollwood hub) ~4–5 days E; Hollowmere → Saltmargin ~5 days W, → Wrackmouth ~7–8 days W; Wrackmouth → Caradril ~6–7 days by sea/Verdance.
- **Grid:** the 0–100 normalized grid in `WORLD_MAP_COORDINATES.md` spans **only the mapped NW quarter**, not all Orrun. (0,0) = NW corner; (100,100) = SE corner.
- **Rough physical span of the grid:** corner-to-corner ≈ **200–260 miles** (consistent with ~12-day longest run). One grid unit ≈ **2–2.6 miles**. Treat as approximate.

## 10. New Geographic Names Coined This Pass

All checked against `NAMING_REGISTRY.md` (no collisions) and registered there:

| Name | Type | Status | Secrecy |
|---|---|---|---|
| **The Pale Sea** | Ocean (W/NW, against the Pale Coast) | player-safe | player-safe |
| **The Highmark Spine** | Mountain range (far N/NE barrier; parent of the Sunder Heights) | player-safe (placeholder region) | player-safe |
| **The Verdance Reaches** | Region (Ring 2 placeholder; up the Verdance, SE) | player-safe (placeholder) | player-safe |
| **The Concord Deep** | DM-only buried node-network ("map beneath the map") | DM-only (placeholder) | dm-only |

(Existing names — Verdance, Stillwater, Mirewend, Ammet, Skerries, Sunder Heights, Greyfens, etc. — are already registered and unchanged.)

## 11. Secrecy Section

### Known to the player (player-safe)
- The five regions (Reach, Vale, Tollwood, Coast, Caradril) and their relative directions.
- The Pale Sea to the west; the Verdance river and the Stillwater; the Mirewend and Ammet rivers.
- The Sunder Heights to the north; the Tollwood to the east; the Greyfens; the southern downs.
- That all roads (and the sea-route) lead to Caradril; that Caradril plugs into a wider, richer Orrun to the southeast.
- That the Hollowmere basin holds a great drowned Concord ruin (what it *is* is unknown).

### Rumored / half-known to the player
- That something far north past the Heights closes the land (the Highmark Spine is a name folk use loosely for the cold wall on the horizon).
- That the dead "walk toward the water" — toward the basin. (True; the spatial tell of the keystone.)
- That the Concord's roads and shrines form a network (folk see ruins everywhere; the *network* truth is gated).

### Unknown to the player (until earned)
- That the basin is the **center and lowest point** of a deliberate drainage geography (the keystone).
- The existence/shape of **the Concord Deep** (the buried node-network).
- That the endgame place is **straight down beneath Hollowmere**, not a distant land.

### DM-only (never narrate as map fact)
- The Concord Deep, the Under-Shrine/Drowned Keystone, the Hollow Court's seat, the Quiet Country's "geography," and the node-network linking the basin, the Deep Adit, the Sunken Wards, Saint Veddow's, the Drowned Lamp, the Sunken Tollhouse, and the Tollwood's pre-Concord deep. See `DM_ONLY_CANON.md` and `WORLD_MAP_LAYERS.md` Layers 2 and 7.

## Related Files

- [`MAP_DESCRIPTION.md`](MAP_DESCRIPTION.md) · [`WORLD_OVERVIEW.md`](WORLD_OVERVIEW.md)
- [`WORLD_MAP_COORDINATES.md`](WORLD_MAP_COORDINATES.md) · [`WORLD_MAP_LAYERS.md`](WORLD_MAP_LAYERS.md) · [`WORLD_MAP_PROMPTS.md`](WORLD_MAP_PROMPTS.md)
- [`TRAVEL_ROUTES_RING1.md`](TRAVEL_ROUTES_RING1.md) · [`REGION_INDEX.md`](REGION_INDEX.md)
- [`../05_regions/SUNDERING_REACH.md`](../05_regions/SUNDERING_REACH.md) · [`../05_regions/ASHGARDEN_VALE.md`](../05_regions/ASHGARDEN_VALE.md) · [`../05_regions/TOLLWOOD.md`](../05_regions/TOLLWOOD.md) · [`../05_regions/PALE_COAST.md`](../05_regions/PALE_COAST.md) · [`../06_settlements/CARADRIL.md`](../06_settlements/CARADRIL.md)
- [`../03_canon/CANON.md`](../03_canon/CANON.md) · [`../03_canon/PLAYER_SAFE_CANON.md`](../03_canon/PLAYER_SAFE_CANON.md) · [`../03_canon/DM_ONLY_CANON.md`](../03_canon/DM_ONLY_CANON.md)
