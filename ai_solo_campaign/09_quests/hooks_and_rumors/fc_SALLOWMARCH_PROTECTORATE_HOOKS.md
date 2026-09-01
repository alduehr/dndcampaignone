# fc_SALLOWMARCH_PROTECTORATE_HOOKS.md — Far-Continent Hooks, Rumors & Jobs (Stage 10)

---
type: quest
secrecy: mixed
status: static
region: The Sallowmarch Protectorate
factions: [all]
level_range: 9-13
related: [../by_region/SALLOWMARCH_PROTECTORATE_QUESTS.md, ../../08_npcs/by_region/SALLOWMARCH_PROTECTORATE_NPCS.md, ../../04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md]
tags: [type:quest, function:quest-hook, far-continent, stage-10, region:sallowmarch-protectorate, secrecy:mixed]
---

## AI Use

Short-form hooks, rumors, and jobs for the Sallowmarch Protectorate (a fever-ridden deltaic wetland under a distant crown's garrison; Fenward, Reedmouth, the Rice Sallows, the Fever Channels; Lvl 9–13). Surface through fiction (the garrison-town, the smuggling-villages, the paddy-country, the deep backwaters), never as a menu. Cast from `08_npcs/by_region/SALLOWMARCH_PROTECTORATE_NPCS.md`. Never leak the apex truth; the delta's troubled dead are oblique. 10 hooks + 8 rumors + 5 jobs.

## Hooks (H_SP_NNN)

| # | Hook text (player-facing) | Where / Who | Points toward | Related | Risk | Truth |
|---|---|---|---|---|---|---|
| H_SP_001 | "The crown's Legate needs a deniable hand the garrison can't be seen to use." | Fenward / Vorr Sallow's aide | Protectorate intrigue | Q_SP_001 | medium | True |
| H_SP_002 | "Marsh-Healer Doll Fenn keeps the delta alive where the garrison can't — and the fever's winning." | Reedmouth / a sick villager | Plague-crisis | Q_SP_002 | medium | True |
| H_SP_003 | "'Heron' Maddox runs the delta's smuggling — and the garrison can't catch a man who knows the channels." | Reedmouth / a reed-cutter | Smuggler-king thread | Q_SP_003 | high | True |
| H_SP_004 | "Fen-Witch Mother Reed sings the delta's griefs — and says the rice-paddies' dead won't lie still." | The Rice Sallows / a paddy-wife | Mourner old-songs (oblique) | Q_SP_004 | low | Partial (oblique) |
| H_SP_005 | "Something in the Fever Channels takes those who go too deep — fever or worse." | A backwater fisher | Deep-delta danger (oblique) | Q_SP_005 | high | Partial (oblique) |
| H_SP_006 | "The garrison taxes the rice-villages to starvation while the Legate looks away." | A village-speaker | Protectorate injustice | Q_SP_006 | medium | True |
| H_SP_007 | "The Ledger buys the delta's rice cheap and its 'fen-relics' cheaper." | A Reedmouth factor | Ledger exploitation (M3) | Q_SP_007 | medium | Partial (oblique) |
| H_SP_008 | "Rice-Moot Speaker Pell Sallows would lead the villages — if someone broke the garrison's grip." | The Rice Sallows / Pell Sallows | Village-politics | Q_SP_006 | medium | True |
| H_SP_009 | "A garrison patrol vanished in the Fever Channels and the Legate wants it found — quietly." | Fenward / a sergeant | Rescue / deep-delta | Q_SP_005 | high | True |
| H_SP_010 | "'Heron' Maddox will move you (and anything) through the delta — for the right price or favor." | Reedmouth / a smuggler | Travel / smuggling | Q_SP_003 | medium | True |

## Rumors (R_SP_NNN)

| # | Rumor (player-facing) | Source | Truth | Points toward | Notes |
|---|---|---|---|---|---|
| R_SP_001 | "The crown that holds the Sallowmarch is far away and barely cares." | A villager | True | Protectorate nature | distant crown |
| R_SP_002 | "Doll Fenn, not the Legate, is the delta's real leader." | A patient | Partial | Q_SP_002 | the true leader |
| R_SP_003 | "The fever isn't all that takes folk in the deep channels." | A fisher | Partial (oblique) | Q_SP_005 | M5-oblique |
| R_SP_004 | "The paddy-dead walk the dykes at night, the rice-wives say." | A paddy-wife | Partial (oblique) | Q_SP_004 | M5-oblique |
| R_SP_005 | "'Heron' Maddox knows every channel the garrison's maps don't." | A reed-cutter | True | Q_SP_003 | smuggler-king |
| R_SP_006 | "The Ledger's 'fen-relics' come up out of the deep backwaters." | A factor | Partial (oblique) | Q_SP_007 | M3-oblique |
| R_SP_007 | "The Legate would sell the whole delta to save his career." | A garrison clerk | Partial | Q_SP_001 | Legate's pressure |
| R_SP_008 | "Mother Reed's songs are older than the crown, older than the Concord." | A pilgrim | Partial (oblique) | Q_SP_004 | M6-oblique |

## Jobs & Events (JOB_SP_NNN)

| # | Job/Event (player-facing) | Source / Trigger | Type | Reward | Risk | Notes |
|---|---|---|---|---|---|---|
| JOB_SP_001 | "Carry medicine through the Rice Sallows for Doll Fenn." | Doll Fenn | Escort/relief | Delta goodwill | medium | Q_SP_002 |
| JOB_SP_002 | "Find the patrol lost in the Fever Channels." | A garrison sergeant | Rescue | Coin + Legate favor | high | Q_SP_005 |
| JOB_SP_003 | "Smuggle a cargo (or a person) past the garrison." | 'Heron' Maddox | Smuggling | Coin + smuggler favor | high | Q_SP_003 |
| JOB_SP_004 | "Settle a paddy-dead that walks the dyke." | A paddy-wife | Rite/mercy | Mourner goodwill | low | Q_SP_004 |
| JOB_SP_005 | "Speak for the rice-villages at the garrison's tax-moot." | Pell Sallows | Mediation/politics | Village goodwill | medium | Q_SP_006 |

## Related Files
- [`../by_region/SALLOWMARCH_PROTECTORATE_QUESTS.md`](../by_region/SALLOWMARCH_PROTECTORATE_QUESTS.md) · [`../../08_npcs/by_region/SALLOWMARCH_PROTECTORATE_NPCS.md`](../../08_npcs/by_region/SALLOWMARCH_PROTECTORATE_NPCS.md)
