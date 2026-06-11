# TAG_INDEX.md

## Purpose

Master index of retrieval tags used across the campaign repository. Makes campaign content searchable by type, secrecy, status, level, region, faction, and play function.

## Current Status

**Stages 1, 2, 3, 4, and 5 complete.** Stage 1 foundation + Stage 2 AI runtime + Stage 3 Starting Region Deep Build + Stage 4 First Major City Deep Build (Caradril) + **Stage 5 Level 1–4 Play Arc**. Stage 4 added the Caradril files (see `region:caradril`). **Stage 5 added:** `12_campaign_arc/ACT_1_LEVELS_1_4.md`, `ACT_1_MILESTONES.md`, `ACT_1_FAILURE_STATES.md`; `09_quests/act_1_quests/` (6 faction quests); `13_encounters_and_bestiary/ACT_1_THREATS.md`; `11_mysteries_and_secrets/ACT_1_CLUE_TRAILS.md`; `08_npcs/ACT_1_NPC_GUIDE.md`. New tag introduced: `act:1`. All Stage 5 files registered below. No active content files remain placeholder-only; future-stage placeholder files (`_PLACEHOLDER.md`) still exist by design as structural anchors. Stage 6 (first full audit) is complete. **Stage 7 (Regional Expansion Ring 1) is complete:** the three adjacent regions (Ashgarden Vale, Tollwood, Pale Coast) added 3 region files, 8 settlements, 3 wilderness files, 9 dungeons, 3 encounter tables, 6 hooks/rumors files, 20 developed quests, 40 NPCs (in the existing NPC files), 1 minor regional faction (the Tollmen), and `04_world_atlas/TRAVEL_ROUTES_RING1.md`. New tags introduced: `ring-1`, `region:ashgarden-vale`, `region:tollwood`, `region:pale-coast`. All Stage 7 files registered below. **Full-World Cartographic Expansion pass (post-Stage-7):** added 4 full-continent atlas files (`FULL_WORLD_MAP_AUTHORITY/COORDINATES/LAYERS/PROMPTS.md`); new tags introduced: `full-continent` (and `campaign-area` to disambiguate the existing `WORLD_MAP_*` files). Both sets are registered under `type:map / function:cartography`.

> Caradril file membership is consolidated under **`region:caradril`** (Region Tags section) for fast retrieval; individual files also appear under their type/secrecy/status tags.

---

## How To Use

When an AI DM or production agent needs to find content of a certain type, search by tag. Each entry lists files that carry that tag.

---

## Type Tags

### type:region
- `05_regions/SUNDERING_REACH.md`
- `05_regions/ASHGARDEN_VALE.md` (ring-1)
- `05_regions/TOLLWOOD.md` (ring-1)
- `05_regions/PALE_COAST.md` (ring-1)
- `04_world_atlas/WORLD_OVERVIEW.md`
- `04_world_atlas/MAP_DESCRIPTION.md`
- `04_world_atlas/TRAVEL_ROUTES_RING1.md` (ring-1 travel)
- `04_world_atlas/WORLD_MAP_AUTHORITY.md` (type:map; cartography; campaign-area)
- `04_world_atlas/WORLD_MAP_COORDINATES.md` (type:map; cartography; campaign-area)
- `04_world_atlas/WORLD_MAP_LAYERS.md` (type:map; cartography; campaign-area)
- `04_world_atlas/WORLD_MAP_PROMPTS.md` (type:map; cartography; campaign-area)
- `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` (type:map; cartography; full-continent)
- `04_world_atlas/FULL_WORLD_MAP_COORDINATES.md` (type:map; cartography; full-continent)
- `04_world_atlas/FULL_WORLD_MAP_LAYERS.md` (type:map; cartography; full-continent)
- `04_world_atlas/FULL_WORLD_MAP_PROMPTS.md` (type:map; cartography; full-continent)

### full-continent (Full-World Cartographic Expansion)
- `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md`
- `04_world_atlas/FULL_WORLD_MAP_COORDINATES.md`
- `04_world_atlas/FULL_WORLD_MAP_LAYERS.md`
- `04_world_atlas/FULL_WORLD_MAP_PROMPTS.md`

### type:map / function:cartography
**Campaign-area (NW Orrun cluster):**
- `04_world_atlas/WORLD_MAP_AUTHORITY.md` — campaign-area cartographic authority (cluster shape, placement, scale, secrecy)
- `04_world_atlas/WORLD_MAP_COORDINATES.md` — campaign-area 0–100 grid (~3× zoom on the NW corner); confidence-rated; DM-only rows flagged
- `04_world_atlas/WORLD_MAP_LAYERS.md` — 7 campaign-area map layers (player-safe → hidden-truth)
- `04_world_atlas/WORLD_MAP_PROMPTS.md` — 4 campaign-area image-generation prompts

**Full continent (Orrun + Vael landmasses):**
- `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` — full-continent master reference (NW→SE axis, all features, 18 regions, routes, forbidden zones, scale, secrecy)
- `04_world_atlas/FULL_WORLD_MAP_COORDINATES.md` — full-continent 0–100 grid (124 entries; embeds the cluster in the NW corner); confidence-rated; DM-only rows flagged
- `04_world_atlas/FULL_WORLD_MAP_LAYERS.md` — 8 full-world map layers (incl. campaign-area inset)
- `04_world_atlas/FULL_WORLD_MAP_PROMPTS.md` — 5 full-world image-generation prompts
- `04_world_atlas/REGION_INDEX.md` — region index incl. placeholders (type:index)

