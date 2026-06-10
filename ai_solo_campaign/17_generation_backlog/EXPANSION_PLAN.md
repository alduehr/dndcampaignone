# EXPANSION_PLAN.md

## Purpose

Forward-looking development roadmap. Tracks what to build next and in what order. This is a roadmap, not a task queue — use `TODO.md` for actionable tasks.

## Current Status

**Stages 0, 1, 2, 3, 4, and 5 complete (Stage 5: 2026-06-10).** The campaign foundation, the full AI runtime layer, the deep-built starting region, the first major city (Caradril), and now the **Level 1–4 Act 1 play kit** all exist. The Sundering Reach supports 10–20 sessions; Caradril adds the mid-game hub; **Stage 5** makes the early game runnable end-to-end (open-world arc spine, 6 faction-alignment quests, 5 recurring early-threat profiles, an existing-clue Act 1 access overlay with an R1 cap, 9 failure-redirect states, milestone/XP triggers, and an Act 1 NPC casting guide — all reusing existing content, no new central mystery/faction/god/cosmology/artifact). **The Stage 6 First Full Audit is the recommended next pass** (spanning Stages 1–5); do not scale outward (Stage 7+) until it clears.

---

## Current Stage

| Field | Value |
|---|---|
| Stage | 6 — First Full Audit (recommended next) |
| Goal | Verify the Stage 1–5 foundation before scaling outward (canon, secrecy, R1 gating, three-clue solvability, faction agency, solo-safety, state, indexes) |
| Status | Not started |
| Blocking Issues | None — Stages 1–5 are complete |

---

## Next Production Passes

### Pass 1 — DONE: Starting Region Deep Build (Stage 3)

**Complete 2026-06-09.** Delivered 8 settlements, 4 wilderness zone-files (~25 sites), 6 dungeons/ruins, ~56 secondary+minor NPCs (~21 secondary + ~35 minor), 14 developed quests, 39 hooks + 50 rumors, and 4 solo-tuned zone encounter tables; clue paths and faction clocks anchored to real sites; all indexed and cross-linked. Targets met or exceeded. (Keystone drowned-shrine dungeon deferred to Stage 12 by design.)

### Pass 2 — DONE: Level 1–4 Play Arc (Stage 5)

**Complete 2026-06-10.** Delivered the open-world Act 1 play kit: the arc spine `ACT_1_LEVELS_1_4.md` (Five Doors + seven faction doors, multi-route to R1, ignore-consequences, Act 2 triggers); 6 faction-alignment quests in `09_quests/act_1_quests/` (Wardens, Compact, Ledger, Mourners, Gravecallers, Remnant — the Hollow Court has none by design); 5 recurring early-threat profiles `ACT_1_THREATS.md` (full stat profiles, solo-safe, scaling); the DM-only `ACT_1_CLUE_TRAILS.md` overlay (existing M1–M9 only; R1 cap; three-clue check); 9 redirect-not-end failure states `ACT_1_FAILURE_STATES.md`; multi-path milestone/XP triggers `ACT_1_MILESTONES.md`; and the Act 1 NPC casting guide `ACT_1_NPC_GUIDE.md`. Runtime ACTIVE_QUESTS/OPEN_THREADS seeded; anti-railroad verified; all L1–4 content mechanically complete; no new central mystery/faction/god/cosmology/artifact; reveals capped at R1. (Act 1 routes dungeon beats through the 6 Stage 3 Concord sites; a dedicated Act 1 climax dungeon is optional/deferred, and the keystone shrine stays Stage 12.)

### Pass 3 — First Full Audit (Stage 6) — RECOMMENDED NEXT

- **Goal:** Verify the foundation is sound before scaling outward. Do not scale broken content.
- **Files to create/edit:**
  - `18_audits/STAGE_1_TO_5_AI_READINESS_AUDIT.md`
  - Update `00_control/CONSISTENCY_AUDIT.md`, `00_control/TODO.md`, `17_generation_backlog/CONTENT_GAPS.md`
- **Suggested agent:** `canon-continuity-auditor`
- **Completion criteria:** Canon consistency, secret separation, clue solvability, faction agency, solo-play safety, state tracking, and index completeness all checked; critical issues identified; no major scaling until critical issues are fixed.

### Pass 4 — DONE: First Major City Deep Build (Stage 4)

**Complete 2026-06-10.** Built **Caradril**: city overview + 8 district files (incl. the Sunken Wards sub-dungeon), 15 city secondary + 25 city minor NPCs, 11 developed city quests, 36 hooks + 30 rumors, city encounter/social-scene tables, 4 city-internal factions + 3 city clocks (C1/C2/C3), Ledger HQ + Remnant seat located, M2/M3/M4/M6/M8/M9 city clue access added with no new central mysteries. Solo-safe, secrecy-separated, fully indexed/cross-linked. (Full room-by-room dungeon builds for the Sunken Wards and Sealed Archive deferred to Stage 12 by design; the "Magisterium correspondent" left as an intentional open lead for Stage 5/15.)

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
