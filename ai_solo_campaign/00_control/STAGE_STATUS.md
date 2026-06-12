# STAGE_STATUS.md

## Purpose

Live status of each development stage. Updated after every stage completes, partially completes, or is blocked.

## Current Status

**Active Stage:** Stage 9 — NPC Codex Expansion (not started)
**Last Completed Stage:** Stage 8 — Faction Deepening (complete 2026-06-11)

---

## Stage Table

| Stage | Name | Status | Completion | Blocking Issues | Notes |
|---|---|---|---|---|---|
| 0 | Repository Setup | complete | 100% | none | Scaffold created 2026-06-09 |
| 1 | Campaign Foundation | complete | 100% | none | "The Long Remembering" established and locked; all required outputs created and indexed 2026-06-09 |
| 2 | AI Runtime Foundation | complete | 100% | none | All 18 runner protocols + 5 session-pack files written; 8 runtime state files seeded from Stage 1; start/resume prompts ready; all completion criteria met 2026-06-09. Cleanup pass 2026-06-09: stale tracking files (CONTENT_GAPS, EXPANSION_PLAN, CONSISTENCY_AUDIT) corrected; CLUE_INDEX + HIDDEN_CLUES populated; D&D mechanical fields added to the 5 content-standards templates (Critical TODO cleared) |
| 3 | Starting Region Deep Build | complete | 100% | none | 2026-06-09: 8 settlements, 4 wilderness zone-files (~25 sites), 6 dungeons/ruins, ~56 new NPCs (~21 secondary + ~35 minor), 14 developed quests, 39 hooks + 50 rumors, 4 zone encounter tables; all indexed/cross-linked; clue access anchored to the existing mystery web; clocks anchored to region sites. Targets met or exceeded. Keystone drowned shrine dungeon deferred to Stage 12 by design |
| 4 | First Major City Deep Build | complete | 100% | none | 2026-06-10: **Caradril** deep-built — city overview + 8 district files (incl. the Sunken Wards sub-dungeon), 15 city secondary + 25 city minor NPCs, 11 developed city quests, 36 hooks + 30 rumors, city encounter/social-scene tables; 4 city-internal factions + 3 city clocks (C1/C2/C3); city clue access feeds existing M2/M3/M4/M6/M8/M9; Ledger HQ + Remnant seat located; all indexed/cross-linked. Targets met or exceeded. No new central mystery/faction/god/cosmology/artifact created |
| 5 | Level 1–4 Play Arc | complete | 100% | none | 2026-06-10: open-world Act 1 play kit — arc spine + 6 faction-alignment quests (`act_1_quests/`) + 5 recurring early-threat profiles (`ACT_1_THREATS.md`) + Act 1 clue-trails overlay (existing M1–M9; R1 cap) + 9 failure-redirect states + L2/3/4 milestone/XP triggers + Act 1 NPC casting guide; runtime ACTIVE_QUESTS/OPEN_THREADS seeded; anti-railroad verified; all L1–4 content mechanically complete. No new central mystery/faction/god/cosmology/artifact; reveals capped at R1; Hollow Court never exposed (no friendly Court quest by design) |
| 6 | First Full Audit | complete | 100% | none | 2026-06-10: all 10 audit categories run across Stages 1–5; foundation sound (0 Critical, 1 High fixed inline, 4 Medium, 5 Low). Report: `18_audits/STAGE_1_TO_5_AI_READINESS_AUDIT.md`. Scaling to Stage 7 approved |
| 7 | Regional Expansion Ring 1 | complete | 100% | none | 2026-06-10: three adjacent regions deep-built — **Ashgarden Vale** (S), **Tollwood** (E), **Pale Coast** (W). 3 region files + 8 settlements (Saltmargin reused as Coast gateway) + 3 wilderness files (10 named sites per region; Ashgarden also has 3 hamlets) + 9 dungeons (3 gated higher-tier) + 3 encounter tables + 66 hooks/60 rumors + **24 developed regional quests (8 per region)** + ~62 Ring 1 NPCs (29 secondary + 33 minor; below per-region target of 30–60 — expand in Stage 9) + 1 minor regional faction (the Tollmen) + **6 regional clocks (2 per region: V1/V2, T1/T2, C-PC1/C-PC2)** + `TRAVEL_ROUTES_RING1.md` (6 routes). Player can leave the Reach in 3 directions; all routes funnel to Caradril. No new central mystery/major faction/god/cosmology/artifact; gated/oblique reveals feed existing M2/M3/M5 (gated M6); Hollow Court never named. All indexed/cross-linked |
| 8 | Faction Deepening | complete | 100% | none | 2026-06-11: all 7 major factions made fully operational — 4-quest chains per faction (28 quests + 7 chain indexes in `09_quests/faction_quests/`); "Combat Capability And Stat References" sections with rank-and-file adversary profiles added to all 7 faction files; `FACTION_RELATIONSHIP_MAP.md` (full pairwise + Hollow Court hidden ties + blocs) and `FACTION_TURN_RULES.md` (between-session behavior) created; `FACTION_INDEX.md`/`FACTION_STATE.md`/`WORLD_CLOCKS.md` updated with chain-lever references. Every faction has agency, a clock, named members at multiple levels, quests (join/oppose/from/against), and can help/hinder/recruit/deceive/retaliate. No new proper nouns/central mystery/major faction/god/cosmology/artifact; Hollow Court secrecy preserved (DM-only chain; no early recruit). All completion criteria met |
| 9 | NPC Codex Expansion | not started | 0% | — | Depends on Stages 1, 3 |
| 10 | Quest Library Expansion | not started | 0% | — | Depends on Stages 3, 8 |
| 11 | Mystery, Secret, Clue Expansion | not started | 0% | — | Depends on Stage 1 |
| 12 | Dungeons, Ruins, Adventure Sites | not started | 0% | — | Depends on Stage 3 |
| 13 | Encounter and Bestiary Expansion | not started | 0% | — | Depends on Stage 3 |
| 14 | Treasure, Artifacts, Rewards | not started | 0% | — | Depends on Stages 1, 5 |
| 15 | Level 5–20 Arc Expansion | not started | 0% | — | Depends on Stages 5, 6 |
| 16 | Pre-Play Readiness Audit | not started | 0% | — | Depends on all prior stages |
| 17 | Live Campaign Operation | not started | 0% | — | Begins after Stage 16 |
| 18 | Periodic Live Audits | not started | 0% | — | Ongoing during Stage 17 |
| 19 | Campaign Completion and Epilogues | not started | 0% | — | End of campaign |

---

## Completion Percentage Guide

| % | Meaning |
|---|---|
| 0% | Not started |
| 25% | Skeleton exists |
| 50% | Substantial content, gaps remain |
| 75% | Usable, needs audit/fixes |
| 90% | Audit complete, minor gaps only |
| 100% | All completion criteria met per DEVELOPMENT_STAGES.md |

---

## Related Files

- [`DEVELOPMENT_STAGES.md`](DEVELOPMENT_STAGES.md)
- [`PROGRESS_LOG.md`](PROGRESS_LOG.md)
- [`TODO.md`](TODO.md)
- [`MANIFEST.md`](MANIFEST.md)
