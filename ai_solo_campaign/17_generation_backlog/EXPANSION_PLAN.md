# EXPANSION_PLAN.md

## Purpose

Forward-looking development roadmap. Tracks what to build next and in what order. This is a roadmap, not a task queue — use `TODO.md` for actionable tasks.

## Current Status

**Stages 0–15/15B complete (Stage 15B Full Character Arc Playability Fill: 2026-06-15).** The campaign now has a deep-built starting region, first major city, Level 1–4 arc, three Ring 1 regions, all 7 factions operational, a full NPC codex (94 major / 368 secondary / 953 minor), a quest library (28 major / ~165 developed / 304 hooks), a complete mystery infrastructure (10 revelations, ~100 clues, 6 regional trail files), **36 authored adventure sites spanning L1–20**, a full encounter/bestiary library, a complete reward layer, and a **full level 5–20 campaign arc** (31 files in `15_campaign_arcs/`: tier overviews, 6 Tier-3 paths, 9 Tier-4 endgame playbooks, 20-region arc packs, continental pressure timeline, transition guide, revelation/ending paths, and completion audit PASS). **Stage 16 — Pre-Play Readiness Audit is the recommended next pass.**

---

## Current Stage

| Field | Value |
|---|---|
| Stage | 16 — Pre-Play Readiness Audit (recommended next) |
| Goal | Full-repo AI-readiness and continuity audit (`18_audits/PRE_PLAY_READINESS_AUDIT.md`). Confirm the first 10–20 sessions are runnable, apex truth is protected, opening scene is ready, runtime state is ready, and no critical issues remain before live play begins. |
| Status | Not started |
| Blocking Issues | None — Stages 0–15/15B complete |

> **Stage 14 — Treasure, Artifacts, and Rewards: COMPLETE 2026-06-14.** 15 files in `14_treasure_and_artifacts/`; 12 artifacts + 38 custom items + 10 cursed + 6 sentient; all 20 regions × 5 level bands; 7+4 faction reward tracks; 36 dungeon reward hooks; reward-placement audit PASS; two-track source handling (no copied official text); solo-tuned; apex truth gated. See `STAGE_14_PROGRESS.md`.

---

## Next Production Passes

### Pass 1 — DONE: Starting Region Deep Build (Stage 3)

**Complete 2026-06-09.** Delivered 8 settlements, 4 wilderness zone-files (~25 sites), 6 dungeons/ruins, ~56 secondary+minor NPCs (~21 secondary + ~35 minor), 14 developed quests, 39 hooks + 50 rumors, and 4 solo-tuned zone encounter tables; clue paths and faction clocks anchored to real sites; all indexed and cross-linked. Targets met or exceeded. (Keystone drowned-shrine dungeon deferred to Stage 12 by design.)

### Pass 2 — DONE: Level 1–4 Play Arc (Stage 5)

**Complete 2026-06-10.** Delivered the open-world Act 1 play kit: the arc spine `ACT_1_LEVELS_1_4.md` (Five Doors + seven faction doors, multi-route to R1, ignore-consequences, Act 2 triggers); 6 faction-alignment quests in `09_quests/act_1_quests/` (Wardens, Compact, Ledger, Mourners, Gravecallers, Remnant — the Hollow Court has none by design); 5 recurring early-threat profiles `ACT_1_THREATS.md` (full stat profiles, solo-safe, scaling); the DM-only `ACT_1_CLUE_TRAILS.md` overlay (existing M1–M9 only; R1 cap; three-clue check); 9 redirect-not-end failure states `ACT_1_FAILURE_STATES.md`; multi-path milestone/XP triggers `ACT_1_MILESTONES.md`; and the Act 1 NPC casting guide `ACT_1_NPC_GUIDE.md`. Runtime ACTIVE_QUESTS/OPEN_THREADS seeded; anti-railroad verified; all L1–4 content mechanically complete; no new central mystery/faction/god/cosmology/artifact; reveals capped at R1. (Act 1 routes dungeon beats through the 6 Stage 3 Concord sites; a dedicated Act 1 climax dungeon is optional/deferred, and the keystone shrine stays Stage 12.)

### Pass 3 — DONE: First Full Audit (Stage 6)

