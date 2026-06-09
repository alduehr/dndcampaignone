# EXPANSION_PLAN.md

## Purpose

Forward-looking development roadmap. Tracks what to build next and in what order. This is a roadmap, not a task queue — use `TODO.md` for actionable tasks.

## Current Status

Stage 0 complete. No world content yet. Ready to begin Stage 1.

---

## Current Stage

| Field | Value |
|---|---|
| Stage | 1 — Campaign Foundation |
| Goal | Establish the campaign's premise, world identity, and core elements |
| Status | Not started |
| Blocking Issues | None |

---

## Next 5 Production Passes

### Pass 1 — Campaign Foundation (Stage 1)

- **Goal:** Establish the original campaign premise, central conflict, hidden truth, starting region and settlement, 5–8 major factions, 20 major NPCs, 20 major secrets, 10 session hooks, 20 rumors, level 1–20 arc shape, and three opening scenes.
- **Files to create/edit:**
  - `03_canon/CANON.md`
  - `03_canon/PLAYER_SAFE_CANON.md`
  - `03_canon/DM_ONLY_CANON.md`
  - `04_world_atlas/WORLD_OVERVIEW.md`
  - `04_world_atlas/MAP_DESCRIPTION.md`
  - `12_campaign_arc/MAIN_ARC_OVERVIEW.md`
  - `12_campaign_arc/LEVEL_1_TO_20_PROGRESSION.md`
  - `11_mysteries_and_secrets/MYSTERY_WEB.md`
  - `11_mysteries_and_secrets/REVELATION_MAP.md`
  - `07_factions/major_factions/` — 5–8 files
  - `08_npcs/` — 20 major NPC files
  - `MANIFEST.md` — campaign identity section
- **Suggested agent:** `campaign-architect`
- **Completion criteria:** Campaign can be summarized in one page. Starting location defined. First session can begin. Main arc has level 1–20 shape. All foundational content is indexed.

### Pass 2 — AI Runtime Foundation (Stage 2)

- **Goal:** Fill all runner protocol files, create session start/end prompts, populate runtime state templates.
- **Files to create/edit:**
  - All files in `01_runner_protocol/` that are currently placeholders
  - `16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md`
  - `16_ai_session_packs/RESUME_CAMPAIGN_PROMPT.md`
  - `16_ai_session_packs/STATE_UPDATE_TEMPLATE.md`
  - `16_ai_session_packs/COMPACT_CONTEXT_TEMPLATE.md`
  - `02_runtime_state/` — populate with starting campaign state
- **Suggested agent:** `ai-dm-runtime-engineer`
- **Completion criteria:** AI DM knows how to start, run, and end a session. State files show what must be tracked. Solo-play protocols cover combat, social, travel, exploration, and clue delivery.

### Pass 3 — Starting Region Deep Build (Stage 3)

- **Goal:** Build enough starting region content for 10–20 sessions of open-world play.
- **Files to create/edit:**
  - `05_regions/[starting-region].md`
  - `06_settlements/[starting-settlement].md`
  - 5–10 additional settlement files
  - 15–25 wilderness location files
  - 5–8 dungeon/ruin files
  - Regional quest, NPC, encounter, and rumor files
- **Suggested agent:** `world-atlas-builder`
- **Completion criteria:** Player can travel in multiple directions. Factions act if ignored. Mysteries have clue paths. AI rarely needs to invent major locations.

### Pass 4 — Level 1–4 Arc (Stage 5)

- **Goal:** Develop the early campaign arc with a default path, alternate paths, faction hooks, first major dungeon, and failure states.
- **Files to create/edit:**
  - `12_campaign_arc/ACT_1_LEVELS_1_4.md`
  - Early quest files
  - First major dungeon file
  - First villain profile
- **Suggested agent:** `quest-arc-designer`
- **Completion criteria:** Solo campaign can begin and run through level 4. Player has real agency. Main arc foreshadowed. Failure states playable.

### Pass 5 — First Full Audit (Stage 6)

- **Goal:** Check foundation before scaling.
- **Files to create/edit:**
  - `18_audits/STAGE_1_TO_5_AI_READINESS_AUDIT.md`
  - `00_control/CONSISTENCY_AUDIT.md` — update
  - `00_control/TODO.md` — reorganize
  - `17_generation_backlog/CONTENT_GAPS.md` — update
- **Suggested agent:** `canon-continuity-auditor`
- **Completion criteria:** Critical issues identified. No major scaling until critical issues fixed.

---

## Later Expansion (Stages 7–15)

Rough order after the first audit:

1. **Stage 4** — First major city (can be done before or after stage 5, depending on arc needs)
2. **Stage 7** — Regional expansion ring 1 (adjacent regions)
3. **Stage 8** — Faction deepening (all major factions fully operational)
4. **Stage 9** — NPC codex expansion (100+ major NPCs, 200+ secondary)
5. **Stage 10** — Quest library expansion (300+ hooks)
6. **Stage 11** — Mystery and clue expansion
7. **Stage 12** — Dungeons and adventure sites
8. **Stage 13** — Encounter and bestiary expansion
9. **Stage 14** — Treasure, artifacts, and rewards
10. **Stage 15** — Level 5–20 arc expansion
11. **Stage 16** — Pre-play readiness audit

---

## Deferred Ideas

*To be added as development generates ideas that are out of scope for current stages.*

---

## Do Not Build Yet

- Level 17–20 content (premature without a tested foundation)
- Specific puzzle solutions (build puzzles with alternate solutions first)
- Sequel hooks (campaign is not yet running)
- Epilogue content
