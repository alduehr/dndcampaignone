# fc_CONCORD_HEARTLANDS_HOOKS.md — Far-Continent Hooks, Rumors & Jobs (Stage 10)

---
type: quest
secrecy: mixed
status: static
region: The Concord Heartlands / The Ruin'd Crown
factions: [all]
level_range: 13-17
related: [../by_region/CONCORD_HEARTLANDS_QUESTS.md, ../../08_npcs/by_region/CONCORD_HEARTLANDS_NPCS.md, ../../04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md]
tags: [type:quest, function:quest-hook, far-continent, stage-10, region:concord-heartlands, secrecy:mixed]
---

## AI Use

Short-form hooks, rumors, and jobs for the Concord Heartlands / the Ruin'd Crown (the shattered SURFACE seat of the old Concord; Crownmouth, the Ruin'd Crown, the Greatspine passes, the Pilgrim Camps; Lvl 13–17, late-game). Surface through fiction (the scavenger-town, the great ruin, the contested passes, the refugee camps), never as a menu. Cast from `08_npcs/by_region/CONCORD_HEARTLANDS_NPCS.md`.

**CRITICAL:** This is the Concord's *surface* fallen-capital. It is NOT the Concord Deep, NOT the Under-Shrine / Drowned Keystone beneath Hollowmere, NOT the Hollow Court's seat. It corroborates the theme but NEVER houses the apex truth. No NPC knows it. The Crown's deepest secret is a *record*, not the living machine. Hollin Vane is a magnificent dupe — never confirm the Court/keystone. 10 hooks + 8 rumors + 5 jobs.

## Hooks (H_CH_NNN)

| # | Hook text (player-facing) | Where / Who | Points toward | Related | Risk | Truth |
|---|---|---|---|---|---|---|
| H_CH_001 | "Crownmouth — the last safe town at the great ruin — is pressed on all sides, and Warden Lyssa needs hands that won't try to own it." | Crownmouth / Lyssa Crownmouth | Town-defense / base | Q_CH_001 | high | True |
| H_CH_002 | "'Old Crown' Mab is the only guide who goes deep into the Crown and comes back — and even she fears it's 'waking.'" | Crownmouth / Old Crown Mab | Deep-ruin delve | Q_CH_002 | deadly | Partial (oblique) |
| H_CH_003 | "Magister Hollin Vane leads the great expedition to 'reclaim the Concord' — and pays for deniable hands." | Crownmouth / Vane's lector | Remnant patron (apex-adjacent) | Q_CH_003 | high | Partial |
| H_CH_004 | "In the Pilgrim Camps, a gentle priest has begun to wonder if the held dead should be 'freed by force.'" | The Pilgrim Camps / Father Casian Ord | Gravecaller-mirror tragedy | Q_CH_004 | high | Partial (oblique) |
| H_CH_005 | "The Greatspine passes are contested by bandits, horrors, and faction armies — Brask Tarn holds the toll-gate." | The Greatspine / Brask Tarn | Contested-pass travel | Q_CH_005 | high | True |
| H_CH_006 | "Grave-Sister Onn Crale buries Crownmouth's dead — and re-buries them, for here the rites fail worst of all." | Crownmouth / Onn Crale | Mourner old-songs (near-source) | Q_CH_006 | medium | Partial (oblique) |
| H_CH_007 | "The Crown 'kept' a famous delver last season — his kin will pay to recover the body." | Crownmouth / a grieving kin | Deep-ruin recovery | Q_CH_002 | deadly | True |
| H_CH_008 | "The Emberfell fire-cult's agents are racing the Remnant for the Crown's deepest vaults." | The Greatspine / a pilgrim | Faction-convergence | Q_CH_005 | high | True |
| H_CH_009 | "Bandit-Lord 'Crow' Maddox raids the pilgrim roads in a salvaged Concord-gilt crown." | The Crown Road / a refugee | Road-banditry | Q_CH_005 | high | True |
| H_CH_010 | "Ruin-Surveyor Onaia Tarn swears the Crown's very geometry 'shifts' — her maps go wrong." | Crownmouth / Onaia Tarn | Shifting-ruin clue (oblique) | Q_CH_002 | medium | Partial (oblique) |

## Rumors (R_CH_NNN)

| # | Rumor (player-facing) | Source | Truth | Points toward | Notes |
|---|---|---|---|---|---|
| R_CH_001 | "The Crown is the fallen seat of the greatest civilization the world ever knew." | A scholar | True | surface history | NOT the keystone |
| R_CH_002 | "The Concord's inner circle 'vanished rather than died' in the fall." | A Remnant scribe | Partial (oblique) | surface history | Vane reads as tragedy; NEVER the Court |
| R_CH_003 | "Crownmouth's own dead won't stay buried — worse than anywhere in the world." | A gravedigger | Partial (oblique) | Q_CH_001/006 | crisis-worst-here |
| R_CH_004 | "Hollin Vane believes the Concord can be *restored* for good." | A Remnant porter | True | Q_CH_003 | the grand dupe |
| R_CH_005 | "The Door fails worst at the Crown — even the priests' blessings stutter." | A camp-pilgrim | Partial (oblique) | Q_CH_004/006 | M5 extreme |
| R_CH_006 | "'Old Crown' Mab says passages she's known thirty years now 'go wrong.'" | A delver | Partial (oblique) | Q_CH_002 | the Crown reactivating |
| R_CH_007 | "Every great faction wants the Crown — and none can hold it." | Crownmouth-talk | True | Q_CH_005 | convergence |
| R_CH_008 | "The vaults hold *records* of what the Concord did — not the doing of it." | A field-lector | Partial (oblique) | Q_CH_002 | NOT the machine; surface |

## Jobs & Events (JOB_CH_NNN)

| # | Job/Event (player-facing) | Source / Trigger | Type | Reward | Risk | Notes |
|---|---|---|---|---|---|---|
| JOB_CH_001 | "Defend Crownmouth's walls from a ruin-horror." | Lyssa Crownmouth | Defense | Coin + base | high | Q_CH_001 |
| JOB_CH_002 | "Delve a Crown vault with 'Old Crown' Mab's guidance." | Old Crown Mab | Dungeon | Salvage + Script-lore | deadly | Q_CH_002 |
| JOB_CH_003 | "Run a deniable errand for Magister Hollin Vane." | Hollin Vane | Faction-errand | Coin + Remnant power | high | Q_CH_003 |
| JOB_CH_004 | "Ease Father Ord and the camps' dead before grief turns to catastrophe." | Father Casian Ord | Rite/prevention | Camps' trust | high | Q_CH_004 |
| JOB_CH_005 | "Win passage through the contested Greatspine to the Crown." | Brask Tarn | Travel/negotiation | Passage + intel | high | Q_CH_005 |

## Related Files
- [`../by_region/CONCORD_HEARTLANDS_QUESTS.md`](../by_region/CONCORD_HEARTLANDS_QUESTS.md) · [`../../08_npcs/by_region/CONCORD_HEARTLANDS_NPCS.md`](../../08_npcs/by_region/CONCORD_HEARTLANDS_NPCS.md)
