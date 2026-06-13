# QUEST_INDEX.md

---
type: index
secrecy: mixed
status: static
region:
settlement:
factions:
level_range: 1-20
related: [act_1_quests/, city_quests/, regional_quests/, faction_quests/, hooks_and_rumors/, HOOKS_TABLE.md, RUMORS_TABLE.md]
tags: [type:index, function:quest-index, quest, all-regions, all-factions]
---

## AI Use

Master index of all authored quests across the campaign. Use this to locate a quest by level, region, faction, or type without loading individual files. Load the specific quest file when the player engages with it. DM-only quest chains (Hollow Court) must never be surfaced to the player.

---

## Current Status

**Stage 10 (Quest Library Expansion) complete.** Quest library:

| Category | Count | Folder / File |
|---|---|---|
| **Major campaign questlines** | **28** | `MAJOR_CAMPAIGN_QUESTS.md` (Q_MAJOR_001–028) |
| Act 1 faction-alignment quests | 6 | `act_1_quests/` |
| City quests (Caradril) | 11 | `city_quests/` |
| Sundering Reach regional quests | 14 | `regional_quests/` (Reach files) |
| Ring 1 regional quests | 24 | `regional_quests/` (Ring 1 files) |
| Faction quest chains (Stage 8) | 28 | `faction_quests/[FACTION]/` |
| Far-continent developed quests (Stage 10) | 82 | `by_region/` (12 region files) |
| **Total developed quests** | **~165** | (~83 pre-Stage-10 + 82 far-continent) |
| Hooks tables (Reach/Caradril/Ring 1) | 10 files | `hooks_and_rumors/` + `HOOKS_TABLE.md` |
| Rumors tables (Reach/Caradril/Ring 1) | incl. above | `hooks_and_rumors/` + `RUMORS_TABLE.md` |
| Far-continent hooks/rumors/jobs (Stage 10) | 13 files; 304 entries | `hooks_and_rumors/fc_*` (12 region + 1 cross-region) |

**Stage 10 totals:** 28 major campaign quests · ~165 developed quests · 304 far-continent hooks/rumors/jobs (132 hooks + 104 rumors + 68 jobs) on top of the pre-Stage-10 hook/rumor tables. See `DEVELOPED_QUESTS_INDEX.md`, `HOOKS_JOBS_RUMORS_INDEX.md`, `by_level/QUESTS_BY_LEVEL.md`, `by_faction/QUESTS_BY_FACTION.md`, `by_type/QUESTS_BY_TYPE.md` for cross-cut indexes.

### Far-continent developed quests by region (Stage 10)

| Region | File (`by_region/`) | Quests | Level | IDs |
|---|---|---|---|---|
| Verdance Reaches | `VERDANCE_REACHES_QUESTS.md` | 7 | 8–12 | Q_VR_001–007 |
| Glassmere League | `GLASSMERE_LEAGUE_QUESTS.md` | 8 | 8–13 | Q_GL_001–008 |
| Hollow Gulf Ports | `HOLLOW_GULF_PORTS_QUESTS.md` | 8 | 9–14 | Q_HGP_001–008 |
| Emberfell Theocracy | `EMBERFELL_THEOCRACY_QUESTS.md` | 8 | 10–15 | Q_ET_001–008 |
| Sallowmarch Protectorate | `SALLOWMARCH_PROTECTORATE_QUESTS.md` | 7 | 9–13 | Q_SP_001–007 |
| Hethewald Free Holds | `HETHEWALD_FREE_HOLDS_QUESTS.md` | 7 | 8–13 | Q_HFH_001–007 |
| Saltmere Reaches | `SALTMERE_REACHES_QUESTS.md` | 7 | 11–15 | Q_SALT_001–007 |
| Karran Marches | `KARRAN_MARCHES_QUESTS.md` | 7 | 9–14 | Q_KM_001–007 |
| Sunmark | `SUNMARK_QUESTS.md` | 7 | 8–13 | Q_SUN_001–007 |
| Marrowdowns | `MARROWDOWNS_QUESTS.md` | 5 | 6–10 | Q_MD_001–005 |
| Wender Steppe | `WENDER_STEPPE_QUESTS.md` | 5 | 8–13 | Q_WS_001–005 |
| Concord Heartlands | `CONCORD_HEARTLANDS_QUESTS.md` | 6 | 13–17 | Q_CH_001–006 |

