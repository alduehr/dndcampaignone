# STAGE_11_PROGRESS.md

## Stage 11 Objective

Mystery, Secret, and Clue Expansion for "The Long Remembering." Make the campaign's secrets deep, fair, discoverable, and AI-runnable. Build a formal revelation map (REV-IDs, each with >=3 independent clue sources), expand the clue index with region-coded IDs and redundancy paths, author regional clue trails (5 home regions + far-continent echoes), faction & NPC knowledge maps, false leads, discovery paths, a DM-only secret protection matrix, and a live mystery-state tracker template. Cross-link Stage 10 quests to clues/revelations. Run a secrecy audit. **Preserve all established canon (M0-M10, the harvest, the deliberate Quietfall, the Hollow Court keystone). Never leak apex truth into player-safe text.**

## Prerequisite Bookkeeping (checked)

- `09_quests/QUEST_INDEX.md` — already shows Stage 10 complete with correct counts (28 major / ~165 developed / 304 fc hooks-rumors-jobs). NO FIX NEEDED.
- `00_control/STAGE_10_PROGRESS.md` — already final/complete, no Run-2 continuation prompt. NO FIX NEEDED.
- `09_quests/DEVELOPED_QUESTS_INDEX.md` — titles match region files (full title tables present). NO FIX NEEDED.

## Files Read (context)

STAGE_STATUS, CONTENT_INDEX, MYSTERY_STANDARDS, CANON_AUTHORITY, GENERATION_GUARDRAILS, NAMING_REGISTRY (via CLAUDE.md), CANON, DM_ONLY_CANON, PLAYER_SAFE_CANON, WORLD_HISTORY, MYSTERY_WEB, CLUE_INDEX, REVELATION_MAP, SECRET_INDEX, ACT_1_CLUE_TRAILS, CLUE_DELIVERY_PROTOCOL, SECRET_REVEAL_PROTOCOL, MAIN_ARC_OVERVIEW, NPC_INDEX, NPC_SECRET_LEDGER, MAJOR_CAMPAIGN_QUESTS (head), QUEST_INDEX, DEVELOPED_QUESTS_INDEX, STAGE_10_PROGRESS, HIDDEN_CLUES, HOLLOW_COURT (head).

## Existing Infrastructure Assessment (Task 1 audit — in progress)

The Stage-1 mystery web is mature and well-built:
- M0-M10 mysteries, each with 3-4 authored clue paths (three-clue rule met).
- REVELATION_MAP has R1-R8 with act/level pacing and "must not leak" guards.
- SECRET_INDEX has 20 numbered secrets with reveal conditions.
- CLUE_INDEX has C-M<n>-<k> clues + Stage 3/4 region anchors.
- NPC_SECRET_LEDGER is effectively a near-complete NPC knowledge map already (94 majors routed by secret tier + mystery fed).
- Hollow Court (M7) protection is consistent and strong across all files.

**Stage 11 approach:** ADD a formal REV-ID revelation layer and the seven new map/index files the spec requires, EXTEND (not replace) the existing web, and cross-link Stage 10 quests + far-continent echoes. Preserve all M-codes and R-codes; map REV-IDs onto them.

## Files Created

- `11_mysteries_and_secrets/by_region/SUNDERING_REACH_CLUES.md`
- `11_mysteries_and_secrets/by_region/CARADRIL_CLUES.md`
- `11_mysteries_and_secrets/by_region/ASHGARDEN_VALE_CLUES.md`
- `11_mysteries_and_secrets/by_region/TOLLWOOD_CLUES.md`
- `11_mysteries_and_secrets/by_region/PALE_COAST_CLUES.md`
- `11_mysteries_and_secrets/by_region/FAR_CONTINENT_ECHO_CLUES.md`
- `00_control/STAGE_11_PROGRESS.md`
- (pending: FACTION_KNOWLEDGE_MAP, NPC_KNOWLEDGE_MAP, FALSE_LEADS_AND_MISDIRECTIONS, DISCOVERY_PATHS, SECRET_PROTECTION_MATRIX, MYSTERY_STATE_TRACKER_TEMPLATE, audit)

## Files Modified

