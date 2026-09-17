# STAGE_16_PROGRESS.md

## Status: COMPLETE — READY FOR LIVE PLAY (final cleanup pass, 2026-06-16)

> Stage 16 is fully complete. The initial audit, deep re-verification, correction
> pass (C1–C8), and final cleanup pass (items 1–8 below) are all done. Verdict:
> READY FOR LIVE PLAY. Stage 17 (Live Campaign Operation) may begin.

## Status: COMPLETE (full from-scratch re-audit, 2026-06-15)

> This pass re-verified every readiness claim by READING the actual files
> (canon tiers cross-checked; clue files traced to source; NPC mechanical
> profiles opened; dungeon DCs read; apex gating confirmed in every location;
> all 16 runtime state files opened). The earlier Stage 16 pass reached the
> same verdict but was shallow; this pass confirms it on evidence.

## Final Verdict: READY FOR LIVE PLAY
0 Critical / 0 High / 0 Medium blockers found this pass. The 2 Medium hygiene
items from the prior pass (stale canon status headers; the arc-forwarding
pointer) were already fixed and verified current. Only previously-known
non-blocking gaps remain (random tables, RtHW pending, map images, far-region
quest-title index polish).

## Audit Categories
- [x] 1. Canon and contradiction audit — read all 8 canon files + 2 arc files; cross-checked Hollow Court/Custodians/Quietfall/Remembrance/harvest across all 3 tiers; timeline (AQ 0 / Hollowmere AQ 12 / restart AQ 95) coherent; names match NAMING_REGISTRY; apex absent from PLAYER_SAFE_CANON; CANON revision log covers through Stage 15. PASS.
- [x] 2. Player-safe vs DM-only separation — read START/RESUME prompts, PLAYER_SAFE_CANON, CURRENT_STATE, NEXT_SESSION_START, CURRENT_SCENE, ACTIVE_QUESTS, KNOWN_CLUES, OPEN_THREADS, CURRENT_LOCATION. No apex leak in any player-facing block; DM-only notes correctly fenced in DM-loaded files. PASS.
- [x] 3. Runtime readiness — all 18 runner protocols present; read SECRET_REVEAL + COMBAT in full, grepped all protocols for TBD/placeholder (none); START/RESUME self-contained and name files that exist; all 16 state files verified (9 seeded, 7 correctly templated for play). PASS.
- [x] 4. Retrieval readiness — CONTENT_INDEX/NPC_INDEX/FACTION_INDEX/DUNGEON_INDEX/ARTIFACT_INDEX read with real, spot-checked entries that resolve to actual files. PASS.
- [x] 5. Starting play readiness — START prompt, NEXT_SESSION_START, CURRENT_SCENE, HOLLOWMERE-anchored location, all opening NPCs (Wren/Tomas/Wend/Iola/Sefra/Halla/Sashe + Othetha/Hale/Coalmont/Reke) present with full profiles. Opener A immediately runnable. PASS.
- [x] 6. Full-arc readiness — LEVEL_1_TO_20_PROGRESSION covers all 20 levels; MAIN_ARC_OVERVIEW forwards to 15_campaign_arcs/; TIER_2 verified as real runnable content; ACT_2 legacy stub forwards correctly; endgame (FINAL_REVELATION_AND_ENDING_PATHS, ENDGAME_STRUCTURE) present. PASS.
- [x] 7. Regional readiness — 5 core regions have region+settlement+dungeon+faction+level coverage; 12 far regions have NPC files, dungeon sites (D24–D36), quest files, encounter tables, and arc packs. PASS.
- [x] 8. Quest readiness — read Q_ACT1_WARDEN_THE_TRUE_RITE in full (level/DCs/hook/NPCs/approaches/hidden truth/solo notes); 6 Act 1 faction quests + 7 faction chains (QW/QL/QM/QC/QG/QR/QH 1–4) + regional/city/far quests all present. PASS.
- [x] 9. Mystery and clue readiness — read REVELATION_MAP in full: every REV_001–010 has 3+ independent clue sources; REV_007 (apex) has no single-source path and is L13+/Act 4 gated; traced REV_001 (5 sources) and REV_005 clue paths to SUNDERING_REACH_CLUES.md (clues exist with DCs + alt-paths). KNOWN/HIDDEN split maintained. PASS.
- [x] 10. Faction readiness — read HOLLOW_COURT + FACTION_INDEX + FACTION_STATE; all 7 majors have clock + 4-quest chain + tier/endgame posture; FACTION_STATE seeded with starting disposition; WORLD_CLOCKS has all 10 master + 3 city + 6 Ring-1 clocks. PASS.
- [x] 11. NPC readiness — read MAJOR_NPCS opening cast + Veyl/Maire (DM-only gated); NPC_INDEX lists 94 majors (50 core + 44 far) with mechanical profiles (Tier 1/2). PASS.
- [x] 12. Dungeon/adventure-site readiness — DUNGEON_INDEX lists all 36 sites with level/danger/REV links; read THE_PEAT_CHAPEL (full zones/DCs/encounters) and THE_UNDER_SHRINE_APPROACH (DM-only, L16-20, REV_007-gated). PASS.
- [x] 13. Encounter/bestiary readiness — read SUNDERING_REACH_ENCOUNTERS (d12 tables w/ stat refs, solo danger, non-combat outs); encounter tables exist for all 20 regions; custom creatures use D&D-compatible "X-like (AC,HP)" profiles. RtHW pending documented. PASS.
- [x] 14. Treasure/reward readiness — read ARTIFACT_INDEX: 12 named relics with access gates; Harvest Engine Shard (L16+, M8, DM-ONLY) and Quiet Country Vessel (L13+, M8) gated; rewards by tier present. PASS.
- [x] 15. Mechanical readiness — quest DCs (DC 11–15 bands), NPC AC/HP/actions, and dungeon trap DCs verified in opened files; RULESET_ASSUMPTIONS + DND_MECHANICS_REQUIREMENTS present. No "mechanics TBD" in play-ready content. PASS.
- [x] 16. File hygiene — STAGE_STATUS accurate through Stage 16; TODO marks Stage 1–16 done; no stale "next stage" claims in canon; 6 Stage 16 audit files present and indexed; placeholder files in empty dirs (15_random_tables, minor_factions) are intentional and gap-tracked. PASS.

