# CONTENT_INDEX.md

## Purpose

Global inventory of campaign content. Tells the AI DM what exists and where to find it. Updated after every production pass that creates or materially changes content files.

## Current Status

**Stage 1 complete.** Campaign foundation content indexed below. Regions, settlements, factions, major NPCs, mystery infrastructure, hooks/rumors, and opening packs exist. Deep region/quest/NPC expansion continues in Stages 3+.

---

## How To Use

When the AI DM needs a file, search this index by type, region, faction, level, or tag. Each entry includes file path, secrecy level, and a short summary. Load DM-only files only when running a session — never surface them to the player.

---

## Regions

| Name | File | Secrecy | Status | Summary | Tags |
|---|---|---|---|---|---|
| Sundering Reach | `05_regions/SUNDERING_REACH.md` | mixed | static (frame; deep build Stage 3) | Starting region; ruin-haunted frontier; keystone of the harvest | starting-region |
| (Orrun world overview) | `04_world_atlas/WORLD_OVERVIEW.md` | mixed | static | Continent overview; 5 named regions | world |

---

## Settlements

| Name | File | Region | Secrecy | Status | Summary | Tags |
|---|---|---|---|---|---|---|
| Hollowmere | `06_settlements/HOLLOWMERE.md` | Sundering Reach | mixed | static | Starting town/hub on the drowned basin | starting-settlement, hub |

---

## Factions

| Name | File | Scope | Secrecy | Summary | Tags |
|---|---|---|---|---|---|
| Ashen Wardens | `07_factions/major_factions/ASHEN_WARDENS.md` | Reach/Orrun | mixed | Rite-keepers; unknowing seal-guardians | patron, solo-safety |
| Cinder Ledger | `07_factions/major_factions/CINDER_LEDGER.md` | Orrun | mixed | Merchant-bank; Remembrance monopoly schemer | patron, social |
| Mourners' Circle | `07_factions/major_factions/MOURNERS_CIRCLE.md` | Reach | mixed | Folk grief-faith; moral truth; may break shrines | social, secret |
| Reachward Compact | `07_factions/major_factions/REACHWARD_COMPACT.md` | Reach | mixed | Frontier council; infiltrated; basin scheme | quest-hook, social |
| Gravecallers | `07_factions/major_factions/GRAVECALLERS.md` | Reach | mixed | Outlawed cult; truth-source; catastrophic method | clue, secret |
| Concord Remnant | `07_factions/major_factions/CONCORD_REMNANT.md` | Orrun/Caradril | mixed | Scholars; inner circle would seize the harvest | clue, secret |
| Hollow Court | `07_factions/major_factions/HOLLOW_COURT.md` | Reach (under-shrine) | dm-only | Apex power; surviving Custodians; restarts harvest | boss, main-arc |
| (Faction index) | `07_factions/FACTION_INDEX.md` | — | mixed | Master faction table + relationship map | index |

---

## NPCs

| Name | File | Tier | Location | Faction | Secrecy | Summary | Tags |
|---|---|---|---|---|---|---|---|
| 20 Major NPCs | `08_npcs/MAJOR_NPCS.md` | Major | Reach/Caradril | all | mixed | Full profiles for the 20 foundation NPCs | major-npc |
| (NPC index) | `08_npcs/NPC_INDEX.md` | — | — | — | mixed | Master NPC table | index |

---

## Quests

| Name | File | Type | Level | Region | Status | Summary | Tags |
|---|---|---|---|---|---|---|---|
| First 10 Hooks | `09_quests/HOOKS_TABLE.md` | Hooks | 1-4 | Sundering Reach | static | Session-sized Act 1 hooks (Hook 1 = default opener) | quest-hook, act-1 |
| First 20 Rumors | `09_quests/RUMORS_TABLE.md` | Rumors | 1-4 | Sundering Reach | static | Act 1 rumors, all pointing to authored content | rumor, act-1 |

---

## Mysteries

| Name | File | Secrecy | Status | Summary | Related Clues |
|---|---|---|---|---|---|
| Mystery Web (M0–M10) | `11_mysteries_and_secrets/MYSTERY_WEB.md` | dm-only | static | Full mystery network; 3+ clue paths each | CLUE_INDEX (Stage 3) |
| Revelation Map (R1–R8) | `11_mysteries_and_secrets/REVELATION_MAP.md` | dm-only | static | Act-by-act revelation pacing | — |
| Secret Index (20) | `11_mysteries_and_secrets/SECRET_INDEX.md` | dm-only | static | The 20 major campaign secrets | — |