- `11_mysteries_and_secrets/REVELATION_MAP.md` (added formal REV_001-REV_010 layer; dependency graph; per-REV 3+ sources)
- `11_mysteries_and_secrets/CLUE_INDEX.md` (added region-coded clue layer + per-REV three-source verification table)
- `11_mysteries_and_secrets/MYSTERY_WEB.md` (added 7-layer mystery hierarchy + far-continent echo cross-reference)

## Running Counts

- Revelations mapped (REV-IDs): 10 (REV_001-REV_010), each >=3 independent sources
- Clue sources per major revelation (range): 3-8 (min REV_007 = 3 via convergence; max REV_002 = 8+)
- Region-coded clues added to CLUE_INDEX: ~60 (C_SR_* 38, C_CAR_* 12, Ring1/far ~15)
- Regional clue trail files: 6/6
- Faction knowledge coverage: 7/7 (FACTION_KNOWLEDGE_MAP.md; Hollow Court section apex-DM-only)
- NPC knowledge entries: ~60 mapped (apex/mid/surface tiers + old-songs network + cover-up + far + false-lead creators) in NPC_KNOWLEDGE_MAP.md
- False leads: 9 (FL_001-FL_009), all fair/recoverable
- Discovery paths: pending (next)
- Created: FACTION_KNOWLEDGE_MAP.md, NPC_KNOWLEDGE_MAP.md, FALSE_LEADS_AND_MISDIRECTIONS.md
- Pending: DISCOVERY_PATHS, SECRET_PROTECTION_MATRIX, MYSTERY_STATE_TRACKER_TEMPLATE, quest cross-links, audit, index updates

## FINAL STATE — Stage 11 COMPLETE (2026-06-13)

### Files Created (11)
- `11_mysteries_and_secrets/by_region/SUNDERING_REACH_CLUES.md`
- `11_mysteries_and_secrets/by_region/CARADRIL_CLUES.md`
- `11_mysteries_and_secrets/by_region/ASHGARDEN_VALE_CLUES.md`
- `11_mysteries_and_secrets/by_region/TOLLWOOD_CLUES.md`
- `11_mysteries_and_secrets/by_region/PALE_COAST_CLUES.md`
- `11_mysteries_and_secrets/by_region/FAR_CONTINENT_ECHO_CLUES.md`
- `11_mysteries_and_secrets/by_faction/FACTION_KNOWLEDGE_MAP.md`
- `11_mysteries_and_secrets/NPC_KNOWLEDGE_MAP.md`
- `11_mysteries_and_secrets/FALSE_LEADS_AND_MISDIRECTIONS.md`
- `11_mysteries_and_secrets/DISCOVERY_PATHS.md`
- `11_mysteries_and_secrets/SECRET_PROTECTION_MATRIX.md`
- `11_mysteries_and_secrets/MYSTERY_STATE_TRACKER_TEMPLATE.md`
- `18_audits/STAGE_11_MYSTERY_SECRECY_AUDIT.md`
- `00_control/STAGE_11_PROGRESS.md`
(13 new content/audit files + this progress file)

### Files Modified (8)
- `11_mysteries_and_secrets/REVELATION_MAP.md`
- `11_mysteries_and_secrets/CLUE_INDEX.md`
- `11_mysteries_and_secrets/MYSTERY_WEB.md`
- `11_mysteries_and_secrets/SECRET_INDEX.md`
- `09_quests/MAJOR_CAMPAIGN_QUESTS.md`
- `00_control/STAGE_STATUS.md`
- `00_control/CONTENT_INDEX.md`
- `00_control/TODO.md`

### Final Counts
- Revelations mapped: **10** (REV_001–REV_010)
- Clue sources per major revelation: **range 3–8** (min REV_007 = 3 via convergence; max REV_002 = 8+)
- Region-coded clues added to CLUE_INDEX: ~60 (C_SR_ 38, C_CAR_ 12, Ring1/far ~14) layered onto the existing ~40 C-M* clues
- Regional clue trails: **6/6** (5 home + far-continent echoes)
- Faction knowledge coverage: **7/7** (Hollow Court section apex-DM-only)
- NPC knowledge entries: **~60** mapped by tier
- False leads: **9** (FL_001–FL_009), all fair/recoverable
- Discovery paths: **10** playstyles
- Player-safe / DM-only separation checks: passed (all 16 mystery files dm-only; player-safe canon clean; quest apex-refs in labeled DM blocks)