**Complete 2026-06-10.** Ran all 10 audit categories across Stages 1–5. Foundation verified sound: 0 Critical, 1 High (two broken Act 1 arc-spine quest pointers — fixed inline), 4 Medium (Caradril NPC density, bestiary, treasure-by-level, Acts 2–5 — all forward-stage and tracked), 5 Low. Secret separation, three-clue solvability, faction agency, solo-play safety, state tracking, and index completeness all pass clean. Report: `18_audits/STAGE_1_TO_5_AI_READINESS_AUDIT.md`. Scaling to Stage 7 approved.

### Pass 4 — DONE: First Major City Deep Build (Stage 4)

**Complete 2026-06-10.** Built **Caradril**: city overview + 8 district files (incl. the Sunken Wards sub-dungeon), 15 city secondary + 25 city minor NPCs, 11 developed city quests, 36 hooks + 30 rumors, city encounter/social-scene tables, 4 city-internal factions + 3 city clocks (C1/C2/C3), Ledger HQ + Remnant seat located, M2/M3/M4/M6/M8/M9 city clue access added with no new central mysteries. Solo-safe, secrecy-separated, fully indexed/cross-linked. (Full room-by-room dungeon builds for the Sunken Wards and Sealed Archive deferred to Stage 12 by design; the "Magisterium correspondent" left as an intentional open lead for Stage 5/15.)

### Pass 5 — DONE: Regional Expansion Ring 1 (Stage 7)

**Complete 2026-06-10.** Built three adjacent regions: **Ashgarden Vale** (south — 3 settlements; 3 dungeons; **8 quests**; 10 wilderness sites + 3 hamlets; M2/M5/M6 clue access; 2 clocks V1/V2), **Tollwood** (east — 3 settlements; 3 dungeons incl. gated Old Mast; **8 quests**; 10 wilderness sites; 1 minor regional faction the Tollmen; 2 clocks T1/T2), **Pale Coast** (west — 2 settlements + Saltmargin as gateway; 3 dungeons incl. gated Skerry Shrine; **8 quests**; 10 wilderness sites; M2/M3/M5 sea-shrine clue access; 2 clocks C-PC1/C-PC2). Plus `TRAVEL_ROUTES_RING1.md` (6 routes). **~62 Ring 1 NPCs total (29 secondary + 33 minor)** — below the per-region 30–60 target; Ring 1 NPC density deferred to Stage 9 NPC Codex Expansion. All proper nouns registered. Solo-safe, secrecy-separated, fully indexed/cross-linked. No new central mystery/faction/god/cosmology/artifact.

### Pass 6 — DONE: Faction Deepening (Stage 8)

**Complete 2026-06-11.** All seven major factions made fully operational. Delivered: 4-quest chains per faction (28 quest files + 7 `_CHAIN_INDEX.md` files in `09_quests/faction_quests/`); "Combat Capability And Stat References" sections with rank-and-file adversary profiles + leader/champion abbreviated stat profiles added to all seven faction files; `FACTION_RELATIONSHIP_MAP.md` (full pairwise table incl. Hollow Court hidden ties) and `FACTION_TURN_RULES.md` (AI DM inter-session faction turn rules) created; `FACTION_INDEX.md`, `FACTION_STATE.md`, and `WORLD_CLOCKS.md` updated. No new proper nouns, central mysteries, gods, cosmology, or artifacts. Hollow Court secrecy fully preserved. All Stage 8 completion criteria met per `DEVELOPMENT_STAGES.md`.

### Pass 7 — DONE: NPC Codex Expansion (Stage 9)

Complete. 94 major / 368 secondary / 953 minor NPCs; NPC_RELATIONSHIP_WEB, NPC_SECRET_LEDGER, NPC_VOICE_GUIDE created.

### Pass 8 — DONE: Quest Library Expansion (Stage 10)

Complete. 28 major quests, ~165 developed quests, 304 far-continent hooks/rumors/jobs.

### Pass 9 — DONE: Mystery, Secret, Clue Expansion (Stage 11)

Complete. 10 revelations, ~100 clues, 6 regional trail files, faction/NPC knowledge maps, false leads, discovery paths, secret protection matrix.

### Pass 10 — DONE: Dungeons, Ruins, and Adventure Sites (Stage 12)

