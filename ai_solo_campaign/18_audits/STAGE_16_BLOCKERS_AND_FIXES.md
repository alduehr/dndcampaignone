# Stage 16 — Blockers and Fixes

---
type: audit
secrecy: dm-only
status: static
date: 2026-06-15
tags: [audit, stage-16, blockers, fixes]
related: [STAGE_16_PRE_PLAY_READINESS_AUDIT.md, ../00_control/STAGE_16_PROGRESS.md]
---

## Purpose

Single ledger of every blocker/issue found in the Stage 16 pre-play readiness audit, its severity, and its disposition (fixed / deferred / N-A).

## Blockers Found and Fixed

| # | Severity | Issue | File(s) | Disposition |
|---|---|---|---|---|
| F1 | Medium (non-blocking hygiene) | Stale canon "Current Status" headers (Stage 1 / 1–5 / 1–5 and 7) while project is at Stage 15B. | `03_canon/CANON.md`, `03_canon/PLAYER_SAFE_CANON.md`, `03_canon/DM_ONLY_CANON.md` | **FIXED** — headers updated to "Stages 1–15B complete; Stage 16 underway," each noting later stages changed no core facts. |
| F2 | Medium (non-blocking hygiene) | `MAIN_ARC_OVERVIEW.md` referenced Act 2–5 / endgame files by bare name; those files live in `15_campaign_arcs/`, so the runnable L5–20 arc was not navigable from the legacy overview. | `12_campaign_arc/MAIN_ARC_OVERVIEW.md` | **FIXED** — added a "Where the runnable arc lives (Stage 15/15B)" pointer block routing to `15_campaign_arcs/`. |

## No Critical or High Blockers

No Critical or High issues were found. There were:
- no canon contradictions,
- no player-facing apex-truth leaks,
- no missing runtime state files,
- no break in opening runnability,
- no unfindable level 1–20 arc content,
- no stale top-level stage-status file.

## Deferred / Non-Blocking (logged, not fixed)

| # | Severity | Issue | Where Tracked |
|---|---|---|---|
| D1 | Low | Far-region settlement/NPC deep-builds are light (arc packs lean on Stage 9.5 rosters). | `CONTENT_GAPS.md`, `TODO.md` |
| D2 | Low | Map images not generated (prompts/manifests ready). | `TODO.md` (Medium queue) |
| D3 | Low | `/15_random_tables/` unpopulated. | `TODO.md` (Low) |
| D4 | Low | RtHW bestiary integration pending 2026-06-16 release. | `TODO.md` (Low, blocked) |
| D5 | Low | Lift exact far-region quest titles into `DEVELOPED_QUESTS_INDEX.md` (cosmetic). | `TODO.md` |

## N/A

- No JSON render manifest exists; the markdown manifest is the sole source (already logged in the Stage-13/map audits). Not a play blocker.

## Deep Re-Verification Pass (2026-06-15, second run)

The first Stage 16 pass was shallow, so this ledger was re-checked against the actual files (not index summaries). The deep pass found **zero new blockers** of any severity and required **no content changes**: F1 and F2 were confirmed still correctly fixed; no canon contradiction, apex leak, missing/blank-by-mistake state file, broken file reference, or arc-navigability gap surfaced on a substantive read. One item examined and cleared as a non-defect: `SECRET_REVEAL_PROTOCOL.md` uses the legacy "R1–R8" revelation labels, but `REVELATION_MAP.md` documents the explicit 1:1 R↔REV_001–010 mapping, so the two are consistent.

## Correction Pass (2026-06-16) — Issues the Prior Passes Missed

The first two Stage 16 passes (initial + deep re-verification) declared READY but **overclaimed**: they checked content runnability deeply yet missed several control/retrieval/classification/hygiene defects. A targeted correction pass found and fixed them. None was a content gap — all were navigation, accuracy, or classification issues that would have degraded live play.

