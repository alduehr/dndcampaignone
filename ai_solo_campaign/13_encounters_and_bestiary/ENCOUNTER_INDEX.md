# ENCOUNTER_INDEX.md — Master Index of Encounter Files & Tables

---
type: index
secrecy: mixed
status: static
region: Orrun
level_range: 1-20
related: [BESTIARY_INDEX.md, REGIONAL_ENCOUNTER_TABLES.md, ../00_control/CONTENT_INDEX.md]
tags: [type:index, secrecy:mixed, function:encounter-index, master]
---

## AI Use

The **master index for the entire `13_encounters_and_bestiary/` folder**. Start here to find any encounter table, bestiary entry, boss, faction encounter, or scaling rule. Load the foundational files (bestiary, source-reference, solo-scaling) once; load the regional/travel/faction files as the situation needs.

## Load-When Guide

| Situation | Load |
|---|---|
| Building/reading any encounter | `SOLO_ENCOUNTER_SCALING.md` |
| Need a creature | `BESTIARY_INDEX.md` → its full-notes file |
| Confirm source-handling | `CREATURE_SOURCE_REFERENCE.md` |
| PC is in region X | region's `*_ENCOUNTERS.md` (via `REGIONAL_ENCOUNTER_TABLES.md`) |
| Travelling between regions | `TRAVEL_ENCOUNTERS.md` + `BIOME_ENCOUNTER_MATRIX.md` |
| A faction is active | `FACTION_ENCOUNTERS.md` |
| Delivering a mystery clue | `MYSTERY_ENCOUNTERS.md` |
| In a dungeon/ruin | `DUNGEON_ENCOUNTER_SUPPORT.md` + `STAGE_12_ADVERSARIES.md` |
| Boss/apex fight | `BOSS_AND_APEX_THREATS.md` |
| Undead/curse/haunt | `HORROR_AND_CURSE_THREATS.md` |

---

## A. Foundational / Cross-Cutting Files

| File | Purpose | Secrecy |
|---|---|---|
| `ENCOUNTER_INDEX.md` | this master index | mixed |
| `BESTIARY_INDEX.md` | every creature, type, CR, source, location | mixed |
| `CREATURE_SOURCE_REFERENCE.md` | how official/original creatures are handled (copyright-safe) | player-safe |
| `SOLO_ENCOUNTER_SCALING.md` | adjust encounters for one PC; CR/XP budget; when not to roll | player-safe |
| `BIOME_ENCOUNTER_MATRIX.md` | biome → creature-type cross-reference | player-safe |
| `BOSS_AND_APEX_THREATS.md` | elite/boss/apex by level & region; recurring-villain framing | mixed |
| `HORROR_AND_CURSE_THREATS.md` | Remembrance undead, hauntings, curses (original) | mixed |
| `FACTION_ENCOUNTERS.md` | all 7 majors + city + regional minor faction tables | mixed |
| `MYSTERY_ENCOUNTERS.md` | M1–M9 / REV clue-bearing encounters | mixed |
| `TRAVEL_ENCOUNTERS.md` | terrain × level-band travel tables (1–4…17–20) | mixed |
| `DUNGEON_ENCOUNTER_SUPPORT.md` | wandering/adversary support for all 36 dungeons | mixed |
| `STAGE_12_ADVERSARIES.md` | original dungeon adversary profiles (Stage 12) | mixed |
| `REGIONAL_ENCOUNTER_TABLES.md` | all-regions coverage master | mixed |
| `ACT_1_THREATS.md` | levels 1–4 threat overview (pre-Stage 13) | mixed |

## B. Regional Encounter Files (20 regions)

