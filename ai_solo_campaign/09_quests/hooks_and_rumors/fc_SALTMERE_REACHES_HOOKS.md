# fc_SALTMERE_REACHES_HOOKS.md — Far-Continent Hooks, Rumors & Jobs (Stage 10)

---
type: quest
secrecy: mixed
status: static
region: The Saltmere Reaches
factions: [all]
level_range: 11-15
related: [../by_region/SALTMERE_REACHES_QUESTS.md, ../../08_npcs/by_region/SALTMERE_REACHES_NPCS.md, ../../04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md]
tags: [type:quest, function:quest-hook, far-continent, stage-10, region:saltmere-reaches, secrecy:mixed]
---

## AI Use

Short-form hooks, rumors, and jobs for the Saltmere Reaches (a dying brackish inland-sea basin of salt-clans and drowned towns; Brackhold, the Drowned Towns, the Bonepan Flats, Saltcairn; Lvl 11–15). Surface through fiction (the salt-hold, the receding lake-edge, the white flats, the dying clan-towns), never as a menu. Cast from `08_npcs/by_region/SALTMERE_REACHES_NPCS.md`. The "going-down" is a **pre-Concord echo**, NOT the keystone or harvest. Drowned towns are pre-Concord ruins. No NPC knows the apex truth. 10 hooks + 8 rumors + 5 jobs.

## Hooks (H_SALT_NNN)

| # | Hook text (player-facing) | Where / Who | Points toward | Related | Risk | Truth |
|---|---|---|---|---|---|---|
| H_SALT_001 | "The lake gave back a whole drowned town — and its dead are walking onto the flats." | Brackhold / Matriarch Bryd Saltmere | Pre-Concord echo (oblique) | Q_SALT_001 | high | Partial (oblique) |
| H_SALT_002 | "Delver Oss found something in a deep drowned town he won't speak of — and he won't go back alone." | The lake-edge / Oss | Deep drowned-ruin delve | Q_SALT_002 | high | Partial (oblique) |
| H_SALT_003 | "The Ledger's strangling the salt-trade — the clans will starve before they'll bow." | Brackhold / Salt-Master Sera Brackhold | Anti-Ledger trade-war | Q_SALT_003 | medium | True |
| H_SALT_004 | "Salt-Mother Tess keeps the 'going-down' lament — older than the Concord, the clans say." | The salt-shrines / Tess Brackhold | Mourner old-songs (oblique) | Q_SALT_004 | low | Partial (oblique) |
| H_SALT_005 | "Marek Bonepan's salt-trains keep vanishing on the white flats — to 'Mirage' and to the salt itself." | The trade-track / Marek Bonepan | Flats survival/banditry | Q_SALT_005 | high | True |
| H_SALT_006 | "A hollow-eyed wanderer at the water is teaching the grieving to 'listen' to the drowned." | The lake-edge / a bereaved clanfolk | Gravecaller emissary (DM) | Q_SALT_006 | medium | Partial (oblique) |
| H_SALT_007 | "Saltcairn is dying, and a feud with a rival hold is finishing what the lake started." | Saltcairn / Clan-Elder Tess Saltcairn | Clan-feud / humane aid | Q_SALT_007 | medium | True |
| H_SALT_008 | "Fence Doll Tallow buys drowned-town finds — and some of them are 'wrong,' she knows it." | The lake-edge / Doll Tallow | Relic-trade (M2-oblique) | Q_SALT_002 | medium | Partial (oblique) |
| H_SALT_009 | "Old Salt the hermit 'talks to the going-down' in the Ghostmark hills — half-mad, but he knows things." | The Ghostmark edge | Oblique lore-source | Q_SALT_004 | low | Partial (oblique) |
| H_SALT_010 | "Marek Bonepan knows the one land-road out of the dying basin — south, to the wider world." | The trade-track / Marek Bonepan | Route onward | Q_SALT_005 | medium | True |

## Rumors (R_SALT_NNN)

| # | Rumor (player-facing) | Source | Truth | Points toward | Notes |
|---|---|---|---|---|---|
| R_SALT_001 | "The Saltmere is dying — the lake takes a town a year, as it did in the going-down." | A salt-clanner | Partial | basin decline | older fall |
| R_SALT_002 | "The drowned towns went under in a fall older than the Concord itself." | A clan-elder | Partial (oblique) | the older fall | NOT keystone |
| R_SALT_003 | "The drowned dead stir worse than they have in a hundred years." | A lake-pilot | Partial (oblique) | Q_SALT_001/002 | M5-resonant |
| R_SALT_004 | "Salt-Mother Tess's lament names the same grey hands the far Mourners sing of." | A salt-singer | Partial (oblique) | Q_SALT_004 | M6-oblique |
| R_SALT_005 | "Delver Oss is the only soul who goes into the drowned towns and comes back." | A clanner | True | Q_SALT_002 | deep access |
| R_SALT_006 | "The Ledger pays 'strange prices' for what the delvers raise." | A fence | Partial (oblique) | Q_SALT_003 | M3-oblique |
| R_SALT_007 | "The Ghostmark hills 'hum' lately, the shepherds say." | A salt-goat herder | Partial (oblique) | atmosphere | M2-resonant |
| R_SALT_008 | "Two dying clans are killing each other over a grudge neither remembers the start of." | A clanner | Partial | Q_SALT_007 | feud |

## Jobs & Events (JOB_SALT_NNN)

| # | Job/Event (player-facing) | Source / Trigger | Type | Reward | Risk | Notes |
|---|---|---|---|---|---|---|
| JOB_SALT_001 | "Settle a drowned town's walking dead before they reach the hold." | Matriarch Bryd | Rite/defense | Clan-welcome | high | Q_SALT_001 |
| JOB_SALT_002 | "Guard Delver Oss on a dive into the drowned towns." | Oss | Escort/dungeon | Coin + deep loot | high | Q_SALT_002 |
| JOB_SALT_003 | "Escort a salt-caravan across the Bonepan Flats." | Marek Bonepan | Escort/survival | Coin + route south | high | Q_SALT_005 |
| JOB_SALT_004 | "Carry the going-down lament to a far Mourner elder." | Salt-Mother Tess | Courier/lore | Mourner network | low | Q_SALT_004 |
| JOB_SALT_005 | "Mediate the feud bleeding the dying clans." | Clan-Elder Tess Saltcairn | Mediation | Clan goodwill | medium | Q_SALT_007 |

## Related Files
- [`../by_region/SALTMERE_REACHES_QUESTS.md`](../by_region/SALTMERE_REACHES_QUESTS.md) · [`../../08_npcs/by_region/SALTMERE_REACHES_NPCS.md`](../../08_npcs/by_region/SALTMERE_REACHES_NPCS.md)
