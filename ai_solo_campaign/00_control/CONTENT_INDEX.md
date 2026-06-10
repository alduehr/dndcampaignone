# CONTENT_INDEX.md

## Purpose

Global inventory of campaign content. Tells the AI DM what exists and where to find it. Updated after every production pass that creates or materially changes content files.

## Current Status

**Stages 1, 2, 3, and 4 complete.** Campaign foundation (Stage 1) + AI runtime (Stage 2) + Starting Region Deep Build (Stage 3) + **First Major City Deep Build (Stage 4 — Caradril)**. The Sundering Reach has 8 settlements, 4 wilderness zone-files (~25 sites), 6 dungeons/ruins, and zone encounter tables. **Caradril** now adds: a city overview + 8 district files (incl. the Sunken Wards sub-dungeon), 15 city secondary NPCs + 25 city minor NPCs, 11 developed city quests, 36 city hooks + 30 city rumors, and a city encounter/social-scene table. City clue access feeds the existing M2/M3/M4/M6/M8/M9 chains; 3 city faction clocks (C1/C2/C3) and 4 city-internal factions added. **No new central mystery/faction/god/cosmology/artifact created.** The Act 1 arc (Stage 5) and the first full audit (Stage 6) are next.

---

## How To Use

When the AI DM needs a file, search this index by type, region, faction, level, or tag. Each entry includes file path, secrecy level, and a short summary. Load DM-only files only when running a session — never surface them to the player.

---

## Regions

| Name | File | Secrecy | Status | Summary | Tags |
|---|---|---|---|---|---|
| Sundering Reach | `05_regions/SUNDERING_REACH.md` | mixed | static (deep-built Stage 3) | Starting region; ruin-haunted frontier; keystone of the harvest; 8 settlements, 4 wilderness zones, 6 dungeons | starting-region |
| Caradril (city-state, SE) | `06_settlements/CARADRIL.md` | mixed | static (deep-built Stage 4) | First major city; mid-game hub; 8 districts; Ledger HQ + Remnant seat | major-city, region:caradril |
| (Orrun world overview) | `04_world_atlas/WORLD_OVERVIEW.md` | mixed | static | Continent overview; 5 named regions | world |

---

## Settlements

| Name | File | Region | Secrecy | Status | Summary | Tags |
|---|---|---|---|---|---|---|
| Hollowmere | `06_settlements/HOLLOWMERE.md` | Sundering Reach | mixed | static | Starting town/hub on the drowned basin | starting-settlement, hub |
| Kettle Bridge | `06_settlements/KETTLE_BRIDGE.md` | Sundering Reach | mixed | static | Second town; Mirewend crossing & toll-town (E) | town, travel-hub |
| Saltmargin | `06_settlements/SALTMARGIN.md` | Sundering Reach | mixed | static | Western salt-trade gateway town | town, trade |
| Candlewick | `06_settlements/CANDLEWICK.md` | Sundering Reach | mixed | static | Southern candle/farm village; Concord Script gate | village, clue |
| Greywater Holm | `06_settlements/GREYWATER_HOLM.md` | Sundering Reach | mixed | static | Greyfens-edge village; rites fail worst; cult spread | village, clue |
| Harrowgast | `06_settlements/HARROWGAST.md` | Sundering Reach | mixed | static | Heights mining ruin-town (Lvl 2–5); Deep Adit | mining-village, exploration |
| Reedford | `06_settlements/REEDFORD.md` | Sundering Reach | mixed | static | Tiny ford-hamlet; gentle Lvl-1 waypoint | hamlet |
| The Ashwalk Rest | `06_settlements/THE_ASHWALK_REST.md` | Sundering Reach | mixed | static | Warden waystation; open-Reach solo-safety sanctuary | outpost, solo-safety, patron |
| **Caradril** | `06_settlements/CARADRIL.md` | Caradril (Orrun, SE) | mixed | static | **First major city**; city-state; Ledger HQ + Remnant seat; mid-game hub (Lvl 5–12); 8 districts | major-city, hub |

### Caradril Districts (Stage 4)

