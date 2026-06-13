# fc_CROSS_REGION_TRAVEL.md — Far-Continent Cross-Region & Travel Hooks (Stage 10)

---
type: quest
secrecy: mixed
status: static
region: Far Continent (cross-region)
factions: [all]
level_range: 8-17
related: [../by_region/, ../../04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md, ../../08_npcs/by_region/]
tags: [type:quest, function:quest-hook, far-continent, stage-10, cross-region, travel, secrecy:mixed]
---

## AI Use

Cross-region and travel hooks, rumors, and events for the wider continent — the connective tissue that moves a player between the 12 far-continent regions and ties their threads together. Surface through fiction (road-talk, caravan-fires, river-landings, trade-meets), never as a menu. These reinforce the spreading-crisis theme (the troubled dead, the Ledger's reach, the Mourner old-songs network) WITHOUT ever leaking the apex truth (Hollow Court / harvest / keystone / Under-Shrine). The crisis is worst at the Concord's heart and the frontiers; it is barely felt in the living Sunmark and the never-Concord steppe. 12 travel hooks + 8 cross-region rumors + 8 cross-region jobs/events = 28 entries.

## Travel Hooks (H_XR_NNN)

| # | Hook text (player-facing) | Where / Who | Points toward | Related | Risk | Truth |
|---|---|---|---|---|---|---|
| H_XR_001 | "Up the Verdance lies Glassmere, and beyond it the whole wider world — a barge will take you on." | Any river-landing / a barge-captain | The far continent opens | VR/GL quests | low | True |
| H_XR_002 | "The Mourner elders pass old songs hand to hand across the continent — carry one, and doors open." | Any Mourner shrine / a grief-keeper | The old-songs network (oblique) | M6-oblique; all Mourner nodes | low | Partial (oblique) |
| H_XR_003 | "The Cinder Ledger's reach runs from the frontier to the sea — wherever there's coin or relics, they're there." | Any market / a factor | The Ledger's continental web | Q_MAJOR_004 | low | True |
| H_XR_004 | "The dead grow restless everywhere — worse near the old Concord's heart, barely at all in the living south." | A well-traveled pilgrim | The crisis-map (oblique) | M1/M5; all regions | low | Partial (oblique) |
| H_XR_005 | "The Concord Remnant's scholars are everywhere the old ruins are — and they all answer up a chain that ends at the Crown." | A traveling scholar | The Remnant chain | Q_MAJOR_011/012 | medium | Partial |
| H_XR_006 | "Refugees drift south and inland from the failing frontiers — the roads are full of folk fleeing something they can't name." | Any road / a refugee | Population-flow (oblique) | KM/SP/CH | medium | Partial (oblique) |
| H_XR_007 | "The Gravecallers' grief-cult follows the worst-failing dead — wherever a region's dead wake worst, they come." | A Mourner / a watchman | Cult-spread (DM-oblique) | all crisis-regions | medium | Partial (oblique) |
| H_XR_008 | "Trade-meets at the world's edges — Spine-Foot in the north, the Gulf ports in the south — bridge the settled and the strange." | A caravan-master | Cross-world bridges | WS/HGP | low | True |
| H_XR_009 | "A trustworthy guide is worth a fortune in the wild lands — the steppe, the flats, the deep wood, the great ruin all kill the unguided." | Any frontier town / a guide | Survival-guides | all wild regions | medium | True |
| H_XR_010 | "The far south keeps a faith that still holds its dead — they say in the Sunmark the rites have never failed." | A pilgrim / a trader | The hopeful contrast (oblique) | SUN quests | low | Partial (oblique) |
| H_XR_011 | "The Emberfell fire-priests, the Glassmere bankers, the salt-clans — each holds a piece of the world's old grief in their own tongue." | A traveling sage | Thematic web (oblique) | ET/GL/SALT | low | Partial (oblique) |
| H_XR_012 | "There's a continent across the sea — Surren — that never knew the Concord at all." | A Gulf foreign-factor | World-horizon | HGP / Surren scaffold | low | True |

## Cross-Region Rumors (R_XR_NNN)

| # | Rumor (player-facing) | Source | Truth | Points toward | Notes |
|---|---|---|---|---|---|
| R_XR_001 | "The same sickness of the dead is spreading across the whole continent." | Road-talk | Partial (oblique) | the crisis-spread | M1/M5; never the cause |
| R_XR_002 | "The old Mourner songs, sung from the Reach to the Gulf, all name 'the grey hands.'" | A grief-keeper | Partial (oblique) | the old-songs network | M6-oblique |
| R_XR_003 | "The Cinder Ledger will be the only power left standing when the dust settles." | A factor | Partial | Q_MAJOR_004 | the monopoly |
| R_XR_004 | "The Concord Remnant means to *rebuild* the old empire — and that should frighten everyone." | A scholar | Partial | Q_MAJOR_011/012 | the bad-ending lever |
| R_XR_005 | "It's worst at the Ruin'd Crown — the dead there never stay buried." | A traveler | Partial (oblique) | CH quests | crisis-worst-here; NOT the cause |
| R_XR_006 | "The steppe-clans and the grove-tribes say the trouble is the *settled* world's doom, not theirs." | A trader | Partial (oblique) | the outside views | WS/SUN |
| R_XR_007 | "Every dying frontier sends its folk fleeing toward the settled lands." | A refugee | Partial | population-flow | KM/SP |
| R_XR_008 | "Whatever started all this, it started long ago and far to the north and west — in the old country." | A wandering sage | Partial (oblique) | toward the Reach/Hollowmere | NEVER confirm the keystone |

## Cross-Region Jobs & Events (JOB_XR_NNN)

| # | Job/Event (player-facing) | Source / Trigger | Type | Reward | Risk | Notes |
|---|---|---|---|---|---|---|
| JOB_XR_001 | "Escort a Mourner elder's token and song to a far-region grief-keeper." | A Mourner elder | Courier/lore | Network goodwill | medium | M6-oblique; links nodes |
| JOB_XR_002 | "Guard a long-haul caravan across a region-border (flats, passes, wood, or grass)." | A caravan-master | Escort/travel | Coin + route | medium | reinforces travel |
| JOB_XR_003 | "Carry a Ledger (or anti-Ledger) dispatch between two regional factors." | A factor | Courier | Coin + faction rep | medium | Q_MAJOR_004 |
| JOB_XR_004 | "Hire a wild-lands guide and survive a crossing the unguided don't." | Any frontier guide | Survival | Safe passage | medium | guide-economy |
| JOB_XR_005 | "Investigate why a stretch of road has 'gone bad' — the dead, or bandits, or both." | A road-village | Investigation | Coin + safe road | medium | M5-oblique or mundane |
| JOB_XR_006 | "Ferry a refugee family from a failing frontier to safer ground." | A refugee | Escort/mercy | Goodwill | low | humane; population-flow |
| JOB_XR_007 | "Carry word of one region's troubles to a region that's never heard of them." | A traveler | Courier | Coin + contacts | low | the 'outside view' |
| JOB_XR_008 | "Track a Gravecaller emissary moving between two regions' worst-failing dead." | A Mourner / a watchman | Investigation/pursuit | Anti-cult intel | high | DM-oblique; cult-spread |

## Related Files
- [`../by_region/`](../by_region/) (all 12 far-continent quest files)
- [`../../04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md`](../../04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md)
- [`../../08_npcs/by_region/`](../../08_npcs/by_region/) (far-continent NPC rosters)
