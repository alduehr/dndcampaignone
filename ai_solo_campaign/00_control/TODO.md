# TODO.md

## Purpose

Prioritized, actionable work queue. When no specific task is given, use this file to determine what to do next.

---

## Critical

*None open.*

## High

- [ ] Begin Stage 12: Dungeons, Ruins, and Adventure Sites
  - Why it matters: **Stage 11 (Mystery/Secret/Clue Expansion) is complete** — Stage 12 is next per `DEVELOPMENT_STAGES.md`. The keystone drowned-shrine / Under-Shrine dungeon and the Caradril deep-dungeon treatment were deferred to Stage 12 by design; existing dungeons should also be cross-linked to the new region-coded clue layer (`C_SR_*`/`C_CAR_*`) and REV IDs.
  - Related files: `10_dungeons_and_ruins/`, `11_mysteries_and_secrets/by_region/*_CLUES.md`, `04_world_atlas/WORLD_MAP_LAYERS.md` (Under-Shrine, DM-only)
  - Suggested agent: `world-atlas-builder` / `encounter-bestiary-designer`
  - Stage: 12
  - Blocker: none — Stage 11 complete.

- [x] (Stage 11 follow-up) Mirror region-coded clue IDs into runtime `HIDDEN_CLUES.md` — done 2026-06-13 (Stage 11 cleanup pass); Stage 11 anchor section added to `02_runtime_state/HIDDEN_CLUES.md`.

- [ ] (Recommended, low-priority polish) Lift exact quest titles for Glassmere/Hollow Gulf/Emberfell/Hethewald/Sallowmarch into `DEVELOPED_QUESTS_INDEX.md`
  - Why it matters: those region files' quest blocks were authored by the prior Stage 10 run; the index currently summarizes their titles descriptively. A quick read-and-fill pass would tidy the index. Non-blocking.
  - Related files: `09_quests/by_region/{GLASSMERE_LEAGUE,HOLLOW_GULF_PORTS,EMBERFELL_THEOCRACY,HETHEWALD_FREE_HOLDS,SALLOWMARCH_PROTECTORATE}_QUESTS.md`, `09_quests/DEVELOPED_QUESTS_INDEX.md`
  - Suggested agent: `indexer-librarian`
  - Stage: 10 (follow-up)

## Completed Recently

