# REGION_INDEX.md — Region Index

---
type: index
secrecy: mixed
status: static
region: Orrun
tags: [type:index, secrecy:mixed, regions, orrun, cartography]
related: [WORLD_MAP_AUTHORITY.md, WORLD_MAP_COORDINATES.md, WORLD_OVERVIEW.md, ../00_control/CONTENT_INDEX.md]
---

## AI Use

Quick index of all regions of Orrun — authored (playable now), Ring 2/midgame placeholders, and **full-continent placeholders** (the whole continent, named/positioned, not yet deep-built). For campaign-area cartographic data see `WORLD_MAP_AUTHORITY.md` / `WORLD_MAP_COORDINATES.md`; for **full-continent** data see `FULL_WORLD_MAP_AUTHORITY.md` / `FULL_WORLD_MAP_COORDINATES.md`. **Do not surface DM-only placeholder rows to the player.**

> **Map packets (Cartography Authority Pass, 2026-06-16):** every map-authoritative region below now has a regional map packet in `region_map_packets/REGION_[NAME].md` (local grid, terrain/water/routes/settlements/dungeons, player-safe vs DM-only layers). The four major cities have city packets in `../06_settlements/city_map_packets/`; important settlements have packets in `../06_settlements/settlement_map_packets/`; all 36 adventure sites are coordinate-anchored in `../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`. Master geometry: `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`.

> **Eagle-test depth (Exploration-Determinism Pass, 2026-06-18):** all 13 far-region map packets have been deepened to full D&D-usable depth (level range, solo danger, encounter themes with stat refs, service/facility notes, NPC roster links, mechanical anchors). All 3 far city packets (Glassmere, Calderport, Ashfast) deepened to Caradril-style depth. All 40 settlement map packets (16 NW cluster + 24 far-continent; glob-verified) are at eagle-test floor: 4–8 notable areas at fixed local-grid coords, services, NPC links, 2–3 quest hooks, encounter/treasure refs, Player-Safe + DM-Only layers. Verdict: **CONTINENT IS EXPLORATION-DETERMINISTIC.**

> **Region count note:** you may see "18 regions" in cartography files and "20 regions" in Stage 13/14 encounter/treasure files. Both are correct for their context — the Cindern Waste (Emberfell terrain sub-zone) and the Drowned Steps (Sallowmarch sub-area) are not standalone map regions but do get their own encounter/treasure files. See `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md` §10 and `00_control/STAGE_STATUS.md` (Cartography Determinism Cleanup pass entry) for the definitive reconciliation.

## Authored Regions (Playable Now)

| Region | Dir from Reach | File | Map packet | Level | Secrecy | Grid (X,Y) | Status |
|---|---|---|---|---|---|---|---|
| Sundering Reach | center | `../05_regions/SUNDERING_REACH.md` | `region_map_packets/REGION_SUNDERING_REACH.md` | 1–6/8 | mixed | (50,42) | Deep-built (Stage 3); starting region |
| Ashgarden Vale | south | `../05_regions/ASHGARDEN_VALE.md` | `region_map_packets/REGION_ASHGARDEN_VALE.md` | 1–6 | mixed | (52,68) | Deep-built (Stage 7); Ring 1 |
| Tollwood | east | `../05_regions/TOLLWOOD.md` | `region_map_packets/REGION_TOLLWOOD.md` | 2–7 | mixed | (74,40) | Deep-built (Stage 7); Ring 1 |
| Pale Coast | west | `../05_regions/PALE_COAST.md` | `region_map_packets/REGION_PALE_COAST.md` | 2–7 | mixed | (18,38) | Deep-built (Stage 7); Ring 1 |
| Caradril (city-state) | southeast | `../06_settlements/CARADRIL.md` | `region_map_packets/REGION_CARADRIL.md` + `../06_settlements/city_map_packets/CARADRIL_CITY_MAP.md` | 5–12 | mixed | (82,80) | Deep-built (Stage 4); first major city / mid-game hub |