### type:settlement
- `06_settlements/HOLLOWMERE.md`
- `06_settlements/KETTLE_BRIDGE.md`
- `06_settlements/SALTMARGIN.md`
- `06_settlements/CANDLEWICK.md`
- `06_settlements/GREYWATER_HOLM.md`
- `06_settlements/HARROWGAST.md`
- `06_settlements/REEDFORD.md`
- `06_settlements/THE_ASHWALK_REST.md`
- `06_settlements/CARADRIL.md` (major-city)
- `06_settlements/caradril_districts/THE_MAGISTERIUM.md` (district)
- `06_settlements/caradril_districts/THE_COUNTING_QUAYS.md` (district)
- `06_settlements/caradril_districts/THE_LANTERN_REACH.md` (district)
- `06_settlements/caradril_districts/THE_ASHMARKET.md` (district)
- `06_settlements/caradril_districts/HIGHMOURN.md` (district)
- `06_settlements/caradril_districts/THE_CRUCIBLE.md` (district)
- `06_settlements/caradril_districts/THE_SILL.md` (district)
- `06_settlements/caradril_districts/THE_SUNKEN_WARDS.md` (district/ruin)
- `06_settlements/ORCHARDMERE.md` (ring-1, Vale hub)
- `06_settlements/SAINT_VEDDOWS_REST.md` (ring-1, Vale)
- `06_settlements/TILBROOK.md` (ring-1, Vale)
- `06_settlements/HARTFELL.md` (ring-1, Tollwood hub)
- `06_settlements/COLDHEARTH.md` (ring-1, Tollwood)
- `06_settlements/TOLLSTONE_CROSS.md` (ring-1, Tollwood)
- `06_settlements/WRACKMOUTH.md` (ring-1, Coast hub)
- `06_settlements/COBBLE_STRAND.md` (ring-1, Coast)

### type:wilderness_location
- `05_regions/wilderness/GREYFENS_SITES.md`
- `05_regions/wilderness/SUNDER_HEIGHTS_SITES.md`
- `05_regions/wilderness/MIREWEND_AND_ROADS_SITES.md`
- `05_regions/wilderness/BASIN_SHORE_AND_HOLMS_SITES.md`
- `05_regions/wilderness/ASHGARDEN_VALE_SITES.md` (ring-1)
- `05_regions/wilderness/TOLLWOOD_SITES.md` (ring-1)
- `05_regions/wilderness/PALE_COAST_SITES.md` (ring-1)

### type:npc
- `08_npcs/MAJOR_NPCS.md`
- `08_npcs/SECONDARY_NPCS.md`
- `08_npcs/MINOR_NPCS.md`
- `08_npcs/ACT_1_NPC_GUIDE.md` (Act 1 casting guide; act:1)
- `08_npcs/NPC_INDEX.md`

### type:faction
- `07_factions/major_factions/ASHEN_WARDENS.md`
- `07_factions/major_factions/CINDER_LEDGER.md`
- `07_factions/major_factions/MOURNERS_CIRCLE.md`
- `07_factions/major_factions/REACHWARD_COMPACT.md`
- `07_factions/major_factions/GRAVECALLERS.md`
- `07_factions/major_factions/CONCORD_REMNANT.md`
- `07_factions/major_factions/HOLLOW_COURT.md`
- `07_factions/FACTION_INDEX.md`

### type:quest
- `09_quests/HOOKS_TABLE.md`
- `09_quests/RUMORS_TABLE.md`
- `09_quests/hooks_and_rumors/SUNDERING_REACH_HOOKS.md`
- `09_quests/hooks_and_rumors/SUNDERING_REACH_RUMORS.md`
- `09_quests/regional_quests/Q_THE_SALT_RUN.md`
- `09_quests/regional_quests/Q_THE_BROKEN_ARCH.md`
- `09_quests/regional_quests/Q_LIGHT_ON_THE_SCALE.md`
- `09_quests/regional_quests/Q_THE_HOLM_THAT_WONT_BURY_ITS_DEAD.md`
- `09_quests/regional_quests/Q_THE_SOLD_STONE.md`
- `09_quests/regional_quests/Q_RACE_NORTH.md`
- `09_quests/regional_quests/Q_THE_BAILIFFS_LADDER.md`
- `09_quests/regional_quests/Q_THE_REED_HOLMS.md`
- `09_quests/regional_quests/Q_SASHES_WARNING.md`
- `09_quests/regional_quests/Q_THE_GREY_WOMAN_AT_THE_FORD.md`
- `09_quests/regional_quests/Q_THE_SECOND_MARK.md`
- `09_quests/regional_quests/Q_PELLS_DOUBT.md`
- `09_quests/regional_quests/Q_THE_SCHOLARS_REQUEST.md`
- `09_quests/regional_quests/Q_THE_FAILING_FUNERAL.md`
- `09_quests/hooks_and_rumors/CARADRIL_HOOKS.md`
- `09_quests/hooks_and_rumors/CARADRIL_RUMORS.md`
- `09_quests/city_quests/Q_THE_SEALED_LETTER.md`
- `09_quests/city_quests/Q_THE_OPEN_CHARTER.md`
- `09_quests/city_quests/Q_THE_QUAY_CHARTER.md`
- `09_quests/city_quests/Q_THE_LANTERN_AND_THE_LAMP.md`
- `09_quests/city_quests/Q_THE_SEALED_ARCHIVE.md`
- `09_quests/city_quests/Q_QUIET_COIN.md`
- `09_quests/city_quests/Q_THE_FUNERAL_THAT_WOULDNT_TAKE.md`
- `09_quests/city_quests/Q_THE_SMELTING.md`
- `09_quests/city_quests/Q_THE_BELLMANS_PRICE.md`
- `09_quests/city_quests/Q_BELOW_THE_STILLING.md`
- `09_quests/city_quests/Q_THE_TIDE_TURNS.md`
- `09_quests/act_1_quests/Q_ACT1_WARDEN_THE_TRUE_RITE.md`
- `09_quests/act_1_quests/Q_ACT1_COMPACT_THE_REEVES_DOUBT.md`
- `09_quests/act_1_quests/Q_ACT1_LEDGER_A_QUIET_SALVAGE.md`
- `09_quests/act_1_quests/Q_ACT1_MOURNER_SALT_AND_SONG.md`
- `09_quests/act_1_quests/Q_ACT1_GRAVECALLER_A_LAST_WORD.md`
- `09_quests/act_1_quests/Q_ACT1_REMNANT_THE_VISITING_SCHOLAR.md`
- `09_quests/hooks_and_rumors/ASHGARDEN_VALE_HOOKS.md`, `ASHGARDEN_VALE_RUMORS.md` (ring-1)
- `09_quests/hooks_and_rumors/TOLLWOOD_HOOKS.md`, `TOLLWOOD_RUMORS.md` (ring-1)
- `09_quests/hooks_and_rumors/PALE_COAST_HOOKS.md`, `PALE_COAST_RUMORS.md` (ring-1)
- `09_quests/regional_quests/` Vale quests (ring-1): `Q_THE_FUNERAL_DONE_TWICE.md`, `Q_SAINTS_BONES.md`, `Q_THE_SEALED_DOOR.md`, `Q_THE_LOAF_THAT_MOVES.md`, `Q_THE_MARKS_ON_THE_DOORS.md`, `Q_THE_SAINT_WHO_WEEPS.md`, `Q_THE_CROWS_OF_MARROW_CROSS.md`, `Q_WHATS_UNDER_THE_ORCHARD.md`
- `09_quests/regional_quests/` Tollwood quests (ring-1): `Q_THE_MARKED_OAKS.md`, `Q_THE_TOLL_WAR.md`, `Q_THE_DROWNED_VAULT.md`, `Q_THE_BARGAIN.md`, `Q_THE_HANGING_OAKS.md`, `Q_TO_THE_EDGE.md`, `Q_THE_RECKLESS_GUIDE.md`, `Q_THE_LOST_CREW.md`
- `09_quests/regional_quests/` Coast quests (ring-1): `Q_THE_SALT_PRICE.md`, `Q_THE_SALT_MOTHERS_BURDEN.md`, `Q_WHAT_THE_LAMP_HOLDS.md`, `Q_THE_COVE_CAVES.md`, `Q_THE_WRECKERS.md`, `Q_THE_DROWNED_BELL.md`, `Q_THE_SKIPPERS_DEBT.md`, `Q_THE_EMPTY_HEARTH.md`

