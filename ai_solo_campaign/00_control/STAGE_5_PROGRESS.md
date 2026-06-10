# STAGE_5_PROGRESS.md

## Current Stage 5 Objective

Build the **Level 1–4 Open-World Play Kit** for "The Long Remembering." An open-world Act 1 toolkit (not a railroad) that lets an AI DM run levels 1–4 across many possible early paths. Uses existing M1–M9 mysteries, existing major/secondary NPCs, existing factions, existing clocks, existing dungeons. Creates NO new central mysteries, factions, gods, cosmology, or artifacts. Foreshadows 5–8 only; all mechanics stay level 1–4.

## Plan (production batches)

1. **ACT_1_LEVELS_1_4.md** (campaign_arc) — open-world arc spine.
2. **act_1_quests/** folder — 7 faction-aligned developed quests (1 per major faction), QUEST_STANDARDS format, level 1–4, solo-safe.
3. **ACT_1_THREATS.md** (encounters) — 3+ recurring early threat profiles, full adversary stat refs.
4. **ACT_1_CLUE_TRAILS.md** (mysteries) — maps existing clues most likely encountered L1–4, multiple routes, three-clue rule. No new mysteries.
5. **ACT_1_FAILURE_STATES.md** (campaign_arc) — redirect-not-end failure cases.
6. **ACT_1_MILESTONES.md** (campaign_arc) — explicit L2/3/4 milestone + XP-style triggers, multiple paths.
7. **ACT_1_NPC_GUIDE.md** (npcs) — existing NPCs as allies/rivals/patrons/witnesses/complications. No new NPCs.
8. Runtime: update ACTIVE_QUESTS.md, OPEN_THREADS.md (Act 1 only). Do NOT touch CURRENT_STATE/LOCATION/SCENE.
9. Indexes/tracking: NAMING_REGISTRY, CONTENT_INDEX, TAG_INDEX, RETRIEVAL_GUIDE, PROGRESS_LOG, TODO, CONTENT_GAPS, EXPANSION_PLAN, STAGE_STATUS, CONSISTENCY_AUDIT, CANON, PLAYER_SAFE_CANON, CLUE_INDEX (status note only).

## Files Created

- `12_campaign_arc/ACT_1_LEVELS_1_4.md` (arc spine)
- `09_quests/act_1_quests/` (6 faction quests — Wardens, Compact, Ledger, Mourners, Gravecallers, Remnant; Hollow Court has none by design)
- `13_encounters_and_bestiary/ACT_1_THREATS.md` (5 recurring early-threat profiles)
- `11_mysteries_and_secrets/ACT_1_CLUE_TRAILS.md` (existing-clue Act 1 overlay; R1 cap)
- `12_campaign_arc/ACT_1_FAILURE_STATES.md` (9 redirect-not-end cases)
- `12_campaign_arc/ACT_1_MILESTONES.md` (L2/3/4 + L4→5 triggers; multi-path; XP guidance)
- `08_npcs/ACT_1_NPC_GUIDE.md` (existing-NPC Act 1 casting guide + re-entry points)

## Files Changed

- `00_control/STAGE_5_PROGRESS.md` (this file)
- `02_runtime_state/ACTIVE_QUESTS.md`, `OPEN_THREADS.md` (Act 1 quests/threads seeded, pre-play)
- `00_control/CONTENT_INDEX.md`, `TAG_INDEX.md` (+ `act:1` tag), `RETRIEVAL_GUIDE.md` (Stage 5 load entries), `NAMING_REGISTRY.md` (no-new-nouns note)
- `00_control/PROGRESS_LOG.md`, `TODO.md`, `STAGE_STATUS.md`, `CONSISTENCY_AUDIT.md`
- `17_generation_backlog/CONTENT_GAPS.md`, `EXPANSION_PLAN.md`
- `03_canon/CANON.md` (revision log), `PLAYER_SAFE_CANON.md` (Act 1 start situation)

## Completed Stage 5 Requirements

- [x] ACT_1_LEVELS_1_4.md
- [x] act_1_quests/ (6 faction quests — 7th, Hollow Court, intentionally omitted: apex villain, no friendly quest)
- [x] ACT_1_THREATS.md (5 threats; ≥3 required)
- [x] ACT_1_CLUE_TRAILS.md
- [x] ACT_1_FAILURE_STATES.md
- [x] ACT_1_MILESTONES.md
- [x] ACT_1_NPC_GUIDE.md
- [x] Runtime state updates (ACTIVE_QUESTS, OPEN_THREADS)
- [x] Indexes/tracking updates

## Remaining Stage 5 Requirements

None — Stage 5 complete (2026-06-10).

## Anti-Railroad Verification

- [x] AI DM can run L1–4 without a fixed quest order — arc spine presents Five Doors + 7 faction doors, all optional; clocks advance the truth toward a passive player.
- [x] 4+ prepared early routes beyond the default — six faction quests + 14 L1–4 regional quests + four R1 clue routes; default (Wren) is never required.
- [x] Important revelations have 3+ clue paths — `ACT_1_CLUE_TRAILS.md` shows R1 reachable via 4 independent routes; M1/M5 each have 4 paths; three-clue check intact.
- [x] Player can ignore obvious hook and still hit prepared content — Failure Case 5 (fled town) + regional quests deliver the same R1 pattern everywhere; clocks deliver it to a passive player.
- [x] Social/stealth/exploration/research/faction/dungeon/combat all supported — `ACT_1_CLUE_TRAILS.md` "Discovery Method Coverage" maps every playstyle to an R1 path; milestones earnable by any approach.
- [x] No single NPC/clue/dungeon/quest mandatory — every patron has a backup giver (`ACT_1_NPC_GUIDE.md` re-entry), every clue has alternates, no dungeon is required, the Court has no mandatory quest.
- [x] All L1–4 content mechanically complete (no TBD) — all 5 threat profiles fully statted (type/size/CR/AC/HP/speed/abilities/saves/skills/senses/actions/traits/tactics/morale/role/solo-danger/scaling); the 6 quests carry full QUEST_STANDARDS mechanical fields; reuses existing 5e-compatible baselines, no copied stat blocks.

## Reveal-Cap & Secrecy Verification

- [x] Every Act 1 file caps reveals at R1; never surfaces M3-as-substance, M4-Reke-traitor, M8-employer, M6-Concord-sin, M9-deliberate-Quietfall.
- [x] The Hollow Court (M7) is never named or deployed in any Act 1 file; Reke appears only as a reasonable politician (Hook 4 steering).
- [x] DM-only material confined to DM-Only sections; `ACT_1_CLUE_TRAILS.md` is dm-only; player-safe arc facts hold no hidden truth.
- [x] No new central mystery/faction/god/cosmology/artifact; no new proper nouns.

## Open Decisions

- New proper nouns: minimize. Quest titles are NOT registered proper nouns (they reuse existing entities). Will register only if a genuinely new named entity appears (target: none).

## Known Risks

- Must not name the Hollow Court or surface harvest-as-substance (M3) / Concord's sin (M6) in Act 1 content. Act 1 reveals cap at R1 (source/pattern) per REVELATION_MAP.
- Faction-aligned quests must remain solo-safe and noncombat-optional.

## Next Safe Continuation Prompt (if context runs out)

"Resume Stage 5. Read STAGE_5_PROGRESS.md for current state. Continue with the next unchecked file in the Completed Requirements list, matching the established QUEST_STANDARDS / DND_MECHANICS formats already used in 09_quests/regional_quests and 13_encounters_and_bestiary. Do not create new central mysteries/factions/gods/artifacts. Keep all mechanics level 1–4. Update indexes and this progress file when done."
