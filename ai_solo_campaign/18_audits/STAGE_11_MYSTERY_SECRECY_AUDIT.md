# Audit Report: Stage 11 Mystery & Secrecy Audit

---
type: audit
secrecy: dm-only
status: static
related: [../11_mysteries_and_secrets/SECRET_PROTECTION_MATRIX.md, ../03_canon/DM_ONLY_CANON.md, ../03_canon/PLAYER_SAFE_CANON.md]
tags: [audit, secrecy, mystery, stage-11, dm-only]
---

## Scope

Targeted secrecy + mystery-solvability audit run during Stage 11 across: all `11_mysteries_and_secrets/` files (incl. the 11 new Stage 11 files), `09_quests/MAJOR_CAMPAIGN_QUESTS.md`, the 12 `09_quests/by_region/*_QUESTS.md` far-continent quest files, `08_npcs/NPC_SECRET_LEDGER.md`, `03_canon/PLAYER_SAFE_CANON.md`, `03_canon/DM_ONLY_CANON.md`, and the Act 1 clue-trail files. Checked for: premature exposure of apex DM-only truths (the harvest, the deliberate Quietfall, the Hollow Court, the Under-Shrine/Drowned Keystone, the Concord Deep, the death-rite-machine truth), correct secrecy metadata, three-clue-rule compliance, dead-end clue chains, and false-lead fairness.

## Summary

**Healthy. 0 Critical, 0 High, 2 Medium, 3 Low.** The pre-Stage-11 mystery infrastructure was already well-protected and the Stage 11 additions preserved and strengthened it. No apex DM-only truth leaks into any player-safe file. Every apex reference in quest/region files sits inside a clearly labeled DM-Only / Hidden Truth / Critical Secrecy block. All 16 mystery files carry `secrecy: dm-only`. Every major revelation (REV_001-REV_010) has >=3 independent clue sources spanning different regions/NPCs/approaches; no single point of failure; no dead-end chains found. All 9 false leads are fair and recoverable.

## Critical Findings

*(none)*

## High Findings

*(none)*

## Medium Findings

| Issue | File(s) | Why It Matters | Recommended Fix |
|---|---|---|---|
| M1 | (runtime) `02_runtime_state/HIDDEN_CLUES.md` | The new region-coded clue IDs (C_SR_*/C_CAR_*/C_FC_*) are tracked in `CLUE_INDEX.md` but the runtime `HIDDEN_CLUES.md` still lists only the original `C-M*` IDs. | Non-blocking: the C-M* set still covers the same clues; a future runtime pass can mirror the region-coded IDs into HIDDEN_CLUES for 1:1 REV tracking. Flagged for Stage 12/runtime. |
| M2 | `09_quests/by_region/*_QUESTS.md` (other 11 files) | Only the Heartlands far-quest file was spot-verified line-by-line for apex protection; the other 11 were verified by negative grep (no UNSAFE strings) but not full read. | Low risk (grep clean + Stage 10 already audited them); recommend a light confirming read during Stage 12 dungeon work. |

## Low Findings

| Issue | File(s) | Why It Matters | Recommended Fix |
|---|---|---|---|
| L1 | `MYSTERY_WEB.md` | Now carries both the legacy `M0-M10` web and the new `REV_*` layer (via REVELATION_MAP); a reader must cross-file to map them. | Acceptable; each REV entry names its legacy R/M codes. Optional future consolidation. |
| L2 | `CLUE_INDEX.md` | Dual ID scheme (`C-M*` and `C_REGION_*`) could confuse a fast reader. | Mitigated by an explicit note in the status section explaining the mapping. |
| L3 | Far-quest clue cross-links | Far-continent *developed* quests (82) are cross-linked at the region-echo level (`FAR_CONTINENT_ECHO_CLUES.md`) rather than per-quest. | Acceptable for echo content; per-quest clue tags optional in a future polish pass. |

## Apex-Truth Exposure Check (player-safe files)

Searched player-safe files for UNSAFE strings (per `SECRET_PROTECTION_MATRIX.md` audit list). Results:
- `PLAYER_SAFE_CANON.md`: only safe hits — "harvest-moot" (the Vale council, a farming term, not the death-harvest) and "the Hollow Court — a legend ... ghost story" (the correct legend framing). **No leak.**
- `WORLD_HISTORY.md`: True Timeline correctly under a "DM-ONLY — never reveal" header; Public Timeline says the Quietfall's cause was "never officially explained." **No leak.**
- All `09_quests/by_region/*_QUESTS.md`: apex references confined to labeled DM-Only/Critical-Secrecy blocks. **No leak.**
- `NPC_SECRET_LEDGER.md`: correctly `secrecy: dm-only`. **No leak.**
- All 16 `11_mysteries_and_secrets/` files: `secrecy: dm-only`. **No leak.**

## Three-Clue-Rule / Solvability Check

- Every REV_001-REV_010 has **>=3 independent clue sources** (verified in `CLUE_INDEX.md` "Per-REV Three-Source Verification" and `REVELATION_MAP.md`). Range 3-8 sources.
- REV_007 (apex) has no single-source path: convergence of 3 prior REVs, OR a lethal-telegraphed physical descent, OR a heretic/forbidden contact.
- **No dead-end chains:** `DISCOVERY_PATHS.md` confirms 10 playstyles each reach every REV; universal redirect rules + world-clocks backstop a passive player.
- **No required-roll/required-NPC/required-region gates** on any REV.

## False-Lead Fairness Check

All 9 false leads (FL_001-FL_009) verified fair per `MYSTERY_STANDARDS.md`: each has a reason to exist, is disprovable, teaches/points to real content, and never blocks progress. FL_006 (Court = ghost story) and FL_008 (far ruins = the heart) are *deliberately* kept until the apex gate — correct protective design, documented.

## Exposed Secrets

*(none)*

## Solo-Play Risks

*(none new)* — apex sites are lethal-telegraphed; no REV requires winning a fight; clocks deliver truth to a passive player.

## Mystery/Clue Risks

*(none Critical/High)* — see Medium M1 (runtime ID mirroring) for the only follow-up.

## Recommended Fix Order

1. (Medium M1) During the next runtime/state pass, mirror region-coded clue IDs into `HIDDEN_CLUES.md` for 1:1 REV tracking. *(non-blocking)*
2. (Medium M2) Light confirming read of the other 11 far-quest files during Stage 12. *(non-blocking)*
3. (Low L1-L3) Optional consolidation/polish of the dual ID scheme and per-quest far clue tags. *(non-blocking)*

## Conclusion

Stage 11 secrecy posture is sound. No Critical or High issues. The apex truth (harvest / deliberate Quietfall / Hollow Court / Under-Shrine / Concord Deep / death-rite machine) is fully protected; the mystery is fair and solvable through multiple paths for every playstyle. Cleared to mark Stage 11 complete.
