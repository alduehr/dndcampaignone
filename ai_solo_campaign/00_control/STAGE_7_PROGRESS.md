# STAGE_7_PROGRESS.md

## Current Stage 7 Objective

Build **Regional Expansion Ring 1** — the three regions adjacent to the Sundering Reach:

- **Ashgarden Vale** (south) — farmland and shrine-towns
- **Tollwood** (east) — deep forest and old toll-roads
- **Pale Coast** (west) — fishing and salt-trade

Each region must connect to the Sundering Reach, Hollowmere, Caradril, Act 1, and the main campaign mystery. All content must be open-world, solo-safe, D&D 5e / 2024-compatible, and AI-retrievable.

Per `DEVELOPMENT_STAGES.md` Stage 7 targets (per region):
- 1 major settlement or 2–3 towns
- 5–10 villages or small sites
- 10–20 wilderness locations
- 3–6 dungeons/ruins
- 30–60 NPCs
- 20–40 hooks
- 8–15 developed quests
- 3–5 secrets or mystery chains (reuse existing M1–M9; no new central mysteries)
- 2–5 faction clocks

## Plan (production batches)

1. **Ashgarden Vale** — region file, 1–3 settlements, wilderness sites, dungeon/ruins, NPCs, quests/hooks/rumors, encounter table, faction activity, clocks, mystery links.
2. **Tollwood** — same.
3. **Pale Coast** — same.
4. **Travel connectors** — travel routes between the three Ring 1 regions and the Reach/Caradril; travel events/complications.
5. **Indexes/tracking** — NAMING_REGISTRY, CONTENT_INDEX, TAG_INDEX, RETRIEVAL_GUIDE, PROGRESS_LOG, TODO, CONTENT_GAPS, EXPANSION_PLAN, STAGE_STATUS, CONSISTENCY_AUDIT, CANON (revision log), PLAYER_SAFE_CANON.

## Files to Create

### Ashgarden Vale
- [x] `05_regions/ASHGARDEN_VALE.md`
- [x] 3 settlement files: `ORCHARDMERE.md`, `SAINT_VEDDOWS_REST.md`, `TILBROOK.md`
- [x] Wilderness file: `05_regions/wilderness/ASHGARDEN_VALE_SITES.md` (10 sites + 3 hamlets)
- [x] 3 dungeon files: `SAINT_VEDDOWS_TOMB.md`, `THE_BURIED_CLOISTER.md`, `THE_PELLOW_GRANGE.md`
- [x] 8 developed quests (Q_THE_FUNERAL_DONE_TWICE, Q_SAINTS_BONES, Q_THE_SEALED_DOOR, Q_THE_LOAF_THAT_MOVES, Q_THE_MARKS_ON_THE_DOORS, Q_THE_SAINT_WHO_WEEPS, Q_THE_CROWS_OF_MARROW_CROSS, Q_WHATS_UNDER_THE_ORCHARD)
- [x] Encounter table: `ASHGARDEN_VALE_ENCOUNTERS.md`
- [x] Hooks/rumors: `ASHGARDEN_VALE_HOOKS.md`, `ASHGARDEN_VALE_RUMORS.md`

### Tollwood
- [x] `05_regions/TOLLWOOD.md`
- [x] 3 settlement files: `HARTFELL.md`, `COLDHEARTH.md`, `TOLLSTONE_CROSS.md`
- [x] Wilderness file: `05_regions/wilderness/TOLLWOOD_SITES.md` (10 sites)
- [x] 3 dungeon files: `THE_GREENWARD_TOLL_STATION.md`, `THE_HANGING_OAKS.md`, `THE_OLD_MAST.md` (gated)
- [x] 8 developed quests (Q_THE_MARKED_OAKS, Q_THE_TOLL_WAR, Q_THE_DROWNED_VAULT, Q_THE_BARGAIN, Q_THE_HANGING_OAKS, Q_TO_THE_EDGE, Q_THE_RECKLESS_GUIDE, Q_THE_LOST_CREW)
- [x] Encounter table: `TOLLWOOD_ENCOUNTERS.md`
- [x] Hooks/rumors: `TOLLWOOD_HOOKS.md`, `TOLLWOOD_RUMORS.md`