Complete. 23 authored adventure sites (L1–20), master DUNGEON_INDEX, PUZZLE_DUNGEONS, RUIN_INDEX, STAGE_12_ADVERSARIES.

### Pass 10.5 — DONE: Continental Adventure-Site Coverage (Stage 12.5)

Complete. 13 new far-continent sites (D24–D36); campaign total 36 adventure sites. Every map-authoritative far-continent region has at least one authored site. DUNGEON_INDEX, RUIN_INDEX, PUZZLE_DUNGEONS, CLUE_INDEX, TAG_INDEX, NAMING_REGISTRY updated.

### Pass 11 — DONE: Encounter and Bestiary Expansion (Stage 13)

**Complete 2026-06-14 (cleanup/source-reference pass 2026-06-14).** Built a unified bestiary and encounter library (34 files in `13_encounters_and_bestiary/`): master `ENCOUNTER_INDEX` + `BESTIARY_INDEX` (17 creature categories), copyright-safe two-track `CREATURE_SOURCE_REFERENCE`, `SOLO_ENCOUNTER_SCALING`, 15-biome `BIOME_ENCOUNTER_MATRIX`, `BOSS_AND_APEX_THREATS` (18 bosses B1–B18 with weaknesses/foreshadowing/escape-return logic), original Remembrance `HORROR_AND_CURSE_THREATS`, `FACTION_ENCOUNTERS` (all 7 majors + city + regional), `MYSTERY_ENCOUNTERS`, `TRAVEL_ENCOUNTERS` (all terrains × 5 level-bands 1–20), `DUNGEON_ENCOUNTER_SUPPORT` (all 36 dungeons), `REGIONAL_ENCOUNTER_TABLES`, and an encounter file for every one of the 20 major regions. Officials source-referenced (never stat-block-copied); originals abbreviated; solo-tuned throughout (telegraph, morale, escape, noncombat outs). Cleanup pass mapped Track-A official-monster source shorthands, replaced `_PLACEHOLDER.md` with a folder `README.md`, and added an RtHW (Ravenloft: The Horrors Within, June 16 2026) pending-supplement section. No new factions/NPCs/regions/mysteries/gods/artifacts; apex truth DM-only/gated. See `STAGE_13_PROGRESS.md`.

### Pass 12 — DONE: Treasure, Artifacts, and Rewards (Stage 14)

**Complete 2026-06-14.** Built 15 files in `14_treasure_and_artifacts/`: `TREASURE_INDEX` (master/AI DM load guide), `SOLO_REWARD_BALANCE` (single-PC pacing governor), `MAGIC_ITEM_INDEX` (38 custom items, Common–Legendary), `ARTIFACT_INDEX` (12 named relics, all mystery-gated M1–M9), `CURSED_ITEMS` (10 + 3 endgame-class), `SENTIENT_ITEMS` (6, incl. 1 DM-only Hollow Court plant), `CONSUMABLES_AND_MINOR_MAGIC`, `REGIONAL_TREASURE_TABLES` (all 20 regions × 5 level bands), `FACTION_REWARDS` (7 majors + 4 Caradril blocs, ranked R1–R3 + betrayal), `QUEST_REWARD_INDEX`, `DUNGEON_REWARD_INDEX` (36 authored adventure sites), `NONCOMBAT_REWARDS`, `ECONOMY_AND_PRICING_GUIDE`, `REWARD_PLACEMENT_AUDIT` (PASS — 0 Critical/High/Medium), `README`. Two-track source handling: official D&D items = reference-only (no copied text); custom items = ORIGINAL CAMPAIGN ITEM abbreviated 5e prose. Solo-tuned; endgame artifacts M6–M9 gated; Hollow Court rewards are traps; no apex-truth leaks. 12 artifact proper nouns registered. All Stage 14 completion criteria met. See `STAGE_14_PROGRESS.md`.

---

## Later Expansion (Stages 13–16)

1. **Stage 13** — Encounter and bestiary expansion ← **done 2026-06-14**
2. **Stage 14** — Treasure, artifacts, and rewards (by level) ← **done 2026-06-14**
3. **Stage 15 / 15B** — Level 5–20 arc expansion + full character arc playability fill ← **done 2026-06-15**
4. **Stage 16** — Pre-play readiness audit ← **next**

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
