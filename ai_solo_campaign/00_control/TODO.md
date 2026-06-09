# TODO.md

## Purpose

Prioritized, actionable work queue. When no specific task is given, use this file to determine what to do next.

---

## Critical

- [ ] Add D&D mechanical completeness requirements to all NPC, quest, dungeon, encounter, faction, and campaign-act templates.
  - Why it matters: Prevents the campaign from drifting into a generic fantasy RPG or mechanics-free story setting. Important NPCs, monsters, encounters, quests, dungeons, companions, and threats need D&D 5e / 2024-compatible mechanical guidance.
  - Related files: `DND_MECHANICS_REQUIREMENTS.md`, `NPC_STANDARDS.md`, `QUEST_STANDARDS.md`, `CONTENT_STANDARDS.md`, `RULESET_ASSUMPTIONS.md`, `LEVELING_ASSUMPTIONS.md`
  - Note: `DND_MECHANICS_REQUIREMENTS.md` already defines the full mechanical completeness standard. This task is about ensuring all content templates (NPC_STANDARDS, QUEST_STANDARDS, etc.) explicitly reference and enforce those requirements at the field level.
  - Suggested agent: `encounter-bestiary-designer`
  - Stage: Stage 0 / Stage 2

- [ ] Complete Stage 1: Campaign Foundation
  - Why it matters: No campaign world exists. Nothing can be played or tested until the foundation is established.
  - Related files: `DEVELOPMENT_STAGES.md` Stage 1, `PRODUCTION_WORKFLOW.md`, `PROJECT_RULES.md`
  - Suggested agent: `campaign-architect`
  - Stage: 1

---

## High

- [ ] Complete Stage 2: AI Runtime Foundation
  - Why it matters: The AI DM cannot run sessions without protocols, state files, session start/end prompts, and solo-play procedures.
  - Related files: `DEVELOPMENT_STAGES.md` Stage 2, `01_runner_protocol/AI_DM_CORE_RULES.md`, `16_ai_session_packs/`
  - Suggested agent: `ai-dm-runtime-engineer`
  - Stage: 2
  - Blocker: Requires Stage 1 canon to inform starting state

- [ ] Create `/16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md`
  - Why it matters: Without a start prompt, the AI DM has no clean entry point into the campaign.
  - Related files: `01_runner_protocol/AI_DM_CORE_RULES.md`, `02_runtime_state/CURRENT_STATE.md`
  - Suggested agent: `ai-dm-runtime-engineer`
  - Stage: 2

- [ ] Create `/16_ai_session_packs/RESUME_CAMPAIGN_PROMPT.md`
  - Why it matters: The AI DM needs a clean resume path to pick up mid-campaign without context loss.
  - Related files: `16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md`
  - Suggested agent: `ai-dm-runtime-engineer`
  - Stage: 2

- [ ] Populate all runner protocol files in `/01_runner_protocol/`
  - Why it matters: Currently only `AI_DM_CORE_RULES.md` exists. The solo play, session loop, combat, social, travel, clue delivery, and failure protocols are all placeholders.
  - Related files: All files in `01_runner_protocol/`
  - Suggested agent: `ai-dm-runtime-engineer`
  - Stage: 2

---

## Medium

- [ ] Complete Stage 3: Starting Region Deep Build
  - Why it matters: The player needs a populated region to explore. 10–20 sessions of content requires substantial regional depth.
  - Related files: `DEVELOPMENT_STAGES.md` Stage 3, `WORLDBUILDING_STANDARDS.md`
  - Suggested agent: `world-atlas-builder`
  - Stage: 3
  - Blocker: Requires Stage 1 to establish starting region identity

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

## Completed Recently

- [x] Created full repository scaffold — 2026-06-09
- [x] Created all control, tracking, canon, runtime state, protocol, session pack, and backlog placeholder files — 2026-06-09
- [x] Updated README.md — 2026-06-09
