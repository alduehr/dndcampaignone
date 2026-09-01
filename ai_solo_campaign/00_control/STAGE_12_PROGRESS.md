# STAGE_12_PROGRESS.md

## Purpose

Live working-state tracker for Stage 12 (Dungeons, Ruins, and Adventure Sites). Records exactly what has been done, what remains, and a continuation prompt so the pass can be resumed cleanly.

## Stage Goal

Build a large library of explorable places. The 15 Stage 3/4/7 dungeon files already exist and are complete — Stage 12 must:
1. Create the master dungeon index (and a puzzle/investigation index).
2. Cross-link the 15 existing dungeons to the Stage 11 REV/clue IDs (append-only).
3. Create new adventure sites filling the level/region gaps (Caradril 5–10, Reach 5–9, mid-tier 8–12, high-tier 10–16, endgame approach 15–20).
4. Add any needed bestiary adversary profiles.
5. Update all indexes/canon/tracking.

## Secrecy discipline (non-negotiable)

- `THE_UNDER_SHRINE_APPROACH.md` is the ONLY new file that may describe the apex truth (harvest mechanism, Court's full nature, endgame decision). Secrecy `dm-only`. Never rendered to the player.
- `THE_BASIN_KEYSTONE_APPROACH.md` is `mixed` — approach + fragments only; apex truth stays in the DM-only file and DM_ONLY_CANON.
- All other new files treat the keystone, the Concord Deep, and the Hollow Court as oblique/approach references only — never named as confirmed, never the mechanism.

---

## Work Checklist

- [x] 1. Read all context files (canon, 15 existing dungeons, REVELATION_MAP, CLUE_INDEX, bestiary, Sunken Wards district)
- [x] 2. Create STAGE_12_PROGRESS.md
- [x] 3. Create DUNGEON_INDEX.md (covers existing 15)
- [x] 4. Append Stage 11 clue cross-links to the 15 existing dungeon files
- [x] 5. Create THE_SUNKEN_WARDS_DEEP.md (Caradril; highest priority)
- [x] 6. Create THE_BASIN_KEYSTONE_APPROACH.md (player-mixed approach)
- [x] 7. Create THE_UNDER_SHRINE_APPROACH.md (DM-only endgame)
- [x] 8. Create THE_GREYFENS_DEEP.md
- [x] 9. Create THE_CONCORD_RELAY_VAULT.md
- [x] 10. Create THE_CARADRIL_ASHMARKET_UNDERCROFT.md
- [x] 11. Create THE_OLD_CONCORD_HEARTLANDS_RUIN.md
- [x] 12. Create THE_EMBERFELL_CALDERA_DESCENT.md
- [x] 13. Create PUZZLE_DUNGEONS.md
- [x] 14. Add bestiary profiles (STAGE_12_ADVERSARIES.md)
- [x] 15. Update DUNGEON_INDEX with all new sites
- [x] 16. Update CLUE_INDEX with new clue IDs
- [x] 17. Update CONTENT_INDEX, NAMING_REGISTRY, TODO, CONTENT_GAPS, PROGRESS_LOG, STAGE_STATUS
- [x] 18. Finalize STAGE_12_PROGRESS.md
- [x] 19. Cleanup pass (2026-06-13): rewrote `_PLACEHOLDER.md` as folder README; created `RUIN_INDEX.md`; fixed DUNGEON_INDEX "By Region" count (Reach: 8→10); corrected clue ID range in this file (C_SR_039-044→039-041); updated TAG_INDEX (Stage 12 entries, type:dungeon, type:ruin, region tags, STAGE_12_ADVERSARIES); updated current-status language in EXPANSION_PLAN, OPEN_QUESTIONS, CONSISTENCY_AUDIT, NAMING_REGISTRY (all now reflect Stage 12 complete, Stage 13 next).

---

## Completion State

**Status: COMPLETE** (including cleanup pass 2026-06-13). All work-order items finished.

### New dungeon/site files created (8 + 3 indexes + 1 bestiary)
- `THE_SUNKEN_WARDS_DEEP.md` (Caradril, L6–10, mixed)
- `THE_BASIN_KEYSTONE_APPROACH.md` (Reach, L5–9, mixed)
- `THE_UNDER_SHRINE_APPROACH.md` (Reach, L16–20, **dm-only**)
- `THE_GREYFENS_DEEP.md` (Reach, L3–7, mixed)
- `THE_CONCORD_RELAY_VAULT.md` (Reach/Sunder Heights, L7–10, mixed)
- `THE_CARADRIL_ASHMARKET_UNDERCROFT.md` (Caradril, L6–9, mixed)
- `THE_OLD_CONCORD_HEARTLANDS_RUIN.md` (Concord Heartlands, L10–14, mixed)
- `THE_EMBERFELL_CALDERA_DESCENT.md` (Emberfell, L12–16, mixed)
- `DUNGEON_INDEX.md` (master index, 23 sites)
- `PUZZLE_DUNGEONS.md` (puzzle/investigation index)
- `RUIN_INDEX.md` (ruin subset index — cleanup pass)
- `_PLACEHOLDER.md` (rewritten as folder README — cleanup pass)
- `13_encounters_and_bestiary/STAGE_12_ADVERSARIES.md` (abbreviated adversary profiles)

### Existing dungeons cross-linked to Stage 11 (15)
All 15 Stage 3/4/7 dungeon files received an appended `## Stage 11 Clue Cross-Links` section.

### New clue IDs added
`C_SR_039`, `C_SR_040`, `C_SR_041` (Reach deep sites — Basin Keystone Approach, Greyfens Deep, Concord Relay-Vault), `C_CAR_016`–`C_CAR_018` (Caradril deep sites — Sunken Wards Deep, Ashmarket Undercroft ×2), `C_FC_014`–`C_FC_015` (Heartlands ruin, Emberfell descent). All `hidden` at start; all corroboration/fragment-tier, gated per REVELATION_MAP. The Under-Shrine apex content is tracked under the existing apex clue IDs (C_SR_027/032/036, REV_007/008/010) — no new apex clue ID was coined.

### Naming registry additions
New site proper nouns coined (registered in NAMING_REGISTRY): see the Stage 12 subsection there. All are dungeon-internal place labels, not new factions/gods/regions/central mysteries.

---

## Continuation Prompt (if ever resumed)

Stage 12 is complete. If a follow-up pass is wanted, the optional additional sites named in the brief but NOT built this pass are:
- `THE_SALTMERE_DEEP_TOWNS.md` (Saltmere, L11–15)
- `THE_HETHEWALD_OLD_HOLDS.md` (Hethewood, L9–13)
- `THE_MARROWDOWNS_BARROW_COMPLEX.md` (Marrowdowns, L8–12)
- `THE_KARRAN_OLD_IRON_FORTS.md` (Karran Marches, L10–14)
These are placeholder far-continent sites; build only if far-continent play depth is later prioritized. They are logged in CONTENT_GAPS.

## Related Files
- [`DEVELOPMENT_STAGES.md`](DEVELOPMENT_STAGES.md)
- [`STAGE_STATUS.md`](STAGE_STATUS.md)
- [`../10_dungeons_and_ruins/DUNGEON_INDEX.md`](../10_dungeons_and_ruins/DUNGEON_INDEX.md)