---

## Major Campaign Questlines (`MAJOR_CAMPAIGN_QUESTS.md`)

*28 multi-session spines carrying the level 1–20 story and the major faction/regional plots. Q_MAJOR_014 (Hollow Court) is DM-only. See the file's own index table for full per-quest detail.*

| ID range | File | Secrecy |
|---|---|---|
| Q_MAJOR_001 – Q_MAJOR_028 | `MAJOR_CAMPAIGN_QUESTS.md` | mixed (Q_MAJOR_014 dm-only) |

---

## Act 1 Quests (`act_1_quests/`)

*Level range: 1–4. One per major faction. Solo-safe. See `12_campaign_arc/ACT_1_LEVELS_1_4.md` for the full play arc.*

| File | Faction | Level | Summary |
|---|---|---|---|
| `Q_ACT1_WARDEN_THE_TRUE_RITE.md` | Ashen Wardens | 1–2 | A rite is failing; the Wardens need help they won't explain |
| `Q_ACT1_COMPACT_THE_REEVES_DOUBT.md` | Reachward Compact | 1–2 | A reeve's survey doesn't add up; the Compact wants it buried |
| `Q_ACT1_LEDGER_A_QUIET_SALVAGE.md` | Cinder Ledger | 1–2 | A lucrative salvage job with strings attached |
| `Q_ACT1_MOURNER_SALT_AND_SONG.md` | Mourners' Circle | 1–2 | A dead person won't stay settled; the Mourners need a witness |
| `Q_ACT1_GRAVECALLER_A_LAST_WORD.md` | Gravecallers | 1–3 | Someone has been promised a message from the dead |
| `Q_ACT1_REMNANT_THE_VISITING_SCHOLAR.md` | Concord Remnant | 1–3 | A scholar arrives with questions about local ruins |

---

## City Quests — Caradril (`city_quests/`)

*Level range: 2–6. City-state politics, factions, and secrets. See `06_settlements/CARADRIL.md`.*

| File | Type | Level | Faction / District |
|---|---|---|---|
| `Q_THE_OPEN_CHARTER.md` | Political | 2–4 | Tidewater Council / Charter Houses |
| `Q_THE_QUAY_CHARTER.md` | Faction | 2–4 | Cinder Ledger / Counting-Quays |
| `Q_THE_SEALED_LETTER.md` | Mystery | 2–4 | Compact / Magisterium |
| `Q_THE_SMELTING.md` | Faction | 3–5 | Crucible guilds |
| `Q_THE_TIDE_TURNS.md` | Faction | 3–5 | Salt Syndicate / the Sill |
| `Q_THE_BELLMANS_PRICE.md` | Intrigue | 3–5 | The Hush (citywide) |
| `Q_QUIET_COIN.md` | Mystery | 3–5 | Ashmarket / Ledger / M3 |
| `Q_THE_LANTERN_AND_THE_LAMP.md` | Mystery | 3–6 | Remnant / Lantern Reach / M6 |
| `Q_THE_SEALED_ARCHIVE.md` | Mystery | 4–6 | Remnant / Sealed Archive / M6/M9 |
| `Q_BELOW_THE_STILLING.md` | Dungeon | 4–6 | Sunken Wards / M5 |
| `Q_THE_FUNERAL_THAT_WOULDNT_TAKE.md` | Mystery | 2–4 | Mourners / Highmourn |

---

## Regional Quests — Sundering Reach (`regional_quests/` — Reach files)