- [x] Stage 11 cleanup pass — 2026-06-13. Created 4 required wrapper files (MYSTERY_CHAINS, FALSE_LEADS, REVEAL_TIMING, PROPHECIES_AND_OMENS); mirrored region-coded clue IDs into HIDDEN_CLUES.md; updated CONTENT_INDEX, TAG_INDEX, NAMING_REGISTRY, CONTENT_GAPS, EXPANSION_PLAN, CONSISTENCY_AUDIT, OPEN_QUESTIONS, PROGRESS_LOG.
- [x] Stage 11: Mystery, Secret, and Clue Expansion — 2026-06-13. Added a formal **REVELATION_MAP** layer (REV_001–REV_010, each with >=3 independent clue sources spanning different regions/NPCs/approaches; dependency graph; phase gates; legacy R1–R8/M0–M10 mapped); expanded **CLUE_INDEX** with a region-coded clue layer (C_SR_/C_CAR_/C_AV_/C_TW_/C_PC_/C_FC_) + per-REV three-source verification; added a 7-layer **mystery hierarchy** + far-continent echo cross-reference to **MYSTERY_WEB**. New files: 6 regional clue trails (`11_mysteries_and_secrets/by_region/{SUNDERING_REACH,CARADRIL,ASHGARDEN_VALE,TOLLWOOD,PALE_COAST}_CLUES.md` + `FAR_CONTINENT_ECHO_CLUES.md`), `by_faction/FACTION_KNOWLEDGE_MAP.md` (all 7 factions; Hollow Court apex-DM-only), `NPC_KNOWLEDGE_MAP.md` (~60 NPCs), `FALSE_LEADS_AND_MISDIRECTIONS.md` (9 fair leads), `DISCOVERY_PATHS.md` (10 playstyles), `SECRET_PROTECTION_MATRIX.md` (DM-only; 7 apex secrets, safe/unsafe wording + gates), `MYSTERY_STATE_TRACKER_TEMPLATE.md` (blank runtime tracker). Cross-linked Stage 10 major quests to REV/clue IDs. Secrecy audit `18_audits/STAGE_11_MYSTERY_SECRECY_AUDIT.md`: 0 Critical / 0 High / 2 Medium / 3 Low — no apex-truth leaks in player-safe text; all 16 mystery files dm-only; every REV solvable via multiple paths. M0–M10 preserved; no new central mystery/faction/god/cosmology/artifact; Hollow Court protection strengthened. Updated SECRET_INDEX, STAGE_STATUS, CONTENT_INDEX, STAGE_11_PROGRESS.
- [x] Stage 10: Quest Library Expansion — 2026-06-12. **28 major campaign quests** (`09_quests/MAJOR_CAMPAIGN_QUESTS.md`, Q_MAJOR_001–028) + **82 far-continent developed quests** across all 12 regions (`09_quests/by_region/*_QUESTS.md`; 82 unique IDs, no collisions) → **~165 developed quests** total (~83 pre-Stage-10 + 82). **304 far-continent hooks/rumors/jobs** in 13 `fc_*` files (`09_quests/hooks_and_rumors/`; 132 hooks + 104 rumors + 68 jobs) on top of ~281 pre-Stage-10 home-region hooks/rumors. Created indexes `DEVELOPED_QUESTS_INDEX.md`, `HOOKS_JOBS_RUMORS_INDEX.md`, `by_level/QUESTS_BY_LEVEL.md`, `by_faction/QUESTS_BY_FACTION.md`, `by_type/QUESTS_BY_TYPE.md`; updated `QUEST_INDEX.md`, `CONTENT_INDEX.md`, `STAGE_STATUS.md`, `STAGE_10_PROGRESS.md`. All 7 major factions have quest coverage; every quest has noncombat options + solo-safety valves (no four-PC assumptions); all NPC names from authored Stage 9.5 rosters; no apex-truth leaks in player-facing text (Hollow Court/harvest/keystone/Under-Shrine DM-only; far-region echoes oblique & DM-labeled); no canon contradictions.