### Secrecy Audit Result
0 Critical / 0 High / 2 Medium / 3 Low. No apex-truth leaks in player-safe text. See `18_audits/STAGE_11_MYSTERY_SECRECY_AUDIT.md`.

### Completion Criteria Check (all met)
- [x] Major revelations mapped (REVELATION_MAP)
- [x] Every major revelation has >=3 independent clue sources
- [x] CLUE_INDEX expanded and usable
- [x] Regional clue trails for 5 home regions + far-continent echoes
- [x] FACTION_KNOWLEDGE_MAP covers all 7 factions
- [x] NPC_KNOWLEDGE_MAP covers major NPCs
- [x] FALSE_LEADS_AND_MISDIRECTIONS exists
- [x] DISCOVERY_PATHS exists
- [x] SECRET_PROTECTION_MATRIX exists (dm-only)
- [x] MYSTERY_STATE_TRACKER_TEMPLATE exists (blank/instructional)
- [x] Stage 10 quests cross-linked to clues/revelations
- [x] Secrecy audit completed and documented
- [x] No Critical/High player-safe leaks
- [x] STAGE_11_PROGRESS, STAGE_STATUS, CONTENT_INDEX, TODO updated honestly

## Cleanup Pass — COMPLETE (2026-06-13)

### Files Created in Cleanup
- `11_mysteries_and_secrets/MYSTERY_CHAINS.md` — navigation wrapper/index
- `11_mysteries_and_secrets/FALSE_LEADS.md` — alias pointing to FALSE_LEADS_AND_MISDIRECTIONS.md
- `11_mysteries_and_secrets/REVEAL_TIMING.md` — phase gate quick-reference chart (REV_001–010)
- `11_mysteries_and_secrets/PROPHECIES_AND_OMENS.md` — omen delivery policy

### Files Modified in Cleanup
- `02_runtime_state/HIDDEN_CLUES.md` — Stage 11 region-coded clue layer anchor section added (Medium M1 gap resolved)
- `00_control/CONTENT_INDEX.md` — 4 new wrapper file entries added
- `00_control/TAG_INDEX.md` — Current Status + Stage 11 sections updated
- `00_control/NAMING_REGISTRY.md` — Current Status note updated (Stages 0–11 complete; Stage 12 next)
- `00_control/CONTENT_GAPS.md` — Current Status updated
- `00_control/EXPANSION_PLAN.md` — Current Stage updated
- `00_control/CONSISTENCY_AUDIT.md` — Stage 11 self-check prepended
- `00_control/OPEN_QUESTIONS.md` — Status line updated
- `00_control/PROGRESS_LOG.md` — Cleanup pass entry added
- `00_control/TODO.md` — Medium M1 gap marked resolved; cleanup pass entry added to Completed Recently
- `00_control/STAGE_STATUS.md` — Stage 11 row updated with cleanup note

### Open Gaps After Cleanup (non-blocking)
- (Medium M2) 11 of 12 far-quest files verified by negative grep only; light confirming read recommended in Stage 12.
- (Low) Dual clue-ID scheme documented but not consolidated; optional per-quest far clue tags.

## Open Gaps (non-blocking)

- ~~(Medium M1) Runtime `HIDDEN_CLUES.md` still tracks only C-M* IDs; mirror region-coded IDs in a future runtime pass.~~ **RESOLVED — cleanup pass 2026-06-13.**
- (Medium M2) 11 of 12 far-quest files verified by negative grep (no UNSAFE strings) rather than full read; Heartlands spot-verified line-by-line. Light confirming read recommended in Stage 12.
- (Low) Dual clue-ID scheme (C-M* + region-coded) documented but not consolidated; per-quest far clue tags optional.

## Known Risks (mitigated)

- REV-IDs map cleanly onto existing M/R codes (no contradiction). ✓
- Far-continent echoes kept oblique (no keystone mechanism, no Court). ✓
- SECRET_PROTECTION_MATRIX + FACTION_KNOWLEDGE_MAP Hollow Court section dm-only and never surfaced. ✓

## Continuation Prompt (if context limit reached)

Not needed — Stage 11 complete.