### type:mystery
- `11_mysteries_and_secrets/MYSTERY_WEB.md`
- `11_mysteries_and_secrets/REVELATION_MAP.md`
- `11_mysteries_and_secrets/SECRET_INDEX.md`

### type:clue
- `11_mysteries_and_secrets/MYSTERY_WEB.md` (clue paths embedded)
- `11_mysteries_and_secrets/CLUE_INDEX.md` (all authored clues; populated)
- `11_mysteries_and_secrets/ACT_1_CLUE_TRAILS.md` (Act 1 L1–4 access overlay; act:1)
- `02_runtime_state/HIDDEN_CLUES.md` (runtime mirror; all hidden at start)

### type:dungeon
- `10_dungeons_and_ruins/THE_SUNKEN_TOLLHOUSE.md`
- `10_dungeons_and_ruins/THE_LEDGER_VAULT.md`
- `10_dungeons_and_ruins/THE_BARROW_OF_NINE_DOORS.md`
- `10_dungeons_and_ruins/THE_DEEP_ADIT.md`
- `10_dungeons_and_ruins/THE_PELLOW_GRANGE.md` (ring-1, Vale)
- `10_dungeons_and_ruins/THE_GREENWARD_TOLL_STATION.md` (ring-1, Tollwood)
- `10_dungeons_and_ruins/THE_HANGING_OAKS.md` (ring-1, Tollwood)
- `10_dungeons_and_ruins/THE_OLD_MAST.md` (ring-1, Tollwood; gated)
- `10_dungeons_and_ruins/THE_DROWNED_LAMP.md` (ring-1, Coast; secondary-node)
- `10_dungeons_and_ruins/THE_WRECKERS_CAVES.md` (ring-1, Coast)
- `10_dungeons_and_ruins/THE_SKERRY_SHRINE.md` (ring-1, Coast; gated)
- Drowned shrine — referenced in `07_factions/major_factions/HOLLOW_COURT.md` (full build Stage 12)

### type:ruin
- `10_dungeons_and_ruins/THE_PEAT_CHAPEL.md`
- `10_dungeons_and_ruins/THE_WHISPERING_CAIRN.md`
- `10_dungeons_and_ruins/SAINT_VEDDOWS_TOMB.md` (ring-1, Vale; secondary-node)
- `10_dungeons_and_ruins/THE_BURIED_CLOISTER.md` (ring-1, Vale)

### type:encounter
- `13_encounters_and_bestiary/SUNDERING_REACH_ENCOUNTERS.md`
- `13_encounters_and_bestiary/CARADRIL_ENCOUNTERS.md`
- `13_encounters_and_bestiary/ACT_1_THREATS.md` (5 recurring Act 1 adversary profiles; act:1)
- `13_encounters_and_bestiary/ASHGARDEN_VALE_ENCOUNTERS.md` (ring-1)
- `13_encounters_and_bestiary/TOLLWOOD_ENCOUNTERS.md` (ring-1)
- `13_encounters_and_bestiary/PALE_COAST_ENCOUNTERS.md` (ring-1)

### type:artifact
- Remembrance relics — referenced in `03_canon/MAGIC_RULES.md` (full build Stage 14)

### type:canon
- `03_canon/CANON.md`
- `03_canon/PLAYER_SAFE_CANON.md`
- `03_canon/DM_ONLY_CANON.md`
- `03_canon/CAMPAIGN_IDENTITY_LOCK.md`
- `03_canon/WORLD_HISTORY.md`
- `03_canon/COSMOLOGY.md`
- `03_canon/GODS_AND_FAITHS.md`
- `03_canon/MAGIC_RULES.md`
- `03_canon/CALENDAR.md`
- `03_canon/LANGUAGES.md`
- `03_canon/LEVELING_ASSUMPTIONS.md`
- `12_campaign_arc/ACT_1_LEVELS_1_4.md` (Act 1 arc spine; act:1)
- `12_campaign_arc/ACT_1_MILESTONES.md` (act:1)
- `12_campaign_arc/ACT_1_FAILURE_STATES.md` (act:1)