### Pale Coast
- [x] `05_regions/PALE_COAST.md`
- [x] 2 settlement files: `WRACKMOUTH.md`, `COBBLE_STRAND.md` (Saltmargin reused as existing gateway)
- [x] Wilderness file: `05_regions/wilderness/PALE_COAST_SITES.md` (10 sites)
- [x] 3 dungeon files: `THE_DROWNED_LAMP.md`, `THE_WRECKERS_CAVES.md`, `THE_SKERRY_SHRINE.md` (gated)
- [x] 8 developed quests (Q_THE_SALT_PRICE, Q_THE_SALT_MOTHERS_BURDEN, Q_WHAT_THE_LAMP_HOLDS, Q_THE_COVE_CAVES, Q_THE_WRECKERS, Q_THE_DROWNED_BELL, Q_THE_SKIPPERS_DEBT, Q_THE_EMPTY_HEARTH)
- [x] Encounter table: `PALE_COAST_ENCOUNTERS.md`
- [x] Hooks/rumors: `PALE_COAST_HOOKS.md`, `PALE_COAST_RUMORS.md`

### Travel
- [x] `04_world_atlas/TRAVEL_ROUTES_RING1.md`

## Files to Update

- [x] `00_control/NAMING_REGISTRY.md`
- [x] `00_control/CONTENT_INDEX.md`
- [x] `00_control/TAG_INDEX.md`
- [x] `00_control/RETRIEVAL_GUIDE.md`
- [x] `00_control/PROGRESS_LOG.md`
- [x] `00_control/STAGE_STATUS.md`
- [x] `00_control/TODO.md`
- [x] `00_control/CONSISTENCY_AUDIT.md`
- [x] `17_generation_backlog/CONTENT_GAPS.md`
- [x] `17_generation_backlog/EXPANSION_PLAN.md`
- [x] `03_canon/CANON.md` (revision log)
- [x] `03_canon/PLAYER_SAFE_CANON.md`
- [x] `08_npcs/SECONDARY_NPCS.md`
- [x] `08_npcs/MINOR_NPCS.md`
- [x] `08_npcs/NPC_INDEX.md`

## Progress Log

| Time | What Was Done |
|---|---|
| 2026-06-10 | Stage 7 progress file created. Agent launched. |
| 2026-06-10 | All three regions fully authored. Completion pass added 1 Tollwood quest, 3 Coast quests, 4 wilderness sites per region, ~22 NPCs, 6 regional clocks. All tracking files updated. Stage 7 complete. |

## Region Build Status

| Region | Status |
|---|---|
| Ashgarden Vale | **Complete** — region, 3 settlements, 1 wilderness file (10 sites + 3 hamlets), 3 dungeons, encounter table, hooks/rumors, **8 developed quests**, 2 regional clocks (V1/V2), M2/M5/M6 clue access |
| Tollwood | **Complete** — region, 3 settlements, 1 wilderness file (10 sites), 3 dungeons (incl. gated Old Mast), encounter table, hooks/rumors, **8 developed quests**, 1 minor faction (Tollmen), 2 regional clocks (T1/T2) |
| Pale Coast | **Complete** — region, 2 settlements (Saltmargin as gateway), 1 wilderness file (10 sites), 3 dungeons (incl. gated Skerry Shrine), encounter table, hooks/rumors, **8 developed quests**, 2 regional clocks (C-PC1/C-PC2), M2/M3/M5 sea-shrine clue access |
| Travel connectors | **Complete** — TRAVEL_ROUTES_RING1.md (6 routes: Reach→each region, each region→Caradril) |
| Indexes/tracking | **Complete** |

## Completion Criteria (from DEVELOPMENT_STAGES.md)

- [x] Player can leave the starting region in multiple directions
- [x] Nearby regions have enough authored content for extended play
- [x] Travel between regions is meaningful
- [x] Adjacent regions connect to the main arc and local arcs
- [x] All new proper nouns registered in NAMING_REGISTRY
- [x] All new files indexed and cross-linked
- [x] Canon updated

## Status

**Complete — 2026-06-10.**
