# STAGE_13_PROGRESS.md — Encounter and Bestiary Expansion

## Stage
Stage 13 — Encounter and Bestiary Expansion. **Status: complete (2026-06-14).**

## Goal
Create solo-friendly threats and adversaries across the whole continent and all level tiers: a full bestiary, boss/apex designs, faction/mystery/travel/dungeon encounter support, and an encounter table for every major region — all tuned for one player character and copyright-safe.

## Summary
Built **28 newly generated Stage 13 files** in `13_encounters_and_bestiary/` (35 total .md files in the folder including README, inherited support files, and pre-existing Ring 1/Caradril encounter files). The campaign now has: a master encounter index and bestiary index; a documented copyright-safe source-handling decision; solo-PC scaling rules; a 15-biome ecology matrix; 18 tiered bosses with recurring-villain logic; an original Remembrance-linked horror/curse bestiary (the world is original and is NOT Ravenloft; gothic-horror *creatures* are referenced Track-A via VRGtR — no copied stat blocks, no imported setting lore); faction encounter tables for all 7 majors + city + regional minors; mystery clue-bearing encounter tables (M2–M6, with M9/Court gated); travel tables for all 6 terrains × all 5 level bands (1–20); dungeon encounter support for all 36 dungeons; and a dedicated encounter file for **every one of the 20 major regions** of Orrun. Official monsters are **source-referenced, never stat-block-copied**; originals carry abbreviated 5e-compatible summaries. Everything is solo-tuned (telegraph, morale, escape, non-combat outs). No new factions, NPCs, regions, mysteries, gods, or artifacts were created; far regions corroborate (never relocate) the keystone/Court/endgame; apex truth stays DM-only and gated.

## Files Created (28 newly generated; 35 total in folder)

### Cross-cutting / foundational (13)
- `13_encounters_and_bestiary/ENCOUNTER_INDEX.md` — master index + load-when guide
- `13_encounters_and_bestiary/BESTIARY_INDEX.md` — 17 creature categories, track/CR/location/source
- `13_encounters_and_bestiary/CREATURE_SOURCE_REFERENCE.md` — copyright-safe two-track decision
- `13_encounters_and_bestiary/SOLO_ENCOUNTER_SCALING.md` — 7 one-PC scaling rules + solo CR/XP budget
- `13_encounters_and_bestiary/BIOME_ENCOUNTER_MATRIX.md` — 15 biomes → creature types + overlays
- `13_encounters_and_bestiary/BOSS_AND_APEX_THREATS.md` — 18 bosses (B1–B18) + recurring-villain logic
- `13_encounters_and_bestiary/HORROR_AND_CURSE_THREATS.md` — original Remembrance undead/hauntings/curses
- `13_encounters_and_bestiary/FACTION_ENCOUNTERS.md` — all 7 majors + city + regional minor factions
- `13_encounters_and_bestiary/MYSTERY_ENCOUNTERS.md` — M2–M6 clue-bearing encounters (M9/Court gated)
- `13_encounters_and_bestiary/TRAVEL_ENCOUNTERS.md` — terrain × 5 level-bands (1–20) + variants
- `13_encounters_and_bestiary/DUNGEON_ENCOUNTER_SUPPORT.md` — wandering layer + all 36 dungeons cross-ref
- `13_encounters_and_bestiary/REGIONAL_ENCOUNTER_TABLES.md` — all-regions coverage master
- `00_control/STAGE_13_PROGRESS.md` — this file

### Per-region encounter files (15 new far/mid-continent)
- `VERDANCE_REACHES_ENCOUNTERS.md` (8–12) · `GLASSMERE_LEAGUE_ENCOUNTERS.md` (9–13) · `MARROWDOWNS_ENCOUNTERS.md` (6–10) · `SALLOWMARCH_ENCOUNTERS.md` (10–14) · `HOLLOW_GULF_ENCOUNTERS.md` (10–15) · `WENDER_STEPPE_ENCOUNTERS.md` (8–13) · `KARRAN_MARCHES_ENCOUNTERS.md` (9–14) · `EMBERFELL_ENCOUNTERS.md` (12–16) · `SALTMERE_REACHES_ENCOUNTERS.md` (11–15) · `CONCORD_HEARTLANDS_ENCOUNTERS.md` (13–17) · `HETHEWALD_ENCOUNTERS.md` (7–12) · `SUNMARK_ENCOUNTERS.md` (8–13) · `HIGHMARK_PASSES_ENCOUNTERS.md` (12–16) · `CINDERN_WASTE_ENCOUNTERS.md` (13–16) · `DROWNED_STEPS_ENCOUNTERS.md` (10–16)

*(The 5 pre-existing region files — Sundering Reach, Ashgarden Vale, Tollwood, Pale Coast, Caradril — and `STAGE_12_ADVERSARIES.md` / `ACT_1_THREATS.md` are now indexed alongside the new ones; 20 regions covered total.)*

## Files Changed
- `00_control/CONTENT_INDEX.md` — status line + 28 encounter/bestiary rows
- `00_control/TAG_INDEX.md` — status line + Stage 13 file/tag entry
- `00_control/PROGRESS_LOG.md` — Stage 13 entry
- `00_control/TODO.md` — Stage 13 marked done; Stage 14 flagged next
- `17_generation_backlog/CONTENT_GAPS.md` — bestiary/boss/encounter gaps closed