- [x] Stage 9.5: Full-Continent NPC Readiness — 2026-06-12. Created 12 far-continent region NPC files in `08_npcs/by_region/` (`{VERDANCE_REACHES, CONCORD_HEARTLANDS, GLASSMERE_LEAGUE, HETHEWALD_FREE_HOLDS, HOLLOW_GULF_PORTS, SALTMERE_REACHES, EMBERFELL_THEOCRACY, SALLOWMARCH_PROTECTORATE, MARROWDOWNS, WENDER_STEPPE, KARRAN_MARCHES, SUNMARK}_NPCS.md`). **+44 major / +168 secondary / +432 minor** (cumulative 94 / 368 / 953). All 12 regions meet minimums (3+ major, 12+ secondary, 30+ minor). Updated `NPC_RELATIONSHIP_WEB.md`, `NPC_SECRET_LEDGER.md`, `NPC_VOICE_GUIDE.md`, `NPC_INDEX.md`, `NAMING_REGISTRY.md`, `CONTENT_INDEX.md`, `STAGE_STATUS.md`, `STAGE_9_5_PROGRESS.md` (Stage 9.5 sections). No new major geography/factions; no far-region NPC knows the apex truth (Hollow Court/harvest never exposed); pre-Concord echoes and the Emberfell mirror kept distinct from the Hollowmere keystone. `FAR_CONTINENT_NPCS.md` superseded (retained for compatibility).
- [x] Stage 9: NPC Codex Expansion — 2026-06-12 (pass 1 + pass 2 + completion/cleanup pass). Final counts: **50 major** (24 in `MAJOR_NPCS.md` + 8 in `by_region/CARADRIL_MAJOR_NPCS.md` + 18 new/elevated in `by_region/STAGE_9_MAJOR_NPCS.md`), **~200 secondary** (64 base + 136 in `by_region/STAGE_9_SECONDARY_NPCS.md`), **521 minor** (92 base + 403 in `by_region/STAGE_9_MINOR_NPCS.md` Waves 1–7 + 26 far-continent). Infrastructure (`NPC_RELATIONSHIP_WEB.md`, `NPC_SECRET_LEDGER.md` [DM-only], `NPC_VOICE_GUIDE.md`) created and now covers all 50 majors. Faction ladders complete at every level; Hollow Court secrecy preserved; no new factions/gods/mysteries/artifacts. Counts reconciled across STAGE_9_PROGRESS / STAGE_STATUS / NPC_INDEX / CONTENT_INDEX.
- [x] Stage 8: Faction Deepening — 2026-06-11. All seven major factions made fully operational: 4-quest chains per faction (28 quest files + 7 chain indexes in `09_quests/faction_quests/`), "Combat Capability And Stat References" sections with rank-and-file profiles added to all seven faction files, `FACTION_RELATIONSHIP_MAP.md` (full pairwise + Court hidden ties) and `FACTION_TURN_RULES.md` created, `FACTION_INDEX.md`/`FACTION_STATE.md`/`WORLD_CLOCKS.md` updated. No new proper nouns/central mysteries/factions; Hollow Court secrecy preserved.

---

## Medium

- [ ] Generate the actual map images
  - Why it matters: cartographic canon and prompts are ready (campaign-area AND full-continent); the visual maps themselves do not exist yet. **Recommended order:** `FULL_WORLD_MAP_PROMPTS.md` Prompt 5 (campaign-area standalone zoom map = the day-to-day play map; a separate map, not an inset on the player-safe full-continent map) first; then Prompt 1 (player-safe full continent); then Prompt 3 (parchment artifact to hand the player); then Prompt 2 / Prompt 4-toggle (DM-only). The campaign-area-only prompts in `WORLD_MAP_PROMPTS.md` remain valid for cluster-only renders. The player-safe full continent (Prompt 1) is repo-aware via `PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md`; for an external image model that cannot read repo files, use `PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET.md`.
  - Related files: `04_world_atlas/FULL_WORLD_MAP_PROMPTS.md`, `FULL_WORLD_MAP_COORDINATES.md`, `FULL_WORLD_MAP_LAYERS.md`; `WORLD_MAP_PROMPTS.md` (campaign-area)
  - Suggested agent: world-atlas-builder (or external image tool)
  - Stage: interstitial (post-Stage-7)

- [ ] Note: `WORLD_MAP_AUTHORITY.md` / `WORLD_MAP_COORDINATES.md` are now the **campaign-area (NW Orrun)** authority; `FULL_WORLD_MAP_*` supersede them for **whole-continent** use
  - Why it matters: the Full-World Cartographic Expansion pass split map scope into campaign-area vs full-continent. The two `WORLD_MAP_*` files are retained and authoritative for the NW cluster; the four `FULL_WORLD_MAP_*` files are authoritative for the whole continent. Keep them consistent when either is edited.
  - Related files: `04_world_atlas/WORLD_MAP_AUTHORITY.md`, `WORLD_MAP_COORDINATES.md`, `FULL_WORLD_MAP_AUTHORITY.md`, `FULL_WORLD_MAP_COORDINATES.md`
  - Suggested agent: world-atlas-builder / indexer-librarian
  - Stage: interstitial (post-Stage-7)

