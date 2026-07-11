# README — /13_encounters_and_bestiary/

---
type: index
secrecy: mixed
status: static
region: Orrun
level_range: 1-20
related: [ENCOUNTER_INDEX.md, BESTIARY_INDEX.md, CREATURE_SOURCE_REFERENCE.md]
tags: [type:index, function:bestiary, function:encounter, folder-readme, navigation]
---

## AI Use

Load this first when you need to find encounter or adversary material. It is the **front door** to the encounter and bestiary library: it explains the folder at a glance, lists every file, describes the copyright-safe source approach, and tells the AI DM how to navigate during play. For deep lookups, jump from here to `ENCOUNTER_INDEX.md` (encounter files) or `BESTIARY_INDEX.md` (creatures).

## The Library At A Glance

This folder is the campaign's **solo-tuned encounter and bestiary system** (built in Stage 13, on top of the Stage 3/4/5/7/12 encounter tables). It covers:

- **Every one of the 20 major regions** of Orrun has encounter support.
- **All five level-bands, levels 1–20**, are covered (1–4 / 5–8 / 9–12 / 13–16 / 17–20).
- **All 17 creature categories** are represented with biome-appropriate homes.
- **18 tiered bosses/apex threats** (B1–B18) with weaknesses, foreshadowing, and escape/return logic.
- A campaign-original **horror/curse bestiary** built on the world's Remembrance/harvest cosmology (grief, not gore).
- **Faction, mystery, travel, and dungeon** encounter support layers.

Everything is designed for **one player character**: telegraphed danger, enemy goals, morale, retreat routes, and noncombat outs throughout. No table assumes a four-PC party.

## Two-Track Source Approach (copyright-safe)

The bestiary never reproduces a published stat block. It uses two tracks (full rules in `CREATURE_SOURCE_REFERENCE.md`):

- **Track A — Official reference.** Standard fantasy creatures that exist in published 5e books are **named and source-referenced** (e.g. "Wolf — 2024 MM, Beast, CR 1/4"), then given only the campaign's own placement, tactics, and solo-tuning notes. The AI DM pulls the actual numbers from the named book. **No ability lines, no verbatim action blocks, no copied trait text.** Source shorthands: `2024 MM`, `2014 MM`, `MotM`, `MToF`, `VGtM`, `VRGtR`, `RtHW`, `FToD`, `XGtE`, `TCoE`, `GoS`, `ToA`. All name-and-book attributions were verified against the published books in the 2026-07-07 pass.
- **Track B — Original campaign creatures/variants.** Creatures unique to the world (Remembrance-linked dead, Concord constructs, memory-echo threats, salt/ash-preserved dead, etc.) get a **campaign-original abbreviated prose summary** (AC/HP/key attacks in prose) **anchored to a named official chassis** (see `BESTIARY_INDEX.md` §"Track-B Official-Chassis Anchors"), never a reproduced layout. `STAGE_12_ADVERSARIES.md` is the model Track-B file.

