# TODO.md

## Purpose

Prioritized, actionable work queue. When no specific task is given, use this file to determine what to do next.

---

## Critical

*None open.*

## High

- [ ] Complete Stage 3: Starting Region Deep Build
  - Why it matters: The player needs a populated region to explore. 10–20 sessions of open-world content requires substantial regional depth beyond Hollowmere — additional settlements, wilderness sites, local dungeons/ruins, and regional quest/encounter/rumor tables.
  - Related files: `DEVELOPMENT_STAGES.md` Stage 3, `WORLDBUILDING_STANDARDS.md`, `05_regions/SUNDERING_REACH.md`, `06_settlements/HOLLOWMERE.md`
  - Suggested agent: `world-atlas-builder`
  - Stage: 3
  - Note: Stages 1 and 2 are complete; the campaign is runnable for opening sessions. Stage 3 expands the Reach so play does not run out of authored material.

---

## Medium

- [ ] Complete Stage 4: First Major City Deep Build
  - Why it matters: A major city provides a political and social hub for mid-campaign play.
  - Related files: `DEVELOPMENT_STAGES.md` Stage 4
  - Suggested agent: `world-atlas-builder`
  - Stage: 4
  - Blocker: Requires Stages 1 and 3

- [ ] Complete Stage 5: Level 1–4 Play Arc
  - Why it matters: The early arc gives the AI DM a shaped narrative while preserving open-world freedom.
  - Related files: `DEVELOPMENT_STAGES.md` Stage 5, `QUEST_STANDARDS.md`
  - Suggested agent: `quest-arc-designer`
  - Stage: 5
  - Blocker: Requires Stages 1–3

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

## Stage 3 Follow-Ups (from Stage 1)

- [ ] Create full entries for secondary NPCs referenced in faction files
  - Who: Warden Pell, Tallytooth Ren, Bann Oester, Clerk Pevin Oss, Custodian Orre, Reach Remnant agents.
  - Related files: faction files, `08_npcs/NPC_INDEX.md`
  - Stage: 3 / 9

- [ ] (Optional) Build individual per-clue files for `11_mysteries_and_secrets/CLUE_INDEX.md`
  - Why it matters: CLUE_INDEX.md and HIDDEN_CLUES.md are now populated as index/runtime tables (all clues hidden at start). Per-clue files would add finer retrieval but are not required for play.
  - Related files: `CLUE_INDEX.md`, `HIDDEN_CLUES.md`, `MYSTERY_WEB.md`, `SECRET_INDEX.md`
  - Stage: 11 (deferred)

- [ ] Build the drowned shrine dungeon
  - Why it matters: The campaign keystone location needs a full dungeon build with solo-safety valves and scaling.
  - Related files: `07_factions/major_factions/HOLLOW_COURT.md`, `10_dungeons_and_ruins/`
  - Stage: 12

- [ ] Deep-build the Sundering Reach (settlements, wilderness sites, encounter/rumor tables)
  - Related files: `05_regions/SUNDERING_REACH.md`, `WORLDBUILDING_STANDARDS.md`
  - Stage: 3

---

## Completed Recently

- [x] Stage 2 cleanup pass — 2026-06-09 (fixed stale CONTENT_GAPS/EXPANSION_PLAN/CONSISTENCY_AUDIT to reflect Stages 1–2 complete; populated CLUE_INDEX and HIDDEN_CLUES from the mystery web with all clues hidden at start; added D&D mechanical completeness fields/sections to NPC, quest, content, faction, and worldbuilding standards templates — Critical TODO cleared)
- [x] Complete Stage 2: AI Runtime Foundation — 2026-06-09 (all 18 runner protocols written as full operational content (17 new + AI_DM_CORE_RULES.md from Stage 0); START/RESUME prompts + 3 session-pack templates ready; 8 runtime state files seeded from Stage 1; solo-first, three-clue-rule, secrecy-preserving; indexes and tracking updated)
- [x] Seed runtime state files from Stage 1 content — 2026-06-09 (CURRENT_STATE, CURRENT_LOCATION, CURRENT_SCENE, ACTIVE_QUESTS = Hook 1 + Hooks 5–7, OPEN_THREADS, FACTION_STATE, NEXT_SESSION_START, PLAYER_CHARACTER scaffold)
- [x] Create START_NEW_CAMPAIGN_PROMPT.md and RESUME_CAMPAIGN_PROMPT.md — 2026-06-09 (DM-only, self-contained, spoiler-safe)
- [x] Populate all runner protocol files in 01_runner_protocol/ — 2026-06-09
- [x] Complete Stage 1: Campaign Foundation — 2026-06-09 ("The Long Remembering"; world, region, settlement, 7 factions, 20 NPCs, mystery web, arc, hooks, rumors, opening scenes, solo-safety, 10 clocks; all indexed)
- [x] Created full repository scaffold — 2026-06-09
- [x] Created all control, tracking, canon, runtime state, protocol, session pack, and backlog placeholder files — 2026-06-09
- [x] Updated README.md — 2026-06-09