| District | File | Power Bloc | Secrecy | Summary | Tags |
|---|---|---|---|---|---|
| The Magisterium | `06_settlements/caradril_districts/THE_MAGISTERIUM.md` | Tidewater Council | mixed | Government quarter; charter politics; correspondent thread | district, social |
| The Counting-Quays | `06_settlements/caradril_districts/THE_COUNTING_QUAYS.md` | Cinder Ledger | mixed | Banking/harbor; Ledger Keep; Vyre–Quorrin deal (M3/M6) | district, clue, patron |
| The Lantern Reach | `06_settlements/caradril_districts/THE_LANTERN_REACH.md` | Concord Remnant | mixed | Scholars; Concord Script gate; Sealed Archive (M6/M9) | district, clue, secret |
| The Ashmarket | `06_settlements/caradril_districts/THE_ASHMARKET.md` | Salt Syndicate | mixed | Relic/salvage trade; quiet-coin (M3) | district, clue |
| Highmourn | `06_settlements/caradril_districts/HIGHMOURN.md` | clergy/Mourners | mixed | Temples/cemetery; raise-dead cover-up (Secret 7); solo-safety | district, clue, solo-safety |
| The Crucible | `06_settlements/caradril_districts/THE_CRUCIBLE.md` | Craft guilds | mixed | Foundries; relic-smelting (M3); gear commerce | district, clue |
| The Sill | `06_settlements/caradril_districts/THE_SILL.md` | The Hush | mixed | Poor undercity; refugees (M10); the Bellman; Sealgate | district, social, clue |
| The Sunken Wards | `06_settlements/caradril_districts/THE_SUNKEN_WARDS.md` | (delvers/Remnant) | mixed | Flooded sub-dungeon; M2/M3 cousin-site; Lvl 6–14 | district, ruin, exploration |

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
| Tidewater Council / Charter Houses | `06_settlements/caradril_districts/THE_MAGISTERIUM.md` | Caradril | mixed | City-internal: merchant government; complacent | city-faction, social |
| Tide-Watch | `06_settlements/caradril_districts/THE_MAGISTERIUM.md` | Caradril | mixed | City-internal: city watch (turnable captain) | city-faction |
| Salt Syndicate | `06_settlements/caradril_districts/THE_ASHMARKET.md` | Caradril | mixed | City-internal: smuggling + relic black market (M3) | city-faction, clue |
| The Hush | `06_settlements/caradril_districts/THE_SILL.md` | Caradril | mixed | City-internal: information/blackmail; clue-shortcuts | city-faction, clue |
| (Faction index) | `07_factions/FACTION_INDEX.md` | — | mixed | Master faction table + relationship map (incl. city factions) | index |

---

## NPCs

| Name | File | Tier | Location | Faction | Secrecy | Summary | Tags |
|---|---|---|---|---|---|---|---|
| 20 Major NPCs | `08_npcs/MAJOR_NPCS.md` | Major | Reach/Caradril | all | mixed | Full profiles for the 20 foundation NPCs | major-npc |
| ~36 Secondary NPCs | `08_npcs/SECONDARY_NPCS.md` | Secondary | Reach + Caradril | all | mixed | Stage 3 Reach locals + Stage 4 15 Caradril city NPCs | secondary-npc |
| ~60 Minor NPCs | `08_npcs/MINOR_NPCS.md` | Minor | Reach + Caradril | all | mixed | Stage 3 Reach + Stage 4 25 Caradril minor NPCs by district | minor-npc |
| (NPC index) | `08_npcs/NPC_INDEX.md` | — | — | — | mixed | Master NPC table (major/secondary/minor; Reach + Caradril) | index |

---

## Quests