*Level range: 1–5. Starting region. See `05_regions/SUNDERING_REACH.md`.*

| File | Settlement / Zone | Level |
|---|---|---|
| `Q_THE_FAILING_FUNERAL.md` | Hollowmere | 1–2 |
| `Q_THE_GREY_WOMAN_AT_THE_FORD.md` | Reedford | 1–2 |
| `Q_THE_HOLM_THAT_WONT_BURY_ITS_DEAD.md` | Greywater Holm | 1–3 |
| `Q_THE_SALT_RUN.md` | Saltmargin | 1–3 |
| `Q_THE_BAILIFFS_LADDER.md` | Kettle Bridge | 2–3 |
| `Q_THE_BROKEN_ARCH.md` | Sunder Heights / ruins | 2–4 |
| `Q_THE_REED_HOLMS.md` | Basin shore | 2–4 |
| `Q_THE_SCHOLARS_REQUEST.md` | Hollowmere | 2–4 |
| `Q_SASHES_WARNING.md` | Hollowmere | 1–3 |
| `Q_THE_SCHOLARS_REQUEST.md` | Cross-region | 2–4 |
| `Q_PELLS_DOUBT.md` | Saltmargin | 2–3 |
| `Q_LIGHT_ON_THE_SCALE.md` | Kettle Bridge | 2–4 |
| `Q_RACE_NORTH.md` | Heights / Harrowgast | 3–5 |

---

## Regional Quests — Ring 1 (`regional_quests/` — Ring 1 files)

*Level range: 2–6. Three adjacent regions. See region files in `05_regions/`.*

### Ashgarden Vale (south) — 8 quests

| File | Location | Level |
|---|---|---|
| `Q_THE_FUNERAL_DONE_TWICE.md` | Orchardmere | 2–3 |
| `Q_SAINTS_BONES.md` | Saint Veddow's Rest | 2–4 |
| `Q_THE_SEALED_DOOR.md` | Saint Veddow's Tomb | 3–5 |
| `Q_THE_LOAF_THAT_MOVES.md` | Tilbrook | 2–3 |
| `Q_THE_MARKS_ON_THE_DOORS.md` | Vale countryside | 2–4 |
| `Q_THE_SAINT_WHO_WEEPS.md` | Saint Veddow's Rest | 3–5 |
| `Q_THE_CROWS_OF_MARROW_CROSS.md` | Marrow Cross | 2–3 |
| `Q_WHATS_UNDER_THE_ORCHARD.md` | Orchardmere | 3–5 |

### Tollwood (east) — 8 quests

| File | Location | Level |
|---|---|---|
| `Q_THE_MARKED_OAKS.md` | Hartfell outskirts | 2–3 |
| `Q_THE_TOLL_WAR.md` | Tollstone Cross | 2–4 |
| `Q_THE_DROWNED_VAULT.md` | Greenward Toll-Station | 3–5 |
| `Q_THE_BARGAIN.md` | Coldhearth | 3–5 |
| `Q_THE_HANGING_OAKS.md` | Hanging Oaks ruin | 3–5 |
| `Q_TO_THE_EDGE.md` | Deep Tollwood | 4–6 |
| `Q_THE_RECKLESS_GUIDE.md` | Coldhearth | 2–4 |
| `Q_THE_LOST_CREW.md` | Tollwood roads | 2–3 |

### Pale Coast (west) — 8 quests

| File | Location | Level |
|---|---|---|
| `Q_THE_SALT_PRICE.md` | Wrackmouth | 2–3 |
| `Q_THE_SALT_MOTHERS_BURDEN.md` | Cobble Strand | 2–4 |
| `Q_WHAT_THE_LAMP_HOLDS.md` | Drowned Lamp headland | 3–5 |
| `Q_THE_COVE_CAVES.md` | Wreckers' Caves | 3–5 |
| `Q_THE_WRECKERS.md` | Wild coast | 3–5 |
| `Q_THE_DROWNED_BELL.md` | Cobble Strand | 2–3 |
| `Q_THE_SKIPPERS_DEBT.md` | Wrackmouth | 2–4 |
| `Q_THE_EMPTY_HEARTH.md` | Cobble Strand | 2–3 |