- [ ] Deep-build the placeholder regions when play warrants
  - Why it matters: Ring 2 placeholders (Verdance Reaches SE Lvl 8–12; deep Sunder Heights N Lvl 6–10; Highmark passes far-N Lvl 12–16) AND the 13 new full-continent placeholders (Glassmere League, Marrowdowns, Sallowmarch Protectorate, Hollow Gulf Ports, Wender Steppe, Karran Marches, Emberfell Theocracy, Saltmere Reaches, Concord Heartlands/Ruin'd Crown, Hethewald Free Holds, Sunmark) are named/positioned with political form + 1-sentence identity only. They need full region builds before any play ranges into them. **The Concord Heartlands is a surface fallen-ruin — NEVER the keystone/Hollow Court seat.**
  - Related files: `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` §6, `WORLD_MAP_AUTHORITY.md` §6–§8, `REGION_INDEX.md`
  - Suggested agent: world-atlas-builder
  - Stage: future (Ring 2+ / continental expansion)

- [ ] Pin down low-confidence map coordinates as regions are built
  - Why it matters: 22 campaign-area grid entries (`WORLD_MAP_COORDINATES.md`) and ~86 full-continent entries (`FULL_WORLD_MAP_COORDINATES.md`) are low-confidence placeholders; deep-building those areas should upgrade them to medium/high and keep both grids self-consistent.
  - Related files: `04_world_atlas/WORLD_MAP_COORDINATES.md`, `FULL_WORLD_MAP_COORDINATES.md`
  - Suggested agent: world-atlas-builder
  - Stage: ongoing

- [ ] Build the standalone bestiary (mid/high tiers especially)
  - Why it matters: Stage 6 audit Medium finding. Adversary stats currently live only inside zone/city encounter tables + the 5 Act 1 threat profiles; Acts 2–5 threats above ~L6 are not yet mechanically usable.
  - Related files: `13_encounters_and_bestiary/`
  - Suggested agent: `encounter-bestiary-designer`
  - Stage: 13

- [ ] Build `REWARDS_BY_LEVEL.md` and stat referenced dungeon/quest rewards
  - Why it matters: Stage 6 audit Medium finding. Rewards currently reference "level-appropriate items" abstractly, forcing the AI DM to improvise specifics for a solo PC.
  - Related files: `14_treasure_and_artifacts/`, `10_dungeons_and_ruins/`
  - Suggested agent: `encounter-bestiary-designer`
  - Stage: 14

- [ ] Build standalone Acts 2–5 arc files
  - Why it matters: Stage 6 audit Medium finding. The arc above level 4 exists as shape only; play beyond L4 is not yet runnable in detail.
  - Related files: `12_campaign_arc/`
  - Suggested agent: `campaign-architect`
  - Stage: 15

- [ ] Build the first major Act 1 dungeon as a dedicated set-piece (optional enrichment)
  - Why it matters: Act 1 currently routes its dungeon beats through the six Stage 3 Concord sites (Peat Chapel, Sunken Tollhouse, Whispering Cairn, Ledger Vault, Barrow, Deep Adit), which is sufficient for play. A purpose-built Act 1 climax dungeon could sharpen the level 3→4 beat, but is not required (the keystone shrine is deferred to Stage 12 by design).
  - Related files: `12_campaign_arc/ACT_1_LEVELS_1_4.md`, `10_dungeons_and_ruins/`
  - Suggested agent: `encounter-bestiary-designer`
  - Stage: 5 (optional) / 12

---

## Low

- [ ] Populate `/15_random_tables/` with travel, weather, event, and wilderness tables
  - Why it matters: Random tables reduce AI improvisation burden during travel and downtime.
  - Related files: `WORLDBUILDING_STANDARDS.md`
  - Suggested agent: `world-atlas-builder`
  - Stage: 3+

- [ ] Resolve any duplicate content between `CLAUDE.md` and `PROJECT_RULES.md`
  - Why it matters: Duplicate rules diverge over time and create confusion.
  - Related files: `CLAUDE.md`, `PROJECT_RULES.md`
  - Suggested agent: —
  - Stage: optional cleanup

---

## Post-Stage-4 Follow-Ups

- [ ] Create `QUEST_INDEX.md` covering all authored quests across stages
  - Why it matters: Quests currently indexed inline in `CONTENT_INDEX.md`; a dedicated QUEST_INDEX would allow faster lookup by level, region, type, and faction as the quest library grows.
  - Related files: `09_quests/regional_quests/`, `09_quests/city_quests/`, `09_quests/hooks_and_rumors/`
  - Suggested agent: `indexer-librarian`
  - Stage: 10 (Quest Library Expansion)

---

## Post-Stage-3 Follow-Ups

- [ ] (Optional) Build individual per-clue files for `11_mysteries_and_secrets/CLUE_INDEX.md`
  - Why it matters: clues are tracked in index/runtime tables and now anchored to region sites; per-clue files would add finer retrieval but are not required for play.
  - Stage: 11 (deferred)

- [ ] Build the drowned shrine dungeon (the keystone)
  - Why it matters: the campaign keystone location needs a full dungeon build; intentionally deferred from Stage 3.
  - Related files: `07_factions/major_factions/HOLLOW_COURT.md`, `05_regions/wilderness/BASIN_SHORE_AND_HOLMS_SITES.md`, `10_dungeons_and_ruins/`
  - Stage: 12

- [ ] Full dungeon-file build for the Sunken Wards and the Sealed Archive (Caradril)
  - Why it matters: Stage 4 specced both richly as district/quest content (encounter list, hazards, retreat, scaling); a full room-by-room dungeon file is deferred to Stage 12 to match the keystone-shrine treatment.
  - Related files: `06_settlements/caradril_districts/THE_SUNKEN_WARDS.md`, `THE_LANTERN_REACH.md`, `09_quests/city_quests/Q_BELOW_THE_STILLING.md`, `Q_THE_SEALED_ARCHIVE.md`
  - Stage: 12

- [ ] Resolve the "Magisterium correspondent" thread in play/arc (Caradril ↔ Reke)
  - Why it matters: Stage 4 left this as an intentional open lead (M8-adjacent), never a named second Court agent. Stage 5 confirmed it stays a *lead* through Act 1 (Act 1 caps at R1; the steering employer is murky — R4 is Act 2–3). Stage 15 (Act 2/3) should decide how it resolves through play without pre-revealing the Hollow Court.
  - Related files: `06_settlements/caradril_districts/THE_MAGISTERIUM.md`, `02_runtime_state/HIDDEN_CLUES.md` (C-M8 city anchor), `11_mysteries_and_secrets/ACT_1_CLUE_TRAILS.md` (M8 ceiling), `12_campaign_arc/`
  - Stage: 15

- [ ] Stat the Stage 3 dungeon rewards by level (e.g. the Barrow of Nine Doors magic item) and create `REWARDS_BY_LEVEL.md`
  - Why it matters: Stage 3 dungeon files reference level-appropriate rewards that need concrete items.
  - Stage: 14

- [ ] Add `/15_random_tables/` (travel/weather/event) — lower priority now that zone encounter tables exist
  - Stage: 3+ / low

---

## Completed Recently

- [x] Stage 6: First Full Audit — 2026-06-10 (ran all 10 audit categories across Stages 1–5; foundation verified sound: 0 Critical, 1 High [two broken Act 1 arc-spine quest pointers — FIXED inline], 4 Medium, 5 Low; secret separation/three-clue/faction-agency/solo-safety/state-tracking all pass clean; report in `18_audits/STAGE_1_TO_5_AI_READINESS_AUDIT.md`; CONSISTENCY_AUDIT/CONTENT_GAPS/STAGE_STATUS/EXPANSION_PLAN updated; scaling to Stage 7 approved)
- [x] Stage 5: Level 1–4 Play Arc (Act 1) — 2026-06-10 (open-world Act 1 play kit: arc spine `ACT_1_LEVELS_1_4.md` + 6 faction-alignment quests `act_1_quests/` + 5 recurring early-threat profiles `ACT_1_THREATS.md` + Act 1 clue-trails overlay `ACT_1_CLUE_TRAILS.md` (existing M1–M9; R1 cap; three-clue check) + 9 failure-redirect states `ACT_1_FAILURE_STATES.md` + L2/3/4 milestone/XP triggers `ACT_1_MILESTONES.md` + Act 1 NPC casting guide `ACT_1_NPC_GUIDE.md`; runtime ACTIVE_QUESTS/OPEN_THREADS seeded; anti-railroad verified; all L1–4 content mechanically complete; no new central mystery/faction/god/cosmology/artifact; reveals capped at R1; Hollow Court never exposed)
- [x] Stage 4: First Major City Deep Build (Caradril) — 2026-06-10 (city overview + 8 district files incl. the Sunken Wards sub-dungeon; 15 city secondary + 25 city minor NPCs; 11 developed city quests; 36 hooks + 30 rumors; city encounter/social-scene tables; 4 city-internal factions + 3 city clocks (C1/C2/C3); Ledger HQ + Remnant seat located; M2/M3/M4/M6/M8/M9 city clue access added with no new mysteries; M7/Hollow Court never named in the city; Act-3 gating on the Sealed Archive; solo-safe and secrecy-separated; indexes/canon/registry/state updated)
- [x] Stage 3: Starting Region Deep Build — 2026-06-09 (8 settlements, 4 wilderness zone-files/~25 sites, 6 dungeons/ruins, ~56 NPCs (~21 secondary + ~35 minor), 14 developed quests, 39 hooks + 50 rumors, 4 zone encounter tables; all five registered secondary-NPC placeholders completed; clue/clock anchors added; indexes/canon/registry updated; solo-safe and secrecy-separated throughout)
- [x] Stage 2 cleanup pass — 2026-06-09 (fixed stale CONTENT_GAPS/EXPANSION_PLAN/CONSISTENCY_AUDIT to reflect Stages 1–2 complete; populated CLUE_INDEX and HIDDEN_CLUES from the mystery web with all clues hidden at start; added D&D mechanical completeness fields/sections to NPC, quest, content, faction, and worldbuilding standards templates — Critical TODO cleared)
- [x] Complete Stage 2: AI Runtime Foundation — 2026-06-09 (all 18 runner protocols written as full operational content (17 new + AI_DM_CORE_RULES.md from Stage 0); START/RESUME prompts + 3 session-pack templates ready; 8 runtime state files seeded from Stage 1; solo-first, three-clue-rule, secrecy-preserving; indexes and tracking updated)
- [x] Seed runtime state files from Stage 1 content — 2026-06-09 (CURRENT_STATE, CURRENT_LOCATION, CURRENT_SCENE, ACTIVE_QUESTS = Hook 1 + Hooks 5–7, OPEN_THREADS, FACTION_STATE, NEXT_SESSION_START, PLAYER_CHARACTER scaffold)
- [x] Create START_NEW_CAMPAIGN_PROMPT.md and RESUME_CAMPAIGN_PROMPT.md — 2026-06-09 (DM-only, self-contained, spoiler-safe)
- [x] Populate all runner protocol files in 01_runner_protocol/ — 2026-06-09
- [x] Complete Stage 1: Campaign Foundation — 2026-06-09 ("The Long Remembering"; world, region, settlement, 7 factions, 20 NPCs, mystery web, arc, hooks, rumors, opening scenes, solo-safety, 10 clocks; all indexed)
- [x] Created full repository scaffold — 2026-06-09
- [x] Created all control, tracking, canon, runtime state, protocol, session pack, and backlog placeholder files — 2026-06-09
- [x] Updated README.md — 2026-06-09
