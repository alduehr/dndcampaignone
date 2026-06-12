# NAMING_REGISTRY.md

## Purpose

Master registry of all proper nouns used in the campaign. Check this file before creating any major NPC, faction, region, settlement, god, artifact, ancient order, or specialized setting term. Prevents naming collisions and accidental duplication.

## Current Status

**Stages 1–9 populated (Stage 9 NPC Codex Expansion: pass-1 2026-06-12 registered 12 new majors; pass-2 2026-06-12 registered 9 new majors [M33–M48 + M49b/M50b bring the roster to 50; the other 9 pass-2 majors are elevations of already-registered secondaries — see the "Stage 9 Pass-2 Major NPC additions" subsection]; Stage 8 Faction Deepening 2026-06-11 — no new proper nouns; Stage 7 complete incl. completion pass; Full-World Cartographic Expansion pass added full-continent geographic placeholders.** The Full-World pass registered the rest of the continent of Orrun (oceans, seas, ranges, rivers, forests, badlands, wetlands, steppe, islands) and ~11 placeholder political/cultural regions, plus 3 placeholder overseas landmasses of Vael — all map-authoritative placeholders only (named/positioned, NOT deep-built); **no new factions, gods, central mysteries, or artifacts.** See the "Full-World Cartographic Expansion" subsection under Place Names and `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md`. Core campaign proper nouns registered through Stage 4 (Caradril city: districts, city factions, city NPCs, new terms). **Stage 5 (Level 1–4 Play Arc) introduced NO new proper nouns.** **Stage 7 (Regional Expansion Ring 1) added the three adjacent regions' proper nouns** — Ashgarden Vale, Tollwood, and Pale Coast settlements, landmark sites, dungeons, one minor regional faction (the Tollmen), Ring 1 NPCs, and a few setting terms; see the Stage 7 subsections below. **The Stage 7 completion pass added 4 new quests, 12 new wilderness landmark-sites (4/region), 9 new secondary + 13 new minor Ring 1 NPCs, and 6 named regional clocks (V1/V2, T1/T2, C-PC1/C-PC2 — see each region file's "Regional Clocks" and `02_runtime_state/WORLD_CLOCKS.md`).** No new central mystery, major faction, god, cosmology, or legendary artifact in the completion pass. **No new central mystery, major faction, god, cosmology, or legendary artifact was created in Stage 7;** new sites feed existing M1–M9 (mostly M2/M3/M5 fragments, gated/oblique M6) and the deep-wood/maritime "presences" are regional landmark-powers, NOT the Hollow Court or new gods. Quest titles and file names are not registered proper nouns. Add new entries immediately when creating named content.

> **Stage 7 naming disambiguation:** "Pell" is a common frontier surname for several distinct minor figures (Warden Pell [Reach Ashen Warden, secondary]; Pell Oster [Saltmargin salt-warden, minor]; Factor Wymar Pell [Vale Ledger, secondary]; Ale-wife Pell [Tollstone Cross, minor]) — always keep epithet/role. "Sennet" names two distinct elders: **Mother Sennet** (Saint Veddow's shrine-keeper) and **Goodwife Sennet** (Coldhearth forest-elder) — always qualify by location. **Wren-of-the-Wood** (Coldhearth minor guide) is distinct from major NPC **Wren Hollowmere** — always use the full epithet. "Pilgrim Goodman Sael" (Saint Veddow's minor) is distinct from "Domic Sael" (Ledger major) and "Sael Brunt" (Tilbrook secondary) — given name only; keep surnames.

> **Stage 8 (Faction Deepening) — no new proper nouns.** Stage 8 made all seven major factions operational (4-quest chains, rank-and-file "Combat Capability" profiles, `FACTION_RELATIONSHIP_MAP.md`, `FACTION_TURN_RULES.md`). It introduced **no new named NPCs, factions, faction sub-groups, places, gods, artifacts, or setting terms** — only generic rank-and-file adversary *types* (e.g. "Warden Initiate", "Ledger collector / caravan guard", "Circle grave-digger", "town watchman", "Gravecaller cultist", "Remnant scholar / Reclaimer agent", "leaked Remembrance"), which are descriptive role-types, not registered proper nouns. All named faction members referenced already exist in `08_npcs/`. Quest titles and file names are not registered proper nouns.

## Rules

- Check this registry before naming anything major.
- Add an entry immediately after creating a named entity.
- Do not reuse names across different entity types without a documented reason.
- Mark retired names with a reason so they are not accidentally reused.

---

## Reserved Proper Nouns

| Name | Type | File | Notes |
|---|---|---|---|
| Vael | World | `04_world_atlas/WORLD_OVERVIEW.md` | The world. |
| Orrun | Continent | `04_world_atlas/WORLD_OVERVIEW.md` | The known continent. |
| The Long Remembering | Campaign title | `03_canon/CAMPAIGN_IDENTITY_LOCK.md` | Locked. |
| Custodian Concord | Ancient order | `03_canon/WORLD_HISTORY.md` | The fallen order; central to hidden truth. |
| Custodians | Title (inner Concord) | `03_canon/DM_ONLY_CANON.md` | Became the Hollow Court (DM). |
| Quietfall | Historical event | `03_canon/WORLD_HISTORY.md` | The collapse; AQ 0. |
| Remembrance | Setting term | `03_canon/COSMOLOGY.md`, `MAGIC_RULES.md` | The harvestable substance of identity. |
| Quiet Country | Afterlife | `03_canon/COSMOLOGY.md` | The finite afterlife. |
| Last Door | Cosmological/divine | `03_canon/GODS_AND_FAITHS.md` | Death threshold. |
| Three Thresholds | Religion | `03_canon/GODS_AND_FAITHS.md` | Birth/Living/Death principles. |
| After Quietfall (AQ) / Concord Reckoning (CR) | Calendar | `03_canon/CALENDAR.md` | Dating systems. |
| Thin-born | Setting term | `03_canon/DM_ONLY_CANON.md` | People born "empty." |

## Faction Names

| Name | Type | File | Notes |
|---|---|---|---|
| Ashen Wardens | Rite-keeper order | `07_factions/major_factions/ASHEN_WARDENS.md` | Unknowing seal-guardians. |
| Cinder Ledger | Merchant-bank | `07_factions/major_factions/CINDER_LEDGER.md` | Monopoly schemer. |
| Mourners' Circle | Folk faith | `07_factions/major_factions/MOURNERS_CIRCLE.md` | Grief-keepers. |
| Reachward Compact | Government council | `07_factions/major_factions/REACHWARD_COMPACT.md` | Infiltrated. |
| Gravecallers | Outlawed cult | `07_factions/major_factions/GRAVECALLERS.md` | Speak with the dead. |
| Concord Remnant | Scholar society | `07_factions/major_factions/CONCORD_REMNANT.md` | Would-be heirs. |
| Hollow Court | Apex hidden power | `07_factions/major_factions/HOLLOW_COURT.md` | DM-only; surviving Custodians. |
| Mourner's Cant | Ritual register | `03_canon/LANGUAGES.md` | Mourners' speech. |
| Gravecaller Knock | Secret code | `03_canon/LANGUAGES.md` | Cult signaling. |
| The Reclaimers | Faction sub-group | `07_factions/major_factions/CONCORD_REMNANT.md` | Remnant inner circle (DM). |
| The Tidewater Council | City government (Caradril) | `06_settlements/CARADRIL.md` | Ruling council of magisters. |
| The Charter Houses | Power bloc (Caradril merchant families) | `06_settlements/CARADRIL.md` | Old chartered trade dynasties. |
| The Wardmoot | Civic body (Caradril district reps) | `06_settlements/CARADRIL.md` | Commoners' assembly; little power. |
| The Tide-Watch | City watch/guard (Caradril) | `06_settlements/CARADRIL.md` | Caradril law enforcement. |
| The Quay Charter | Sub-faction (Ledger's Caradril guild-arm) | `06_settlements/caradril_districts/THE_COUNTING_QUAYS.md` | Cinder Ledger's trade-guild front. |
| The Salt Syndicate | Criminal network (Caradril) | `06_settlements/CARADRIL.md` | Smuggling + relic black market. |
| The Hush | Criminal network (Caradril) | `06_settlements/CARADRIL.md` | Information/blackmail brokers. |
| The Lampwrights' Collegium | Guild (Caradril scholars' guild; Remnant-linked) | `06_settlements/caradril_districts/THE_LANTERN_REACH.md` | Public face of Remnant scholarship. |
| The Tollmen | Minor regional faction (Tollwood road-bandits) | `06_settlements/TOLLSTONE_CROSS.md` | Stage 7 — East Road toll-bandits at Tollstone Cross; turnable (Renn) vs. murderous (Skell). NOT a major faction. |

## Place Names