---

## Clues

| Name | File | Mystery | Discovery Status | Location | Secrecy |
|---|---|---|---|---|---|
| (Clue paths embedded) | `11_mysteries_and_secrets/MYSTERY_WEB.md` | M0–M10 | hidden | various | dm-only |
| (Individual clue files) | `11_mysteries_and_secrets/CLUE_INDEX.md` | — | — | — | dm-only (Stage 3 build-out) |

---

## Dungeons / Ruins

| Name | File | Region | Level | Status | Summary | Tags |
|---|---|---|---|---|---|---|
| Drowned shrine (referenced) | `07_factions/major_factions/HOLLOW_COURT.md` | Sundering Reach | scaling | concept (full build Stage 12) | The harvest keystone / under-shrine | boss, main-arc, dm-only |

---

## Encounter / Bestiary Content

| Name | File | Type | Level | Summary | Tags |
|---|---|---|---|---|---|
| — | — | — | — | Not yet created | — |

---

## Artifacts / Magic Items

| Name | File | Level | Lore Connection | Secrecy |
|---|---|---|---|---|
| — | — | — | Not yet created | — |

---

## Campaign Arc Files

| Name | File | Level Range | Secrecy | Status | Summary |
|---|---|---|---|---|---|
| Main Arc Overview | `12_campaign_arc/MAIN_ARC_OVERVIEW.md` | 1–20 | dm-only | static | Full arc shape, hidden truth, 5 endgame branches, villain escalation |
| Level 1–20 Progression | `12_campaign_arc/LEVEL_1_TO_20_PROGRESSION.md` | 1–20 | dm-only | static | Level-by-level pacing + milestone triggers (Act 1 concrete) |

---

## World Atlas Files

| Name | File | Secrecy | Status | Summary |
|---|---|---|---|---|
| World Overview | `04_world_atlas/WORLD_OVERVIEW.md` | mixed | static | Top-level world description — player-safe overview + DM truth |
| Map Description | `04_world_atlas/MAP_DESCRIPTION.md` | player-safe | static | Written map + travel table for AI DM navigation |

---

## Mystery Infrastructure Files

*These are DM-only structural files, not individual mystery content. Individual mystery files go in the Mysteries table above.*

| Name | File | Secrecy | Status | Purpose |
|---|---|---|---|---|
| Mystery Web | `11_mysteries_and_secrets/MYSTERY_WEB.md` | dm-only | static | M0–M10 network; 3+ clue paths each |
| Revelation Map | `11_mysteries_and_secrets/REVELATION_MAP.md` | dm-only | static | R1–R8 act-by-act revelation pacing |
| Clue Index | `11_mysteries_and_secrets/CLUE_INDEX.md` | dm-only | placeholder | Individual clue files — built out in Stage 3 |
| Secret Index | `11_mysteries_and_secrets/SECRET_INDEX.md` | dm-only | static | The 20 major campaign secrets |

---

## Canon Files

| Name | File | Secrecy | Status | Purpose |
|---|---|---|---|---|
| Canon | `03_canon/CANON.md` | mixed | static | Authoritative world facts — check before adding new facts |
| Player-Safe Canon | `03_canon/PLAYER_SAFE_CANON.md` | player-safe | runtime | Baseline player-safe facts; grows via discovery |
| DM-Only Canon | `03_canon/DM_ONLY_CANON.md` | dm-only | static | Hidden truths — the harvest, Hollow Court, mystery answers |
| Campaign Identity Lock | `03_canon/CAMPAIGN_IDENTITY_LOCK.md` | dm-only | static (LOCKED) | Locked core campaign identity |
| World History | `03_canon/WORLD_HISTORY.md` | mixed | static | Public + true timelines of the Quietfall |
| Cosmology | `03_canon/COSMOLOGY.md` | mixed | static | Afterlife, Remembrance, the Quiet Country |
| Gods and Faiths | `03_canon/GODS_AND_FAITHS.md` | mixed | static | Three Thresholds; Mourners; clergy |
| Magic Rules | `03_canon/MAGIC_RULES.md` | mixed | static | 5e + Remembrance wrinkles (resurrection risk, etc.) |
| Calendar | `03_canon/CALENDAR.md` | player-safe | static | AQ/CR reckoning; months; Greyfall start |
| Languages | `03_canon/LANGUAGES.md` | player-safe | static | Concord Script clue gate; Mourner's Cant; Knock |
| Leveling Assumptions | `03_canon/LEVELING_ASSUMPTIONS.md` | player-safe | static | Milestone leveling; Act 1 triggers |