## Coverage Confirmation (final audit checklist)
- [x] Every major region (20) has encounter support
- [x] Levels 1–20 covered in TRAVEL_ENCOUNTERS + regional tables (5 level bands)
- [x] Every major biome has appropriate creature types (BIOME_ENCOUNTER_MATRIX, 15 biomes)
- [x] Faction encounters for all 7 major factions + city + regional minors
- [x] Dungeon encounter support for all 36 dungeons in `10_dungeons_and_ruins/`
- [x] Horror/curse/Remembrance threats exist (HORROR_AND_CURSE_THREATS.md)
- [x] Official monsters source-referenced, NOT stat-block-reproduced (CREATURE_SOURCE_REFERENCE.md)
- [x] No biome-inappropriate creatures (ecology don'ts enforced)
- [x] No pure-combat tables — noncombat options in every region file
- [x] Solo-play scaling rules exist and are usable (SOLO_ENCOUNTER_SCALING.md)
- [x] All 17 required creature categories represented (BESTIARY_INDEX coverage line)
- [x] All new files in CONTENT_INDEX.md and TAG_INDEX.md
- [x] PROGRESS_LOG.md and TODO.md updated

## Ravenloft / Van Richten Handling (corrected in the 2026-06-14 cleanup pass)
All horror is built from the campaign's **original Remembrance/harvest cosmology** (grief-not-gore: mournful dead resolvable by rite/parley, memory-echoes, revenants, original curses) — the world Vael/Orrun is **original and is NOT Ravenloft, the Domains of Dread, or any proprietary setting**; no darklord, domain, named-NPC, or setting lore is imported. For **mechanical creature references**, the horror bestiary *does* draw on the published gothic-horror sourcebook **Van Richten's Guide to Ravenloft (VRGtR, 2021)** — handled **exactly like the Monster Manual (Track A: name + source + role + solo notes, no stat blocks copied)**, only where the campaign's own themes already call for the creature (memory-drain, soul-consumption, grief-swarms, hollow/thin-born dread). See `HORROR_AND_CURSE_THREATS.md` §VRGtR and `CREATURE_SOURCE_REFERENCE.md`.

> **Note:** An earlier draft of this file claimed "zero Ravenloft / Van Richten material." That was inaccurate and was corrected in the 2026-06-14 cleanup pass — VRGtR creature *references* are present and are copyright-safe (Track A). No copied stat blocks and no imported setting lore exist anywhere.

## RtHW (Ravenloft: The Horrors Within) — pending
*Ravenloft: The Horrors Within* (RtHW) releases **June 16 2026**, after Stage 13 completion, and was **not available** at completion. A placeholder **"Horror Expansion Supplement (Pending)"** section with ~28 named creatures (each "source check needed — RtHW") was added to `CREATURE_SOURCE_REFERENCE.md` in the cleanup pass. A focused **RtHW supplement pass** should run once the book is accessible, adding apt creatures (Track-A discipline) to `HORROR_AND_CURSE_THREATS.md`, `BESTIARY_INDEX.md`, `MYSTERY_ENCOUNTERS.md`, and the deep-horror regional files. Logged as a low-priority TODO/CONTENT_GAPS item + an OPEN_QUESTION.

## Cleanup / Source-Reference Pass (2026-06-14)
- Marked Stage 13 **complete (100%)** and Stage 14 next in all tracking files (STAGE_STATUS, EXPANSION_PLAN, TODO, OPEN_QUESTIONS, CONSISTENCY_AUDIT, NAMING_REGISTRY status block).
- Replaced `_PLACEHOLDER.md` with a real folder `README.md` (at-a-glance summary, full file list, two-track source approach, RtHW-pending note, in-play navigation).
- Mapped **Track-A official-monster source shorthands** in `BESTIARY_INDEX.md` (most classic creatures → `2024 MM`; VRGtR/MToF/MotM where applicable; one `source check needed` for the unspecified deep-water aberration).
- Added the RtHW pending-supplement section + ~28 placeholder creatures to `CREATURE_SOURCE_REFERENCE.md`; corrected the stale "no Ravenloft material" claims here and in CONTENT_INDEX/PROGRESS_LOG.
- Updated CONTENT_INDEX (README row, corrected horror-file summary) and TAG_INDEX (`type:encounter` file list completed for all Stage 13 files).

## Source-Handling Approach
Two-track, copyright-safe (`CREATURE_SOURCE_REFERENCE.md`): **Track A** = official creatures *named + source-referenced* (e.g. "Wolf (2024 MM, Beast, CR 1/4)") with original placement/tactics/solo notes — **no stat blocks copied**; **Track B** = campaign originals with abbreviated prose 5e-compatible summaries (AC/HP/key attacks in prose), never a reproduced layout. Matches `RULESET_ASSUMPTIONS.md` and `DND_MECHANICS_REQUIREMENTS.md`.

## Remaining Gaps / Notes
- No standalone `NONCOMBAT_OBSTACLES.md` library file — noncombat obstacles are folded into each region file's "Noncombat Encounters" + travel variants + scaling rules (optional future consolidation; logged Low in CONTENT_GAPS).
- Recurring-villain *full stat blocks* live in their NPC files; this stage provides their **boss-fight framing** (BOSS_AND_APEX_THREATS). Deepening individual high-tier villain profiles can continue in Stage 15.
- Treasure/rewards-by-level (the "what you get for winning") is **Stage 14**, not built here.

## Next Recommended Pass
- **Stage 14: Treasure, Artifacts, and Rewards** — `TREASURE_INDEX`, `ARTIFACTS`, `MAGIC_ITEMS`, `REWARDS_BY_LEVEL`; tie rewards to the encounters/bosses built here and to the Remembrance-relic lore; keep solo survivability supported without removing danger.
