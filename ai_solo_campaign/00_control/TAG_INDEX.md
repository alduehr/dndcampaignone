# TAG_INDEX.md

## Purpose

Master index of retrieval tags used across the campaign repository. Makes campaign content searchable by type, secrecy, status, level, region, faction, and play function.

## Current Status

**Stages 1 and 2 complete.** Campaign foundation content registered: starting region/settlement, 7 factions, 20 major NPCs, hooks/rumors, mystery infrastructure, arc files, opening packs, world clocks (Stage 1). All 17 runner protocols and the START/RESUME prompts are now `status:complete`; session-pack templates are `status:template`; 8 runtime state files are seeded at campaign-start baseline (Stage 2). The Stage 2 cleanup pass populated `CLUE_INDEX.md` and `HIDDEN_CLUES.md` (all clues hidden at start) and added D&D mechanical fields to the five content-standards templates. No `status:placeholder` files remain. Deep expansion continues in Stages 3+.

---

## How To Use

When an AI DM or production agent needs to find content of a certain type, search by tag. Each entry lists files that carry that tag.

---

## Type Tags

### type:region
- `05_regions/SUNDERING_REACH.md`
- `04_world_atlas/WORLD_OVERVIEW.md`
- `04_world_atlas/MAP_DESCRIPTION.md`

### type:settlement
- `06_settlements/HOLLOWMERE.md`

### type:npc
- `08_npcs/MAJOR_NPCS.md`
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

### type:mystery
- `11_mysteries_and_secrets/MYSTERY_WEB.md`
- `11_mysteries_and_secrets/REVELATION_MAP.md`
- `11_mysteries_and_secrets/SECRET_INDEX.md`

### type:clue
- `11_mysteries_and_secrets/MYSTERY_WEB.md` (clue paths embedded)
- `11_mysteries_and_secrets/CLUE_INDEX.md` (all authored clues; populated)
- `02_runtime_state/HIDDEN_CLUES.md` (runtime mirror; all hidden at start)

### type:dungeon
- Drowned shrine — referenced in `07_factions/major_factions/HOLLOW_COURT.md` (full build Stage 12)

### type:ruin
- Concord ruins/archive cairns — referenced in `05_regions/SUNDERING_REACH.md` (full build Stage 3/12)

### type:encounter
- *Encounter tables: Stage 13*

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
- `06_settlements/HOLLOWMERE.md`
- `07_factions/major_factions/ASHEN_WARDENS.md`
- `07_factions/major_factions/CINDER_LEDGER.md`
- `07_factions/major_factions/MOURNERS_CIRCLE.md`
- `07_factions/major_factions/REACHWARD_COMPACT.md`
- `07_factions/major_factions/GRAVECALLERS.md`
- `07_factions/major_factions/CONCORD_REMNANT.md`
- `07_factions/major_factions/HOLLOW_COURT.md`
- `07_factions/FACTION_INDEX.md`
- `08_npcs/MAJOR_NPCS.md`
- `08_npcs/NPC_INDEX.md`
- `09_quests/HOOKS_TABLE.md`
- `09_quests/RUMORS_TABLE.md`
- `16_ai_session_packs/OPENING_SCENES.md`
- `16_ai_session_packs/SOLO_SAFETY_START.md`
- `12_campaign_arc/MAIN_ARC_OVERVIEW.md`
- `12_campaign_arc/LEVEL_1_TO_20_PROGRESSION.md`
- `11_mysteries_and_secrets/MYSTERY_WEB.md`
- `11_mysteries_and_secrets/REVELATION_MAP.md`
- `11_mysteries_and_secrets/SECRET_INDEX.md`
- `11_mysteries_and_secrets/CLUE_INDEX.md`

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

### function:rumor
- `09_quests/RUMORS_TABLE.md`

### function:combat
- `01_runner_protocol/COMBAT_PROTOCOL.md`

### function:social
- `01_runner_protocol/SOCIAL_SCENE_PROTOCOL.md`

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
- `06_settlements/HOLLOWMERE.md`
- `09_quests/HOOKS_TABLE.md`
- `09_quests/RUMORS_TABLE.md`
- `16_ai_session_packs/OPENING_SCENES.md`
- All seven major faction files (present in the Reach)

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
