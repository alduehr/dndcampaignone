# GAZETTEER_INDEX.md — Orrun World Reference Index

---
type: index
secrecy: player-safe
status: static
tags: [index, gazetteer, orrun]
---

## AI Use

Start here when using `/locations/vael/orrun`. This indexes every file in the folder by category so a DM (running this campaign or any other game in this world) can find what they need without reading `/ai_solo_campaign`.

## Geography — `01_geography/`

| File | Covers |
|---|---|
| [`CONTINENT_OVERVIEW.md`](CONTINENT.md) | Vael/Orrun at a glance — seas, rivers, mountains, all 16 regions, overseas landmasses, scale/travel assumptions |
| [`TRAVEL_AND_ROUTES.md`](travel/travel-and-routes.md) | How travel works, travel-rate tables, major routes across the continent |
| [`regions/*.md`](regions/) | 16 region files: Sundering Reach, Ashgarden Vale, Tollwood, Pale Coast, Verdance Reaches, Glassmere League, Marrowdowns, Sunmark, Sallowmarch Protectorate, Hollow Gulf Ports, Saltmere Reaches, Concord Heartlands, Emberfell Theocracy, Hethewald Free Holds, Wender Steppe, Karran Marches |
| [`wilderness/*.md`](wilderness/) | 7 wilderness zones in play-ready detail — terrain, named natural features, hazards with DCs, fauna, resources: Greyfens, Sunder Heights, Mirewend & Roads, Basin Shore & Holms, Ashgarden Vale Wilds, Tollwood Wilds, Pale Coast Wilds |

