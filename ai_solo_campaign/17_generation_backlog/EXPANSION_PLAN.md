# EXPANSION_PLAN.md

## Purpose

Forward-looking development roadmap. Tracks what to build next and in what order. This is a roadmap, not a task queue — use `TODO.md` for actionable tasks.

## Current Status

**Stages 0, 1, 2, and 3 complete (2026-06-09).** The campaign foundation, the full AI runtime layer, and the **deep-built starting region** all exist. The Sundering Reach now supports 10–20 sessions of open-world solo play (8 settlements, 4 wilderness zones, 6 dungeons, ~56 NPCs (~21 secondary + ~35 minor), 14 developed quests, 39 hooks + 50 rumors, zone encounter tables). **Stage 5 — Level 1–4 Play Arc is the recommended next pass** (shape the Act 1 narrative atop the now-deep region), with Stage 4 (First Major City — Caradril) slotted before or after, and the Stage 6 audit following.

---

## Current Stage

| Field | Value |
|---|---|
| Stage | 5 — Level 1–4 Play Arc (recommended next) / 4 — First Major City |
| Goal | Shape the Act 1 arc (default + alternate paths, first major dungeon, early villain, failure states) atop the deep region |
| Status | Not started |
| Blocking Issues | None — Stages 1–3 are complete |

---

## Next Production Passes

### Pass 1 — DONE: Starting Region Deep Build (Stage 3)

**Complete 2026-06-09.** Delivered 8 settlements, 4 wilderness zone-files (~25 sites), 6 dungeons/ruins, ~56 secondary+minor NPCs (~21 secondary + ~35 minor), 14 developed quests, 39 hooks + 50 rumors, and 4 solo-tuned zone encounter tables; clue paths and faction clocks anchored to real sites; all indexed and cross-linked. Targets met or exceeded. (Keystone drowned-shrine dungeon deferred to Stage 12 by design.)

### Pass 2 — Level 1–4 Play Arc (Stage 5)

- **Goal:** Develop the early campaign arc with a default path, alternate paths, faction hooks, the first major dungeon, an early villain/threat profile, and playable failure states — while preserving open-world freedom.
- **Files to create/edit:**
  - `12_campaign_arc/ACT_1_LEVELS_1_4.md`
  - Developed Act 1 quest files in `09_quests/`
  - First major dungeon file in `10_dungeons_and_ruins/`
  - Early villain/threat profile in `13_encounters_and_bestiary/`
- **Suggested agent:** `quest-arc-designer` (with `encounter-bestiary-designer` for the dungeon and villain)
- **Completion criteria:** A solo campaign can begin and run cleanly through level 4; the main arc is foreshadowed but not over-explained; failure states are playable; the first recurring adversary is established.
- **Note:** Stage 4 (first major city) may be slotted before or after this pass depending on whether the Act 1 arc needs the city; current plan defers the city until after Act 1 is shaped.

### Pass 3 — First Full Audit (Stage 6)

- **Goal:** Verify the foundation is sound before scaling outward. Do not scale broken content.
- **Files to create/edit:**
  - `18_audits/STAGE_1_TO_5_AI_READINESS_AUDIT.md`
  - Update `00_control/CONSISTENCY_AUDIT.md`, `00_control/TODO.md`, `17_generation_backlog/CONTENT_GAPS.md`
- **Suggested agent:** `canon-continuity-auditor`
- **Completion criteria:** Canon consistency, secret separation, clue solvability, faction agency, solo-play safety, state tracking, and index completeness all checked; critical issues identified; no major scaling until critical issues are fixed.

### Pass 4 — First Major City Deep Build (Stage 4)

- **Goal:** Build the first major city as a dense political/social hub: districts, government, law/crime, services, guilds/temples/houses/criminal groups, city NPCs, city quests, rumor tables, faction clocks, and city secrets.
- **Files to create/edit:**
  - City overview + district files in `06_settlements/`
  - City NPCs in `08_npcs/`; city quests in `09_quests/`
  - City faction activity in `07_factions/`
- **Suggested agent:** `world-atlas-builder` (with `faction-weaver` and `npc-codex-builder`)
- **Completion criteria:** The city can serve as a long-term hub, feels politically alive, has major services, supports repeated visits, and changes when ignored.

### Pass 5 — Faction Deepening (Stage 8)

- **Goal:** Make all major factions fully operational: full quest chains, internal conflict, relationship maps, named members at multiple levels, and concrete "what they do if ignored" behavior tied to the world clocks.
- **Files to create/edit:**
  - Expand each file in `07_factions/major_factions/`
  - Update `07_factions/FACTION_INDEX.md`, `02_runtime_state/FACTION_STATE.md`, `02_runtime_state/WORLD_CLOCKS.md`
- **Suggested agent:** `faction-weaver`
- **Completion criteria:** Every major faction can help, hinder, recruit, deceive, or retaliate; every faction has a clock, named members, resources, and a quest chain.

---

## Later Expansion (Stages 9–16)

Rough order after the first audit and the passes above:

1. **Stage 7** — Regional expansion ring 1 (adjacent regions)
2. **Stage 9** — NPC codex expansion (toward 50–100 major, 200–500 secondary, 500+ minor)
3. **Stage 10** — Quest library expansion (toward 300–600 hooks)
4. **Stage 11** — Mystery, secret, and clue expansion (false leads, omens, per-clue files)
5. **Stage 12** — Dungeons and adventure sites (including the keystone dungeon)
6. **Stage 13** — Encounter and bestiary expansion (solo-safe threats, bosses)
7. **Stage 14** — Treasure, artifacts, and rewards (by level)
8. **Stage 15** — Level 5–20 arc expansion (Acts 2–5, villain escalation, endgame states)
9. **Stage 16** — Pre-play readiness audit

---

## Deferred Ideas

*To be added as development generates ideas that are out of scope for current stages.*

---

## Do Not Build Yet

- Level 17–20 content (premature without a tested mid-game foundation)
- Specific puzzle solutions (build puzzles with alternate solutions first)
- Sequel hooks (campaign is not yet running)
- Epilogue content

---

## Related Files

- [`../00_control/DEVELOPMENT_STAGES.md`](../00_control/DEVELOPMENT_STAGES.md)
- [`../00_control/STAGE_STATUS.md`](../00_control/STAGE_STATUS.md)
- [`../00_control/TODO.md`](../00_control/TODO.md)
- [`CONTENT_GAPS.md`](CONTENT_GAPS.md)