---

## Faction Quest Chains (`faction_quests/`)

*4-quest chains per faction: intro → trust → moral complication → decision point. See each `_CHAIN_INDEX.md` for the full chain summary.*

### Ashen Wardens (`ASHEN_WARDENS/`)

| File | Level | Stage in Chain |
|---|---|---|
| `QW1_THE_EMPTY_CLOAK.md` | 1–2 | Intro hook |
| `QW2_SALT_AND_ASH.md` | 2–3 | Trust-building |
| `QW3_THE_RITE_THAT_WONT_TAKE.md` | 3–4 | Moral complication |
| `QW4_THE_OATH_AND_THE_DOUBT.md` | 4–5 | Decision point |

### Cinder Ledger (`CINDER_LEDGER/`)

| File | Level | Stage in Chain |
|---|---|---|
| `QL1_THE_DEBT_OF_THE_DROWNED.md` | 1–3 | Intro hook |
| `QL2_THE_QUIET_BUYER.md` | 2–4 | Trust-building |
| `QL3_WHAT_THE_VAULT_REMEMBERS.md` | 3–5 | Moral complication |
| `QL4_THE_FACTORS_CONSCIENCE.md` | 4–6 | Decision point |

### Mourners' Circle (`MOURNERS_CIRCLE/`)

| File | Level | Stage in Chain |
|---|---|---|
| `QM1_THE_UNWASHED_DEAD.md` | 1–2 | Intro hook |
| `QM2_THE_OLD_SONGS.md` | 2–3 | Trust-building |
| `QM3_THE_BUYER_AT_THE_GRAVESIDE.md` | 3–4 | Moral complication |
| `QM4_SALT_OIL_AND_IRON.md` | 4–5 | Decision point |

### Reachward Compact (`REACHWARD_COMPACT/`)

| File | Level | Stage in Chain |
|---|---|---|
| `QC1_THE_WATCH_CANT_SPARE_A_MAN.md` | 1–2 | Intro hook |
| `QC2_THE_DOCTORED_SURVEY.md` | 2–3 | Trust-building |
| `QC3_THE_REED_HOLMS_EVICTION.md` | 3–4 | Moral complication |
| `QC4_THE_BASIN_VOTE.md` | 4–5 | Decision point |

### Gravecallers (`GRAVECALLERS/`)

| File | Level | Stage in Chain |
|---|---|---|
| `QG1_A_KNOCK_IN_THE_DARK.md` | 1–3 | Intro hook |
| `QG2_THE_TALLOW_MANS_WORD.md` | 2–4 | Trust-building |
| `QG3_WHAT_THE_DEAD_WANT.md` | 3–5 | Moral complication |
| `QG4_THE_BREAKING_TOOLS.md` | 4–6 | Decision point |

### Concord Remnant (`CONCORD_REMNANT/`)

| File | Level | Stage in Chain |
|---|---|---|
| `QR1_THE_VISITING_SCHOLARS_ERRAND.md` | 1–3 | Intro hook |
| `QR2_THE_READER_OF_RUINS.md` | 2–4 | Trust-building |
| `QR3_THE_IDEALIST_AND_THE_ARCHIVIST.md` | 3–5 | Moral complication |
| `QR4_THE_RECLAIMERS_GAMBIT.md` | 4–6 | Decision point |

### Hollow Court (`HOLLOW_COURT/`) — DM-ONLY

*The player never receives a friendly Hollow Court quest; this chain tracks the Court's moves from the DM side only. Never surface to the player.*