| Name | Type | Region | File |
|---|---|---|---|
| Sundering Reach | Region | Sundering Reach | `05_regions/SUNDERING_REACH.md` |
| Hollowmere | Town (start) | Sundering Reach | `06_settlements/HOLLOWMERE.md` |
| Hollowmere basin | Geographic/landmark | Sundering Reach | `06_settlements/HOLLOWMERE.md` |
| Drowned shrine | Dungeon/landmark (DM keystone) | Sundering Reach | `07_factions/major_factions/HOLLOW_COURT.md` |
| Greyfens | Wilderness | Sundering Reach | `05_regions/SUNDERING_REACH.md` |
| Sunder Heights | Highlands | Sundering Reach | `05_regions/SUNDERING_REACH.md` |
| Mirewend River | River | Sundering Reach | `04_world_atlas/MAP_DESCRIPTION.md` |
| Concord roads | Travel route | Sundering Reach | `04_world_atlas/MAP_DESCRIPTION.md` |
| The Drowned Lantern | Inn | Hollowmere | `06_settlements/HOLLOWMERE.md` |
| Mourner's Green | Cemetery | Hollowmere | `06_settlements/HOLLOWMERE.md` |
| Ashgarden Vale | Region (south) | Orrun | `04_world_atlas/WORLD_OVERVIEW.md` |
| Tollwood | Region (east) | Orrun | `04_world_atlas/WORLD_OVERVIEW.md` |
| Pale Coast | Region (west) | Orrun | `04_world_atlas/WORLD_OVERVIEW.md` |
| Caradril | City-state (SE) | Orrun | `04_world_atlas/WORLD_OVERVIEW.md` |
| Kettle Bridge | Town | Sundering Reach | `06_settlements/KETTLE_BRIDGE.md` |
| Saltmargin | Town | Sundering Reach | `06_settlements/SALTMARGIN.md` |
| Candlewick | Village | Sundering Reach | `06_settlements/CANDLEWICK.md` |
| Greywater Holm | Village | Sundering Reach | `06_settlements/GREYWATER_HOLM.md` |
| Harrowgast | Mining village | Sundering Reach | `06_settlements/HARROWGAST.md` |
| Reedford | Hamlet | Sundering Reach | `06_settlements/REEDFORD.md` |
| The Ashwalk Rest | Warden waystation | Sundering Reach | `06_settlements/THE_ASHWALK_REST.md` |
| The Sunken Tollhouse | Dungeon (river node) | Sundering Reach | `10_dungeons_and_ruins/THE_SUNKEN_TOLLHOUSE.md` |
| The Deep Adit | Dungeon (secondary node) | Sundering Reach | `10_dungeons_and_ruins/THE_DEEP_ADIT.md` |
| The Whispering Cairn | Ruin (archive-cairn) | Sundering Reach | `10_dungeons_and_ruins/THE_WHISPERING_CAIRN.md` |
| The Peat Chapel | Ruin (fen chapel; first delve) | Sundering Reach | `10_dungeons_and_ruins/THE_PEAT_CHAPEL.md` |
| The Barrow of Nine Doors | Dungeon (pre-Concord barrow) | Sundering Reach | `10_dungeons_and_ruins/THE_BARROW_OF_NINE_DOORS.md` |
| The Ledger Vault | Dungeon (heist; Hollowmere) | Sundering Reach | `10_dungeons_and_ruins/THE_LEDGER_VAULT.md` |
| Star-Stones | Landmark (road relay-markers) | Sundering Reach | `05_regions/wilderness/MIREWEND_AND_ROADS_SITES.md` |
| The Sundered Ridge | Landmark (Heights) | Sundering Reach | `05_regions/wilderness/SUNDER_HEIGHTS_SITES.md` |
| The Roofless Hall | Landmark (Heights ruin) | Sundering Reach | `05_regions/wilderness/SUNDER_HEIGHTS_SITES.md` |
| The Drift-Line | Landmark (Greyfens; M5) | Sundering Reach | `05_regions/wilderness/GREYFENS_SITES.md` |
| The Drowned Blind | Landmark (Gravecaller cell) | Sundering Reach | `05_regions/wilderness/GREYFENS_SITES.md` |
| Mother Tongue Pool | Landmark (Gravecaller sacred) | Sundering Reach | `05_regions/wilderness/GREYFENS_SITES.md` |
| The Bone Weir | Landmark (Greyfens snag) | Sundering Reach | `05_regions/wilderness/GREYFENS_SITES.md` |
| The Lantern Maze | Landmark (Greyfens wisps) | Sundering Reach | `05_regions/wilderness/GREYFENS_SITES.md` |
| The Reed Holms | Landmark (basin islands) | Sundering Reach | `05_regions/wilderness/BASIN_SHORE_AND_HOLMS_SITES.md` |
| The Lantern Shallows | Landmark (basin leakage) | Sundering Reach | `05_regions/wilderness/BASIN_SHORE_AND_HOLMS_SITES.md` |
| The Drowned Mile | Landmark (flooded causeway) | Sundering Reach | `05_regions/wilderness/MIREWEND_AND_ROADS_SITES.md` |
| The Knotted Hand | Inn (Saltmargin) | Sundering Reach | `06_settlements/SALTMARGIN.md` |
| The Drowned Kettle | Inn (Kettle Bridge) | Sundering Reach | `06_settlements/KETTLE_BRIDGE.md` |
| The Cold Drum | Tavern (Harrowgast) | Sundering Reach | `06_settlements/HARROWGAST.md` |

### World Map Authority Pass (geographic features)

| Name | Type | Region | File |
|---|---|---|---|
| The Pale Sea | Ocean (W/NW; against the Pale Coast) | Orrun | `04_world_atlas/WORLD_MAP_AUTHORITY.md` |
| The Highmark Spine | Mountain range (far-N barrier; parent of the Sunder Heights); also a low-confidence placeholder late-frontier region | Orrun | `04_world_atlas/WORLD_MAP_AUTHORITY.md` |
| The Verdance Reaches | Region (Ring 2 placeholder; up the Verdance, SE toward inland Orrun; Lvl 8–12) | Orrun | `04_world_atlas/WORLD_MAP_AUTHORITY.md` |
| The Concord Deep | **DM-ONLY** — buried node-network ("map beneath the map") radiating from the Hollowmere keystone; NOT a surface region, entity, god, or faction | Orrun (subsurface) | `04_world_atlas/WORLD_MAP_LAYERS.md`, `WORLD_MAP_AUTHORITY.md` |

> **Map Authority Pass note:** "The Under-Shrine / the Drowned Keystone" (DM-only endgame place beneath the Hollowmere basin) is a *descriptive label* for the already-registered "Drowned shrine" / Hollow Court seat, not a new proper noun. "The Verdance Reaches" reuses the registered river-name "Verdance." No new factions, gods, cosmology, or central mysteries were coined this pass; the new names are geographic features supporting the existing world.

### Caradril (Stage 4 — First Major City; SE Orrun)