| # | Severity | Issue the prior pass missed | File(s) | Disposition |
|---|---|---|---|---|
| C1 | Medium (retrieval) | `RETRIEVAL_GUIDE.md` was stale — said only Stages 1–5 and 7 complete; gave no load guidance for the Stage 8–15B faction/NPC/quest/mystery/dungeon/encounter/treasure/arc systems. | `00_control/RETRIEVAL_GUIDE.md` | **FIXED** — rewritten with a full per-scenario scenario load map covering new-campaign/resume/opening/settlement/region/far-region/dungeon/faction/quest/clue/encounter/treasure/tier-entry/off-route/ignore-arc/endgame, pointing to every Stage 8–15B system that exists on disk. |
| C2 | Medium (accuracy) | `MANIFEST.md` Current Status still said "Stage 1 complete / Stage 2 next." | `00_control/MANIFEST.md` | **FIXED** — status + stage table + folder summary updated to Stages 0–16 complete, Stage 17 next; live-play entry pointer added. |
| C3 | Medium (completeness) | No master `18_audits/PRE_PLAY_READINESS_AUDIT.md` existed — Stage 16's named required output was absent (only the six detailed reports existed). | `18_audits/PRE_PLAY_READINESS_AUDIT.md` | **FIXED** — created as the one-page master verdict pointing to the six detailed reports. |
| C4 | Low (hygiene) | Active-folder `_PLACEHOLDER.md` files still said "Empty — Stage 0 scaffold" for fully populated folders. | `05_regions/`, `06_settlements/`, `07_factions/major_factions/`, `07_factions/minor_factions/`, `08_npcs/`, `09_quests/`, `18_audits/`, `15_random_tables/` placeholders | **FIXED** — each updated to a brief status note reflecting real contents (or, for minor_factions/random_tables, intentional-deferral notes). |
| C5 | Medium (secrecy classification) | Map-render files tagged `secrecy: player-safe` actually contain the apex secret names in "do-not-render" exclusion lists — not safe to hand to the player directly. | `04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md`, `PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md`, `PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET.md` | **FIXED** — reclassified `secrecy: dm-facing-player-safe-output` with an explanatory note: the *output* is player-safe, the *file* is not for direct sharing. |
| C6 | Low (classification) | `LANGUAGES.md` and `LEVELING_ASSUMPTIONS.md` were tagged `player-safe` but contain DM-only references (Old Custodial↔Hollow Court↔inner Custodians; act labels naming the harvest/Concord truth). | `03_canon/LANGUAGES.md`, `03_canon/LEVELING_ASSUMPTIONS.md` | **FIXED** — reclassified `secrecy: mixed` with secrecy notes flagging the DM-only sections; mechanically useful content retained. `PLAYER_SAFE_CANON.md` Hollow-Court entry annotated (name-as-folklore only). |
| C7 | Medium (missing forwarding file) | `REWARDS_BY_LEVEL.md` was referenced by quests/dungeons/standards as "when built" but never created. | `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` | **FIXED** — created as a by-level forwarding/index file over the Stage 14 treasure library; stale "when built" references repointed. |
| C8 | Low (stale tracking) | Stale Medium issues in `CONSISTENCY_AUDIT.md` (no REWARDS_BY_LEVEL, no Acts 2–5, endgame artifacts pending, NPC tools missing) were already resolved by Stages 14/15 but still listed open. | `00_control/CONSISTENCY_AUDIT.md`, `17_generation_backlog/CONTENT_GAPS.md` | **FIXED** — closed/reclassified; Caradril NPC density downgraded to non-blocking optional. |

## Final Cleanup Pass (2026-06-16) — Residual Classification and Stale-Contradiction Fixes

A final cleanup pass after the correction pass cleared residual secrecy classifications and stale Stage 14/15 contradictions the correction pass had not reached. None is a content gap; all are classification/accuracy/navigation fixes.

