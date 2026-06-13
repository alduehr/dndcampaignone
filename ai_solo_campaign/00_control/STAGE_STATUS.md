# STAGE_STATUS.md

## Purpose

Live status of each development stage. Updated after every stage completes, partially completes, or is blocked.

## Current Status

**Active Stage:** Stage 12 (Dungeons, Ruins, Adventure Sites) — next
**Last Completed Stage:** Stage 11 — Mystery, Secret, Clue Expansion (complete 2026-06-13)

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
| 9 | NPC Codex Expansion | complete | 100% | none | 2026-06-12 (pass 1 + pass 2 + completion/cleanup pass): created 3 infrastructure files (`NPC_RELATIONSHIP_WEB.md`, `NPC_SECRET_LEDGER.md` [DM-only], `NPC_VOICE_GUIDE.md`); expanded from 20 → **50 major NPCs** (pass-1 +12: Drane, 3 Ring-1 Mourner anchors, 8 Caradril majors C25–C32; pass-2 +18: `by_region/STAGE_9_MAJOR_NPCS.md` — M33–M48 + M49b/M50b); **secondary ~64→~200** (`STAGE_9_SECONDARY_NPCS.md`, waves 1–7); **minor 92→521** (`STAGE_9_MINOR_NPCS.md` waves 1–7 [403] + base [92] + far-continent scaffold [26]). Completion pass (2026-06-12) re-counted honestly, added Voice Guide entries for all 30 Stage 9 majors (guide now covers all 50), added a Wave-7 minor buffer (16) to put the minor pool comfortably past 500, and reconciled all count references. All targets met (50–100 major: **50 ✓**, 200–500 secondary: **~200 ✓**, 500+ minor: **521 ✓**). Voice/relationship/secret infrastructure covers all 50 majors. Faction ladders complete; Hollow Court secrecy preserved; no new factions/gods/mysteries/artifacts. All indexes reconciled |
| 9.5 | Full-Continent NPC Readiness | complete | 100% | none | 2026-06-12 (+ honest-recount cleanup pass 2026-06-12): 12 far-continent region NPC files created (`08_npcs/by_region/{VERDANCE_REACHES,CONCORD_HEARTLANDS,GLASSMERE_LEAGUE,HETHEWALD_FREE_HOLDS,HOLLOW_GULF_PORTS,SALTMERE_REACHES,EMBERFELL_THEOCRACY,SALLOWMARCH_PROTECTORATE,MARROWDOWNS,WENDER_STEPPE,KARRAN_MARCHES,SUNMARK}_NPCS.md`); **44 major / 168 secondary [164 distinct-authored + 4 cross-listed] / 432 minor** (verified by hand + script; cumulative: 94 major / 368 secondary / 953 minor). Cleanup pass added 6 secondary NPCs (Marek Bonepan, Edony Marrow, Tamur-Sai, Hessa Teeth, Tamsin Greenway, Pell Sallows) to bring 5 regions 11→12 and Sallowmarch to 12 distinct-authored, and registered all Stage 9.5 **light NPC-facing anchors** in NAMING_REGISTRY. Relationship web, secret ledger, and voice guide cover all 44 majors. **No new major geography created; several lightweight NPC-facing anchors were added and registered — these are not full settlements or major map features.** No new factions; no far-region NPC knows the apex truth (Hollow Court / harvest never exposed); pre-Concord echoes (Saltmere/Marrowdowns/Karran Old Iron forts) and thematic mirrors (Emberfell) kept distinct from the Hollowmere keystone. All 12 regions meet minimums (3+ major, 12+ secondary, 30+ minor). `FAR_CONTINENT_NPCS.md` superseded (retained for compatibility). NAMING_REGISTRY + NPC_INDEX + CONTENT_INDEX + STAGE_9_5_PROGRESS reconciled and in agreement |
| 10 | Quest Library Expansion | complete | 100% | none | 2026-06-12: **28 major campaign quests** (`09_quests/MAJOR_CAMPAIGN_QUESTS.md`, Q_MAJOR_001–028) + **82 far-continent developed quests** across all 12 regions (`09_quests/by_region/*_QUESTS.md`; 82 unique IDs verified, no collisions) bringing total developed quests to **~165** (~83 pre-Stage-10 + 82) + **304 far-continent hooks/rumors/jobs** (13 `fc_*` files: 132 hooks + 104 rumors + 68 jobs) on top of ~281 pre-Stage-10 home-region hooks/rumors. All 7 major factions have quest coverage (Stage 8 chains + Stage 10 anti-Ledger/Remnant/Mourner/Gravecaller far-continent quests). Indexes created: `DEVELOPED_QUESTS_INDEX.md`, `HOOKS_JOBS_RUMORS_INDEX.md`, `by_level/`, `by_faction/`, `by_type/`; `QUEST_INDEX.md` updated. **No apex-truth leaks in player-facing text** (Hollow Court/harvest/keystone/Under-Shrine DM-only; far-region echoes oblique & DM-labeled); all NPC names from authored Stage 9.5 rosters; no canon contradictions. All completion criteria met. See `STAGE_10_PROGRESS.md`. Depends on Stages 3, 8 (met) |
| 11 | Mystery, Secret, Clue Expansion | complete | 100% | none | 2026-06-13: formal **REVELATION_MAP** layer (REV_001-REV_010, each >=3 independent clue sources spanning regions/NPCs/approaches; dependency graph; phase gates) + region-coded **CLUE_INDEX** expansion (~60 C_SR_/C_CAR_/C_AV_/C_TW_/C_PC_/C_FC_ clues + per-REV three-source verification) + 7-layer **mystery hierarchy** + far-continent echo cross-reference in MYSTERY_WEB. New files: 6 regional clue trails (`by_region/{SUNDERING_REACH,CARADRIL,ASHGARDEN_VALE,TOLLWOOD,PALE_COAST}_CLUES.md` + `FAR_CONTINENT_ECHO_CLUES.md`), `by_faction/FACTION_KNOWLEDGE_MAP.md` (all 7 factions; Hollow Court section apex-DM-only), `NPC_KNOWLEDGE_MAP.md` (~60 NPCs by knowledge tier), `FALSE_LEADS_AND_MISDIRECTIONS.md` (9 fair/recoverable leads), `DISCOVERY_PATHS.md` (10 playstyles, anti-railroad), `SECRET_PROTECTION_MATRIX.md` (DM-only; 7 apex secrets w/ safe/unsafe wording + gates), `MYSTERY_STATE_TRACKER_TEMPLATE.md` (blank runtime tracker). Stage 10 quests cross-linked to REV/clue IDs (MAJOR_CAMPAIGN_QUESTS table). Secrecy audit (`18_audits/STAGE_11_MYSTERY_SECRECY_AUDIT.md`): 0 Critical / 0 High / 2 Medium / 3 Low — no apex-truth leaks in player-safe text; all 16 mystery files dm-only; every REV solvable via multiple paths. No new central mystery/faction/god/cosmology/artifact; M0-M10 preserved; Hollow Court protection strengthened. **Cleanup pass 2026-06-13:** 4 wrapper files created (MYSTERY_CHAINS, FALSE_LEADS, REVEAL_TIMING, PROPHECIES_AND_OMENS); region-coded clue ID layer mirrored into HIDDEN_CLUES.md; CONTENT_INDEX/TAG_INDEX/NAMING_REGISTRY/tracking files updated |
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