| Region | File | Level | Pre/Stage-13 |
|---|---|---|---|
| Sundering Reach | `SUNDERING_REACH_ENCOUNTERS.md` | 1–6 | pre |
| Ashgarden Vale | `ASHGARDEN_VALE_ENCOUNTERS.md` | 1–6 | pre |
| Tollwood | `TOLLWOOD_ENCOUNTERS.md` | 2–7 | pre |
| Pale Coast | `PALE_COAST_ENCOUNTERS.md` | 2–7 | pre |
| Caradril | `CARADRIL_ENCOUNTERS.md` | 3–14 | pre |
| Verdance Reaches | `VERDANCE_REACHES_ENCOUNTERS.md` | 8–12 | **Stage 13** |
| Glassmere League | `GLASSMERE_LEAGUE_ENCOUNTERS.md` | 9–13 | **Stage 13** |
| Marrowdowns | `MARROWDOWNS_ENCOUNTERS.md` | 6–10 | **Stage 13** |
| Sallowmarch | `SALLOWMARCH_ENCOUNTERS.md` | 10–14 | **Stage 13** |
| Hollow Gulf Ports | `HOLLOW_GULF_ENCOUNTERS.md` | 10–15 | **Stage 13** |
| Wender Steppe | `WENDER_STEPPE_ENCOUNTERS.md` | 8–13 | **Stage 13** |
| Karran Marches | `KARRAN_MARCHES_ENCOUNTERS.md` | 9–14 | **Stage 13** |
| Emberfell Theocracy | `EMBERFELL_ENCOUNTERS.md` | 12–16 | **Stage 13** |
| Saltmere Reaches | `SALTMERE_REACHES_ENCOUNTERS.md` | 11–15 | **Stage 13** |
| Concord Heartlands | `CONCORD_HEARTLANDS_ENCOUNTERS.md` | 13–17 | **Stage 13** |
| Hethewald Free Holds | `HETHEWALD_ENCOUNTERS.md` | 7–12 | **Stage 13** |
| Sunmark | `SUNMARK_ENCOUNTERS.md` | 8–13 | **Stage 13** |
| Highmark Passes | `HIGHMARK_PASSES_ENCOUNTERS.md` | 12–16 | **Stage 13** |
| Cindern Waste | `CINDERN_WASTE_ENCOUNTERS.md` | 13–16 | **Stage 13** |
| Drowned Steps | `DROWNED_STEPS_ENCOUNTERS.md` | 10–16 | **Stage 13** |

## C. Level-Band → Where To Look

| Band | Primary regions | Travel table |
|---|---|---|
| **1–4** | Sundering Reach, Vale, Tollwood, Pale Coast | TRAVEL 1–4 |
| **5–8** | Caradril, Tollwood/Coast deep, Marrowdowns, Hethewald, Verdance, Wender | TRAVEL 5–8 |
| **9–12** | Verdance, Glassmere, Karran, Hethewald, Wender, Sunmark, Marrowdowns | TRAVEL 9–12 |
| **13–16** | Emberfell, Saltmere, Sallowmarch, Hollow Gulf, Heartlands, Highmark, Cindern, Drowned Steps | TRAVEL 13–16 |
| **17–20** | Heartlands apex, Highmark far-apex, endgame (Under-Shrine, DM-only) | TRAVEL 17–20 |

## D. Creature-Category → File

| Category | Where |
|---|---|
| Beasts / Monstrosities / Giants / Dragons | BESTIARY_INDEX + regional + BOSS |
| Undead / Hauntings / Spirits / Curses | HORROR_AND_CURSE_THREATS |
| Constructs / Concord guardians | STAGE_12_ADVERSARIES + DUNGEON_SUPPORT |
| Humanoid faction adversaries | FACTION_ENCOUNTERS |
| Fey / Celestials / Fiends / Elementals / Plants / Oozes / Swarms / Aberrations | BESTIARY_INDEX + BIOME_MATRIX + regional |
| Apex / bosses / recurring villains | BOSS_AND_APEX_THREATS |

## E. Cross-System Links

- Dungeons: `../10_dungeons_and_ruins/DUNGEON_INDEX.md`
- Factions: `../07_factions/`, runtime `../02_runtime_state/FACTION_STATE.md`
- Mysteries: `../11_mysteries_and_secrets/REVELATION_MAP.md`, `CLUE_INDEX.md`
- NPCs (recurring villains/allies): `../08_npcs/MAJOR_NPCS.md`, `by_region/`
- Protocols: `../01_runner_protocol/COMBAT_PROTOCOL.md`, `TRAVEL_PROTOCOL.md`, `SOLO_PLAY_PRINCIPLES.md`
- Rewards (Stage 14, forthcoming): `../14_treasure_and_artifacts/`

## Stage 13 Status

All required Stage 13 encounter/bestiary files exist and are indexed. See `../00_control/STAGE_13_PROGRESS.md`.

## Related Files

- [`BESTIARY_INDEX.md`](BESTIARY_INDEX.md) · [`REGIONAL_ENCOUNTER_TABLES.md`](REGIONAL_ENCOUNTER_TABLES.md)
- [`../00_control/CONTENT_INDEX.md`](../00_control/CONTENT_INDEX.md)