### type:runtime
- `01_runner_protocol/AI_DM_CORE_RULES.md`
- `01_runner_protocol/SOLO_PLAY_PRINCIPLES.md`
- `01_runner_protocol/SESSION_LOOP.md`
- `01_runner_protocol/SCENE_FRAMING.md`
- `01_runner_protocol/PLAYER_CHOICE_PROTOCOL.md`
- `01_runner_protocol/ROLL_AND_CHECK_PROTOCOL.md`
- `01_runner_protocol/COMBAT_PROTOCOL.md`
- `01_runner_protocol/SOCIAL_SCENE_PROTOCOL.md`
- `01_runner_protocol/EXPLORATION_PROTOCOL.md`
- `01_runner_protocol/TRAVEL_PROTOCOL.md`
- `01_runner_protocol/DOWNTIME_PROTOCOL.md`
- `01_runner_protocol/CLUE_DELIVERY_PROTOCOL.md`
- `01_runner_protocol/SECRET_REVEAL_PROTOCOL.md`
- `01_runner_protocol/FAILURE_AND_CONSEQUENCES.md`
- `01_runner_protocol/TONE_AND_NARRATION.md`
- `01_runner_protocol/WHEN_TO_ASK_QUESTIONS.md`
- `01_runner_protocol/WHEN_TO_IMPROVISE.md`
- `01_runner_protocol/SESSION_END_PROTOCOL.md`
- `16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md`
- `16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md`
- `16_ai_session_packs/RESUME_CAMPAIGN_PROMPT.md`
- `16_ai_session_packs/STATE_UPDATE_TEMPLATE.md`
- `16_ai_session_packs/COMPACT_CONTEXT_TEMPLATE.md`
- `16_ai_session_packs/DM_HIDDEN_RECAP_TEMPLATE.md`
- `02_runtime_state/CURRENT_STATE.md`
- `02_runtime_state/PLAYER_CHARACTER.md`
- `02_runtime_state/CURRENT_LOCATION.md`
- `02_runtime_state/CURRENT_SCENE.md`
- `02_runtime_state/ACTIVE_QUESTS.md`
- `02_runtime_state/OPEN_THREADS.md`
- `02_runtime_state/KNOWN_CLUES.md`
- `02_runtime_state/HIDDEN_CLUES.md`
- `02_runtime_state/NPC_MEMORY.md`
- `02_runtime_state/FACTION_STATE.md`
- `02_runtime_state/WORLD_CLOCKS.md`
- `02_runtime_state/INVENTORY_AND_REWARDS.md`
- `02_runtime_state/RELATIONSHIPS.md`
- `02_runtime_state/CONSEQUENCES.md`
- `02_runtime_state/SESSION_RECAP.md`
- `02_runtime_state/NEXT_SESSION_START.md`

### type:protocol
- `01_runner_protocol/AI_DM_CORE_RULES.md`
- `01_runner_protocol/SOLO_PLAY_PRINCIPLES.md`
- `01_runner_protocol/SESSION_LOOP.md`
- `01_runner_protocol/SCENE_FRAMING.md`
- `01_runner_protocol/PLAYER_CHOICE_PROTOCOL.md`
- `01_runner_protocol/ROLL_AND_CHECK_PROTOCOL.md`
- `01_runner_protocol/COMBAT_PROTOCOL.md`
- `01_runner_protocol/SOCIAL_SCENE_PROTOCOL.md`
- `01_runner_protocol/EXPLORATION_PROTOCOL.md`
- `01_runner_protocol/TRAVEL_PROTOCOL.md`
- `01_runner_protocol/DOWNTIME_PROTOCOL.md`
- `01_runner_protocol/CLUE_DELIVERY_PROTOCOL.md`
- `01_runner_protocol/SECRET_REVEAL_PROTOCOL.md`
- `01_runner_protocol/FAILURE_AND_CONSEQUENCES.md`
- `01_runner_protocol/TONE_AND_NARRATION.md`
- `01_runner_protocol/WHEN_TO_ASK_QUESTIONS.md`
- `01_runner_protocol/WHEN_TO_IMPROVISE.md`
- `01_runner_protocol/SESSION_END_PROTOCOL.md`

### type:state
- `02_runtime_state/CURRENT_STATE.md`
- `02_runtime_state/PLAYER_CHARACTER.md`
- `02_runtime_state/CURRENT_LOCATION.md`
- `02_runtime_state/CURRENT_SCENE.md`
- `02_runtime_state/ACTIVE_QUESTS.md`
- `02_runtime_state/OPEN_THREADS.md`
- `02_runtime_state/KNOWN_CLUES.md`
- `02_runtime_state/HIDDEN_CLUES.md`
- `02_runtime_state/NPC_MEMORY.md`
- `02_runtime_state/FACTION_STATE.md`
- `02_runtime_state/WORLD_CLOCKS.md`
- `02_runtime_state/INVENTORY_AND_REWARDS.md`
- `02_runtime_state/RELATIONSHIPS.md`
- `02_runtime_state/CONSEQUENCES.md`
- `02_runtime_state/SESSION_RECAP.md`
- `02_runtime_state/NEXT_SESSION_START.md`

### type:index
- `00_control/CONTENT_INDEX.md`
- `00_control/TAG_INDEX.md`
- `00_control/NAMING_REGISTRY.md`
- `00_control/RETRIEVAL_GUIDE.md`
- `07_factions/FACTION_INDEX.md`
- `08_npcs/NPC_INDEX.md`
- `11_mysteries_and_secrets/CLUE_INDEX.md`
- `11_mysteries_and_secrets/SECRET_INDEX.md`

---

## Secrecy Tags

### secrecy:player-safe
- `03_canon/PLAYER_SAFE_CANON.md`
- `03_canon/CALENDAR.md`
- `03_canon/LANGUAGES.md`
- `03_canon/LEVELING_ASSUMPTIONS.md`
- `04_world_atlas/MAP_DESCRIPTION.md`
- `02_runtime_state/PLAYER_CHARACTER.md`
- `02_runtime_state/CURRENT_LOCATION.md`
- `02_runtime_state/KNOWN_CLUES.md`
- `02_runtime_state/INVENTORY_AND_REWARDS.md`
- `02_runtime_state/RELATIONSHIPS.md`
- `02_runtime_state/SESSION_RECAP.md`

### secrecy:dm-only
- `03_canon/DM_ONLY_CANON.md`
- `03_canon/CAMPAIGN_IDENTITY_LOCK.md`
- `07_factions/major_factions/HOLLOW_COURT.md`
- `02_runtime_state/HIDDEN_CLUES.md`
- `12_campaign_arc/MAIN_ARC_OVERVIEW.md`
- `12_campaign_arc/LEVEL_1_TO_20_PROGRESSION.md`
- `11_mysteries_and_secrets/MYSTERY_WEB.md`
- `11_mysteries_and_secrets/REVELATION_MAP.md`
- `11_mysteries_and_secrets/CLUE_INDEX.md`
- `11_mysteries_and_secrets/ACT_1_CLUE_TRAILS.md`
- `11_mysteries_and_secrets/SECRET_INDEX.md`
- `16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md`
- `16_ai_session_packs/RESUME_CAMPAIGN_PROMPT.md`
- `16_ai_session_packs/STATE_UPDATE_TEMPLATE.md`
- `16_ai_session_packs/COMPACT_CONTEXT_TEMPLATE.md`
- `16_ai_session_packs/DM_HIDDEN_RECAP_TEMPLATE.md`

