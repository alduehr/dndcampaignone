# CONSISTENCY_AUDIT.md

## Purpose

Running tracker of known continuity, secrecy, and AI-readiness issues. Not a full audit report — those go in `/18_audits/`. This file tracks issues that need fixing and their resolution status.

## Current Status

**Stages 0, 1, 2, 3, 4, and 5 complete (Stage 5: 2026-06-10).** Foundation + AI runtime + deep-built starting region + first major city (Caradril) + Level 1–4 Act 1 play kit exist and are indexed. No formal AI-readiness audit has been run yet (Stage 6) — Stages 3, 4, and 5 added large bodies of new content that the Stage 6 audit should review for canon consistency, secrecy separation, clue solvability, and solo-play balance.

**Stage 5 self-check (Act 1 play kit):** no contradictions with CANON or Stages 1–4 found — Stage 5 created no new world facts, only play-layer structure (arc spine, milestones, failure redirects, threat profiles, clue-access overlay, NPC casting guide). Reveal cap held at **R1** in every Act 1 file (no Remembrance-as-substance, no Reke-as-traitor, no steering employer, no Concord's sin, no deliberate Quietfall, and **the Hollow Court [M7] is never named or deployed** — and correctly gets no friendly faction quest). DM-only material (hidden faction links in the threat profiles, the clue ceilings, the steering note) is confined to DM-Only sections; `ACT_1_CLUE_TRAILS.md` is dm-only. Three-clue rule preserved: every Act 1 conclusion (R1) has 3–4 independent routes; no single NPC/clue/dungeon/quest is mandatory. Solo-safety preserved: all 5 threat profiles telegraph + offer a noncombat out + allow retreat + scale for one PC; no four-PC assumptions; combat is never required to level (milestones earnable multiple ways). All new files indexed/tagged (`act:1`); no new proper nouns (registry note added). Stat references reuse existing baselines (specter/wraith/guard/spy/mage-lite), consistent with `SUNDERING_REACH_ENCOUNTERS.md` and the NPC profiles; no copied stat blocks.

**Stage 4 self-check (Caradril):** no contradictions with CANON found (Caradril's map position, ~10–12 day distance, Ledger HQ + Remnant seat all match Stage 1 map/faction canon); no DM-only truth placed in player-facing sections (the "Stilling = harvest's pause," the Vyre–Quorrin deal, the Sealed Archive's M6/M9 proof, the Sunken Wards' network touch, and the Magisterium correspondent are all confined to DM-Only sections and gated); the Hollow Court (M7) is never named in any Caradril file; no new central mystery/faction/god/cosmology/artifact was created; M3/M6/M9 remain reachable outside Caradril (three-clue rule intact); the city is a safe-rest hub with combat confined to the Sunken Wards and telegraphed reprisals (no four-PC assumptions); all new proper nouns registered in NAMING_REGISTRY; all new files indexed and tagged.

---

## Current Issues

| Severity | Issue | File(s) | Why It Matters | Recommended Fix | Status |
|---|---|---|---|---|---|
| Medium | No formal AI-readiness audit has been run against Stage 1–2 content | `/18_audits/` (none yet) | Tracking is self-reported; an independent audit may find canon/secrecy/clue gaps | Run Stage 6 first full audit | open (Stage 6) |
| Low | Individual per-clue files do not exist; clues are tracked in index rows only | `11_mysteries_and_secrets/CLUE_INDEX.md` | Fine for now; finer retrieval may be wanted later | Create per-clue files if play demands (Stage 11) | open (deferred) |
| Low | Stage 3 added ~56 new NPCs, 8 settlements, 6 dungeons, 12 quests not yet independently audited | Stage 3 files | Self-reported as consistent/secrecy-separated; a formal audit should confirm | Run Stage 6 audit over Stage 3 content | open (Stage 6) |
| Low | Stage 4 added Caradril (8 districts, 40 city NPCs, 10 quests, hooks/rumors, encounters, 4 factions, 3 clocks) not yet independently audited | Caradril files | Self-reported as consistent/secrecy-separated/solo-safe; a formal audit should confirm (esp. M7 non-exposure and Act-3 gating) | Run Stage 6 audit over Stage 4 content | open (Stage 6) |
| Low | Stage 5 added the Act 1 play kit (arc spine, 6 faction quests, 5 threat profiles, clue-trails overlay, 9 failure states, milestones, NPC guide) not yet independently audited | Stage 5 files | Self-reported as consistent/secrecy-separated/solo-safe with reveals capped at R1 and M7 never named; a formal audit should confirm | Run Stage 6 audit over Stage 5 content | open (Stage 6) |
| Low | "Magisterium correspondent" (Reke ↔ a Caradril magister) is an intentional unresolved lead | `THE_MAGISTERIUM.md`, `HIDDEN_CLUES.md` | By design — must stay a lead, never a named second Court agent, until earned in play | Resolve in Stage 5/15 play/arc | open (by design) |
| Low | Stage 3 dungeon rewards reference level-appropriate items (e.g. Barrow magic item) not yet statted; `REWARDS_BY_LEVEL.md` does not exist | dungeon files | Rewards are described but not mechanically itemized | Build treasure-by-level | open (Stage 14) |
| Low | `KNOWN_CLUES.md`, `NPC_MEMORY.md`, `RELATIONSHIPS.md`, `INVENTORY_AND_REWARDS.md`, `CONSEQUENCES.md`, `SESSION_RECAP.md` remain at empty baselines | `/02_runtime_state/` | By design — these populate during live play, not pre-play | None; populate in Stage 17 | open (by design) |

---

## Resolved Issues

| Date | Issue | Resolution | Files Updated |
|---|---|---|---|
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