---

## Runtime State Files

*All files in `/02_runtime_state/`. Load at session start per `RETRIEVAL_GUIDE.md`. Updated at session end.*

| Name | File | Secrecy | Purpose |
|---|---|---|---|
| Current State | `02_runtime_state/CURRENT_STATE.md` | mixed | Single-page campaign snapshot — load first every session |
| Player Character | `02_runtime_state/PLAYER_CHARACTER.md` | player-safe | Full PC stats, resources, conditions |
| Current Location | `02_runtime_state/CURRENT_LOCATION.md` | player-safe | Where the player is and what has changed |
| Current Scene | `02_runtime_state/CURRENT_SCENE.md` | mixed | Immediate scene — has DM-only hidden notes |
| Active Quests | `02_runtime_state/ACTIVE_QUESTS.md` | mixed | All active quests with current status |
| Open Threads | `02_runtime_state/OPEN_THREADS.md` | mixed | Loose ends, dangling hooks, unresolved situations |
| Known Clues | `02_runtime_state/KNOWN_CLUES.md` | player-safe | Clues the player has discovered and understood |
| Hidden Clues | `02_runtime_state/HIDDEN_CLUES.md` | dm-only | Undiscovered clues — DM only, never show player |
| NPC Memory | `02_runtime_state/NPC_MEMORY.md` | mixed | How NPCs remember and feel about the player |
| Faction State | `02_runtime_state/FACTION_STATE.md` | mixed | Current faction attitudes and clock positions |
| World Clocks | `02_runtime_state/WORLD_CLOCKS.md` | mixed | 10 campaign clocks populated (Stage 1); master = The Harvest Restarts |
| Inventory and Rewards | `02_runtime_state/INVENTORY_AND_REWARDS.md` | player-safe | All player possessions, currency, favors |
| Relationships | `02_runtime_state/RELATIONSHIPS.md` | player-safe | Significant long-term relationships |
| Consequences | `02_runtime_state/CONSEQUENCES.md` | mixed | Known and secret consequences of player choices |
| Session Recap | `02_runtime_state/SESSION_RECAP.md` | player-safe | Player-safe summary of each completed session |
| Next Session Start | `02_runtime_state/NEXT_SESSION_START.md` | mixed | Ready-to-use session opening — has DM-only notes |

---

## Runtime / Protocol Files

| Name | File | Purpose | Status |
|---|---|---|---|
| AI DM Core Rules | `01_runner_protocol/AI_DM_CORE_RULES.md` | Core AI DM behavior during play | complete |
| Solo Play Principles | `01_runner_protocol/SOLO_PLAY_PRINCIPLES.md` | Solo-play adjustments — encounter scaling, failure, allies | placeholder |
| Session Loop | `01_runner_protocol/SESSION_LOOP.md` | Standard session start/during/end loop | placeholder |
| Scene Framing | `01_runner_protocol/SCENE_FRAMING.md` | How to open, run, and close scenes | placeholder |
| Player Choice Protocol | `01_runner_protocol/PLAYER_CHOICE_PROTOCOL.md` | How to present choices immersively | placeholder |
| Roll and Check Protocol | `01_runner_protocol/ROLL_AND_CHECK_PROTOCOL.md` | When and how to call for rolls | placeholder |
| Combat Protocol | `01_runner_protocol/COMBAT_PROTOCOL.md` | Solo combat running — enemies, scaling, retreat | placeholder |
| Social Scene Protocol | `01_runner_protocol/SOCIAL_SCENE_PROTOCOL.md` | NPC conversations, negotiations, social encounters | placeholder |
| Exploration Protocol | `01_runner_protocol/EXPLORATION_PROTOCOL.md` | Dungeon and wilderness exploration | placeholder |
| Travel Protocol | `01_runner_protocol/TRAVEL_PROTOCOL.md` | Overland travel, journey pacing, events | placeholder |
| Downtime Protocol | `01_runner_protocol/DOWNTIME_PROTOCOL.md` | Downtime activities and time-passing | placeholder |
| Clue Delivery Protocol | `01_runner_protocol/CLUE_DELIVERY_PROTOCOL.md` | When and how to surface clues | placeholder |
| Secret Reveal Protocol | `01_runner_protocol/SECRET_REVEAL_PROTOCOL.md` | When and how to deliver revelations | placeholder |
| Failure and Consequences | `01_runner_protocol/FAILURE_AND_CONSEQUENCES.md` | What failure costs and how it changes situations | placeholder |
| Tone and Narration | `01_runner_protocol/TONE_AND_NARRATION.md` | Campaign voice, style, and narration standards | placeholder |
| When to Ask Questions | `01_runner_protocol/WHEN_TO_ASK_QUESTIONS.md` | When to ask vs. when to decide and proceed | placeholder |
| When to Improvise | `01_runner_protocol/WHEN_TO_IMPROVISE.md` | What the AI may and must not improvise | placeholder |
| Session End Protocol | `01_runner_protocol/SESSION_END_PROTOCOL.md` | Session closing beat and state update procedure | placeholder |
| Opening Scenes | `16_ai_session_packs/OPENING_SCENES.md` | Three session-1 openers + recommended default | complete |
| Solo Safety Start | `16_ai_session_packs/SOLO_SAFETY_START.md` | Starting solo-play safety mechanism | complete |
| Session End Checklist | `16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md` | End-of-session state update checklist | complete |
| Start New Campaign Prompt | `16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md` | First-session opening prompt for AI DM | placeholder |
| Resume Campaign Prompt | `16_ai_session_packs/RESUME_CAMPAIGN_PROMPT.md` | Standard session-resume prompt | placeholder |
| State Update Template | `16_ai_session_packs/STATE_UPDATE_TEMPLATE.md` | Copy-paste template for session-end state updates | placeholder |
| Compact Context Template | `16_ai_session_packs/COMPACT_CONTEXT_TEMPLATE.md` | Compressed single-doc state summary for long campaigns | placeholder |
| DM Hidden Recap Template | `16_ai_session_packs/DM_HIDDEN_RECAP_TEMPLATE.md` | DM-only post-session hidden consequence log | placeholder |