### secrecy:mixed
- `03_canon/CANON.md`
- `03_canon/WORLD_HISTORY.md`
- `03_canon/COSMOLOGY.md`
- `03_canon/GODS_AND_FAITHS.md`
- `03_canon/MAGIC_RULES.md`
- `04_world_atlas/WORLD_OVERVIEW.md`
- `05_regions/SUNDERING_REACH.md`
- `06_settlements/HOLLOWMERE.md`
- `07_factions/major_factions/ASHEN_WARDENS.md`
- `07_factions/major_factions/CINDER_LEDGER.md`
- `07_factions/major_factions/MOURNERS_CIRCLE.md`
- `07_factions/major_factions/REACHWARD_COMPACT.md`
- `07_factions/major_factions/GRAVECALLERS.md`
- `07_factions/major_factions/CONCORD_REMNANT.md`
- `07_factions/FACTION_INDEX.md`
- `08_npcs/MAJOR_NPCS.md`
- `08_npcs/NPC_INDEX.md`
- `09_quests/HOOKS_TABLE.md`
- `09_quests/RUMORS_TABLE.md`
- `16_ai_session_packs/OPENING_SCENES.md`
- `16_ai_session_packs/SOLO_SAFETY_START.md`
- `02_runtime_state/CURRENT_STATE.md`
- `02_runtime_state/CURRENT_SCENE.md`
- `02_runtime_state/ACTIVE_QUESTS.md`
- `02_runtime_state/OPEN_THREADS.md`
- `02_runtime_state/NPC_MEMORY.md`
- `02_runtime_state/FACTION_STATE.md`
- `02_runtime_state/WORLD_CLOCKS.md`
- `02_runtime_state/CONSEQUENCES.md`
- `02_runtime_state/NEXT_SESSION_START.md`
- `16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md`
- **All Stage 4 Caradril content files** (`06_settlements/CARADRIL.md`, the 8 `caradril_districts/` files, `09_quests/city_quests/*`, `09_quests/hooks_and_rumors/CARADRIL_HOOKS.md` + `CARADRIL_RUMORS.md`, `13_encounters_and_bestiary/CARADRIL_ENCOUNTERS.md`) — see the consolidated `region:caradril` block
- **All Stage 5 Act 1 content files except the dm-only clue trails:** `12_campaign_arc/ACT_1_LEVELS_1_4.md`, `ACT_1_MILESTONES.md`, `ACT_1_FAILURE_STATES.md`; `13_encounters_and_bestiary/ACT_1_THREATS.md`; `08_npcs/ACT_1_NPC_GUIDE.md`; `09_quests/act_1_quests/*` — see the `act:1` block

---

## Status Tags

### status:static
- `03_canon/CANON.md`
- `03_canon/DM_ONLY_CANON.md`
- `03_canon/CAMPAIGN_IDENTITY_LOCK.md`
- `03_canon/WORLD_HISTORY.md`
- `03_canon/COSMOLOGY.md`
- `03_canon/GODS_AND_FAITHS.md`
- `03_canon/MAGIC_RULES.md`
- `03_canon/CALENDAR.md`
- `03_canon/LANGUAGES.md`
- `03_canon/LEVELING_ASSUMPTIONS.md`
- `04_world_atlas/WORLD_OVERVIEW.md`
- `04_world_atlas/MAP_DESCRIPTION.md`
- `05_regions/SUNDERING_REACH.md`
- `05_regions/wilderness/GREYFENS_SITES.md`
- `05_regions/wilderness/SUNDER_HEIGHTS_SITES.md`
- `05_regions/wilderness/MIREWEND_AND_ROADS_SITES.md`
- `05_regions/wilderness/BASIN_SHORE_AND_HOLMS_SITES.md`
- `06_settlements/HOLLOWMERE.md`
- `06_settlements/KETTLE_BRIDGE.md`
- `06_settlements/SALTMARGIN.md`
- `06_settlements/CANDLEWICK.md`
- `06_settlements/GREYWATER_HOLM.md`
- `06_settlements/HARROWGAST.md`
- `06_settlements/REEDFORD.md`
- `06_settlements/THE_ASHWALK_REST.md`
- `07_factions/major_factions/ASHEN_WARDENS.md`
- `07_factions/major_factions/CINDER_LEDGER.md`
- `07_factions/major_factions/MOURNERS_CIRCLE.md`
- `07_factions/major_factions/REACHWARD_COMPACT.md`
- `07_factions/major_factions/GRAVECALLERS.md`
- `07_factions/major_factions/CONCORD_REMNANT.md`
- `07_factions/major_factions/HOLLOW_COURT.md`
- `07_factions/FACTION_INDEX.md`
- `08_npcs/MAJOR_NPCS.md`
- `08_npcs/SECONDARY_NPCS.md`
- `08_npcs/MINOR_NPCS.md`
- `08_npcs/NPC_INDEX.md`
- `09_quests/HOOKS_TABLE.md`
- `09_quests/RUMORS_TABLE.md`
- `09_quests/hooks_and_rumors/SUNDERING_REACH_HOOKS.md`
- `09_quests/hooks_and_rumors/SUNDERING_REACH_RUMORS.md`
- `09_quests/regional_quests/` (14 developed quests)
- `10_dungeons_and_ruins/` (6 dungeons/ruins)
- `13_encounters_and_bestiary/SUNDERING_REACH_ENCOUNTERS.md`
- `16_ai_session_packs/OPENING_SCENES.md`
- `16_ai_session_packs/SOLO_SAFETY_START.md`
- `12_campaign_arc/MAIN_ARC_OVERVIEW.md`
- `12_campaign_arc/LEVEL_1_TO_20_PROGRESSION.md`
- `11_mysteries_and_secrets/MYSTERY_WEB.md`
- `11_mysteries_and_secrets/REVELATION_MAP.md`
- `11_mysteries_and_secrets/SECRET_INDEX.md`
- `11_mysteries_and_secrets/CLUE_INDEX.md`
- **All Stage 4 Caradril content files** (`06_settlements/CARADRIL.md`, the 8 `caradril_districts/` files, `09_quests/city_quests/*`, `09_quests/hooks_and_rumors/CARADRIL_*.md`, `13_encounters_and_bestiary/CARADRIL_ENCOUNTERS.md`) — see `region:caradril`
- **All Stage 5 Act 1 content files** (`12_campaign_arc/ACT_1_LEVELS_1_4.md`, `ACT_1_MILESTONES.md`, `ACT_1_FAILURE_STATES.md`; `09_quests/act_1_quests/*`; `13_encounters_and_bestiary/ACT_1_THREATS.md`; `11_mysteries_and_secrets/ACT_1_CLUE_TRAILS.md`; `08_npcs/ACT_1_NPC_GUIDE.md`) — see `act:1`

