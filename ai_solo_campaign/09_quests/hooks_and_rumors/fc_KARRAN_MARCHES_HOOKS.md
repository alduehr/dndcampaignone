# fc_KARRAN_MARCHES_HOOKS.md — Far-Continent Hooks, Rumors & Jobs (Stage 10)

---
type: quest
secrecy: mixed
status: static
region: The Karran Marches
factions: [all]
level_range: 9-14
related: [../by_region/KARRAN_MARCHES_QUESTS.md, ../../08_npcs/by_region/KARRAN_MARCHES_NPCS.md, ../../04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md]
tags: [type:quest, function:quest-hook, far-continent, stage-10, region:karran-marches, secrecy:mixed]
---

## AI Use

Short-form hooks, rumors, and jobs for the Karran Marches (a jagged outlaw-and-mining frontier in the NE Karran Teeth; Brask's Hold, Karran-Gate, the Deep Cuts, the Old Iron forts; Lvl 9–14). Surface through fiction (the warlord holds, the lawless gate-town, the deep mines, the high-peaks ruins), never as a menu. Cast from `08_npcs/by_region/KARRAN_MARCHES_NPCS.md`. The Old Iron forts are **peripheral Concord ruins**, NOT the keystone. No NPC knows the apex truth. 10 hooks + 8 rumors + 5 jobs.

## Hooks (H_KM_NNN)

| # | Hook text (player-facing) | Where / Who | Points toward | Related | Risk | Truth |
|---|---|---|---|---|---|---|
| H_KM_001 | "'Iron' Brask's richest mine has 'gone wrong' — his diggers come up changed, and his men won't go down." | Brask's Hold / Iron Brask | Mine-crisis / patron | Q_KM_001 | high | Partial (oblique) |
| H_KM_002 | "Reclaimer-Captain Stone loses people every season in the Old Iron forts — and is half-broken by it." | Karran-Gate / Wenna Stone | Remnant ruin-delve | Q_KM_002 | high | Partial (oblique) |
| H_KM_003 | "'Red' Karr is building a coalition to break Iron Brask — and both warlords want a sword." | The holds / a war-captain | Warlord war / moral choice | Q_KM_003 | high | True |
| H_KM_004 | "Ore-Factor Mully Karr trades 'humming old iron' south and the Ledger wants in." | Karran-Gate / Mully Karr | Relic-trade (M2/M3-oblique) | Q_KM_004 | medium | Partial (oblique) |
| H_KM_005 | "Gate-Boss Sera Gate keeps lawless Karran-Gate from burning by nerve alone — and she's overstretched." | Karran-Gate / Sera Gate | Frontier-town trouble | Q_KM_005 | medium | True |
| H_KM_006 | "A hollow-eyed stranger 'hears the old iron's dead' near the forts — and the holds want to hang them." | The forts' edge / a hold-folk | Gravecaller emissary (DM) | Q_KM_006 | medium | Partial (oblique) |
| H_KM_007 | "Refugees fleeing the 'going-wrong' deep are jamming the only pass south — Hessa Teeth's gate." | The pass / Hessa Teeth | Refugee crisis / route out | Q_KM_007 | medium | True |
| H_KM_008 | "Fort-Guide 'Old Iron' Doss will take you into the forts and back — for the rare few worth guiding." | Karran-Gate / Old Iron Doss | Fort-delve guide | Q_KM_002 | high | True |
| H_KM_009 | "Brask's brother needs a hand holding the hold while the warlord's away." | Brask's Hold / Doss Brask | Hold-defense | Q_KM_003 | medium | True |
| H_KM_010 | "There's a road south past the Karran Teeth, if you can get through Hessa Teeth's toll." | The pass / a refugee | Route onward | Q_KM_007 | medium | True |

## Rumors (R_KM_NNN)

| # | Rumor (player-facing) | Source | Truth | Points toward | Notes |
|---|---|---|---|---|---|
| R_KM_001 | "The Marches have no law but the strong hand." | A sell-sword | True | Karran nature | warlord rule |
| R_KM_002 | "The Old Iron forts are Concord ruins, and the old dead in them won't lie still." | A fort-survivor | Partial (oblique) | Q_KM_002 | NOT keystone |
| R_KM_003 | "Iron Brask never lies and never forgives a lie." | A mercenary | True | Q_KM_003 | straight-dealing |
| R_KM_004 | "The 'humming old iron' from the deep mines is worth a fortune — and a curse." | An ore-assayer | Partial (oblique) | Q_KM_004 | M2/M3-oblique |
| R_KM_005 | "The deep dead in the mines wake worse each season." | A digger | Partial (oblique) | Q_KM_001 | M5-resonant |
| R_KM_006 | "Reclaimer-Captain Stone is starting to *fear* the works her order covets." | A Remnant porter | Partial | Q_KM_002 | turnable conscience |
| R_KM_007 | "Whole holds are emptying south — folk fleeing the 'going-wrong' deep." | A refugee | Partial (oblique) | Q_KM_007 | population-flow |
| R_KM_008 | "The Reach down south has the same troubles, a runaway swears." | A frontier-runaway | Partial (oblique) | cross-frontier | oblique |

## Jobs & Events (JOB_KM_NNN)

| # | Job/Event (player-facing) | Source / Trigger | Type | Reward | Risk | Notes |
|---|---|---|---|---|---|---|
| JOB_KM_001 | "Clear (or seal) Iron Brask's gone-wrong deep mine." | Iron Brask | Dungeon | Coin + patron | high | Q_KM_001 |
| JOB_KM_002 | "Help the Remnant recover a relic from an Old Iron fort." | Wenna Stone | Dungeon/escort | Coin + Script-lore | high | Q_KM_002 |
| JOB_KM_003 | "Guard Mully Karr's metals-caravan south." | Mully Karr | Escort | Coin + trade-ally | medium | Q_KM_004 |
| JOB_KM_004 | "Keep the peace at the Broken Pick for Sera Gate." | Sera Gate | Town-work | Coin + Gate standing | medium | Q_KM_005 |
| JOB_KM_005 | "Escort a refugee column over the pass south." | Hessa Teeth | Escort/travel | Coin + route south | medium | Q_KM_007 |

## Related Files
- [`../by_region/KARRAN_MARCHES_QUESTS.md`](../by_region/KARRAN_MARCHES_QUESTS.md) · [`../../08_npcs/by_region/KARRAN_MARCHES_NPCS.md`](../../08_npcs/by_region/KARRAN_MARCHES_NPCS.md)
