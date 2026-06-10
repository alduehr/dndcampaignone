# TODO.md

## Purpose

Prioritized, actionable work queue. When no specific task is given, use this file to determine what to do next.

---

## Critical

*None open.*

## High

- [ ] Complete Stage 5: Level 1–4 Play Arc
  - Why it matters: With the region now deep-built (Stage 3), the next highest-value pass is the shaped Act 1 narrative — a default path, alternate paths, faction decision points, the first major dungeon, an early villain/threat profile, and playable failure states — while preserving open-world freedom.
  - Related files: `DEVELOPMENT_STAGES.md` Stage 5, `QUEST_STANDARDS.md`, `12_campaign_arc/`, the 14 Stage 3 developed quests in `09_quests/regional_quests/`
  - Suggested agent: `quest-arc-designer` (+ `encounter-bestiary-designer`)
  - Stage: 5

---

## Medium

- [ ] Run Stage 6: First Full Audit
  - Why it matters: Do not scale a broken foundation. Audit before major expansion.
  - Related files: `AUDIT_STANDARDS.md`, `DEVELOPMENT_STAGES.md` Stage 6
  - Suggested agent: `canon-continuity-auditor`
  - Stage: 6
  - Blocker: Requires Stages 1–5

---

## Low

- [ ] Populate `/15_random_tables/` with travel, weather, event, and wilderness tables
  - Why it matters: Random tables reduce AI improvisation burden during travel and downtime.
  - Related files: `WORLDBUILDING_STANDARDS.md`
  - Suggested agent: `world-atlas-builder`
  - Stage: 3+

- [ ] Create `NPC_RELATIONSHIP_WEB.md`, `NPC_SECRET_LEDGER.md`, `NPC_VOICE_GUIDE.md`
  - Why it matters: These are quality-of-life tools for managing large NPC populations.
  - Related files: `NPC_STANDARDS.md`
  - Suggested agent: `npc-codex-builder`
  - Stage: 9

- [ ] Resolve any duplicate content between `CLAUDE.md` and `PROJECT_RULES.md`
  - Why it matters: Duplicate rules diverge over time and create confusion.
  - Related files: `CLAUDE.md`, `PROJECT_RULES.md`
  - Suggested agent: —
  - Stage: optional cleanup

---

## Post-Stage-4 Follow-Ups

- [ ] Expand Caradril NPC count to approach Stage 4 target (75–100 total city NPCs)
  - Why it matters: Stage 4 delivered ~40 useful city NPCs (20 major from Stage 1 + 15 secondary + 25 minor); the target was 75–100. Quality over quantity was the right call, but the gap should be closed before heavy city play begins.
  - Related files: `08_npcs/SECONDARY_NPCS.md`, `08_npcs/MINOR_NPCS.md`, `08_npcs/NPC_INDEX.md`, `06_settlements/caradril_districts/`
  - Suggested agent: `npc-codex-builder`
  - Stage: 9 (NPC Codex Expansion)

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
  - Why it matters: Stage 4 left this as an intentional open lead (M8-adjacent), never a named second Court agent. Stage 5/15 should decide how it resolves through play without pre-revealing the Hollow Court.
  - Related files: `06_settlements/caradril_districts/THE_MAGISTERIUM.md`, `02_runtime_state/HIDDEN_CLUES.md` (C-M8 city anchor), `12_campaign_arc/`
  - Stage: 5 / 15

- [ ] Stat the Stage 3 dungeon rewards by level (e.g. the Barrow of Nine Doors magic item) and create `REWARDS_BY_LEVEL.md`
  - Why it matters: Stage 3 dungeon files reference level-appropriate rewards that need concrete items.
  - Stage: 14

- [ ] Add `/15_random_tables/` (travel/weather/event) — lower priority now that zone encounter tables exist
  - Stage: 3+ / low

---

## Completed Recently

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