### status:runtime
- `03_canon/PLAYER_SAFE_CANON.md` — updated as player discovers facts
- `02_runtime_state/CURRENT_STATE.md`
- `02_runtime_state/PLAYER_CHARACTER.md`
- `02_runtime_state/CURRENT_LOCATION.md`
- `02_runtime_state/CURRENT_SCENE.md`
- `02_runtime_state/ACTIVE_QUESTS.md`
- `02_runtime_state/OPEN_THREADS.md`
- `02_runtime_state/KNOWN_CLUES.md`
- `02_runtime_state/HIDDEN_CLUES.md`
- `02_runtime_state/NPC_MEMORY.md`
- `02_runtime_state/FACTION_STATE.md`
- `02_runtime_state/WORLD_CLOCKS.md`
- `02_runtime_state/INVENTORY_AND_REWARDS.md`
- `02_runtime_state/RELATIONSHIPS.md`
- `02_runtime_state/CONSEQUENCES.md`
- `02_runtime_state/SESSION_RECAP.md`
- `02_runtime_state/NEXT_SESSION_START.md`

### status:seeded (campaign-start baseline; become status:active on play)
- `02_runtime_state/CURRENT_STATE.md`
- `02_runtime_state/CURRENT_LOCATION.md`
- `02_runtime_state/CURRENT_SCENE.md`
- `02_runtime_state/ACTIVE_QUESTS.md`
- `02_runtime_state/OPEN_THREADS.md`
- `02_runtime_state/FACTION_STATE.md`
- `02_runtime_state/WORLD_CLOCKS.md`
- `02_runtime_state/NEXT_SESSION_START.md`
- `02_runtime_state/PLAYER_CHARACTER.md` (scaffold — awaiting character creation)

### status:active
- *No live campaign state yet — runtime files are seeded but play has not begun*

### status:template
- `16_ai_session_packs/STATE_UPDATE_TEMPLATE.md`
- `16_ai_session_packs/COMPACT_CONTEXT_TEMPLATE.md`
- `16_ai_session_packs/DM_HIDDEN_RECAP_TEMPLATE.md`

### status:draft
- *No world content draft files yet*

### status:needs-audit
- *No files flagged yet*

### status:placeholder
- *None — all index/state files now populated or seeded.*

### status:complete
- `00_control/AUDIT_STANDARDS.md`
- `00_control/CANON_AUTHORITY.md`
- `00_control/CONTENT_STANDARDS.md`
- `00_control/DEVELOPMENT_STAGES.md`
- `00_control/DND_MECHANICS_REQUIREMENTS.md`
- `00_control/FACTION_STANDARDS.md`
- `00_control/GENERATION_GUARDRAILS.md`
- `00_control/MYSTERY_STANDARDS.md`
- `00_control/NAMING_REGISTRY.md`
- `00_control/NPC_STANDARDS.md`
- `00_control/PRODUCTION_WORKFLOW.md`
- `00_control/PROJECT_RULES.md`
- `00_control/QUEST_STANDARDS.md`
- `00_control/RULESET_ASSUMPTIONS.md`
- `00_control/TRACKING_SYSTEM.md`
- `00_control/WORLDBUILDING_STANDARDS.md`
- `01_runner_protocol/AI_DM_CORE_RULES.md`
- `01_runner_protocol/SOLO_PLAY_PRINCIPLES.md`
- `01_runner_protocol/SESSION_LOOP.md`
- `01_runner_protocol/SCENE_FRAMING.md`
- `01_runner_protocol/PLAYER_CHOICE_PROTOCOL.md`
- `01_runner_protocol/ROLL_AND_CHECK_PROTOCOL.md`
- `01_runner_protocol/COMBAT_PROTOCOL.md`
- `01_runner_protocol/SOCIAL_SCENE_PROTOCOL.md`
- `01_runner_protocol/EXPLORATION_PROTOCOL.md`
- `01_runner_protocol/TRAVEL_PROTOCOL.md`
- `01_runner_protocol/DOWNTIME_PROTOCOL.md`
- `01_runner_protocol/CLUE_DELIVERY_PROTOCOL.md`
- `01_runner_protocol/SECRET_REVEAL_PROTOCOL.md`
- `01_runner_protocol/FAILURE_AND_CONSEQUENCES.md`
- `01_runner_protocol/TONE_AND_NARRATION.md`
- `01_runner_protocol/WHEN_TO_ASK_QUESTIONS.md`
- `01_runner_protocol/WHEN_TO_IMPROVISE.md`
- `01_runner_protocol/SESSION_END_PROTOCOL.md`
- `16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md`
- `16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md`
- `16_ai_session_packs/RESUME_CAMPAIGN_PROMPT.md`
- `16_ai_session_packs/OPENING_SCENES.md`
- `16_ai_session_packs/SOLO_SAFETY_START.md`

---

## Level Tags

### level:1-4
- `05_regions/SUNDERING_REACH.md`
- `06_settlements/HOLLOWMERE.md`
- `09_quests/HOOKS_TABLE.md`
- `09_quests/RUMORS_TABLE.md`
- `16_ai_session_packs/OPENING_SCENES.md`
- `16_ai_session_packs/SOLO_SAFETY_START.md`
- `12_campaign_arc/ACT_1_LEVELS_1_4.md`
- `12_campaign_arc/ACT_1_MILESTONES.md`
- `12_campaign_arc/ACT_1_FAILURE_STATES.md`
- `09_quests/act_1_quests/` (6 faction quests)
- `13_encounters_and_bestiary/ACT_1_THREATS.md`
- `11_mysteries_and_secrets/ACT_1_CLUE_TRAILS.md`
- `08_npcs/ACT_1_NPC_GUIDE.md`

