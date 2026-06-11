# ASHGARDEN_VALE_HOOKS.md — Regional Hooks (Stage 7, Ring 1)

---
type: quest
secrecy: mixed
status: static
region: Ashgarden Vale
factions: [all]
level_range: 1-6
related: [../regional_quests/, ../../05_regions/ASHGARDEN_VALE.md, ASHGARDEN_VALE_RUMORS.md]
tags: [type:quest, function:quest-hook, secrecy:mixed, region:ashgarden-vale, ring-1]
---

## AI Use

Region-wide hooks for the Ashgarden Vale (the Reach's gentle southern neighbor). Surface through fiction (jobs, NPCs in need, postings, overheard talk), never as a menu. Each lists level, source, surface goal, the authored content it points to, and the hidden link (DM-only). **Cap Vale reveals at R1 in Act-1-level play; hidden links are DM-only.** 22 hooks.

## Hooks by Area

### Tilbrook & the Northern Vale (the honest window)
| # | Hook | Lvl | Source | Surface Goal | Points To (authored) | Hidden Link (DM) |
|---|---|---|---|---|---|---|
| AV-H11 | "The Loaf That Moves" (dev) | 1-2 | Old Mam Tace | Settle a grave-field grave that won't stay closed | Q_THE_LOAF_THAT_MOVES; Tilbrook | M5 drift in the Vale; honest M1 window |
| AV-H12 | "The Marks on the Doors" (dev) | 2-3 | Miller Sael Brunt | Fight or expose Pell's foreclosures | Q_THE_MARKS_ON_THE_DOORS; Pellow Grange | M3 relic-quarrying; Monopoly clock |
| AV-H13 | "A Last Word in the Vale" | 2-3 | Ale-wife Genna / village | Reach Widow Hessit before the Gravecallers do | Tilbrook; Marrow Cross | Vale cult-seed; M3 door |
| AV-H14 | "Grain for the South" | 1-2 | Brunt / a Caradril carter | Escort a grain-cart south toward Caradril | South Road; TRAVEL_ROUTES_RING1 | opens the Caradril approach |

### Orchardmere & the Lake
| # | Hook | Lvl | Source | Surface Goal | Points To | Hidden Link (DM) |
|---|---|---|---|---|---|---|
| AV-H1 | "The Funeral Done Twice" (dev) | 1-3 | A grieving family | Find why a reburied mother won't rest | Q_THE_FUNERAL_DONE_TWICE; Orchardmere | M1/M5 Vale echo; the cover-up |
| AV-H2 | "The Moot's Silence" | 2-4 | Mother Ezrith Combe / a clerk | Document or break the harvest-moot's cover-up | Orchardmere (Moot-Hall) | suppressed failure-reports (M1/M5) |
| AV-H3 | "Saint's Bones" (dev) | 2-4 | Mother Combe | Investigate Pell's relic-buying | Q_SAINTS_BONES; Pell's Counting-Yard | M3 (relics = the dead) |
| AV-H4 | "The Press-Cellar" | 1-2 | Goodwife Orrel | Clear foul air / a haunting from a cider-cellar | Orchardmere (Pressyards) | gentle M5; cellar hazard |
| AV-H5 | "The Reeve's Trust" | 2-3 | Moot-Reeve Halsa Tindle | Help the Reeve keep the Vale calm (the cover-up's side) | Orchardmere | the cover-up from inside; moral choice |

### Saint Veddow's Rest & the Pilgrim Road
| # | Hook | Lvl | Source | Surface Goal | Points To | Hidden Link (DM) |
|---|---|---|---|---|---|---|
| AV-H8 | "The Saint Who Weeps" (dev) | 2-4 | A pilgrim / Mother Sennet | Find why the shrine's rests are failing | Q_THE_SAINT_WHO_WEEPS; Saint Veddow's | M1/M5 echo; M2 telegraph (the node) |
| AV-H9 | "The Sealed Door" (dev) | 4-6 | Oneth Vael / curiosity | Get into (or keep shut) the inner tomb | Q_THE_SEALED_DOOR; Saint Veddow's Tomb | M2/M6 fragments; the seal |
| AV-H6 | "The Scholar's Bargain" | 3-5 | Sub-Lector Oneth Vael | Help the Remnant gain tomb access | Saint Veddow's; the Remnant | Reclamation clock at a Vale node |
| AV-H7 | "Adwen's Doubt" | 3-5 | Warden Sister Adwen | Help a seal-keeper who can't explain her dread | Saint Veddow's; Wardens | Warden truth-fragment (M6; conditional) |
| AV-H10 | "Crowd of the Faithful" | 2-3 | A keeper | Prevent a pilgrim panic when a rite fails publicly | Saint Veddow's | crowd hazard; the failing promise |

### The Orchard Ruins & the Country
| # | Hook | Lvl | Source | Surface Goal | Points To | Hidden Link (DM) |
|---|---|---|---|---|---|---|
| AV-H15 | "The Sheep Stone" | 1-3 | Goodman Orrick (Nettlecombe) | Settle the dusk-walker of an orchard hamlet | ASHGARDEN_VALE_SITES (Nettlecombe) | gentle M3/M5 |
| AV-H16 | "What's Under the Orchard" (dev) | 2-4 | Remnant / a curious local | Explore the Buried Cloister | Q_WHATS_UNDER_THE_ORCHARD; The Buried Cloister | M2/M6 fragment; M3 |
| AV-H17 | "The Crows of Marrow Cross" (dev) | 3-5 | Gibbet-keeper Sorle / Mourners | Lay the gibbet's wrathful dead; find the recruiter | Q_THE_CROWS_OF_MARROW_CROSS; Marrow Cross | wrathful dead; Vale cult-seed |
| AV-H18 | "The Grey Woman of the Down" | 2-4 | A shepherd | Lay a Remembrance walking the southern downs | ASHGARDEN_VALE_SITES (Downs) | M5; the drift reaches the downs |

### Faction & Travel Threads
| # | Hook | Lvl | Source | Surface Goal | Points To | Hidden Link (DM) |
|---|---|---|---|---|---|---|
| AV-H19 | "The Ledger's Quiet Cart" | 2-4 | A drover / Mourner | Stop or trace a relic-cart bound south | Downs; Pellow Grange | M3; Monopoly clock; Caradril thread |
| AV-H20 | "The Mourner's Errand" | 1-3 | Mother Combe | Carry a message/song to a Reach or Caradril Mourner | links Reach ↔ Vale ↔ Caradril Mourners | M6 folk-truth network (gated) |
| AV-H21 | "Pilgrim Escort" | 1-2 | A pilgrim family | Guard pilgrims along the pilgrim road | Saint Veddow's; pilgrim road | low-risk on-ramp; rumor delivery |
| AV-H22 | "South to the City" | 3-5 | Any Vale patron | Travel the South Road on to Caradril | TRAVEL_ROUTES_RING1; CARADRIL | bridges Ring 1 → mid-game hub |

## Related Files

- [`../../05_regions/ASHGARDEN_VALE.md`](../../05_regions/ASHGARDEN_VALE.md)
- [`ASHGARDEN_VALE_RUMORS.md`](ASHGARDEN_VALE_RUMORS.md)
- [`../regional_quests/`](../regional_quests/)
- [`../../04_world_atlas/TRAVEL_ROUTES_RING1.md`](../../04_world_atlas/TRAVEL_ROUTES_RING1.md)