The campaign world (Vael / Orrun) is **original** and is **not** Ravenloft, the Domains of Dread, or any proprietary setting. Where gothic-horror creatures are referenced (Van Richten's Guide to Ravenloft, 2021), only the **published creature reference** is borrowed — never setting lore, darklords, domains, or named NPCs — and only where the campaign's own horror themes already call for it.

## Integrated: RtHW (Ravenloft: The Horrors Within) Supplement — 2026-07-07

*Ravenloft: The Horrors Within* (`RtHW`, released June 16 2026; 51 monster stat blocks, largely VRGtR creatures updated to 2024 rules plus new cosmic-horror entries) was **verified as a real published book and integrated on 2026-07-07**. Verified creatures (Gallows Speaker, Mist Horror, Necrichor, Bodytaker Plant, Boneless, Jiangshi, Carrionette, Brain in a Jar, Nightgaunt, Gug, Shoggoth, Greater Star Spawn Emissary, and others) now appear as Track-A references in `HORROR_AND_CURSE_THREATS.md` (#H10–H13), `BESTIARY_INDEX.md`, `MYSTERY_ENCOUNTERS.md`, and the deep-horror regional files. Placeholder entries that could **not** be verified against the published book (and all NPC placeholders) were **removed** — see the "Entries removed in the 2026-07-07 verification pass" note in `CREATURE_SOURCE_REFERENCE.md`. The same pass re-verified **every** Track-A attribution in the folder and corrected several misattributions (Oblex/Allip/Soul Monger/Deathlock/Vampiric Mist → MToF; Bodak → VGtM; the non-official "Caller in Darkness" → replaced by the **Sorrowsworn**, MToF).

## How To Navigate During Play

1. **Need an encounter for where the player is?** → `ENCOUNTER_INDEX.md` (master load-when guide) → the matching regional `*_ENCOUNTERS.md` file.
2. **Need a specific creature fast?** → `BESTIARY_INDEX.md` (find it, confirm its biome, jump to its full-notes file).
3. **Tuning a fight for one PC?** → `SOLO_ENCOUNTER_SCALING.md` (solo CR/XP budget; when not to roll; party→solo boss conversion).
4. **What lives in this terrain?** → `BIOME_ENCOUNTER_MATRIX.md` (15 biomes → creature types; ecology don'ts).
5. **Running a boss / recurring villain?** → `BOSS_AND_APEX_THREATS.md` (B1–B18; weaknesses, telegraphs, escape/return logic).
6. **A faction is reacting?** → `FACTION_ENCOUNTERS.md` (all 7 majors + city + regional minors).
7. **A clue should arrive via an encounter?** → `MYSTERY_ENCOUNTERS.md` (M2–M6 fragments; M9/Court gated).
8. **On the road?** → `TRAVEL_ENCOUNTERS.md` (terrain × 5 level-bands + weather/season variants).
9. **Inside a dungeon?** → `DUNGEON_ENCOUNTER_SUPPORT.md` (wandering layer + per-site cross-ref for all 36 dungeons).
10. **Horror/curse on a grief-saturated site?** → `HORROR_AND_CURSE_THREATS.md` (Remembrance dead, hauntings, curses — most resolvable by rite, not combat).

**Secrecy note:** the Hollow Court Custodian apex and the deep-harvest horror entries are **DM-only**; never surface them before their gates (REV_007 / endgame). Far-region threats **corroborate** the keystone/Court/endgame; they never relocate them.

## File List

### Cross-cutting / foundational

| File | One-line description |
|---|---|
| `README.md` | This file — folder front door and navigation guide |
| `ENCOUNTER_INDEX.md` | Master index of all encounter files/tables + load-when guide |
| `BESTIARY_INDEX.md` | Master creature list (17 categories) with track, source, CR, location, full-notes file |
| `CREATURE_SOURCE_REFERENCE.md` | The copyright-safe two-track source decision; source key; verified RtHW integration section |
| `SOLO_ENCOUNTER_SCALING.md` | One-PC scaling rules; solo CR/XP budget; party→solo boss conversion |
| `BIOME_ENCOUNTER_MATRIX.md` | 15 biomes → creature types + Concord/faction/curse overlays; ecology don'ts |
| `BOSS_AND_APEX_THREATS.md` | 18 tiered bosses (B1–B18) + recurring-villain escape/return logic |
| `HORROR_AND_CURSE_THREATS.md` | Original Remembrance undead/hauntings/curses (grief-not-gore) + MToF/VGtM/VRGtR/RtHW Track-A horror references |
| `FACTION_ENCOUNTERS.md` | Encounter tables for all 7 major factions + Caradril + regional minor factions |
| `MYSTERY_ENCOUNTERS.md` | Clue-bearing encounters (M2–M6 fragments; M9/Court gated) |
| `TRAVEL_ENCOUNTERS.md` | Terrain × 5 level-bands (1–20) + night/storm/fog/cold/heat/season variants |
| `DUNGEON_ENCOUNTER_SUPPORT.md` | Wandering layer + per-site adversary cross-ref for all 36 dungeons |
| `REGIONAL_ENCOUNTER_TABLES.md` | All-regions coverage master; universal table structure; cross-region constants |
| `STAGE_12_ADVERSARIES.md` | 8 abbreviated 5e-compatible Track-B profiles for the Stage 12 sites (incl. DM-only Custodian apex) |
| `ACT_1_THREATS.md` | 5 recurring early-threat profiles for the Level 1–4 arc (full profiles, solo-safe, scaling) |

### Per-region encounter files

**Home region + Ring 1 + Caradril (pre-existing):**
`SUNDERING_REACH_ENCOUNTERS.md` · `CARADRIL_ENCOUNTERS.md` · `ASHGARDEN_VALE_ENCOUNTERS.md` · `TOLLWOOD_ENCOUNTERS.md` · `PALE_COAST_ENCOUNTERS.md`

**Far / mid-continent regions (Stage 13):**
`VERDANCE_REACHES_ENCOUNTERS.md` (8–12) · `GLASSMERE_LEAGUE_ENCOUNTERS.md` (9–13) · `MARROWDOWNS_ENCOUNTERS.md` (6–10) · `SALLOWMARCH_ENCOUNTERS.md` (10–14) · `HOLLOW_GULF_ENCOUNTERS.md` (10–15) · `WENDER_STEPPE_ENCOUNTERS.md` (8–13) · `KARRAN_MARCHES_ENCOUNTERS.md` (9–14) · `EMBERFELL_ENCOUNTERS.md` (12–16) · `SALTMERE_REACHES_ENCOUNTERS.md` (11–15) · `CONCORD_HEARTLANDS_ENCOUNTERS.md` (13–17) · `HETHEWALD_ENCOUNTERS.md` (7–12) · `SUNMARK_ENCOUNTERS.md` (8–13) · `HIGHMARK_PASSES_ENCOUNTERS.md` (12–16) · `CINDERN_WASTE_ENCOUNTERS.md` (13–16) · `DROWNED_STEPS_ENCOUNTERS.md` (10–16)

## Related Files

- [`../01_runner_protocol/COMBAT_PROTOCOL.md`](../01_runner_protocol/COMBAT_PROTOCOL.md)
- [`../01_runner_protocol/SOLO_PLAY_PRINCIPLES.md`](../01_runner_protocol/SOLO_PLAY_PRINCIPLES.md)
- [`../10_dungeons_and_ruins/DUNGEON_INDEX.md`](../10_dungeons_and_ruins/DUNGEON_INDEX.md)
- [`../00_control/STAGE_13_PROGRESS.md`](../00_control/STAGE_13_PROGRESS.md)
