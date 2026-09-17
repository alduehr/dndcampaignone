# REGIONAL_ENCOUNTER_TABLES.md — All-Regions Encounter Master

---
type: encounter
secrecy: mixed
status: static
region: Orrun
factions: [all]
level_range: 1-20
related: [ENCOUNTER_INDEX.md, TRAVEL_ENCOUNTERS.md, BIOME_ENCOUNTER_MATRIX.md, SOLO_ENCOUNTER_SCALING.md]
tags: [type:encounter, secrecy:mixed, function:travel, all-regions, master]
---

## AI Use

The **single-stop master index of every region's encounter coverage** across all of Orrun. Each region has a dedicated file (deep table) and/or a row here pointing to it. Use this to confirm a region is covered, find its file, and read its one-line danger profile fast. For the actual tables, open the region's own file; for connective travel, use `TRAVEL_ENCOUNTERS.md`; for biome rules, `BIOME_ENCOUNTER_MATRIX.md`. All tables are solo-tuned (`SOLO_ENCOUNTER_SCALING.md`).

## All-Regions Coverage Map

| # | Region | Ring/Zone | Biome | Level | Danger | Encounter file |
|---|---|---|---|---|---|---|
| 1 | **Sundering Reach** | Ring 0 (start) | fen / highland / basin | 1–6 | mod (telegraphed) | `SUNDERING_REACH_ENCOUNTERS.md` |
| 2 | **Ashgarden Vale** | Ring 1 S | pastoral farmland / shrine | 1–6 | low–mod | `ASHGARDEN_VALE_ENCOUNTERS.md` |
| 3 | **Tollwood** | Ring 1 E | old-growth forest | 2–7 | mod (deep-wood high) | `TOLLWOOD_ENCOUNTERS.md` |
| 4 | **Pale Coast** | Ring 1 W | coast / sea / cliff | 2–7 | mod (sea high) | `PALE_COAST_ENCOUNTERS.md` |
| 5 | **Caradril** | first city (SE) | city / urban | 3–14 | social/intrigue (Wards high) | `CARADRIL_ENCOUNTERS.md` |
| 6 | **Verdance Reaches** | Ring 2 corridor | river / wetland | 8–12 | mod | `VERDANCE_REACHES_ENCOUNTERS.md` |
| 7 | **Glassmere League** | central | city / great river | 9–13 | social/intrigue | `GLASSMERE_LEAGUE_ENCOUNTERS.md` |
| 8 | **Marrowdowns** | S-central uplands | chalk downs / barrows | 6–10 | low (barrows high) | `MARROWDOWNS_ENCOUNTERS.md` |
| 9 | **Sallowmarch** | S coast delta | deltaic wetland / plague | 10–14 | high | `SALLOWMARCH_ENCOUNTERS.md` |
| 10 | **Hollow Gulf Ports** | S coast | open sea / ports | 10–15 | mod–high | `HOLLOW_GULF_ENCOUNTERS.md` |
| 11 | **Wender Steppe** | N-central | cold steppe | 8–13 | mod | `WENDER_STEPPE_ENCOUNTERS.md` |
| 12 | **Karran Marches** | NE | mountain / mine | 9–14 | high | `KARRAN_MARCHES_ENCOUNTERS.md` |
| 13 | **Emberfell Theocracy** | SE-central | volcanic highland | 12–16 | high | `EMBERFELL_ENCOUNTERS.md` |
| 14 | **Saltmere Reaches** | S-central | salt sea / salt flats | 11–15 | high | `SALTMERE_REACHES_ENCOUNTERS.md` |
| 15 | **Concord Heartlands** | central-SE | ruin-field | 13–17 | very high | `CONCORD_HEARTLANDS_ENCOUNTERS.md` |
| 16 | **Hethewald Free Holds** | E-central | old-growth forest / river | 7–12 | mod | `HETHEWALD_ENCOUNTERS.md` |
| 17 | **Sunmark** | S | warm forest / grove | 8–13 | mod (gentle/hope-mirror) | `SUNMARK_ENCOUNTERS.md` |
| 18 | **Highmark Passes** | far N | high mountain / frost | 12–16 | high (optional) | `HIGHMARK_PASSES_ENCOUNTERS.md` |
| 19 | **Cindern Waste** | SE interior | ash badland | 13–16 | high | `CINDERN_WASTE_ENCOUNTERS.md` |
| 20 | **Drowned Steps** | off S coast | submerged ruin / tidal | 10–16 | high→very high (optional) | `DROWNED_STEPS_ENCOUNTERS.md` |

**Coverage: 20 regions, all with dedicated encounter files.** Ring 0 + Ring 1 + Caradril (1–5) and the Stage 12 dungeon adversaries predate Stage 13; regions 6–20 are the Stage 13 build. Overseas Vael landmasses (Surren, Iron Skards, Sundered Isles) remain non-campaign placeholders with no encounter tables (far-future).

## Universal Region-Table Structure

Every region file follows the same shape (so the AI DM always knows where to look):
1. Region identity line (biome, danger, level)
2. Common (d10/d12) → Uncommon → Rare → Elite/Boss
3. Noncombat encounters (signs, dilemmas, bypass)
4. Social encounters (factions, travelers)
5. Environmental hazards
6. Travel variants (night/storm/fog/cold/heat/season)
7. Solo-play adjustments
8. Level-band guidance
9. Faction-linked + Mystery-linked encounters
10. Dungeon/site encounter support

## Cross-Region Constants (apply everywhere)

- **Concord overlay:** Remembrance dead + Concord constructs appear at any Concord-touched site in *any* region (`BIOME_ENCOUNTER_MATRIX.md`).
- **Faction overlay:** the 7 majors + city/regional factions appear per `FACTION_ENCOUNTERS.md`.
- **Mystery overlay:** M2–M6 fragments are deliverable in many regions; M9/the Court is **DM-only/gated** (`MYSTERY_ENCOUNTERS.md`).
- **Solo tuning:** every table is single-foe/small-group, telegraphed, with morale, escape, and a non-combat out (`SOLO_ENCOUNTER_SCALING.md`).
- **Far regions corroborate, never relocate:** the Heartlands, Drowned Steps, Saltmere, Cindern, Highmark Works are *far-proof echoes* of the harvest — the keystone/Court/endgame stay beneath Hollowmere.

## Related Files

- [`ENCOUNTER_INDEX.md`](ENCOUNTER_INDEX.md) (master file index)
- [`TRAVEL_ENCOUNTERS.md`](TRAVEL_ENCOUNTERS.md) · [`BIOME_ENCOUNTER_MATRIX.md`](BIOME_ENCOUNTER_MATRIX.md)
- [`FACTION_ENCOUNTERS.md`](FACTION_ENCOUNTERS.md) · [`MYSTERY_ENCOUNTERS.md`](MYSTERY_ENCOUNTERS.md)
- [`SOLO_ENCOUNTER_SCALING.md`](SOLO_ENCOUNTER_SCALING.md)
