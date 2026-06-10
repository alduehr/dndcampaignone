# CONSISTENCY_AUDIT.md

## Purpose

Running tracker of known continuity, secrecy, and AI-readiness issues. Not a full audit report — those go in `/18_audits/`. This file tracks issues that need fixing and their resolution status.

## Current Status

**Stages 0–6 complete (Stage 6 First Full Audit: 2026-06-10).** Foundation + AI runtime + deep-built starting region + first major city (Caradril) + Level 1–4 Act 1 play kit exist and are indexed. The Stage 6 first full audit has now been run — see `/18_audits/STAGE_1_TO_5_AI_READINESS_AUDIT.md`. **Result: foundation sound; 0 Critical, 1 High (fixed inline), 4 Medium, 5 Low. Scaling to Stage 7 approved.** The High finding (two broken Act 1 arc-spine quest pointers) was repaired during the audit. All Medium/Low findings are forward-stage gaps already tracked.

**Stage 5 self-check (Act 1 play kit):** no contradictions with CANON or Stages 1–4 found — Stage 5 created no new world facts, only play-layer structure (arc spine, milestones, failure redirects, threat profiles, clue-access overlay, NPC casting guide). Reveal cap held at **R1** in every Act 1 file (no Remembrance-as-substance, no Reke-as-traitor, no steering employer, no Concord's sin, no deliberate Quietfall, and **the Hollow Court [M7] is never named or deployed** — and correctly gets no friendly faction quest). DM-only material (hidden faction links in the threat profiles, the clue ceilings, the steering note) is confined to DM-Only sections; `ACT_1_CLUE_TRAILS.md` is dm-only. Three-clue rule preserved: every Act 1 conclusion (R1) has 3–4 independent routes; no single NPC/clue/dungeon/quest is mandatory. Solo-safety preserved: all 5 threat profiles telegraph + offer a noncombat out + allow retreat + scale for one PC; no four-PC assumptions; combat is never required to level (milestones earnable multiple ways). All new files indexed/tagged (`act:1`); no new proper nouns (registry note added). Stat references reuse existing baselines (specter/wraith/guard/spy/mage-lite), consistent with `SUNDERING_REACH_ENCOUNTERS.md` and the NPC profiles; no copied stat blocks.

**Stage 4 self-check (Caradril):** no contradictions with CANON found (Caradril's map position, ~10–12 day distance, Ledger HQ + Remnant seat all match Stage 1 map/faction canon); no DM-only truth placed in player-facing sections (the "Stilling = harvest's pause," the Vyre–Quorrin deal, the Sealed Archive's M6/M9 proof, the Sunken Wards' network touch, and the Magisterium correspondent are all confined to DM-Only sections and gated); the Hollow Court (M7) is never named in any Caradril file; no new central mystery/faction/god/cosmology/artifact was created; M3/M6/M9 remain reachable outside Caradril (three-clue rule intact); the city is a safe-rest hub with combat confined to the Sunken Wards and telegraphed reprisals (no four-PC assumptions); all new proper nouns registered in NAMING_REGISTRY; all new files indexed and tagged.

---

## Current Issues

| Severity | Issue | File(s) | Why It Matters | Recommended Fix | Status |
|---|---|---|---|---|---|
| Medium | Caradril NPC density (~40) below the Stage 4 target band (75–100) | `08_npcs/SECONDARY_NPCS.md`, `MINOR_NPCS.md`, `caradril_districts/` | Thin city NPC coverage forces improvisation in heavy city play | Expand toward target | open (Stage 9) |
| Medium | No standalone full bestiary; mid/high-tier threats not yet statted | `13_encounters_and_bestiary/` | Acts 2–5 threats not mechanically usable above ~L6 | Build bestiary | open (Stage 13) |
| Medium | No treasure-by-level / `REWARDS_BY_LEVEL.md`; rewards reference "level-appropriate" abstractly | `10_dungeons_and_ruins/`, quest files | AI DM must improvise reward specifics for a solo PC | Build treasure/rewards files | open (Stage 14) |
| Medium | No standalone Acts 2–5 arc files; arc above L4 is shape only | `12_campaign_arc/` | Play beyond L4 not yet runnable in detail | Build act files | open (Stage 15) |
| Low | Individual per-clue files do not exist; clues are tracked in index rows only | `11_mysteries_and_secrets/CLUE_INDEX.md` | Fine for now; finer retrieval may be wanted later | Create per-clue files if play demands | open (Stage 11) |
| Low | `/15_random_tables/` empty (travel/weather/event) | `15_random_tables/` | Mild travel/downtime improvisation burden | Populate when convenient | open (low) |
| Low | NPC relationship/secret/voice tools + `QUEST_INDEX.md` not created | `08_npcs/`, `09_quests/` | QoL tooling for growing rosters/libraries | Create as rosters grow | open (Stages 9–10) |
| Low | "Magisterium correspondent" (Reke ↔ a Caradril magister) is an intentional unresolved lead | `THE_MAGISTERIUM.md`, `HIDDEN_CLUES.md` | By design — must stay a lead, never a named second Court agent, until earned in play | Resolve in Stage 15 play/arc | open (by design) |
| Low | Stage 3 dungeon rewards reference level-appropriate items (e.g. Barrow magic item) not yet statted; `REWARDS_BY_LEVEL.md` does not exist | dungeon files | Rewards are described but not mechanically itemized | Build treasure-by-level | open (Stage 14) |
| Low | `KNOWN_CLUES.md`, `NPC_MEMORY.md`, `RELATIONSHIPS.md`, `INVENTORY_AND_REWARDS.md`, `CONSEQUENCES.md`, `SESSION_RECAP.md` remain at empty baselines | `/02_runtime_state/` | By design — these populate during live play, not pre-play | None; populate in Stage 17 | open (by design) |

---

## Resolved Issues

| Date | Issue | Resolution | Files Updated |
|---|---|---|---|
| 2026-06-10 | **(High)** Act 1 arc spine pointed to two nonexistent quest files (`Q_ACT1_INDEPENDENT_WHAT_THE_FENS_CARRY`, `Q_ACT1_COURT_THE_COUNCILORS_ERRAND`) | Repointed inline during Stage 6 audit: Door 4 → Hook 6 + `Q_SASHES_WARNING.md`; Door 7 → Hook 4 in `HOOKS_TABLE.md` with explicit "no act_1 quest by design" note | `12_campaign_arc/ACT_1_LEVELS_1_4.md` |
| 2026-06-10 | Stages 1–5 content (region, Caradril, Act 1 kit) not independently audited | Stage 6 first full audit run across all 10 categories; foundation verified sound (0 Critical, 1 High fixed, 4 Medium, 5 Low) | `18_audits/STAGE_1_TO_5_AI_READINESS_AUDIT.md`, this file, `TODO.md`, `CONTENT_GAPS.md` |
| 2026-06-09 | `CONTENT_GAPS.md` claimed no regions/settlements/factions/NPCs/quests/arc exist — contradicted Stages 1–2 | Rewrote to reflect Stages 0–2 complete and the real Stage 3+ gaps | `17_generation_backlog/CONTENT_GAPS.md` |
| 2026-06-09 | `EXPANSION_PLAN.md` said Stage 0 complete / Stage 1 not started — two stages stale | Rewrote: Stages 0–2 complete, Stage 3 next, next 5 production passes laid out | `17_generation_backlog/EXPANSION_PLAN.md` |
| 2026-06-09 | `CONSISTENCY_AUDIT.md` said "no campaign content exists" | Rewrote current status and issue list to reflect Stages 1–2 complete | `00_control/CONSISTENCY_AUDIT.md` |
| 2026-06-09 | `CLUE_INDEX.md` was an empty placeholder despite an authored mystery web | Populated with all authored clues (IDs, mystery, method, status=hidden) + three-clue-rule check | `11_mysteries_and_secrets/CLUE_INDEX.md` |
| 2026-06-09 | `HIDDEN_CLUES.md` was an empty placeholder | Seeded with all undiscovered clues at campaign start (location, trigger, status=hidden) | `02_runtime_state/HIDDEN_CLUES.md` |
| 2026-06-09 | Content standards templates did not enforce `DND_MECHANICS_REQUIREMENTS.md` at the field level (Critical TODO) | Added mechanical fields and Mechanical Requirements sections to NPC, quest, content, faction, and worldbuilding standards | `NPC_STANDARDS.md`, `QUEST_STANDARDS.md`, `CONTENT_STANDARDS.md`, `FACTION_STANDARDS.md`, `WORLDBUILDING_STANDARDS.md` |
| 2026-06-09 | Secondary/minor NPC placeholders (Warden Pell, Tallytooth Ren, Bann Oester, Pevin Oss, Custodian Orre) referenced in faction files but unbuilt | All five built as full secondary entries in Stage 3, plus ~16 more secondary and ~35 minor NPCs | `08_npcs/SECONDARY_NPCS.md`, `MINOR_NPCS.md`, `NPC_INDEX.md`, `NAMING_REGISTRY.md` |
| 2026-06-09 | Starting region was a frame only (no settlement spread, wilderness, dungeons, encounter tables) | Stage 3 deep build completed | region/settlement/wilderness/dungeon/quest/encounter files + indexes |

---

## Severity Levels

| Level | Meaning |
|---|---|
| Critical | Breaks campaign, exposes secrets, or prevents AI play |
| High | Likely to confuse AI DM or player; weakens major arc |
| Medium | Weakens usability, retrieval, or play quality |
| Low | Polish issue |

---

## Rules

- Do not bury critical issues.
- Do not delete issues — move to Resolved Issues when fixed.
- Link to audit reports when possible.
- Convert audit findings into TODO tasks.

---

## Related Files

- [`AUDIT_STANDARDS.md`](AUDIT_STANDARDS.md)
- [`TODO.md`](TODO.md)
- [`/17_generation_backlog/CONTENT_GAPS.md`](../17_generation_backlog/CONTENT_GAPS.md)
- `/18_audits/` — formal audit reports