### act:1 (Stage 5 — Level 1–4 Play Arc)
- `12_campaign_arc/ACT_1_LEVELS_1_4.md` — arc spine (mixed)
- `12_campaign_arc/ACT_1_MILESTONES.md` — level-up triggers (mixed)
- `12_campaign_arc/ACT_1_FAILURE_STATES.md` — failure redirects (mixed)
- `09_quests/act_1_quests/` — 6 faction-alignment quests (mixed)
- `13_encounters_and_bestiary/ACT_1_THREATS.md` — recurring early threats (mixed)
- `11_mysteries_and_secrets/ACT_1_CLUE_TRAILS.md` — L1–4 clue access overlay (dm-only)
- `08_npcs/ACT_1_NPC_GUIDE.md` — Act 1 NPC casting guide (mixed)

### level:5-8
- `07_factions/major_factions/CONCORD_REMNANT.md` (rises Act 2–3)

### level:9-12
- `07_factions/major_factions/HOLLOW_COURT.md` (apex; surfaces Act 3–4)

### level:13-16
- `07_factions/major_factions/HOLLOW_COURT.md`

### level:17-20
- `12_campaign_arc/MAIN_ARC_OVERVIEW.md` (endgame branches)

---

## Play Function Tags

### function:quest-hook
- `09_quests/HOOKS_TABLE.md`
- `07_factions/major_factions/REACHWARD_COMPACT.md`

### function:main-arc
- `12_campaign_arc/MAIN_ARC_OVERVIEW.md`
- `12_campaign_arc/LEVEL_1_TO_20_PROGRESSION.md`
- `07_factions/major_factions/HOLLOW_COURT.md`

### function:faction-clock
- `02_runtime_state/WORLD_CLOCKS.md`
- `07_factions/major_factions/ASHEN_WARDENS.md`
- `07_factions/major_factions/CINDER_LEDGER.md`
- `07_factions/major_factions/MOURNERS_CIRCLE.md`
- `07_factions/major_factions/REACHWARD_COMPACT.md`
- `07_factions/major_factions/GRAVECALLERS.md`
- `07_factions/major_factions/CONCORD_REMNANT.md`
- `07_factions/major_factions/HOLLOW_COURT.md`

### function:clue
- `11_mysteries_and_secrets/MYSTERY_WEB.md`
- `11_mysteries_and_secrets/CLUE_INDEX.md`
- `07_factions/major_factions/GRAVECALLERS.md`
- `07_factions/major_factions/CONCORD_REMNANT.md`
- `06_settlements/caradril_districts/THE_COUNTING_QUAYS.md`, `THE_LANTERN_REACH.md`, `THE_ASHMARKET.md`, `THE_CRUCIBLE.md`, `HIGHMOURN.md`, `THE_SUNKEN_WARDS.md`
- `09_quests/city_quests/Q_THE_SEALED_ARCHIVE.md`, `Q_THE_QUAY_CHARTER.md`, `Q_QUIET_COIN.md`, `Q_THE_SMELTING.md`, `Q_THE_FUNERAL_THAT_WOULDNT_TAKE.md`, `Q_BELOW_THE_STILLING.md`

### tag:district / tag:major-city / tag:city-faction (Stage 4)
- `district`: the 8 files in `06_settlements/caradril_districts/`
- `major-city`: `06_settlements/CARADRIL.md`
- `city-faction`: Tidewater Council, Tide-Watch, Salt Syndicate, the Hush (defined in the Caradril district files; indexed in `07_factions/FACTION_INDEX.md`)

### function:rumor
- `09_quests/RUMORS_TABLE.md`

### function:combat
- `01_runner_protocol/COMBAT_PROTOCOL.md`

### function:travel
- `01_runner_protocol/TRAVEL_PROTOCOL.md`

### function:exploration
- `01_runner_protocol/EXPLORATION_PROTOCOL.md`

### function:downtime
- `01_runner_protocol/DOWNTIME_PROTOCOL.md`

### function:solo-safety
- `01_runner_protocol/SOLO_PLAY_PRINCIPLES.md`
- `01_runner_protocol/COMBAT_PROTOCOL.md`
- `01_runner_protocol/FAILURE_AND_CONSEQUENCES.md`
- `16_ai_session_packs/SOLO_SAFETY_START.md`
- `07_factions/major_factions/ASHEN_WARDENS.md`
- `06_settlements/THE_ASHWALK_REST.md`
- `13_encounters_and_bestiary/SUNDERING_REACH_ENCOUNTERS.md`
- `06_settlements/caradril_districts/HIGHMOURN.md` (city healing/rest hub)
- `13_encounters_and_bestiary/CARADRIL_ENCOUNTERS.md` (social-default city; solo-safety pillars)

### function:social
- `01_runner_protocol/SOCIAL_SCENE_PROTOCOL.md`
- `06_settlements/caradril_districts/THE_MAGISTERIUM.md`, `THE_SILL.md` (city intrigue)
- `13_encounters_and_bestiary/CARADRIL_ENCOUNTERS.md`
- `09_quests/city_quests/Q_THE_OPEN_CHARTER.md`, `Q_THE_TIDE_TURNS.md`, `Q_THE_BELLMANS_PRICE.md`

### function:boss
- `07_factions/major_factions/HOLLOW_COURT.md`
- `08_npcs/MAJOR_NPCS.md` (Veyl, Quorrin Vane)

### function:companion
- `16_ai_session_packs/SOLO_SAFETY_START.md` (Brother Hale)
- `08_npcs/MAJOR_NPCS.md`

### function:patron
- `07_factions/major_factions/ASHEN_WARDENS.md`
- `07_factions/major_factions/CINDER_LEDGER.md`
- `07_factions/major_factions/REACHWARD_COMPACT.md`
- `06_settlements/caradril_districts/THE_COUNTING_QUAYS.md` (Ledger HQ patron)
- `06_settlements/caradril_districts/THE_MAGISTERIUM.md` (council/Kade patrons)

### function:secret
- `03_canon/DM_ONLY_CANON.md`
- `03_canon/CAMPAIGN_IDENTITY_LOCK.md`
- `07_factions/major_factions/HOLLOW_COURT.md`
- `11_mysteries_and_secrets/SECRET_INDEX.md`
- `11_mysteries_and_secrets/MYSTERY_WEB.md`
- `11_mysteries_and_secrets/REVELATION_MAP.md`
- `02_runtime_state/HIDDEN_CLUES.md`

---

## Region Tags