| File | Level | Stage in Chain |
|---|---|---|
| `QH1_THE_HAND_THAT_MOVES_THE_VOTE.md` | 3–5 | DM — Court intervention |
| `QH2_THE_PROBES_OWN_STRINGS.md` | 4–6 | DM — Court probe |
| `QH3_THE_COURT_BENEATH.md` | 5–8 | DM — Court exposed (partial) |
| `QH4_THE_FATE_OF_THE_REMEMBRANCE.md` | 8–12 | DM — endgame lever |

---

## Hooks and Rumors (`hooks_and_rumors/`)

| File | Region | Type |
|---|---|---|
| `SUNDERING_REACH_HOOKS.md` | Sundering Reach | Hooks |
| `SUNDERING_REACH_RUMORS.md` | Sundering Reach | Rumors |
| `CARADRIL_HOOKS.md` | Caradril | Hooks |
| `CARADRIL_RUMORS.md` | Caradril | Rumors |
| `ASHGARDEN_VALE_HOOKS.md` | Ashgarden Vale | Hooks |
| `ASHGARDEN_VALE_RUMORS.md` | Ashgarden Vale | Rumors |
| `TOLLWOOD_HOOKS.md` | Tollwood | Hooks |
| `TOLLWOOD_RUMORS.md` | Tollwood | Rumors |
| `PALE_COAST_HOOKS.md` | Pale Coast | Hooks |
| `PALE_COAST_RUMORS.md` | Pale Coast | Rumors |

See also `HOOKS_TABLE.md` and `RUMORS_TABLE.md` in this folder for consolidated tables.

### Far-continent hooks/rumors/jobs (Stage 10, `hooks_and_rumors/fc_*`)

Each `fc_[REGION]_HOOKS.md` carries 10 hooks + 8 rumors + 5 jobs (23 entries) for its region; `fc_CROSS_REGION_TRAVEL.md` adds 12 travel hooks + 8 cross-region rumors + 8 cross-region jobs (28). Total 304 entries.

| File | Region | Entries |
|---|---|---|
| `fc_VERDANCE_REACHES_HOOKS.md` | Verdance Reaches | 23 |
| `fc_GLASSMERE_LEAGUE_HOOKS.md` | Glassmere League | 23 |
| `fc_HOLLOW_GULF_PORTS_HOOKS.md` | Hollow Gulf Ports | 23 |
| `fc_EMBERFELL_THEOCRACY_HOOKS.md` | Emberfell Theocracy | 23 |
| `fc_SALLOWMARCH_PROTECTORATE_HOOKS.md` | Sallowmarch Protectorate | 23 |
| `fc_HETHEWALD_FREE_HOLDS_HOOKS.md` | Hethewald Free Holds | 23 |
| `fc_SALTMERE_REACHES_HOOKS.md` | Saltmere Reaches | 23 |
| `fc_KARRAN_MARCHES_HOOKS.md` | Karran Marches | 23 |
| `fc_SUNMARK_HOOKS.md` | Sunmark | 23 |
| `fc_MARROWDOWNS_HOOKS.md` | Marrowdowns | 23 |
| `fc_WENDER_STEPPE_HOOKS.md` | Wender Steppe | 23 |
| `fc_CONCORD_HEARTLANDS_HOOKS.md` | Concord Heartlands | 23 |
| `fc_CROSS_REGION_TRAVEL.md` | cross-region / travel | 28 |

---

## Related Files

- [`../12_campaign_arc/ACT_1_LEVELS_1_4.md`](../12_campaign_arc/ACT_1_LEVELS_1_4.md) — Act 1 arc spine and door structure
- [`../07_factions/FACTION_INDEX.md`](../07_factions/FACTION_INDEX.md) — faction chain cross-reference
- [`../02_runtime_state/ACTIVE_QUESTS.md`](../02_runtime_state/ACTIVE_QUESTS.md) — current quest state
- [`../00_control/CONTENT_INDEX.md`](../00_control/CONTENT_INDEX.md) — full file inventory