| # | Severity | Issue | File(s) | Disposition |
|---|---|---|---|---|
| C9 | Medium (secrecy) | The player-safe `PLAYER_SAFE_CANON.md` Hollow Court note named DM-only truths (surviving inner Custodians, the harvest, the Under-Shrine / Drowned Keystone, the Concord Deep). | `03_canon/PLAYER_SAFE_CANON.md` | **FIXED** — reduced to a generic DM warning pointing to `DM_ONLY_CANON.md` + `SECRET_PROTECTION_MATRIX.md`; DM-only names excised from the player-safe body. |
| C10 | Low (classification) | The map render manifest and generation packet were correctly tagged `dm-facing-player-safe-output` but their body text still said "this file is player-safe / contains no DM-only geography." | `04_world_atlas/PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md`, `PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET.md` | **FIXED** — body text corrected: the *output* is player-safe; the *file* is DM-facing (hidden "do not render" names) and is never handed to the player. |
| C11 | Medium (secrecy classification) | `18_audits/PLAYER_SAFE_FULL_CONTINENT_MAP_AUDIT.md` was tagged `secrecy: player-safe` but references the excluded apex names (Concord Deep, Under-Shrine, Drowned Keystone, Hollow Court). | `18_audits/PLAYER_SAFE_FULL_CONTINENT_MAP_AUDIT.md` | **FIXED** — reclassified `secrecy: dm-facing`; added a one-line note that the audit verifies player-safe *output* but is itself not player-facing. |
| C12 | Low (classification) | Four `player-safe` files presented DM-only arc terms (the harvest, Hollow Court, Custodians, Concord Deep, harvest-class relics) as plain content rather than DM guidance. | `13_encounters_and_bestiary/CREATURE_SOURCE_REFERENCE.md`, `BIOME_ENCOUNTER_MATRIX.md`, `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md`, `CONSUMABLES_AND_MINOR_MAGIC.md` | **FIXED** — all four reclassified `secrecy: mixed` with DM secrecy notes; useful AI-DM guidance retained. |
| C13 | Low (stale contradiction) | `CONSISTENCY_AUDIT.md` top status read as though Stage 14 was most recent and endgame artifacts were pending Stage 15. | `00_control/CONSISTENCY_AUDIT.md` | **FIXED** — top status now states Stages 0–16 complete, Stage 15/15B resolved the arc/endgame, Stage 14 reward issues resolved, remaining issues Low/non-blocking only. |
| C14 | Low (stale contradiction) | `REWARD_PLACEMENT_AUDIT.md` Forward Note still said "endgame artifact mechanics intentionally light pending Stage 15." | `14_treasure_and_artifacts/REWARD_PLACEMENT_AUDIT.md` | **FIXED** — added a Stage 15/15B update note pointing to the endgame playbooks + `ARTIFACT_INDEX.md`; note resolved. |
| C15 | Low (stale tracking) | `CONTENT_GAPS.md` NPC section listed major/secondary/minor counts and Ring 1 density as active "below target" gaps despite Stage 9/9.5 output. | `17_generation_backlog/CONTENT_GAPS.md` | **FIXED** — corrected to 94 major / 368 secondary / 953 minor and marked resolved. |
| C16 | Low (accuracy) | `MANIFEST.md` folder map omitted `/15_campaign_arcs` (the current L5–20 arc authority) and did not flag `/12_campaign_arc` as the legacy Act 1 folder. | `00_control/MANIFEST.md` | **FIXED** — added `/15_campaign_arcs` description; clarified `/12_campaign_arc`. |

## Net Result

Prior passes: 2 hygiene issues fixed, 0 new blockers on deep re-verification. Correction pass: **8 control/retrieval/classification/hygiene issues fixed** (C1–C8). Final cleanup pass: **8 residual classification/stale-contradiction fixes** (C9–C16). All 16 fixes are non-content, 0 critical/high. Remaining items are optional/non-blocking (far-region deep-builds, map images, deferred random tables, pending RtHW). Campaign verdict: **READY FOR LIVE PLAY**.