| Name | Type | Region | File |
|---|---|---|---|
| Caradril | City-state (first major city) | Orrun | `06_settlements/CARADRIL.md` |
| The Verdance | River (Caradril's waterway) | Orrun/Caradril | `06_settlements/CARADRIL.md` |
| The Stillwater | Inland harbor-lake (Caradril's port) | Caradril | `06_settlements/CARADRIL.md` |
| The Magisterium | District (government quarter) | Caradril | `06_settlements/caradril_districts/THE_MAGISTERIUM.md` |
| The Counting-Quays | District (Ledger banking/docks) | Caradril | `06_settlements/caradril_districts/THE_COUNTING_QUAYS.md` |
| The Lantern Reach | District (scholars; Remnant seat) | Caradril | `06_settlements/caradril_districts/THE_LANTERN_REACH.md` |
| The Ashmarket | District (relic/salvage trade) | Caradril | `06_settlements/caradril_districts/THE_ASHMARKET.md` |
| Highmourn | District (temple/cemetery hill) | Caradril | `06_settlements/caradril_districts/HIGHMOURN.md` |
| The Crucible | District (foundries/guildhalls) | Caradril | `06_settlements/caradril_districts/THE_CRUCIBLE.md` |
| The Sill | District (poor riverside undercity) | Caradril | `06_settlements/caradril_districts/THE_SILL.md` |
| The Sunken Wards | District (old flooded undercity; ruin) | Caradril | `06_settlements/caradril_districts/THE_SUNKEN_WARDS.md` |
| The Ledger Keep | Landmark (Cinder Ledger HQ building) | Caradril | `06_settlements/caradril_districts/THE_COUNTING_QUAYS.md` |
| The Lamplighters' Hall | Landmark (Remnant public college) | Caradril | `06_settlements/caradril_districts/THE_LANTERN_REACH.md` |
| The Sealed Archive | Landmark (Remnant's true archive vault; M6/M9) | Caradril | `06_settlements/caradril_districts/THE_LANTERN_REACH.md` |
| The Threshold Cathedral | Temple (Three Thresholds) | Caradril (Highmourn) | `06_settlements/caradril_districts/HIGHMOURN.md` |
| The Quiet Houses | Cemetery-temple complex | Caradril (Highmourn) | `06_settlements/caradril_districts/HIGHMOURN.md` |
| Magisters' Hall | Landmark (Tidewater Council seat) | Caradril (Magisterium) | `06_settlements/caradril_districts/THE_MAGISTERIUM.md` |
| The Pale Star | Inn (Magisterium edge; player base) | Caradril | `06_settlements/CARADRIL.md` |
| The Last Tally | Tavern (Counting-Quays) | Caradril | `06_settlements/caradril_districts/THE_COUNTING_QUAYS.md` |
| The Brass Ferry | Tavern (the Sill) | Caradril | `06_settlements/caradril_districts/THE_SILL.md` |
| The Sealgate | Landmark (sealed stair into the Sunken Wards) | Caradril | `06_settlements/caradril_districts/THE_SUNKEN_WARDS.md` |

### Ashgarden Vale (Stage 7 — Ring 1, South)

| Name | Type | Region | File |
|---|---|---|---|
| Orchardmere | Town (Vale hub) | Ashgarden Vale | `06_settlements/ORCHARDMERE.md` |
| Saint Veddow's Rest | Town (pilgrimage shrine-town) | Ashgarden Vale | `06_settlements/SAINT_VEDDOWS_REST.md` |
| Saint Veddow | Saint/legend (over a capped Concord shrine) | Ashgarden Vale | `06_settlements/SAINT_VEDDOWS_REST.md` |
| Tilbrook | Village (mill village) | Ashgarden Vale | `06_settlements/TILBROOK.md` |
| The Ammet | River (the Vale's river) | Ashgarden Vale | `05_regions/ASHGARDEN_VALE.md` |
| Orchardmere lake | Geographic (the Vale hub's lake) | Ashgarden Vale | `06_settlements/ORCHARDMERE.md` |
| The South Road | Travel route (Concord causeway) | Ashgarden Vale | `04_world_atlas/TRAVEL_ROUTES_RING1.md` |
| Nettlecombe | Hamlet (orchard/field-shrine) | Ashgarden Vale | `05_regions/wilderness/ASHGARDEN_VALE_SITES.md` |
| Marrow Cross | Hamlet (gibbet crossroads) | Ashgarden Vale | `05_regions/wilderness/ASHGARDEN_VALE_SITES.md` |
| The Pellow Grange | Site/dungeon (Ledger relic-quarry) | Ashgarden Vale | `10_dungeons_and_ruins/THE_PELLOW_GRANGE.md` |
| The Buried Cloister | Dungeon (Concord ruin) | Ashgarden Vale | `10_dungeons_and_ruins/THE_BURIED_CLOISTER.md` |
| Saint Veddow's Tomb (the Inner Shrine) | Dungeon (capped Concord shrine; M2/M6) | Ashgarden Vale | `10_dungeons_and_ruins/SAINT_VEDDOWS_TOMB.md` |
| The Old Circle | Landmark (Orchardmere grave-garden) | Ashgarden Vale | `06_settlements/ORCHARDMERE.md` |
| The Cider Star | Inn (Orchardmere) | Ashgarden Vale | `06_settlements/ORCHARDMERE.md` |
| The Plough & Star | Ale-house (Tilbrook) | Ashgarden Vale | `06_settlements/TILBROOK.md` |
| The Harvest-Moot | Civic body (Vale council) | Ashgarden Vale | `06_settlements/ORCHARDMERE.md` |
| The Cider-Wake Orchard | Landmark (Orchardmere wake-orchard; Stage 7 pass) | Ashgarden Vale | `05_regions/wilderness/ASHGARDEN_VALE_SITES.md` |
| The Drowned Lane | Landmark (Ammet flood-road ford; Stage 7 pass) | Ashgarden Vale | `05_regions/wilderness/ASHGARDEN_VALE_SITES.md` |
| The Beacon Tump | Landmark (downs hill-fort; pre-Concord, false-lead; Stage 7 pass) | Ashgarden Vale | `05_regions/wilderness/ASHGARDEN_VALE_SITES.md` |
| Saint Veddow's Spring | Landmark (holy well over the Tomb works; M2/M3; Stage 7 pass) | Ashgarden Vale | `05_regions/wilderness/ASHGARDEN_VALE_SITES.md` |

### Tollwood (Stage 7 — Ring 1, East)

| Name | Type | Region | File |
|---|---|---|---|
| Hartfell | Town (Tollwood hub) | Tollwood | `06_settlements/HARTFELL.md` |
| Coldhearth | Village (charcoal-burners; deep wood) | Tollwood | `06_settlements/COLDHEARTH.md` |
| Tollstone Cross | Hamlet (bandit toll-station) | Tollwood | `06_settlements/TOLLSTONE_CROSS.md` |
| The East Road | Travel route (Concord toll-causeway) | Tollwood | `04_world_atlas/TRAVEL_ROUTES_RING1.md` |
| The Old Mast | Landmark/dungeon (deep wood; pre-Concord presence; gated) | Tollwood | `10_dungeons_and_ruins/THE_OLD_MAST.md` |
| The Hanging Oaks | Landmark/dungeon (pre-Concord grove; Gravecaller cell) | Tollwood | `10_dungeons_and_ruins/THE_HANGING_OAKS.md` |
| The Greenward Toll-Station (the Drowned Vault) | Dungeon (Concord road-node) | Tollwood | `10_dungeons_and_ruins/THE_GREENWARD_TOLL_STATION.md` |
| The Green Mile | Landmark (drowned road stretch) | Tollwood | `05_regions/wilderness/TOLLWOOD_SITES.md` |
| The Coppice Shrines | Landmark (pre-Concord offering-stones) | Tollwood | `05_regions/wilderness/TOLLWOOD_SITES.md` |
| The Antlers | Inn (Hartfell) | Tollwood | `06_settlements/HARTFELL.md` |
| The Mark-Stone | Landmark (Coldhearth's toll-shrine) | Tollwood | `06_settlements/COLDHEARTH.md` |
| The Charcoal Burns | Landmark (deep-wood camp belt; Stage 7 pass) | Tollwood | `05_regions/wilderness/TOLLWOOD_SITES.md` |
| The Withy Bog | Landmark (bog off the Green Mile; M2/M5 fragment; Stage 7 pass) | Tollwood | `05_regions/wilderness/TOLLWOOD_SITES.md` |
| The Mast-Beasts' Range | Landmark (deep-wood predator country; Stage 7 pass) | Tollwood | `05_regions/wilderness/TOLLWOOD_SITES.md` |
| The Sentinel Oaks | Landmark (offering-road toward the Old Mast; gated; Stage 7 pass) | Tollwood | `05_regions/wilderness/TOLLWOOD_SITES.md` |

### Pale Coast (Stage 7 — Ring 1, West)

| Name | Type | Region | File |
|---|---|---|---|
| Wrackmouth | Town (Coast hub/port) | Pale Coast | `06_settlements/WRACKMOUTH.md` |
| Cobble Strand | Village (shingle-cove fishing village) | Pale Coast | `06_settlements/COBBLE_STRAND.md` |
| The Drowned Lamp | Landmark/dungeon (coastal Concord node; M2/M5/M6) | Pale Coast | `10_dungeons_and_ruins/THE_DROWNED_LAMP.md` |
| The Skerries | Landmark (offshore sea-stacks; gated) | Pale Coast | `05_regions/wilderness/PALE_COAST_SITES.md` |
| The Skerry Shrine | Dungeon (largest coastal node; gated) | Pale Coast | `10_dungeons_and_ruins/THE_SKERRY_SHRINE.md` |
| The Wreckers' Caves | Dungeon (sea-caves; wreckers/cult) | Pale Coast | `10_dungeons_and_ruins/THE_WRECKERS_CAVES.md` |
| The Pale Road | Travel route (coast road) | Pale Coast | `04_world_atlas/TRAVEL_ROUTES_RING1.md` |
| The Gull & Anchor | Inn (Wrackmouth) | Pale Coast | `06_settlements/WRACKMOUTH.md` |
| The Tide-Bell | Landmark (Wrackmouth Mourners' shrine) | Pale Coast | `06_settlements/WRACKMOUTH.md` |
| The Wrack | District (Wrackmouth's rough lower harbor) | Pale Coast | `06_settlements/WRACKMOUTH.md` |
| The Tide-Shrine | Landmark (Cobble Strand salt-and-tide shrine) | Pale Coast | `06_settlements/COBBLE_STRAND.md` |
| The Verdance Mouth | Geographic (river-mouth; water-route to Caradril) | Pale Coast | `05_regions/wilderness/PALE_COAST_SITES.md` |
| The Drowned-Cairns | Landmark (tide-line burial shore; M5; Stage 7 pass) | Pale Coast | `05_regions/wilderness/PALE_COAST_SITES.md` |
| The Salt-Pan Flats | Landmark (salt-pans + workers' camp; Stage 7 pass) | Pale Coast | `05_regions/wilderness/PALE_COAST_SITES.md` |
| The Lantern Stacks | Landmark (false-light wrecking reef; Stage 7 pass) | Pale Coast | `05_regions/wilderness/PALE_COAST_SITES.md` |
| The Weeping Light | Landmark (minor headland sea-shrine node; M2/M5; Stage 7 pass) | Pale Coast | `05_regions/wilderness/PALE_COAST_SITES.md` |

### Full-World Cartographic Expansion (full continent of Orrun + Vael landmasses) — placeholders

New geographic names coined in the Full-World Cartographic Expansion pass. All are **map-authoritative placeholders** (named, positioned, NOT deep-built). None is a new faction, god, or central mystery; placeholder **regions** carry a political/cultural *form* only. See `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md`.

**Other landmasses of Vael (placeholder, non-campaign):**

| Name | Type | Position | File |
|---|---|---|---|
| Surren | Continent (overseas) | Far S/SW, across the ocean | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Iron Skards | Island chain (overseas) | Far N, past the Highmark Spine's seaward end | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Sundered Isles / The Far Wrack | Island chain | Far W, mid-ocean (Pale Sea) | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |

**Bodies of water (full continent):**

| Name | Type | Position | File |
|---|---|---|---|
| The Sunder Ocean | Ocean | N, beyond the Highmark Spine | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Calm Reach | Warm sea | SE/S | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Saltmere | Inland salt sea | S-central interior | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Hollow Gulf | Major bay | S coast | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Wracking Straits | Strait | Far W | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Glasswater | Major river system | Central, runs SE to the Calm Reach | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Mardenflow | Major river system | S-central, runs S to the delta | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Hethe | Major river system | E, runs to the Calm Reach | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |

**Geographic features (full continent):**

| Name | Type | Position | File |
|---|---|---|---|
| The Karran Teeth | Mountain range | NE | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Sundering Wall / The Greatspine | Continental cordillera | Central, NW–SE axis | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Emberfells | Volcanic highland | SE-central | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Ghostmark Range | Low mountains | S-central, ringing the Saltmere | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Hethewood | Great forest | E-central | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Sunmark Wilds | Warm forest | S | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Ashen Reach Woods | Volcanic woodland | Around the Emberfells | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Cindern Waste | Ash badland | SE interior | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Bonepan Flats | Salt badland | Around the Saltmere | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Sallow Marches | Deltaic wetland | S coast (Mardenflow delta) | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Mirewend Sinks | Boglands | NW-to-central transition, S of the cluster | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Wender Steppe | Cold steppe | N-central | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Marrowdowns | Chalk downs | S-central uplands | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Wracking Isles | Island chain | Far W (the Straits) | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Glass Coast | Volcanic-glass coast | SE | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Drowned Steps | Submerged ruin-causeway | Off the S coast | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |

**Placeholder political/cultural regions (full continent; form only, NOT deep-built):**

| Name | Political form | Position | File |
|---|---|---|---|
| The Glassmere League | Mercantile city-league/confederacy | Central, on the Glasswater | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Marrowdowns (region) | Manorial holds / shire-moots | S-central uplands | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Sallowmarch Protectorate | Protectorate (a distant crown's claim) | S coast delta | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Hollow Gulf Ports | Rival port city-states | S coast | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Wender Steppe (region) | Nomadic tribal confederacy | N-central | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Karran Marches | Ungoverned / petty warlord holds | NE | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Emberfell Theocracy / The Ashfast | Theocracy (volcanic fire-cult) | SE-central | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Saltmere Reaches | Salt-clan holds / fallen realm | S-central | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Concord Heartlands / The Ruin'd Crown | Fallen realm (contested ruin) | Central-SE, astride the Greatspine | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Hethewald Free Holds | Confederacy of forest free-holds | E-central | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |
| The Sunmark | Sacred tribal territory | S | `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` |

> **Disambiguation:** "The Emberfell Theocracy" and "the Ashfast" are the same placeholder region (two names). "The Concord Heartlands / the Ruin'd Crown" is a **surface** fallen-ruin region — distinct from the DM-only **Concord Deep** (buried network) and the **Under-Shrine / Drowned Keystone** (endgame, beneath Hollowmere); the Heartlands are NOT the keystone and NOT the Hollow Court's seat. "The Sunmark" (region) shares a root with its forest "the Sunmark Wilds" — keep full names. "The Wracking Straits," "the Wracking Isles," and "the Far Wrack / Sundered Isles" form a far-W naming family — keep full names. The **Greatspine / Sundering Wall** is distinct from the **Sundering Reach** (campaign region) and from the **Sunder Heights / Sunder Ocean** (the "Sunder-" prefix is a deliberate naming family). The **Marrowdowns** (S-central downs) is distinct from **Marrow Cross** (Vale hamlet).

## NPC Names

| Name | Role | Location | File |
|---|---|---|---|
| Warden Sister Othetha | Senior Warden (secret-keeper) | Reach/Hollowmere | `08_npcs/MAJOR_NPCS.md` |
| Warden Brother Hale | Junior Warden / companion | Hollowmere | `08_npcs/MAJOR_NPCS.md` |
| Warden Pell | Veteran Warden (secondary) | Reach | `07_factions/.../ASHEN_WARDENS.md` |
| Mother Calla Vyre | Cinder Ledger matriarch | Caradril/Hollowmere | `08_npcs/MAJOR_NPCS.md` |
| Factor Domic Sael | Ledger factor | Hollowmere | `08_npcs/MAJOR_NPCS.md` |
| Tallytooth Ren | Ledger enforcer (secondary) | Hollowmere | `07_factions/.../CINDER_LEDGER.md` |
| Grandmother Wend | Mourners' eldest | Hollowmere | `08_npcs/MAJOR_NPCS.md` |
| Iola Wend | Mourners apprentice / bridge | Hollowmere | `08_npcs/MAJOR_NPCS.md` |
| Bann Oester | Grave-digger (secondary) | Hollowmere | `07_factions/.../MOURNERS_CIRCLE.md` |
| Reeve Marda Coalmont | Hollowmere reeve | Hollowmere | `08_npcs/MAJOR_NPCS.md` |
| Councilor Aldous Reke | Councilor / Court agent | Hollowmere | `08_npcs/MAJOR_NPCS.md` |
| Clerk Pevin Oss | Compact records-keeper (secondary) | Hollowmere | `07_factions/.../REACHWARD_COMPACT.md` |
| The Tallow Man | Gravecaller speaker | Greyfens | `08_npcs/MAJOR_NPCS.md` |
| Sister Knell | Gravecaller recruiter | Reach | `08_npcs/MAJOR_NPCS.md` |
| Cole Ashby | Gravecaller radical | Fens/shrine | `08_npcs/MAJOR_NPCS.md` |
| Archivist Quorrin Vane | Remnant inner circle | Caradril | `08_npcs/MAJOR_NPCS.md` |
| Lector Briss | Remnant idealist | Caradril/Reach | `08_npcs/MAJOR_NPCS.md` |
| Custodian Veyl | Hollow Court leader (final antagonist) | Under-shrine | `08_npcs/MAJOR_NPCS.md` |
| Custodian Maire | Hollow Court doubter | Under-shrine | `08_npcs/MAJOR_NPCS.md` |
| Custodian Orre | Hollow Court hardliner (secondary) | Under-shrine | `07_factions/.../HOLLOW_COURT.md` |
| Sefra Quick | Fixer / first contact / cutout | Hollowmere | `08_npcs/MAJOR_NPCS.md` |
| Wren Hollowmere (Brevin) | Returned dead (opening) | Hollowmere | `08_npcs/MAJOR_NPCS.md` |
| Tomas Brevin | Wren's husband | Hollowmere | `08_npcs/MAJOR_NPCS.md` |
| Halla Coalmont | Innkeeper / hub | Hollowmere | `08_npcs/MAJOR_NPCS.md` |
| Old Sashe | Fen-guide | Greyfens edge | `08_npcs/MAJOR_NPCS.md` |

### Stage 9 Major NPC additions

| Name | Role | Location | File |
|---|---|---|---|
| Hewett Drane ("the Reedwarden") | Fen warlord (early Reach antagonist; independent) | Greyfens | `08_npcs/MAJOR_NPCS.md` |
| Mother Ezrith Combe | Mourners' eldest (Vale anchor; elevated from secondary) | Vale/Orchardmere | `08_npcs/MAJOR_NPCS.md` |
| Goodwife Sennet (Coldhearth) | Forest-elder (Tollwood anchor; elevated) | Tollwood/Coldhearth | `08_npcs/MAJOR_NPCS.md` |
| Salt-Mother Bryd | Salt-and-tide rite-keeper (Coast anchor; elevated) | Coast/Cobble Strand | `08_npcs/MAJOR_NPCS.md` |
| Magister Otho Brail | Tidewater Council swing vote | Caradril | `08_npcs/by_region/CARADRIL_MAJOR_NPCS.md` |
| Charter-Lady Imris Vane-Tolm | Charter House reforming heir (cadet of House Tolm; NOT kin to Quorrin Vane) | Caradril | `08_npcs/by_region/CARADRIL_MAJOR_NPCS.md` |
| Sister-Commander Veil Ansele | Tide-Watch second/enforcer | Caradril | `08_npcs/by_region/CARADRIL_MAJOR_NPCS.md` |
| Hierarch Casmir Vole | Three Thresholds schismatic preacher | Caradril/Highmourn | `08_npcs/by_region/CARADRIL_MAJOR_NPCS.md` |
| Grandmaster Edrin Cole | Foundry-guilds overlord (NOT kin to Cole Ashby or Maris Cole) | Caradril/Crucible | `08_npcs/by_region/CARADRIL_MAJOR_NPCS.md` |
| Lector-General Sabine Ferrant | Concord Remnant institutional head/true believer | Caradril/Lantern Reach | `08_npcs/by_region/CARADRIL_MAJOR_NPCS.md` |
| "Mother" Silque | Salt Syndicate true head (above "Tidewife" Sorrel) | Caradril/Sill | `08_npcs/by_region/CARADRIL_MAJOR_NPCS.md` |
| Magister Ophir Lensk | Anti-Reach council bloc head | Caradril | `08_npcs/by_region/CARADRIL_MAJOR_NPCS.md` |

> **Stage 9 naming note:** "Vole" names two distinct people — **Hierarch Casmir Vole** (Caradril schismatic priest) and **Mother Senna Vole** (Caradril folk-Mourner, secondary); keep epithets. "Edrin Cole" (Caradril guild grandmaster) is distinct from "Cole Ashby" (Gravecaller) and "Maris Cole" (Coast Ledger factor) — common surname. "Imris **Vane**-Tolm" and minor "Doss Vane" are NOT kin to "Quorrin **Vane**." Stage 9 secondary/minor NPCs reuse the established common-surname families (Pell, Wend, Sael, Coalmont, Vane, Dree, Tull, Strand, Brunt, Gethin, Marrin/Marrock) with disambiguating epithets/locations carried inline in their NPC-file entries; they are not individually registered here (per registry scope: major NPCs + key terms). Far-continent placeholder figures in `08_npcs/by_region/FAR_CONTINENT_NPCS.md` are horizon-scaffolds, not deep-built named powers.

### Stage 9 Pass-2 Major NPC additions (M33–M50b) — `08_npcs/by_region/STAGE_9_MAJOR_NPCS.md`

18 new majors bringing the roster to **50**. Nine are **wholly new** (registered below); nine are **elevations** of already-registered Stage 3/4/7 secondaries given full major profiles (Decca Rull, Tomas Greel, Renna Sill, the Bellman, Old Pater Dunk, Cady Renn, Ond Falk, Tamsin Orr, Tomas Quint — no new proper nouns). M49/M50 are cross-references to existing majors (Tomas Brevin / Sister Knell), not new.

| Name | Role | Location | File |
|---|---|---|---|
| Dredgemaster Osrin Vole | Harrowgast mine-lord (M33) | Reach/Harrowgast | `08_npcs/by_region/STAGE_9_MAJOR_NPCS.md` |
| Bridge-Keeper Mahalf Dunmore | Kettle Bridge toll-family head (M34) | Reach/Kettle Bridge | `08_npcs/by_region/STAGE_9_MAJOR_NPCS.md` |
| Fenwife "Mother Osset" | Greyfens Gravecaller cell-mother (M36) | Reach/Greyfens | `08_npcs/by_region/STAGE_9_MAJOR_NPCS.md` |
| Auctioneer Cassia Mourn | Ashmarket relic-auction mistress (M39) | Caradril/Ashmarket | `08_npcs/by_region/STAGE_9_MAJOR_NPCS.md` |
| Warden-Confessor Brother Halloran Voss | Wardens' dissident-of-conscience (M42) | Reach (roams) | `08_npcs/by_region/STAGE_9_MAJOR_NPCS.md` |
| Magister-Reeve Sela Coalmont | Senior honest Compact authority (M43) | Reach (circuit) | `08_npcs/by_region/STAGE_9_MAJOR_NPCS.md` |
| Collector-Captain Mauld Tallow | Ledger Reach enforcer-captain (M44) | Reach (roams) | `08_npcs/by_region/STAGE_9_MAJOR_NPCS.md` |
| Doctor Onaia Veen | Frontier physician-sage (M45) | Reach/Ring 1 (circuit) | `08_npcs/by_region/STAGE_9_MAJOR_NPCS.md` |
| Ser Aldous Penhew | Vale cross-pressured land-magnate (M46) | Vale/Orchardmere | `08_npcs/by_region/STAGE_9_MAJOR_NPCS.md` |

> **Stage 9 pass-2 naming disambiguation:** **Osrin Vole** (Harrowgast mine-lord) ≠ Hierarch Casmir **Vole** (Caradril) ≠ Mother Senna **Vole** (Caradril Mourner) ≠ Ash-Hierophant **Vole** Cindra (far-continent) — unrelated; "Vole" is a common frontier surname, keep full names. **Mahalf Dunmore** is the elder brother of minor NPC "Keeper Dunmore" (Drowned Kettle inn) and shares the given name "Mahalf" with minor NPC "Widow Mahalf" (Cobble Strand) — keep role/location. **Warden-Confessor Halloran Voss** (Warden) ≠ Magister **Halloran Voss** / Magistra Ondine Voss (Caradril council) — unrelated common name; always say "Warden-Confessor Voss." **Magister-Reeve Sela Coalmont** is kin to Reeve Marda / Halla Coalmont and **is the same person** as the Wave-6 secondary "Bailiff Sela Coalmont" (now given her full major profile); keep the "Magister-Reeve" title to distinguish from Reeve Marda. **Collector-Captain Mauld Tallow** (Ledger) ≠ the Tallow Man (Gravecaller epithet) ≠ Caravan-Master Ode Tallow (Ashmarket) — unrelated; keep full names. **Doctor Onaia Veen** heads the Veen healer-family (Onna/Maud Veen, the apothecary) — "Onaia" ≠ "Onna." **Ser Aldous Penhew** (Vale gentry) ≠ the Caradril "Penhallow" Charter House — different family/region; "Aldous" is shared with Reke, Cray (Aldwin), Frome, Penmark — keep surnames. **Auctioneer Cassia Mourn** shares a root with the Mourners' Circle but is **no kin** and not a Mourner (coincidental city trade-name). **Fenwife "Mother Osset"** is a cult-name with no prior collision.

### Stage 9.5 Far-Continent NPCs — `08_npcs/by_region/*_NPCS.md`

44 new far-continent **major** NPCs across the 12 placeholder regions (Lvl 6–17). Most are **elevations** of the horizon-scaffold figures previously named in `08_npcs/by_region/FAR_CONTINENT_NPCS.md` (now given full profiles in per-region files); the rest are wholly new. All are far-region anchors, NOT deep-built powers; **none knows the apex truth.** No new factions, gods, geography, or central mysteries were coined. (The far-continent **secondary/minor** NPCs carry their disambiguating epithets inline in each region file and are not individually registered here, per registry scope.)

| Name | Role | Region/Location | File |
|---|---|---|---|
| Factor-General Wessel Crane | Ledger inland directorate head (elevated) | Verdance Reaches/Marrowfen Stair | `VERDANCE_REACHES_NPCS.md` |
| Lord Ennis Marrow | Petty lord of the Nine Locks (new) | Verdance Reaches/Lord's Wend | `VERDANCE_REACHES_NPCS.md` |
| River-Captain Mossa Drenn | Independent barge-captain (elevated) | Verdance/the Verdance | `VERDANCE_REACHES_NPCS.md` |
| Sub-Lector Hadwin Vael | Remnant inland chapter (elevated) | Verdance Reaches | `VERDANCE_REACHES_NPCS.md` |
| Crown-Reclaimer Magister Hollin Vane | Remnant expedition-lord (elevated; apex-adjacent) | Concord Heartlands/the Crown | `CONCORD_HEARTLANDS_NPCS.md` |
| Warden Lyssa Crownmouth | Scavenger-town war-captain (new) | Concord Heartlands/Crownmouth | `CONCORD_HEARTLANDS_NPCS.md` |
| Father Casian Ord | Heretic-priest of the Pilgrim Camps (new) | Concord Heartlands/Pilgrim Camps | `CONCORD_HEARTLANDS_NPCS.md` |
| "Old Crown" Mab | Deep-ruin guide (elevated) | Concord Heartlands/the Crown | `CONCORD_HEARTLANDS_NPCS.md` |
| League-Factor Oren Glass | League trade-envoy (elevated) | Glassmere League/Glassmere | `GLASSMERE_LEAGUE_NPCS.md` |
| Banker-Magistra Sefwy Holt | Merchant-bank magnate; Ledger rival (elevated) | Glassmere/Three Bridges | `GLASSMERE_LEAGUE_NPCS.md` |
| Spy-Broker "the Glass Ear" | Information-master (elevated) | Glassmere League | `GLASSMERE_LEAGUE_NPCS.md` |
| Reliquary-Lector Mareth Senn | Remnant grand-chapter head (new) | Glassmere/the Reliquary | `GLASSMERE_LEAGUE_NPCS.md` |
| Mother Wenna Lowwater | Urban Mourner eldest; old-songs node (new) | Glassmere/Lowwater | `GLASSMERE_LEAGUE_NPCS.md` |
| Hold-Speaker Bram Hethe | Free-holds Speaker (elevated) | Hethewald/Hethemoot | `HETHEWALD_FREE_HOLDS_NPCS.md` |
| Forest-Mother Onn Greenward | Grove grief-keeper; old-songs node (elevated) | Hethewald/Greenward | `HETHEWALD_FREE_HOLDS_NPCS.md` |
| Toll-Lord "Greenfinger" Maddoc | Outlaw river-toller (new) | Hethewald/Tollreach | `HETHEWALD_FREE_HOLDS_NPCS.md` |
| Port-Mistress Ive Calder | Gulf port-ruler (elevated) | Hollow Gulf/Calderport | `HOLLOW_GULF_PORTS_NPCS.md` |
| Privateer-Captain Roke Mallin | Licensed sea-raider (elevated) | Hollow Gulf/the Reach Lanes | `HOLLOW_GULF_PORTS_NPCS.md` |
| Saltgate Port-Lord Doss Saltgate | Rival port-lord (new) | Hollow Gulf/Saltgate | `HOLLOW_GULF_PORTS_NPCS.md` |
| Tide-Mother Sera Mardenmouth | Sea-Mourner eldest; old-songs node (new) | Hollow Gulf/Mardenmouth | `HOLLOW_GULF_PORTS_NPCS.md` |
| Foreign-Factor Hadiz of Surren | Overseas merchant; world-horizon (new) | Hollow Gulf/Foreign Quarter | `HOLLOW_GULF_PORTS_NPCS.md` |
| Salt-Clan Matriarch Bryd Saltmere | Salt-clan confederacy head (elevated) | Saltmere/Brackhold | `SALTMERE_REACHES_NPCS.md` |
| Drowned-Town Delver Oss | Drowned-ruin scavenger (elevated) | Saltmere/the Drowned Towns | `SALTMERE_REACHES_NPCS.md` |
| Salt-Mother Tess Brackhold | Salt-clan grief-keeper; old-songs node (new) | Saltmere/Brackhold | `SALTMERE_REACHES_NPCS.md` |
| Ash-Hierophant Vole Cindra | Fire-theocracy ruler (elevated; thematic mirror) | Emberfell/Ashfast | `EMBERFELL_THEOCRACY_NPCS.md` |
| Pyre-Warden Sef Embren | Theocracy enforcer (elevated) | Emberfell/Ashfast | `EMBERFELL_THEOCRACY_NPCS.md` |
| Ember-Sage Mira Cindra | Heretic-scholar (new) | Emberfell/Ashfast | `EMBERFELL_THEOCRACY_NPCS.md` |
| Cinder-Master Doss Ashfast | Volcanic mining-lord (new) | Emberfell/Cinderhold | `EMBERFELL_THEOCRACY_NPCS.md` |
| Protector-Legate Vorr Sallow | Distant crown's legate (elevated) | Sallowmarch/Fenward | `SALLOWMARCH_PROTECTORATE_NPCS.md` |
| Marsh-Healer Doll Fenn | Plague-doctor; delta's true leader (elevated) | Sallowmarch/Reedmouth | `SALLOWMARCH_PROTECTORATE_NPCS.md` |
| Reed-Boss "Heron" Maddox | Delta smuggler-king (new) | Sallowmarch/Reedmouth | `SALLOWMARCH_PROTECTORATE_NPCS.md` |
| Fen-Witch Mother Sela Reed | Delta grief-keeper; old-songs node (new) | Sallowmarch/Rice Sallows | `SALLOWMARCH_PROTECTORATE_NPCS.md` |
| Shire-Reeve Aldous Penmark | Downs landed law (elevated) | Marrowdowns/Penmark Hold | `MARROWDOWNS_NPCS.md` |
| Moot-Mother Senna Crale | Downs grief-keeper; old-songs node (elevated) | Marrowdowns/Marrowmoot | `MARROWDOWNS_NPCS.md` |
| Barrow-Master Doss Wether | Barrow-robber-guide (new) | Marrowdowns/Barrow-Fields | `MARROWDOWNS_NPCS.md` |
| Clan-Speaker Tamur Wend-Khar | Steppe confederacy Speaker (elevated) | Wender Steppe/Cold Springs | `WENDER_STEPPE_NPCS.md` |
| Wind-Singer Esha | Steppe seer; cosmic-echo (elevated) | Wender Steppe/Sky-Stones | `WENDER_STEPPE_NPCS.md` |
| Raid-Lord Borr of the Black Horse | Steppe reaver (new) | Wender Steppe/far steppe | `WENDER_STEPPE_NPCS.md` |
| Warlord "Iron" Brask | Strongest petty warlord (elevated) | Karran Marches/Brask's Hold | `KARRAN_MARCHES_NPCS.md` |
| Ore-Factor Mully Karr | Metals-trader (elevated) | Karran Marches/Karran-Gate | `KARRAN_MARCHES_NPCS.md` |
| Reclaimer-Captain Wenna Stone | Remnant NE expedition (new; turnable) | Karran/Old Iron forts | `KARRAN_MARCHES_NPCS.md` |
| Grove-Keeper Sael Sunmark | Living-faith head (elevated; hopeful contrast) | Sunmark/Sunhollow | `SUNMARK_NPCS.md` |
| Sun-Singer Doll | Grove seer; hopeful echo (elevated) | Sunmark/Sunward Wilds | `SUNMARK_NPCS.md` |
| Plains-Factor Doss Sunward | Cut-and-trade lord (new) | Sunmark/Green Roads | `SUNMARK_NPCS.md` |

> **Stage 9.5 naming disambiguation:** **Hadwin Vael** (Verdance Remnant), **Hollin Vane** (Heartlands Remnant), **Mira/Brann Senn** & city **Sennfort/Cairnwater** & **Mareth Senn** (Glassmere), and **Wenn Vael** (Hethewald) are all **non-kin** to Quorrin Vane, Imris Vane-Tolm, Oneth Vael, Doss Vane, or each other — "Vane / Vael / Senn" are common scholarly/civic surnames; keep full names. **Ash-Hierophant Vole Cindra** (Emberfell, foreign root) ≠ Osrin/Casmir/Senna **Vole** (north) — coincidental; keep full names. **Salt-Clan Matriarch Bryd Saltmere** (Saltmere) ≠ **Salt-Mother Bryd** (Pale Coast/Cobble Strand) — shared salt-folk given-name across distant regions; always full names. **Salt-Mother Tess Brackhold** (Saltmere rite-title) shares the "Salt-Mother" title with Coast's Bryd — distinct people; keep full names. **Senna Crale** (Marrowdowns Mourner) ≠ Mother/Goodwife Sennet (Vale/Tollwood) ≠ the Senns of Glassmere/Emberfell — keep full names. **"Greenfinger" Maddoc** (Hethewald) keeps its spelling, distinct from the **"Maddox"** outlaw-name family (Eel/Carp/Crow/"Heron"/the Crown's bandit-lord — all separate, unrelated common outlaw surname). **"Iron" Brask** (Karran) ≠ Pass-Warden Brask Tarn (Heartlands) ≠ steppe Borr — common hard-frontier names; keep full names. **Tamur Wend-Khar** (steppe clan-name) ≠ the Reach Wends — coincidental root. **Sael Sunmark** (grove given-name) ≠ the northern Saels (Domic, Brunt, Goodman). The many far-region **"Doss"** (Saltgate, Ashfast, Wether, Sunward) and **"Doll"** (Fenn, Sun-Singer, Vard, Cairn, Tull) and **"Wenna"** (Lowwater, Stone, Roke, Drove, Stair) are common given-names across distant regions — always carry the surname/epithet. **Wind-Singer Esha** & **Sun-Singer Doll** are seer-titles, not the minor-NPC "Esha"/"Doll" color-figures.

### Stage 9.5 — Light NPC-Facing Anchors — `08_npcs/by_region/*_NPCS.md`

Local place-names coined to *anchor* the Stage 9.5 far-continent NPC rosters (towns, camps, districts, wharves, gathering-places, ruin-edge camps, roads, groves). **Each is a light NPC-facing anchor — not a full settlement, not a major map feature, and NOT deep-built.** They exist so the AI DM can locate far-region NPCs in play; they reuse or sit within already-registered geographic features (see `FULL_WORLD_MAP_AUTHORITY.md`) and do not add new major geography or factions. Names that ARE already registered as map features (e.g. the Bonepan Flats, the Cindern/Forbidden Waste, the Sunmark Wilds, the Ruin'd Crown, the Greatspine passes, the Reach Lanes, the Summer-Riding host) are not repeated here.

| Name | Type | Region | File | Notes |
|---|---|---|---|---|
| Marrowfen Stair | River-town (locks/wharves; corridor hub) | Verdance Reaches | `VERDANCE_REACHES_NPCS.md` | light NPC-facing anchor — not a full settlement, not a major map feature |
| Lord's Wend | Petty-lord's hall-town | Verdance Reaches | `VERDANCE_REACHES_NPCS.md` | light NPC-facing anchor — not a full settlement, not a major map feature |
| Cresswater | Barge-village | Verdance Reaches | `VERDANCE_REACHES_NPCS.md` | light NPC-facing anchor — not a full settlement, not a major map feature |
| The Nine Locks | Lock-staircase landmark (on the Verdance) | Verdance Reaches | `VERDANCE_REACHES_NPCS.md` | light NPC-facing anchor — not a full settlement, not a major map feature |
| Crownmouth | Fortified scavenger-town (ruin-edge) | Concord Heartlands | `CONCORD_HEARTLANDS_NPCS.md` | light NPC-facing anchor — not a full settlement, not a major map feature |
| The Pilgrim Camps | Refugee/relic-seeker shanty-camps | Concord Heartlands | `CONCORD_HEARTLANDS_NPCS.md` | light NPC-facing anchor — not a full settlement, not a major map feature |
| Glassmere (city) | League-capital city (greatest river-city) | Glassmere League | `GLASSMERE_LEAGUE_NPCS.md` | light NPC-facing anchor — names the placeholder region's capital; not deep-built |
| The Floor | Merchant-exchange (Glassmere) | Glassmere League | `GLASSMERE_LEAGUE_NPCS.md` | light NPC-facing anchor — a city locale, not a settlement |
| The Three Bridges | Banking quarter (Glassmere) | Glassmere League | `GLASSMERE_LEAGUE_NPCS.md` | light NPC-facing anchor — a city locale, not a settlement |
| The Reliquary | Remnant great chapter-house (Glassmere) | Glassmere League | `GLASSMERE_LEAGUE_NPCS.md` | light NPC-facing anchor — a building, not a settlement |
| Lowwater | Poor riverside district (Glassmere) | Glassmere League | `GLASSMERE_LEAGUE_NPCS.md` | light NPC-facing anchor — a city district, not a settlement |
| Sennfort / Cairnwater | Smaller league-cities (referenced) | Glassmere League | `GLASSMERE_LEAGUE_NPCS.md` | light NPC-facing anchors — named-in-passing, not deep-built |
| Hethemoot | Great gathering free-hold | Hethewald Free Holds | `HETHEWALD_FREE_HOLDS_NPCS.md` | light NPC-facing anchor — not a full settlement, not a major map feature |
| Greenward | Grove-village (Onn's seat) | Hethewald Free Holds | `HETHEWALD_FREE_HOLDS_NPCS.md` | light NPC-facing anchor — not a full settlement, not a major map feature |
| Tollreach | Outlaw river-toll camp (on the Hethe) | Hethewald Free Holds | `HETHEWALD_FREE_HOLDS_NPCS.md` | light NPC-facing anchor — not a full settlement, not a major map feature |
| The Old Holds | Deep-wood Concord ruins (forbidden) | Hethewald Free Holds | `HETHEWALD_FREE_HOLDS_NPCS.md` | light NPC-facing anchor — ruin-cluster label, not deep-built (cf. Tollwood's Old Mast) |
| Calderport | Greatest Gulf port city-state | Hollow Gulf Ports | `HOLLOW_GULF_PORTS_NPCS.md` | light NPC-facing anchor — names the placeholder region's chief port; not deep-built |
| Saltgate | Rival Gulf port city-state | Hollow Gulf Ports | `HOLLOW_GULF_PORTS_NPCS.md` | light NPC-facing anchor — not deep-built |
| The Foreign Quarter | Overseas-traders' district (Calderport) | Hollow Gulf Ports | `HOLLOW_GULF_PORTS_NPCS.md` | light NPC-facing anchor — a city locale |
| The Mardenmouth | Delta-mouth wharves (Calderport) | Hollow Gulf Ports | `HOLLOW_GULF_PORTS_NPCS.md` | light NPC-facing anchor — a wharf-district, not a settlement |
| Brackhold | Largest surviving salt-clan hold | Saltmere Reaches | `SALTMERE_REACHES_NPCS.md` | light NPC-facing anchor — not a full settlement, not a major map feature |
| The Drowned Towns | Receding-lake submerged ruins | Saltmere Reaches | `SALTMERE_REACHES_NPCS.md` | light NPC-facing anchor — pre-Concord ruin-cluster, NOT the keystone |
| Saltcairn | Ghostmark-edge clan-town | Saltmere Reaches | `SALTMERE_REACHES_NPCS.md` | light NPC-facing anchor — not a full settlement, not a major map feature |
| Ashfast (city) | Fortress-temple-city (theocracy seat) | Emberfell Theocracy | `EMBERFELL_THEOCRACY_NPCS.md` | light NPC-facing anchor — names the placeholder region's seat; not deep-built |
| Cinderhold | Volcanic mining town | Emberfell Theocracy | `EMBERFELL_THEOCRACY_NPCS.md` | light NPC-facing anchor — not a full settlement, not a major map feature |
| The Ash Roads | Pilgrim-ways through the highland | Emberfell Theocracy | `EMBERFELL_THEOCRACY_NPCS.md` | light NPC-facing anchor — a route-label, not a settlement |
| Fenward | Garrison-capital (the crown's seat) | Sallowmarch Protectorate | `SALLOWMARCH_PROTECTORATE_NPCS.md` | light NPC-facing anchor — not a full settlement, not a major map feature |
| Reedmouth | Delta smuggling-village | Sallowmarch Protectorate | `SALLOWMARCH_PROTECTORATE_NPCS.md` | light NPC-facing anchor — not a full settlement, not a major map feature |
| The Rice Sallows | Flooded paddy-country | Sallowmarch Protectorate | `SALLOWMARCH_PROTECTORATE_NPCS.md` | light NPC-facing anchor — a sub-area label, not a settlement |
| The Fever Channels | Deep delta backwaters | Sallowmarch Protectorate | `SALLOWMARCH_PROTECTORATE_NPCS.md` | light NPC-facing anchor — a waterway-label, not a settlement |
| Marrowmoot | Shire-town (where moots gather) | Marrowdowns | `MARROWDOWNS_NPCS.md` | light NPC-facing anchor — not a full settlement, not a major map feature |
| Penmark Hold | Shire-reeve's manor | Marrowdowns | `MARROWDOWNS_NPCS.md` | light NPC-facing anchor — a manor, not a settlement |
| The Barrow-Fields | Ancient burial-downs | Marrowdowns | `MARROWDOWNS_NPCS.md` | light NPC-facing anchor — pre-Concord barrow-cluster, NOT the keystone |
| Wether | Wool-trade village | Marrowdowns | `MARROWDOWNS_NPCS.md` | light NPC-facing anchor — not a full settlement, not a major map feature |
| The Winter-Camp at Cold Springs | Largest clans' cold-season gathering | Wender Steppe | `WENDER_STEPPE_NPCS.md` | light NPC-facing anchor — a seasonal camp, not a settlement |
| The Sky-Stones | Ancient steppe shrine-circle (NOT Concord) | Wender Steppe | `WENDER_STEPPE_NPCS.md` | light NPC-facing anchor — independent steppe holy site, not deep-built |
| The Spine-Foot trade-meet | Steppe/settled trade-meeting ground | Wender Steppe | `WENDER_STEPPE_NPCS.md` | light NPC-facing anchor — a meeting-ground, not a settlement |
| Brask's Hold | Iron Brask's fortress-town | Karran Marches | `KARRAN_MARCHES_NPCS.md` | light NPC-facing anchor — not a full settlement, not a major map feature |
| Karran-Gate | Mining-and-mercenary town | Karran Marches | `KARRAN_MARCHES_NPCS.md` | light NPC-facing anchor — not a full settlement, not a major map feature |
| The Deep Cuts | Great ore-mines | Karran Marches | `KARRAN_MARCHES_NPCS.md` | light NPC-facing anchor — a mine-complex label, not a settlement |
| The Old Iron forts | Scattered peripheral Concord ruins | Karran Marches | `KARRAN_MARCHES_NPCS.md` | light NPC-facing anchor — ruin-cluster, NOT the keystone |
| The Great Grove at Sunhollow | Grove-tribes' holy heart/gathering-place | Sunmark | `SUNMARK_NPCS.md` | light NPC-facing anchor — a sacred grove + gathering, not a settlement |
| The Grove-Camps | Grove-tribes' settlements | Sunmark | `SUNMARK_NPCS.md` | light NPC-facing anchor — dispersed camps, not deep-built |
| The Green Roads | Pilgrim-and-trade paths through the groves | Sunmark | `SUNMARK_NPCS.md` | light NPC-facing anchor — a route-label, not a settlement |

> **Stage 9.5 cleanup-pass secondary additions (2026-06-12):** six far-region **secondary** NPCs added to bring five regions from 11→12 and Sallowmarch to 12 distinct-authored secondaries — Marek Bonepan (Saltmere salt-caravan master), Horse-Reeve Edony Marrow (Marrowdowns mounted lawkeeper), Kin-Mother Tamur-Sai (Wender clan-matriarch; explicitly no kin to Clan-Speaker Tamur Wend-Khar), Pass-Toll Warlord Hessa Teeth (Karran pass-warlord), Greenway-Warden Tamsin Greenway (Sunmark road-captain; distinct from Sub-Lector Tamsin Orr), Rice-Moot Speaker Pell Sallows (Sallowmarch village-speaker; no kin to the crown's Sallow-line). Per registry scope, far-region secondaries carry disambiguating epithets inline in their region files and are listed here only as a cleanup note.

### Secondary NPCs (Stage 3) — `08_npcs/SECONDARY_NPCS.md`

| Name | Role | Location |
|---|---|---|
| Sergeant Hesk | Compact watch leader | Hollowmere |
| Bailiff Aldwin Cray | Compact bailiff | Kettle Bridge |
| Quenna Bly | Ledger toll-farmer | Kettle Bridge |
| Bargemaster Tibb | Bargeman | Kettle Bridge |
| Iss Marlow | Ledger wharf-factor | Saltmargin |
| Decca Rull | Salt-pan foreman | Saltmargin |
| "Gull" Heddwyn | Smuggler | Saltmargin/Greyfens |
| Elder Mabb Tay | Mourners' elder | Greywater Holm |
| Den Hask | Fowler / half-recruit | Greywater Holm |
| Hayward Tomas Greel | Compact hayward | Candlewick |
| Yorrin Tay | Chandler-master | Candlewick |
| Overseer Brack | Compact overseer | Harrowgast |
| Nessa Coyle | Ledger buyer | Harrowgast |
| Dig-boss Hennet | Mine foreman | Harrowgast |
| Veska Dunn | Remnant reclaimer-agent | Sunder Heights |
| Hospitaller Warden Sirrin | Warden quartermaster | The Ashwalk Rest |

### Minor NPCs (Stage 3) — `08_npcs/MINOR_NPCS.md`

Pim Ostry, Goodwife Harl, Edda Cole, Wat (cooper's-boy), Sexton Marrow, Drell (peat-merchant) [Hollowmere]; Innkeep Brannoch, Sister-of-salt Onna, Crook (carter), Net-wife Sereth [Saltmargin]; Old Marrock, Keeper Dunmore, Toll-guard Pike, Barge-boy Lill [Kettle Bridge]; Goodwife Nan, Ferryman Dob, Widow-mourner Sel [Reedford]; Widow Sarn, Tam (fowler-boy), Goodman Crell [Greywater Holm]; Old Beeman Crick, Mourner Edda, Smith Harrow, Chapel-clerk Vesna [Candlewick]; "Thin" Coll, Cold-Drum Vey, Toolwright Garn, Mab (sorter) [Harrowgast]; Mourner-keeper Ansel, Watch-Warden Doune, Carter Sed [The Ashwalk Rest].

> Note: "Mourner Edda" (Candlewick, minor) and "Edda Cole" (Hollowmere hedge-healer, minor) are distinct people; "Pell Oster" (Saltmargin salt-warden, minor official, mentioned in `SALTMARGIN.md`) is distinct from "Warden Pell" (Ashen Warden, secondary).

### Caradril Secondary NPCs (Stage 4) — `08_npcs/SECONDARY_NPCS.md`

| Name | Role | Location |
|---|---|---|
| Magister Halloran Voss | First Magister (head of council) | Caradril (Magisterium) |
| Magister Sefa Dann | Reform magister (ally lever) | Caradril (Magisterium) |
| Charter-Lord Esren Tolm | Old-money Charter House head (Ledger rival) | Caradril (Magisterium) |
| Captain Yorell Kade | Tide-Watch captain | Caradril (citywide) |
| Provost Anneth Vell | Ledger Keep provost (Vyre's Caradril deputy) | Caradril (Counting-Quays) |
| Underfactor Coll Riis | Ledger clerk (turnable; M3/M6) | Caradril (Counting-Quays) |
| Sub-Lector Tamsin Orr | Remnant scholar (Briss's student; Script tutor) | Caradril (Lantern Reach) |
| Keeper-Archivist Wessel Dree | Sealed Archive gatekeeper (Reclaimer) | Caradril (Lantern Reach) |
| Mother Ysarra | Threshold Cathedral high priest | Caradril (Highmourn) |
| Grave-Magister Lon Quayle | Quiet Houses death-rite official | Caradril (Highmourn) |
| Foundress Beck Harrow | Crucible guild-mistress (relic-smelting) | Caradril (Crucible) |
| "Tidewife" Sorrel | Salt Syndicate boss | Caradril (the Sill/Quays) |
| The Bellman | The Hush broker (information/blackmail) | Caradril (citywide) |
| Renna Sill | Sill community leader (thin-born advocate) | Caradril (the Sill) |
| Old Pater Dunk | Sunken Wards delver-guide | Caradril (Sunken Wards) |

### Caradril Minor NPCs (Stage 4) — `08_npcs/MINOR_NPCS.md`

Steward Maell, Crier Bosh, Doorward Sile [Magisterium]; Tally-clerk Vinn, Wharf-boss Drenn, Moneychanger Oons, Pelt the runner [Counting-Quays]; Copyist Hale-of-Lampgate (see note), Page Wenna, Binder Oslo, Lamplighter Tib [Lantern Reach]; Relic-monger Sabb, Fence Greel-of-the-Ash (see note), Appraiser Mooren, Hawker Liss [Ashmarket]; Sister Onae, Bell-ringer Tomm, Bone-clerk Vass [Highmourn]; Smelt-master Ordo, Guild-steward Phane, Soot the apprentice [Crucible]; Ferryman Quill, Net-girl Bree, "Old Soak" Marrin, Widow Tace [the Sill]; Delver Coorn, Lantern-girl Esha [Sunken Wards].

> Note: "Copyist Hale-of-Lampgate" (Caradril minor) is distinct from "Warden Brother Hale" (major). "Fence Greel-of-the-Ash" (Caradril Ashmarket minor) is distinct from "Hayward Tomas Greel" (Candlewick secondary). Disambiguating epithets are kept in the minor-NPC table.

### Ring 1 Secondary NPCs (Stage 7) — `08_npcs/SECONDARY_NPCS.md`

| Name | Role | Region/Location |
|---|---|---|
| Moot-Reeve Halsa Tindle | Vale governor (cover-up) | Vale/Orchardmere |
| Mother Ezrith Combe | Eldest Vale Mourners' elder (M6) | Vale/Orchardmere |
| Factor Wymar Pell | Ledger Vale factor (M3) | Vale/Orchardmere |
| Warden Sister Adwen | Resident seal-keeper (M6 conditional) | Vale/Saint Veddow's |
| Mother Sennet | Saint Veddow's shrine-keeper | Vale/Saint Veddow's |
| Sub-Lector Oneth Vael | Remnant scholar-pilgrim | Vale/Saint Veddow's |
| Miller Sael Brunt | Tilbrook village leader | Vale/Tilbrook |
| Old Mam Tace | Tilbrook grave-singer (honest M5) | Vale/Tilbrook |
| Factor Hesk Dorr | Ledger logging-driver | Tollwood/Hartfell |
| Road-Warden Captain Brannoch Vey | Road-warden (turnable) | Tollwood/Hartfell |
| Goodwife Edda Sorrel | Forest-custom keeper | Tollwood/Hartfell |
| Brann the Guide | The wood's guide (solo-safety) | Tollwood/Coldhearth |
| Goodwife Sennet | Coldhearth forest-elder (deep secret; gated) | Tollwood/Coldhearth |
| Toll-Boss Cady Renn | Tollmen leader (turnable) | Tollwood/Tollstone Cross |
| Skell | Tollmen lieutenant (murderous) | Tollwood/Tollstone Cross |
| Factor Maris Cole | Ledger coastal factor (salt; M3) | Coast/Wrackmouth |
| Harbor-Reeve Ond Falk | Harbor governor | Coast/Wrackmouth |
| Skipper Wenna Roke | Honest skipper (water-route; solo-safety) | Coast/Wrackmouth |
| Salt-Mother Bryd | Salt-and-tide rite-keeper (M5/M6 gated) | Coast/Cobble Strand |
| Headman Corl Strand | Eldest fisher | Coast/Cobble Strand |

### Ring 1 Secondary NPCs (Stage 7 completion pass) — `08_npcs/SECONDARY_NPCS.md`

| Name | Role | Region/Location |
|---|---|---|
| Wreck-Master Tomas Quint | Wreckers' leader (grey; M3 chain) | Coast/wild coast |
| Tide-Reader Mabon Crale | Tide/weather guide (solo-safety; M5 witness) | Coast/Wrackmouth–Cobble Strand |
| Anchorite Sef | Wandering Warden ("Warden Brother Sef"; M5/M6 gated) | Coast/coast-wide |
| Provost Anselm Verge | Resident Warden seal-keeper at the Lamp (M6 conditional) | Coast/Drowned Lamp headland |
| Sub-Lector Maren Voll | Remnant scholar mapping coastal nodes (M2) | Coast/Wrackmouth |
| Cutter-Captain Holm Dunnal | Ledger camp-guard captain (turnable witness) | Tollwood/Hartfell–camps |
| Warden Brother Ošric | Wandering Tollwood Warden (M5/M6 gated) | Tollwood/wood-wide |
| Moot-Warden Sergeant Idony Frost | Vale road-warden captain (cover-up lever) | Vale/Orchardmere |
| Lay-Sister Petronel | Sennet's deputy; failed-rest cell (conscience-lever) | Vale/Saint Veddow's |

### Ring 1 Minor NPCs (Stage 7) — `08_npcs/MINOR_NPCS.md`

Goodwife Orrel, Innkeep Dab Hollith, Bell-clerk Wessa [Orchardmere]; Relic-monger Coyle Tamm, Hosteler Wenna Frey, Pilgrim Goodman Sael, Well-keeper Brother Ode [Saint Veddow's]; Ale-wife Genna Brunt, Widow Hessit, Goodman Orrick, Gibbet-keeper Sorle, Foreman Drust [Tilbrook/Vale country]; Innkeep Marrec Tull, Smith-master Holt, Cutter-foreman Vask, Widow Sefa Quist, Herbwife Onn [Hartfell]; Smith Doune, Ale-wife Pell, Toll-clerk Wenny [Tollstone Cross]; Old Gethin, Wren-of-the-Wood, Burn-boy Tam [Coldhearth]; Innkeep Sella Vane, Fence "Cuttle" Dree, Harbormaster Oll, Tally-clerk Verrin, Mate Doss [Wrackmouth]; Net-wife Senna, Young Ferec, Boatman Crae, Bell-keeper Odd, Widow Mahalf, Salt-raker Tibba [Cobble Strand].

> Note: See the Stage 7 disambiguation block at the top — "Pell," "Sennet," "Wren-of-the-Wood," and "Goodman Sael" all require epithet/location qualifiers to avoid collision with existing names. Stage 7 completion-pass additions: "Anchorite Sef" / "Warden Brother Sef" is the Coast wandering Warden already named in `PALE_COAST.md`; "Warden Brother Ošric" already named in `TOLLWOOD.md`. "Widow Sefa Quist" (Hartfell) and "Anchorite Sef" (Coast) are distinct (shared name-root; keep epithet/location). "Bell-keeper Odd" (Cobble Strand) is distinct from any "Odd"-rooted term; keep role.

## God and Divine Entity Names

| Name | Domain | Faith File | Notes |
|---|---|---|---|
| The Opening (First Threshold) | Birth, hope | `03_canon/GODS_AND_FAITHS.md` | Distant, real. |
| The Hearth (Threshold We Stand In) | Living, oaths | `03_canon/GODS_AND_FAITHS.md` | Distant, real. |
| The Last Door (Last Threshold) | Death, memory | `03_canon/GODS_AND_FAITHS.md` | Partly a tapped mechanism (DM). |

## Artifact and Item Names

| Name | Type | File | Notes |
|---|---|---|---|
| Remembrance relics | Item class | `03_canon/MAGIC_RULES.md` | Concord salvage that stores the dead. |
| The Ledger vault relic | Specific relic (clue) | `07_factions/.../CINDER_LEDGER.md` | "Remembers" the harvest. (Named in Stage 14.) |
| Concord breaking-tools | Item class | `07_factions/.../GRAVECALLERS.md` | Used to shatter shrines. |

## Terms With Specific Meaning

| Term | Meaning | File |
|---|---|---|
| Remembrance | The harvestable substance of a dead person's identity | `03_canon/COSMOLOGY.md` |
| Remembrance (a Remembrance) | A lingering dead person; folk term for the restless dead | `03_canon/PLAYER_SAFE_CANON.md` |
| The harvest | The Concord's secret consumption of the dead (DM term) | `03_canon/DM_ONLY_CANON.md` |
| Wrong-come-back | A botched/leaked resurrection revenant | `03_canon/MAGIC_RULES.md` |
| The seal / the pause | The sealing of the shrine that halts the harvest | `07_factions/.../ASHEN_WARDENS.md` |
| Concord Script | The Concord's written language (clue gate) | `03_canon/LANGUAGES.md` |
| Old Custodial | The inner Custodians' tongue (late-arc gate) | `03_canon/LANGUAGES.md` |
| Thin-touch | Reversible condition from exposure to raw Remembrance relics (Stage 3 custom mechanic; disadvantage on Death saves until a true rite / shrine long-rest) | `13_encounters_and_bestiary/SUNDERING_REACH_ENCOUNTERS.md`, `10_dungeons_and_ruins/THE_DEEP_ADIT.md` |
| Old glass | Folk term for raw Remembrance relics dug from the Sunder Heights | `06_settlements/HARROWGAST.md` |
| The Gravecaller Knock (second mark) | The cult's door-mark/signal (already registered as Gravecaller Knock; "second mark" is the folk name) | `06_settlements/GREYWATER_HOLM.md` |
| Charter | A Caradril trade-license; basis of the Charter Houses' power and the Tidewater Council franchise | `06_settlements/CARADRIL.md` |
| The Stilling | Caradril's term for its golden age of calm after the Quietfall; folk pride masking complacency | `06_settlements/CARADRIL.md` |
| Quiet-coin | Black-market slang in Caradril for relics rumored to "hold" the dead (raw Remembrance relics) | `06_settlements/caradril_districts/THE_ASHMARKET.md` |
| Saint's relics / saint's-bones | Vale folk/trade term for relics sold at Saint Veddow's that are really Remembrance relics (M3) | `06_settlements/SAINT_VEDDOWS_REST.md` |
| The forest-rules / the bargain | Tollwood woodfolk customs (offer at the toll-shrines, never cut marked trees) that keep the Old Mast's presence asleep | `06_settlements/COLDHEARTH.md` |
| The grey lords | Coldhearth/old-song term for whoever "took the dead before the roads fell" — an oblique pre-Concord half-memory of the harvest (gated M5/M6); NOT a new entity/god | `06_settlements/COLDHEARTH.md`, `10_dungeons_and_ruins/THE_OLD_MAST.md` |
| The salt-and-tide rite | Pale Coast Mourners' death-rite for settling the sea's drowned dead | `06_settlements/COBBLE_STRAND.md` |
| Sea-relics / sea-relic trade | Coast term for Remembrance relics salvaged from sea-shrines and wrecks (M3; the Ledger's coastal Monopoly arm) | `06_settlements/WRACKMOUTH.md` |
| The drowned-tide | Coast term for the sea returning its dead worse than before (the maritime harvest leaking; M5 oblique) | `06_settlements/COBBLE_STRAND.md` |

## Forbidden / Retired Names

| Name | Reason |
|---|---|
| Archivist Sael Quorrin | Retired during Stage 1 — collided with "Domic Sael." Renamed to Archivist Quorrin Vane. Do not reuse "Sael Quorrin." |