## Blockers Found
- None (Critical/High/Medium). The campaign is play-ready as committed.

## Blockers Fixed
- None required this pass. Prior-pass fixes (canon status headers; MAIN_ARC_OVERVIEW arc pointer) verified still correct.

## Non-Blocking Issues Deferred (all previously tracked)
- `/15_random_tables/` holds only `_PLACEHOLDER.md` — random-table content not yet authored (low; CONTENT_GAPS).
- RtHW (Ravenloft: The Horrors Within, releases 2026-06-16) bestiary not yet integrated — placeholders documented in `13_encounters_and_bestiary/CREATURE_SOURCE_REFERENCE.md` (low; CONTENT_GAPS + MEMORY).
- No rendered map images (only prompts/coordinates authored) (low; CONTENT_GAPS).
- Far-region quest titles summarized rather than enumerated in DEVELOPED_QUESTS_INDEX (cosmetic; TODO low).
- Minor naming note (verified, not a defect): SECRET_REVEAL_PROTOCOL uses legacy "R1–R8" labels; REVELATION_MAP documents the explicit 1:1 R↔REV mapping, so no contradiction.

## Indexes Updated
- `CONTENT_INDEX.md` — Stage 16 audit-file rows confirmed present (already listed by prior pass).

## Runtime/State Files Updated
- None required — all 16 verified correct at campaign-start baseline (9 seeded, 7 templated).

## Stage 16 Correction Pass (2026-06-16)

The prior two passes (initial + deep re-verification) declared READY but **overclaimed** on control/retrieval/classification/hygiene — they verified content runnability deeply but missed several navigation/accuracy/classification defects that were not content gaps. A targeted correction pass found and fixed 8 of them (C1–C8 in `18_audits/STAGE_16_BLOCKERS_AND_FIXES.md`):