*Not covered:* the Highmark Passes (uninhabited barrier country, documented only within `CONTINENT_OVERVIEW.md`/`TRAVEL_AND_ROUTES.md`); Caradril (covered under Settlements, since it's a city-state, not a region).

## Settlements — `02_settlements/`

| File | Covers |
|---|---|
| [`SUNDERING_REACH_SETTLEMENTS.md`](settlements/sundering-reach-settlements.md) | Hollowmere, Kettle Bridge, Saltmargin, Candlewick, Greywater Holm, Harrowgast, Reedford, The Ashwalk Rest |
| [`ASHGARDEN_VALE_SETTLEMENTS.md`](settlements/ashgarden-vale-settlements.md) | Orchardmere, Saint Veddow's Rest, Tilbrook |
| [`TOLLWOOD_SETTLEMENTS.md`](settlements/tollwood-settlements.md) | Hartfell, Coldhearth, Tollstone Cross |
| [`PALE_COAST_SETTLEMENTS.md`](settlements/pale-coast-settlements.md) | Wrackmouth, Cobble Strand |
| [`CARADRIL.md`](settlements/caradril.md) | The first major city, with all 8 districts |
| [`FAR_CONTINENT_ANCHORS.md`](settlements/far-continent-anchors.md) | ~35 light settlement anchors across the 12 far-continent regions |

## Culture — `03_culture/`

| File | Covers |
|---|---|
| [`WORLD_OVERVIEW.md`](culture/world-overview.md) | General introduction to Vael/Orrun |
| [`CALENDAR.md`](culture/calendar.md) | Reckoning, months, week, holidays |
| [`COSMOLOGY_PUBLIC.md`](culture/cosmology-public.md) | The Three Thresholds, the Quiet Country, Remembrances, folk theories |
| [`GODS_AND_FAITHS.md`](culture/gods-and-faiths.md) | Clergy, folk protections and customs |
| [`MAGIC_AND_REMEMBRANCE.md`](culture/magic-and-remembrance.md) | Standard magic plus the public-facing Remembrance wrinkles as world flavor |
| [`LANGUAGES.md`](culture/languages.md) | Common and regional languages |
| [`WORLD_HISTORY_PUBLIC.md`](culture/world-history-public.md) | The Concord, its golden age, the Quietfall, the frontier age — public history only |

## Bestiary — `04_bestiary/`

| File | Covers |
|---|---|
| [`WANDERING_ENCOUNTERS_BY_TERRAIN.md`](bestiary/wandering-encounters-by-terrain.md) | d10 terrain tables, night-camp table, travel modifiers |
| [`COMMON_WILDLIFE.md`](bestiary/common-wildlife.md) | Mundane predators/wildlife by terrain |
| [`HUMAN_HAZARDS.md`](bestiary/human-hazards.md) | Bandits, wreckers, poachers, and other generic human threats |
| [`ENVIRONMENTAL_HAZARDS.md`](bestiary/environmental-hazards.md) | Terrain and weather hazards with DCs |
| [`FOLK_UNDEAD.md`](bestiary/folk-undead.md) | The lingering-dead encounter, framed strictly as unexplained folk belief |

## Timelines — `05_timelines/`

New cosmology: **the Unmade**, alternate-timeline travel, and **the Last Telling** (the darkest confirmed Telling).

| File | Covers |
|---|---|
| [`THE_UNMADE_OVERVIEW.md`](timelines/the-unmade-overview.md) | Core cosmology of alternate Tellings |
| [`THE_RITE_OF_THE_BROKEN_THRESHOLD.md`](timelines/the-rite-of-the-broken-threshold.md) | Full mechanics: costs, DCs, tiers, the Return Rite |
| [`THE_LAST_TELLING.md`](timelines/the-last-telling.md) | The darkest timeline, fully written up as a danger site. Known regionally as **the Pall** (NW frontier), **the Waning** (Vale, Sunmark, Hethewald), **the Ashlands** (Emberfell, Karran), or **the Echo Realm** (Caradril, Glassmere, Heartlands) — "the Last Telling" is the scholarly term only |
| [`TELLING_TIERS_AND_RANDOM_TABLES.md`](timelines/telling-tiers-and-random-tables.md) | Generating Near/Far Tellings for one-shots |
| [`UNMADE_ENCOUNTERS.md`](timelines/unmade-encounters.md) | Creatures and hazards native to the Unmade |
| [`NPCS_OF_THE_UNMADE.md`](timelines/npcs-of-the-unmade.md) | Fray-Walkers, brokers, and the "meeting yourself" trope |

## Ruins And Adventure Sites — `06_sites/`

34 ruins described as physical places: approach, layout, hazards with DCs, inhabitants, salvage, retreat. No plot attached.

| File | Covers |
|---|---|
| [`SITE_INDEX.md`](sites/site-index.md) | **Start here** — master table of all 34, plus pick-by-level and pick-by-problem tables |
| [`SUNDERING_REACH_SITES.md`](sites/sundering-reach-sites.md) | 8 sites, levels 1–10 |
| [`RING1_SITES.md`](sites/ring1-sites.md) | 9 sites, levels 2–9 (Vale, Tollwood, Pale Coast) |
| [`CARADRIL_SITES.md`](sites/caradril-sites.md) | 2 sites, levels 6–10 (the city's undercity) |
| [`FAR_CONTINENT_SITES.md`](sites/far-continent-sites.md) | 15 sites, levels 8–16 (one or two per far region) |

## Maps — `maps/`

| File | Covers |
|---|---|
| [`manifest.json`](maps/manifest.json) | 64-entry map catalog (1 full-continent, 1 campaign-area cluster, 18 regions, 4 cities, 40 settlements), all `player-safe` |
| [`assets/`](maps/assets/) | Rendered map images — 9 of 64 currently generated |

Authoritative here — this is the map manifest the DungeonMaster app onboarding contract reads, addressed by canonical key (see this folder's [`README.md`](README.md#maps)). It is no longer a mirror of `/ai_solo_campaign/maps`; that folder was removed when the manifest moved here.

## Audits

| File | Covers |
|---|---|
| [`AUDIT_2026-08-01.md`](AUDIT_2026-08-01.md) | Full cohesion + secrecy audit of all 44 files against campaign canon. Verdict: cohesive and consistent |

## Related Files

- [`README.md`](README.md) — what this folder is and how it relates to `/ai_solo_campaign`
- [`../../../ai_solo_campaign/00_control/NAMING_REGISTRY.md`](../../../ai_solo_campaign/00_control/NAMING_REGISTRY.md) — proper-noun registry (includes the new Timelines terms)