### region:sundering-reach
- `05_regions/SUNDERING_REACH.md`
- `05_regions/wilderness/` (4 zone files)
- `06_settlements/` (8 settlements: Hollowmere, Kettle Bridge, Saltmargin, Candlewick, Greywater Holm, Harrowgast, Reedford, The Ashwalk Rest)
- `08_npcs/SECONDARY_NPCS.md`, `08_npcs/MINOR_NPCS.md`
- `09_quests/HOOKS_TABLE.md`, `09_quests/RUMORS_TABLE.md`
- `09_quests/hooks_and_rumors/` (regional hooks + rumors)
- `09_quests/regional_quests/` (14 developed quests)
- `09_quests/act_1_quests/` (6 Act 1 faction quests — Stage 5)
- `10_dungeons_and_ruins/` (6 dungeons/ruins)
- `13_encounters_and_bestiary/SUNDERING_REACH_ENCOUNTERS.md`, `ACT_1_THREATS.md` (Stage 5)
- `12_campaign_arc/ACT_1_LEVELS_1_4.md`, `ACT_1_MILESTONES.md`, `ACT_1_FAILURE_STATES.md` (Stage 5)
- `11_mysteries_and_secrets/ACT_1_CLUE_TRAILS.md`, `08_npcs/ACT_1_NPC_GUIDE.md` (Stage 5)
- `16_ai_session_packs/OPENING_SCENES.md`
- All seven major faction files (present in the Reach)

### region:caradril
- `06_settlements/CARADRIL.md`
- `06_settlements/caradril_districts/` (8 district files: Magisterium, Counting-Quays, Lantern Reach, Ashmarket, Highmourn, Crucible, Sill, Sunken Wards)
- `08_npcs/SECONDARY_NPCS.md` (Caradril section — 15 city NPCs), `08_npcs/MINOR_NPCS.md` (Caradril section — 25 city NPCs)
- `09_quests/city_quests/` (11 developed city quests)
- `09_quests/hooks_and_rumors/CARADRIL_HOOKS.md`, `CARADRIL_RUMORS.md`
- `13_encounters_and_bestiary/CARADRIL_ENCOUNTERS.md`
- Cinder Ledger + Concord Remnant faction files (HQ/seat in Caradril); city-internal factions listed in `07_factions/FACTION_INDEX.md`

### region:ashgarden-vale (Stage 7 — Ring 1, South)
- `05_regions/ASHGARDEN_VALE.md`
- `05_regions/wilderness/ASHGARDEN_VALE_SITES.md`
- `06_settlements/ORCHARDMERE.md`, `SAINT_VEDDOWS_REST.md`, `TILBROOK.md`
- `10_dungeons_and_ruins/SAINT_VEDDOWS_TOMB.md`, `THE_BURIED_CLOISTER.md`, `THE_PELLOW_GRANGE.md`
- `13_encounters_and_bestiary/ASHGARDEN_VALE_ENCOUNTERS.md`
- `09_quests/hooks_and_rumors/ASHGARDEN_VALE_HOOKS.md`, `ASHGARDEN_VALE_RUMORS.md`; 8 Vale `Q_*` quests
- `08_npcs/SECONDARY_NPCS.md` + `MINOR_NPCS.md` (Vale sections)

### region:tollwood (Stage 7 — Ring 1, East)
- `05_regions/TOLLWOOD.md`
- `05_regions/wilderness/TOLLWOOD_SITES.md`
- `06_settlements/HARTFELL.md`, `COLDHEARTH.md`, `TOLLSTONE_CROSS.md`
- `10_dungeons_and_ruins/THE_GREENWARD_TOLL_STATION.md`, `THE_HANGING_OAKS.md`, `THE_OLD_MAST.md` (gated)
- `13_encounters_and_bestiary/TOLLWOOD_ENCOUNTERS.md`
- `09_quests/hooks_and_rumors/TOLLWOOD_HOOKS.md`, `TOLLWOOD_RUMORS.md`; 7 Tollwood `Q_*` quests
- `08_npcs/SECONDARY_NPCS.md` + `MINOR_NPCS.md` (Tollwood sections); the Tollmen (regional faction)

### region:pale-coast (Stage 7 — Ring 1, West)
- `05_regions/PALE_COAST.md`
- `05_regions/wilderness/PALE_COAST_SITES.md`
- `06_settlements/WRACKMOUTH.md`, `COBBLE_STRAND.md` (Saltmargin reused as gateway)
- `10_dungeons_and_ruins/THE_DROWNED_LAMP.md`, `THE_WRECKERS_CAVES.md`, `THE_SKERRY_SHRINE.md` (gated)
- `13_encounters_and_bestiary/PALE_COAST_ENCOUNTERS.md`
- `09_quests/hooks_and_rumors/PALE_COAST_HOOKS.md`, `PALE_COAST_RUMORS.md`; 5 Coast `Q_*` quests
- `08_npcs/SECONDARY_NPCS.md` + `MINOR_NPCS.md` (Coast sections)

### ring-1 (Stage 7 — all three adjacent regions)
- All `region:ashgarden-vale`, `region:tollwood`, `region:pale-coast` files above
- `04_world_atlas/TRAVEL_ROUTES_RING1.md` (the 6 Ring 1 travel routes)

### region:orrun
- `04_world_atlas/WORLD_OVERVIEW.md`
- `04_world_atlas/MAP_DESCRIPTION.md`

---

## Faction Tags

### faction:ashen-wardens
- `07_factions/major_factions/ASHEN_WARDENS.md`
### faction:cinder-ledger
- `07_factions/major_factions/CINDER_LEDGER.md`
### faction:mourners-circle
- `07_factions/major_factions/MOURNERS_CIRCLE.md`
### faction:reachward-compact
- `07_factions/major_factions/REACHWARD_COMPACT.md`
### faction:gravecallers
- `07_factions/major_factions/GRAVECALLERS.md`
### faction:concord-remnant
- `07_factions/major_factions/CONCORD_REMNANT.md`
### faction:hollow-court
- `07_factions/major_factions/HOLLOW_COURT.md` (dm-only)

---

## Tag Rules

- Add tags consistently across all content files.
- Add new tags to this index whenever a new tag is introduced.
- Prefer useful retrieval tags over excessive tags.
- Keep tag names stable — do not rename tags once in use.
- Use kebab-case for multi-word tag values: `region:silver-coast`, `faction:iron-compact`.
- `status:placeholder` means the file exists with structure but no world content yet.
- `status:complete` means the file is fully written and authoritative (primarily control/standards files).