| Name | File | Type | Level | Region | Status | Summary | Tags |
|---|---|---|---|---|---|---|---|
| First 10 Hooks | `09_quests/HOOKS_TABLE.md` | Hooks | 1-4 | Sundering Reach | static | Session-sized Act 1 hooks (Hook 1 = default opener) | quest-hook, act-1 |
| First 20 Rumors | `09_quests/RUMORS_TABLE.md` | Rumors | 1-4 | Sundering Reach | static | Act 1 rumors, all pointing to authored content | rumor, act-1 |
| Regional Hooks (H11–H39) | `09_quests/hooks_and_rumors/SUNDERING_REACH_HOOKS.md` | Hooks | 1-5 | Sundering Reach | static | 29 more hooks by area (39 total) | quest-hook |
| Regional Rumors (R21–R50) | `09_quests/hooks_and_rumors/SUNDERING_REACH_RUMORS.md` | Rumors | 1-5 | Sundering Reach | static | 30 more rumors by area (50 total) | rumor |
| 14 Developed Quests | `09_quests/regional_quests/*.md` | Regional/Faction/Mystery | 1-5 | Sundering Reach | static | Full-standard quests (Salt Run, Broken Arch, Light on the Scale, Holm That Won't Bury Its Dead, Sold Stone, Race North, Bailiff's Ladder, Reed Holms, Sashe's Warning, Grey Woman, Second Mark, Pell's Doubt, Scholar's Request, Failing Funeral) | quest |
| Caradril Hooks (CH1–36) | `09_quests/hooks_and_rumors/CARADRIL_HOOKS.md` | Hooks | 3-12 | Caradril | static | 36 city hooks by district, all pointing to authored content | quest-hook, region:caradril |
| Caradril Rumors (CR1–30) | `09_quests/hooks_and_rumors/CARADRIL_RUMORS.md` | Rumors | 3-12 | Caradril | static | 30 city rumors by district | rumor, region:caradril |
| 11 Developed City Quests | `09_quests/city_quests/*.md` | City/Faction/Mystery | 3-12 | Caradril | static | Full-standard city quests (Sealed Letter, Open Charter, Quay Charter, Lantern & Lamp, Sealed Archive, Quiet Coin, Funeral That Wouldn't Take, Smelting, Bellman's Price, Below the Stilling, Tide Turns) | quest, region:caradril |

---

## Mysteries

| Name | File | Secrecy | Status | Summary | Related Clues |
|---|---|---|---|---|---|
| Mystery Web (M0–M10) | `11_mysteries_and_secrets/MYSTERY_WEB.md` | dm-only | static | Full mystery network; 3+ clue paths each | CLUE_INDEX (populated) |
| Revelation Map (R1–R8) | `11_mysteries_and_secrets/REVELATION_MAP.md` | dm-only | static | Act-by-act revelation pacing | — |
| Secret Index (20) | `11_mysteries_and_secrets/SECRET_INDEX.md` | dm-only | static | The 20 major campaign secrets | — |

---

## Clues

| Name | File | Mystery | Discovery Status | Location | Secrecy |
|---|---|---|---|---|---|
| (Clue paths embedded) | `11_mysteries_and_secrets/MYSTERY_WEB.md` | M0–M10 | hidden | various | dm-only |
| Clue Index (all authored clues) | `11_mysteries_and_secrets/CLUE_INDEX.md` | M0–M10 | hidden | various | dm-only — populated; clue IDs + methods + three-clue check |

---

## Wilderness Locations

| Name | File | Region | Level | Status | Summary | Tags |
|---|---|---|---|---|---|---|
| Greyfens sites | `05_regions/wilderness/GREYFENS_SITES.md` | Sundering Reach | 2-5 | static | 6 named fen sites; M5 drift, Gravecaller cell | greyfens, clue |
| Sunder Heights sites | `05_regions/wilderness/SUNDER_HEIGHTS_SITES.md` | Sundering Reach | 2-6 | static | 6 named highland-ruin sites; Reclamation race | sunder-heights |
| Mirewend & Roads sites | `05_regions/wilderness/MIREWEND_AND_ROADS_SITES.md` | Sundering Reach | 1-4 | static | Star-Stones, causeways, river; travel layer | roads, river, travel |
| Basin Shore & Holms sites | `05_regions/wilderness/BASIN_SHORE_AND_HOLMS_SITES.md` | Sundering Reach | 1-5 | static | Shore, Surfacing Ruin (M2), Reed Holms; deep basin off-limits early | basin, clue |

---

## Dungeons / Ruins

| Name | File | Region | Level | Status | Summary | Tags |
|---|---|---|---|---|---|---|
| The Peat Chapel | `10_dungeons_and_ruins/THE_PEAT_CHAPEL.md` | Sundering Reach | 1-2 | static | First-delve fen chapel; Remembrance relic (M3) | ruin, level:1-2 |
| The Sunken Tollhouse | `10_dungeons_and_ruins/THE_SUNKEN_TOLLHOUSE.md` | Sundering Reach | 2-3 | static | Drowned river node under Kettle Bridge (M2/M5) | dungeon, clue |
| The Whispering Cairn | `10_dungeons_and_ruins/THE_WHISPERING_CAIRN.md` | Sundering Reach | 1-3 | static | Archive-cairn; Concord Script gate (M6/M9) | ruin, clue |
| The Ledger Vault | `10_dungeons_and_ruins/THE_LEDGER_VAULT.md` | Sundering Reach | 2-4 | static | Social/stealth heist; vault relic (C-M3-3) | dungeon, heist |
| The Barrow of Nine Doors | `10_dungeons_and_ruins/THE_BARROW_OF_NINE_DOORS.md` | Sundering Reach | 3-5 | static | Greyfens barrow; parley-boss; M5/M6 testimony | dungeon, clue |
| The Deep Adit | `10_dungeons_and_ruins/THE_DEEP_ADIT.md` | Sundering Reach | 3-5 | static | Secondary harvest node; M3/M6; Reclamation race | dungeon, clue, secondary-node |
| Drowned shrine (referenced) | `07_factions/major_factions/HOLLOW_COURT.md` | Sundering Reach | scaling | concept (full build Stage 12) | The harvest keystone / under-shrine | boss, main-arc, dm-only |

---

## Encounter / Bestiary Content

| Name | File | Type | Level | Summary | Tags |
|---|---|---|---|---|---|
| Sundering Reach encounters | `13_encounters_and_bestiary/SUNDERING_REACH_ENCOUNTERS.md` | Encounter tables | 1-6 | Four solo-tuned zone tables (Roads/River, Greyfens, Heights, Basin); stat-referenced, non-combat-default | encounter, solo-safety |
| Caradril encounters | `13_encounters_and_bestiary/CARADRIL_ENCOUNTERS.md` | Encounter/social-scene tables | 3-14 | Eight district social/intrigue tables + Sunken Wards dungeon table; social-default, stat-referenced | encounter, social, solo-safety, region:caradril |

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
| Clue Index | `11_mysteries_and_secrets/CLUE_INDEX.md` | dm-only | static | All authored clues with IDs, mystery, discovery method, status (all hidden at start) |
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
| Current State | `02_runtime_state/CURRENT_STATE.md` | mixed | Single-page campaign snapshot — load first every session (seeded: campaign-start baseline) |
| Player Character | `02_runtime_state/PLAYER_CHARACTER.md` | player-safe | Full PC stats, resources, conditions (scaffold: awaiting character creation) |
| Current Location | `02_runtime_state/CURRENT_LOCATION.md` | player-safe | Where the player is and what has changed (seeded: Hollowmere) |
| Current Scene | `02_runtime_state/CURRENT_SCENE.md` | mixed | Immediate scene — has DM-only hidden notes (seeded: opening scene) |
| Active Quests | `02_runtime_state/ACTIVE_QUESTS.md` | mixed | All active quests with current status (seeded: Hook 1 + Hooks 5–7 available) |
| Open Threads | `02_runtime_state/OPEN_THREADS.md` | mixed | Loose ends, dangling hooks, unresolved situations (seeded: 5 opening threads) |
| Known Clues | `02_runtime_state/KNOWN_CLUES.md` | player-safe | Clues the player has discovered and understood |
| Hidden Clues | `02_runtime_state/HIDDEN_CLUES.md` | dm-only | Undiscovered clues — DM only, never show player (seeded: all clues hidden at campaign start) |
| NPC Memory | `02_runtime_state/NPC_MEMORY.md` | mixed | How NPCs remember and feel about the player |
| Faction State | `02_runtime_state/FACTION_STATE.md` | mixed | Current faction attitudes and clock positions (seeded: 7 factions at Stage 1 baseline) |
| World Clocks | `02_runtime_state/WORLD_CLOCKS.md` | mixed | 10 campaign clocks populated (Stage 1); master = The Harvest Restarts |
| Inventory and Rewards | `02_runtime_state/INVENTORY_AND_REWARDS.md` | player-safe | All player possessions, currency, favors |
| Relationships | `02_runtime_state/RELATIONSHIPS.md` | player-safe | Significant long-term relationships |
| Consequences | `02_runtime_state/CONSEQUENCES.md` | mixed | Known and secret consequences of player choices |
| Session Recap | `02_runtime_state/SESSION_RECAP.md` | player-safe | Player-safe summary of each completed session |
| Next Session Start | `02_runtime_state/NEXT_SESSION_START.md` | mixed | Ready-to-use session opening — has DM-only notes (seeded: Session-1 opener) |

---

## Runtime / Protocol Files

| Name | File | Purpose | Status |
|---|---|---|---|
| AI DM Core Rules | `01_runner_protocol/AI_DM_CORE_RULES.md` | Core AI DM behavior during play | complete |
| Solo Play Principles | `01_runner_protocol/SOLO_PLAY_PRINCIPLES.md` | Solo-play adjustments — encounter scaling, failure, allies | complete |
| Session Loop | `01_runner_protocol/SESSION_LOOP.md` | Standard session start/during/end loop | complete |
| Scene Framing | `01_runner_protocol/SCENE_FRAMING.md` | How to open, run, and close scenes | complete |
| Player Choice Protocol | `01_runner_protocol/PLAYER_CHOICE_PROTOCOL.md` | How to present choices immersively | complete |
| Roll and Check Protocol | `01_runner_protocol/ROLL_AND_CHECK_PROTOCOL.md` | When and how to call for rolls | complete |
| Combat Protocol | `01_runner_protocol/COMBAT_PROTOCOL.md` | Solo combat running — enemies, scaling, retreat | complete |
| Social Scene Protocol | `01_runner_protocol/SOCIAL_SCENE_PROTOCOL.md` | NPC conversations, negotiations, social encounters | complete |
| Exploration Protocol | `01_runner_protocol/EXPLORATION_PROTOCOL.md` | Dungeon and wilderness exploration | complete |
| Travel Protocol | `01_runner_protocol/TRAVEL_PROTOCOL.md` | Overland travel, journey pacing, events | complete |
| Downtime Protocol | `01_runner_protocol/DOWNTIME_PROTOCOL.md` | Downtime activities and time-passing | complete |
| Clue Delivery Protocol | `01_runner_protocol/CLUE_DELIVERY_PROTOCOL.md` | When and how to surface clues (three-clue rule) | complete |
| Secret Reveal Protocol | `01_runner_protocol/SECRET_REVEAL_PROTOCOL.md` | When and how to deliver revelations | complete |
| Failure and Consequences | `01_runner_protocol/FAILURE_AND_CONSEQUENCES.md` | What failure costs and how it changes situations | complete |
| Tone and Narration | `01_runner_protocol/TONE_AND_NARRATION.md` | Campaign voice, style, and narration standards | complete |
| When to Ask Questions | `01_runner_protocol/WHEN_TO_ASK_QUESTIONS.md` | When to ask vs. when to decide and proceed | complete |
| When to Improvise | `01_runner_protocol/WHEN_TO_IMPROVISE.md` | What the AI may and must not improvise | complete |
| Session End Protocol | `01_runner_protocol/SESSION_END_PROTOCOL.md` | Session closing beat and state update procedure | complete |
| Opening Scenes | `16_ai_session_packs/OPENING_SCENES.md` | Three session-1 openers + recommended default | complete |
| Solo Safety Start | `16_ai_session_packs/SOLO_SAFETY_START.md` | Starting solo-play safety mechanism | complete |
| Session End Checklist | `16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md` | End-of-session state update checklist | complete |
| Start New Campaign Prompt | `16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md` | First-session opening prompt for AI DM (DM-only) | complete |
| Resume Campaign Prompt | `16_ai_session_packs/RESUME_CAMPAIGN_PROMPT.md` | Standard session-resume prompt (DM-only) | complete |
| State Update Template | `16_ai_session_packs/STATE_UPDATE_TEMPLATE.md` | Copy-paste template for session-end state updates | ready (template) |
| Compact Context Template | `16_ai_session_packs/COMPACT_CONTEXT_TEMPLATE.md` | Compressed single-doc state summary for long campaigns | ready (template) |
| DM Hidden Recap Template | `16_ai_session_packs/DM_HIDDEN_RECAP_TEMPLATE.md` | DM-only post-session hidden consequence log | ready (template) |

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