> **Far-region map packets:** the full-continent placeholders below each have a packet too — `region_map_packets/REGION_VERDANCE_REACHES.md`, `REGION_GLASSMERE_LEAGUE.md`, `REGION_MARROWDOWNS.md`, `REGION_SALLOWMARCH_PROTECTORATE.md`, `REGION_HOLLOW_GULF_PORTS.md`, `REGION_WENDER_STEPPE.md`, `REGION_KARRAN_MARCHES.md`, `REGION_EMBERFELL_THEOCRACY.md`, `REGION_SALTMERE_REACHES.md`, `REGION_CONCORD_HEARTLANDS.md`, `REGION_HETHEWALD_FREE_HOLDS.md`, `REGION_SUNMARK.md`, `REGION_HIGHMARK_PASSES.md`. Far cities: `../06_settlements/city_map_packets/GLASSMERE_CITY_MAP.md`, `CALDERPORT_CITY_MAP.md`, `ASHFAST_CITY_MAP.md`.

## Map-Authoritative Placeholders (Named, Positioned, NOT Yet Built)

| Region | Position | File | Level | Secrecy | Grid (X,Y) | Expansion note |
|---|---|---|---|---|---|---|
| The Verdance Reaches | SE, up-Verdance beyond Caradril | `WORLD_MAP_AUTHORITY.md` §6 | 8–12 | player-safe (placeholder) | (92,92) | Ring 2 hub-corridor; detail when player commits past Caradril |
| Sunder Heights (deep) | N, beyond Harrowgast | `WORLD_MAP_AUTHORITY.md` §6 | 6–10 | mixed | (50,18) | Partly authored (Reach wilderness); deepen as midgame ruin-frontier |
| The Highmark Spine (passes) | far N/NE barrier range | `WORLD_MAP_AUTHORITY.md` §3,§7 | 12–16 | mixed | (55,6)/(60,8) | Optional late frontier; barrier, not arc-required |
| The Concord Deep | DM-only; subsurface, under the basin | `WORLD_MAP_LAYERS.md` Layer 7 | 13–16 | **DM-only** | (50,47) | "Map beneath the map"; the buried node-network |
| The Under-Shrine / Drowned Keystone | DM-only; beneath Hollowmere | `WORLD_MAP_AUTHORITY.md` §8 | 17–20 | **DM-only / forbidden** | (50,45) | Endgame; vertical (straight down), never a lateral region |

## Far-Continent Regions (region files built 2026-07-07 — Phase 5 consolidation)

Every far-continent region now has a canonical `05_regions/` file consolidating its authored layers (map packet, Stage 9.5 NPC roster, Stage 10 quests, Stage 12.5 dungeon, arc pack) into the standard region format. These regions remain **lighter than the NW cluster's deep-builds** (settlement gazetteers are the eagle-test map packets, not full `06_settlements/` files) — deepen further only when play warrants. Level values below follow the **authored content** (quest/NPC/packet layer); a few older placeholder values in this table were reconciled to it on 2026-07-07. Full-grid (X,Y) is the full-continent 0–100 grid (NW=0,0).