- **C1** — Rewrote the stale `RETRIEVAL_GUIDE.md` (was Stages 1–5/7 only) into a full per-scenario load map covering all Stage 8–15B systems.
- **C2** — Updated stale `MANIFEST.md` (was "Stage 1 complete / Stage 2 next") to Stages 0–16 complete / Stage 17 next.
- **C3** — Created the missing master `18_audits/PRE_PLAY_READINESS_AUDIT.md` (Stage 16's named required output).
- **C4** — Updated stale active-folder `_PLACEHOLDER.md` files to reflect real contents.
- **C5** — Reclassified the three map-render files (`FULL_CONTINENT_SETTLEMENT_ANCHORS`, `PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST`, `PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET`) to `dm-facing-player-safe-output` with notes.
- **C6** — Reclassified `LANGUAGES.md` and `LEVELING_ASSUMPTIONS.md` to `mixed` (they carried DM-only apex/act labels); annotated the `PLAYER_SAFE_CANON.md` Hollow-Court entry.
- **C7** — Created `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` (referenced as "when built" but never created); repointed stale references.
- **C8** — Closed/reclassified stale Medium issues in `CONSISTENCY_AUDIT.md` and `CONTENT_GAPS.md` (REWARDS_BY_LEVEL, Acts 2–5, endgame artifacts, NPC tools; Caradril density → non-blocking optional).

All 16 categories above remain verified [x]; the correction pass adds the control/retrieval/classification/hygiene layer the prior passes glossed.

## Final Verdict (post-correction): READY FOR LIVE PLAY
0 Critical / 0 High / 0 content-gap blockers. 8 control/retrieval/classification/hygiene fixes applied (C1–C8). Stage 17 (Live Campaign Operation) may begin.

## Final Cleanup Pass (2026-06-16)

A final cleanup pass ran after the correction pass to clear residual secrecy classifications and stale contradictions the correction pass had not reached. Eight items fixed:

1. **`PLAYER_SAFE_CANON.md`** — reduced the Hollow Court secrecy note to a generic DM warning; excised the named DM-only truths (surviving Custodians, the harvest, the Under-Shrine / Drowned Keystone, the Concord Deep) from the player-safe body.
2. **Map render/generation files** (`PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md`, `PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET.md`) — corrected contradictory "this file is player-safe / contains no DM-only geography" body text to state the *output* is player-safe but the *file* is DM-facing (it lists hidden "do not render" names) and must never be handed to the player.
3. **`18_audits/PLAYER_SAFE_FULL_CONTINENT_MAP_AUDIT.md`** — reclassified `secrecy: player-safe` → `dm-facing` (it references excluded names); added a one-line note.
4. **Four `player-safe` files carrying apex/harvest terms** reclassified `secrecy: mixed` with DM secrecy notes: `CREATURE_SOURCE_REFERENCE.md`, `BIOME_ENCOUNTER_MATRIX.md`, `REWARDS_BY_LEVEL.md`, `CONSUMABLES_AND_MINOR_MAGIC.md`.
5. **`CONSISTENCY_AUDIT.md`** — top status section updated so it no longer reads as if Stage 14 is most recent / endgame artifacts pending Stage 15; now states Stages 0–16 complete, Stage 15/15B resolved the arc/endgame, remaining issues Low/non-blocking only.
6. **`REWARD_PLACEMENT_AUDIT.md`** — added a Stage 15/15B update note resolving the "endgame artifact mechanics intentionally light pending Stage 15" forward note.
7. **`CONTENT_GAPS.md`** — corrected stale NPC counts to the real Stage 9/9.5 output (94 major / 368 secondary / 953 minor) and marked those entries resolved.
8. **`MANIFEST.md`** — added `/15_campaign_arcs` to the folder map and clarified `/12_campaign_arc` as the Act 1 / legacy folder.

No new campaign content was generated. All eight are classification/accuracy/navigation fixes. Stage 16 is cleanly complete.

## Remaining Risks
- None blocking. Only optional far-future depth/polish (deferred list above): far-region deep-builds, map images, deferred `/15_random_tables/`, pending RtHW integration.
