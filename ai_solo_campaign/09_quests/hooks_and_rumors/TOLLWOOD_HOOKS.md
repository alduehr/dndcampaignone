# TOLLWOOD_HOOKS.md — Regional Hooks (Stage 7, Ring 1)

---
type: quest
secrecy: mixed
status: static
region: Tollwood
factions: [all]
level_range: 2-7
related: [../regional_quests/, ../../05_regions/TOLLWOOD.md, TOLLWOOD_RUMORS.md]
tags: [type:quest, function:quest-hook, secrecy:mixed, region:tollwood, ring-1]
---

## AI Use

Region-wide hooks for the Tollwood (the Reach's deep eastern forest). Surface through fiction (jobs, NPCs in need, postings, road-talk), never as a menu. Each lists level, source, surface goal, authored content, and hidden link (DM-only). **The deep-wood secret is gated/oblique — never name the Hollow Court or the harvest mechanism; cap reveals.** 22 hooks.

## Hooks by Area

### Hartfell & the East Road
| # | Hook | Lvl | Source | Surface Goal | Points To (authored) | Hidden Link (DM) |
|---|---|---|---|---|---|---|
| TW-H1 | "The Marked Oaks" (dev) | 3-5 | Woodfolk / Brann / Edda Sorrel | Stop or expose Dorr's deep-cutting | Q_THE_MARKED_OAKS; Hartfell | regional clock (the Old Mast stirs); M5/M6 oblique |
| TW-H2 | "Toll-War" (dev) | 2-4 | Road-Warden Captain Brannoch Vey | Deal with the Tollstone Cross bandits | Q_THE_TOLL_WAR; Tollstone Cross | Renn turnable; toll-war; East Road to Caradril |
| TW-H3 | "A Guide into the Wood" | 2-3 | Innkeep Marrec Tull / Brann | Hire a guide; learn the forest-rules | Hartfell; Coldhearth | the wood's safety on-ramp |
| TW-H8 | "Vey's Doubt" | 3-4 | Brannoch Vey | Help a road-warden who privately keeps the old rules | Hartfell | a turnable Compact ally |
| TW-H9 | "Timber for the City" | 2-4 | Hesk Dorr / a city buyer | Escort a timber-cart east to Caradril | East Road; TRAVEL_ROUTES_RING1 | opens the Caradril approach |

### Tollstone Cross & the Road-Node
| # | Hook | Lvl | Source | Surface Goal | Points To | Hidden Link (DM) |
|---|---|---|---|---|---|---|
| TW-H4 | "Renn or Skell" | 2-4 | Cady Renn / a resident | Tip the Tollmen's internal struggle | Tollstone Cross | Renn (grey ally) vs Skell (murder) |
| TW-H5 | "The Drowned Vault" (dev) | 2-4 | The Tollmen's fear / Smith Doune | Investigate the leaking node below the arch | Q_THE_DROWNED_VAULT; Greenward Toll-Station | M2/M5 fragment; the local drift |
| TW-H13 | "The Honest Corner" | 2-3 | Smith Doune / Ale-wife Pell | Protect the road-hamlet's honest folk | Tollstone Cross | the toll-war's human cost |

### Coldhearth & the Mid-Wood
| # | Hook | Lvl | Source | Surface Goal | Points To | Hidden Link (DM) |
|---|---|---|---|---|---|---|
| TW-H10 | "The Bargain" (dev) | 3-5 | Goodwife Sennet | Earn Coldhearth's trust; learn the forest-rules and history | Q_THE_BARGAIN; Coldhearth | M5/M6 oblique; the deep secret's gateway |
| TW-H11 | "The Reckless Guide" (dev) | 4-5 | Coldhearth / Old Gethin | Find Wren-of-the-Wood, gone too deep | Q_THE_RECKLESS_GUIDE; Coldhearth; Hanging Oaks | the deep's pull; cult-thread |
| TW-H12 | "What Sennet Sings" | 4-6 | Goodwife Sennet | Earn the old songs of the wood | Coldhearth | gated oblique M5/M6 fragment |
| TW-H14 | "Charcoal and Fear" | 2-3 | Old Gethin | Help the burners as the wood turns dangerous | Coldhearth; the camps | the deep-cutting's effect; safety work |

### The Deep Wood & the Old Mast (gated)
| # | Hook | Lvl | Source | Surface Goal | Points To | Hidden Link (DM) |
|---|---|---|---|---|---|---|
| TW-H6 | "The Hanging Oaks" (dev) | 4-6 | Gravecaller cell / Sennet's warning | Confront or learn from the cell and the old dead | Q_THE_HANGING_OAKS; The Hanging Oaks | M6 oblique fragment; the cult in the wood |
| TW-H7 | "To the Edge and No Further" (dev) | 6-8 | Brann / Sennet / curiosity | A guided approach to the Old Mast edge | Q_TO_THE_EDGE; The Old Mast | gated oblique M5/M6; the presence; dread |
| TW-H15 | "Wake Not the Wood" | 5-7 | Sennet / a frightened logger | Stop the Gravecallers/Ledger from waking the Old Mast | The Old Mast; Hanging Oaks; the camps | regional-disaster prevention (clock) |

### Faction & Travel Threads
| # | Hook | Lvl | Source | Surface Goal | Points To | Hidden Link (DM) |
|---|---|---|---|---|---|---|
| TW-H16 | "The Roads That Bend" | 3-5 | A Remnant survey-scholar | Help map why the Concord roads avoid the deep wood | Hartfell; TOLLWOOD_SITES | M2/Old Mast hint; Remnant interest |
| TW-H17 | "The Courier" | 3-5 | The watch / a suspicious local | Trace the Gravecaller courier through Hartfell | Hartfell; the deep cells | M6 oblique door; the wood's cult network |
| TW-H18 | "Wolves on the Road" | 2-4 | Travelers / the watch | Clear a predator pack menacing the East Road | TOLLWOOD_SITES; the road | real-beast threat; road safety |
| TW-H19 | "The Lost Crew" | 3-5 | Hartfell / a foreman | Find a logging crew that didn't come back from the deep | the camps; mid-wood | the deep-cutting danger; the old dead |
| TW-H20 | "The Mourner's Long Road" | 2-4 | Edda Sorrel / Sennet | Carry an old-custom message between Reach/Vale/Tollwood Mourners | links the regional Mourners | M6 folk-truth network (gated) |
| TW-H21 | "Offerings" | 1-2 | A woodfolk elder | Learn and keep the toll-shrine customs (a low on-ramp) | the Coppice Shrines | the wood's rules; safety |
| TW-H22 | "East to the City" | 3-5 | Any Tollwood patron | Travel the East Road on to Caradril | TRAVEL_ROUTES_RING1; CARADRIL | bridges Ring 1 → mid-game hub |

## Related Files

- [`../../05_regions/TOLLWOOD.md`](../../05_regions/TOLLWOOD.md)
- [`TOLLWOOD_RUMORS.md`](TOLLWOOD_RUMORS.md)
- [`../regional_quests/`](../regional_quests/)
- [`../../04_world_atlas/TRAVEL_ROUTES_RING1.md`](../../04_world_atlas/TRAVEL_ROUTES_RING1.md)