---

## Control / Standards Files

| Name | File | Purpose |
|---|---|---|
| Manifest | `00_control/MANIFEST.md` | Project identity and folder map |
| Stage Status | `00_control/STAGE_STATUS.md` | Live stage completion tracker |
| Progress Log | `00_control/PROGRESS_LOG.md` | Chronological production history |
| TODO | `00_control/TODO.md` | Prioritized actionable work queue |
| Open Questions | `00_control/OPEN_QUESTIONS.md` | Unresolved design questions |
| Consistency Audit | `00_control/CONSISTENCY_AUDIT.md` | Running tracker of continuity and AI-readiness issues |
| Retrieval Guide | `00_control/RETRIEVAL_GUIDE.md` | AI DM file load order and pre-generation checks |
| Project Rules | `00_control/PROJECT_RULES.md` | Core design philosophy |
| Canon Authority | `00_control/CANON_AUTHORITY.md` | Source-of-truth hierarchy when files disagree |
| Generation Guardrails | `00_control/GENERATION_GUARDRAILS.md` | Drift prevention checklist for major content |
| Naming Registry | `00_control/NAMING_REGISTRY.md` | Master registry of proper nouns — check before naming anything |
| Ruleset Assumptions | `00_control/RULESET_ASSUMPTIONS.md` | D&D 5e / 2024 mechanical baseline assumptions |
| DnD Mechanics Requirements | `00_control/DND_MECHANICS_REQUIREMENTS.md` | Mechanical completeness requirements for all content types |
| Production Workflow | `00_control/PRODUCTION_WORKFLOW.md` | Per-pass workflow loop |
| Development Stages | `00_control/DEVELOPMENT_STAGES.md` | Full stage-by-stage roadmap |
| Tracking System | `00_control/TRACKING_SYSTEM.md` | How to use tracking files |
| Content Standards | `00_control/CONTENT_STANDARDS.md` | File format and metadata standards |
| Worldbuilding Standards | `00_control/WORLDBUILDING_STANDARDS.md` | Standards for world content |
| Faction Standards | `00_control/FACTION_STANDARDS.md` | Standards for faction content |
| NPC Standards | `00_control/NPC_STANDARDS.md` | Standards for NPC content |
| Quest Standards | `00_control/QUEST_STANDARDS.md` | Standards for quest content |
| Mystery Standards | `00_control/MYSTERY_STANDARDS.md` | Standards for mystery content |
| Audit Standards | `00_control/AUDIT_STANDARDS.md` | Standards for audits |

---

## Generation Backlog Files

| Name | File | Purpose |
|---|---|---|
| Content Gaps | `17_generation_backlog/CONTENT_GAPS.md` | Missing or underdeveloped content by category |
| Expansion Plan | `17_generation_backlog/EXPANSION_PLAN.md` | Forward-looking development roadmap |