| Region | Region file | Position | Political form | Level | Secrecy | Full-grid (X,Y) | Map packet |
|---|---|---|---|---|---|---|---|
| The Verdance Reaches | `../05_regions/VERDANCE_REACHES.md` | SE, up-Verdance past Caradril | River-corridor (lords, Ledger, locks) | 8–12 | mixed | (42,42) | `region_map_packets/REGION_VERDANCE_REACHES.md` |
| The Glassmere League | `../05_regions/GLASSMERE_LEAGUE.md` | central, on the Glasswater | Mercantile city-league | 8–13 | mixed | (55,50) | `region_map_packets/REGION_GLASSMERE_LEAGUE.md` |
| The Marrowdowns | `../05_regions/MARROWDOWNS.md` | S-central uplands | Manorial holds / shire-moots | 6–10 | mixed | (50,66) | `region_map_packets/REGION_MARROWDOWNS.md` |
| The Sallowmarch Protectorate | `../05_regions/SALLOWMARCH_PROTECTORATE.md` | S coast (Mardenflow delta) | Protectorate (distant crown) | 10–14 | mixed | (58,84) | `region_map_packets/REGION_SALLOWMARCH_PROTECTORATE.md` |
| The Hollow Gulf Ports | `../05_regions/HOLLOW_GULF_PORTS.md` | S coast | Rival port city-states | 10–15 | mixed | (66,90) | `region_map_packets/REGION_HOLLOW_GULF_PORTS.md` |
| The Wender Steppe | `../05_regions/WENDER_STEPPE.md` | N-central, beyond the Spine | Nomadic tribal confederacy | 8–13 | mixed | (46,16) | `region_map_packets/REGION_WENDER_STEPPE.md` |
| The Karran Marches | `../05_regions/KARRAN_MARCHES.md` | NE (Karran Teeth) | Ungoverned / warlord holds | 9–14 | mixed | (74,18) | `region_map_packets/REGION_KARRAN_MARCHES.md` |
| The Emberfell Theocracy / Ashfast | `../05_regions/EMBERFELL_THEOCRACY.md` | SE-central (Emberfells) | Theocracy (volcanic fire-cult) | 10–15 | mixed | (80,62) | `region_map_packets/REGION_EMBERFELL_THEOCRACY.md` |
| The Saltmere Reaches | `../05_regions/SALTMERE_REACHES.md` | S-central (inland salt sea) | Salt-clan holds / fallen realm | 11–15 | mixed | (60,70) | `region_map_packets/REGION_SALTMERE_REACHES.md` |
| The Concord Heartlands / Ruin'd Crown | `../05_regions/CONCORD_HEARTLANDS.md` | central-SE, astride the Greatspine | Fallen realm (contested ruin) | 13–17 | mixed | (62,56) | `region_map_packets/REGION_CONCORD_HEARTLANDS.md` |
| The Hethewald Free Holds | `../05_regions/HETHEWALD_FREE_HOLDS.md` | E-central (Hethewood) | Confederacy of forest free-holds | 8–13 | mixed | (72,40) | `region_map_packets/REGION_HETHEWALD_FREE_HOLDS.md` |
| The Sunmark | `../05_regions/SUNMARK.md` | S (warm forest/groves) | Sacred tribal territory | 8–13 | mixed | (44,80) | `region_map_packets/REGION_SUNMARK.md` |

> The Highmark Passes remain a map-packet-only barrier frontier (see the table above; `region_map_packets/REGION_HIGHMARK_PASSES.md`) — optional, not arc-required, no `05_regions/` file needed. Other Vael landmasses (Surren, the Iron Skards, the Sundered Isles/Far Wrack) are off-grid overseas placeholders — see `FULL_WORLD_MAP_AUTHORITY.md` §1. The DM-only subsurface "regions" (the Concord Deep; the Under-Shrine/Drowned Keystone) remain in the table above and are **vertical, beneath the NW cluster** — never lateral continental regions.

## Notes

- The endgame "region" is **vertical** — down through the keystone beneath Hollowmere — not a distant land. The campaign arc keeps the climax at the basin.
- All five authored regions connect to the Reach and funnel to Caradril (SE). See `TRAVEL_ROUTES_RING1.md`.
- New geographic names this pass (Pale Sea, Highmark Spine, Verdance Reaches, Concord Deep) are registered in `../00_control/NAMING_REGISTRY.md`.

## Related Files

- [`WORLD_MAP_AUTHORITY.md`](WORLD_MAP_AUTHORITY.md) · [`WORLD_MAP_COORDINATES.md`](WORLD_MAP_COORDINATES.md) · [`WORLD_MAP_LAYERS.md`](WORLD_MAP_LAYERS.md) · [`WORLD_OVERVIEW.md`](WORLD_OVERVIEW.md) · [`MAP_DESCRIPTION.md`](MAP_DESCRIPTION.md)
