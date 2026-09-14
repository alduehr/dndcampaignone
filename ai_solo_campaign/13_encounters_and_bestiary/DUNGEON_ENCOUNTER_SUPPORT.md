# DUNGEON_ENCOUNTER_SUPPORT.md — Encounter Support for All Dungeons & Ruins

---
type: encounter
secrecy: mixed
status: static
region: Orrun
factions: [all]
level_range: 1-20
related: [STAGE_12_ADVERSARIES.md, BESTIARY_INDEX.md, ../10_dungeons_and_ruins/DUNGEON_INDEX.md, SOLO_ENCOUNTER_SCALING.md]
tags: [type:encounter, secrecy:mixed, function:dungeon-support, solo-tuned]
---

## AI Use

Encounter support for **every dungeon/ruin file in `10_dungeons_and_ruins/`** (36 sites, D1–D36). Each site already has its own occupants and boss in its file; this provides the **wandering/refresh encounter layer, the adversary roster cross-reference, and the solo-tuning notes** so the AI DM can keep a delve alive without inventing biome-wrong foes. The Stage 12 dungeon adversaries (`STAGE_12_ADVERSARIES.md`) cover the original site-foes; this maps them to sites and adds the generic dungeon creature layer.

**Secrecy:** the Under-Shrine (D23) apex is **DM-only/gated**. Never run its wandering layer as a normal dungeon.

## Generic Dungeon Wandering Layer (any ruin interior)

When a delve needs a wandering encounter (noise, time pressure, a failed stealth roll — not a movement tax), roll d8:

| d8 | Wandering encounter | Type | Solo note |
|---|---|---|---|
| 1 | A drifting Remembrance (the site's dead) | [Dead] | rite/parley/avoid; bound to the level |
| 2 | A lesser construct/sentinel waking | [Construct] | 1 only; bound; watchword stands it down |
| 3 | An ooze in a flooded/refuse passage | [Ooze] | slow; avoidable; blocks a route |
| 4 | A swarm (rats/insects/bats) disturbed | [Swarm] | flee-able; area-deny, not lethal |
| 5 | A scavenger humanoid (delver/cultist/agent) | [Social/Combat] | parley first; may be a rival, not a foe |
| 6 | A trap/hazard re-arming or a collapse threat | [Hazard] | a check, not a fight |
| 7 | A memory-echo haunt replaying (a clue) | [Dead/Clue] | atmosphere + fragment; can't pursue |
| 8 | "Nothing — but the cold deepens" (telegraph) | [Noncombat] | warns of the boss/deep zone ahead |

**Solo rule:** wandering encounters in a solo delve are **single foes, avoidable, or hazards** — never a fresh group on a wounded PC. Use them to pace, warn, and deliver clues, then let the PC rest or retreat (bound foes can't chase).

## Generic Dungeon Creature Layer (by site type)

| Site type | Typical occupants | Boss tier | Hazards |
|---|---|---|---|
| **Concord node / relay vault** | Remembrance dead, lesser sentinels, relay-motes | Construct-Guardian / Choir-Keeper (bound) | thinning aura, relay-blast, collapse |
| **Barrow / tomb** | barrow-shades, skeletons, carrion swarm | Barrow-Wight (bound) | grave-traps, cave-in, the dead rousing |
| **Drowned / flooded ruin** | drowned dead, ooze, aberration (deep) | flooded-deep aberration / Choir-Keeper | drowning, dark, current, collapse |
| **Cult site (Gravecaller/heresy)** | cultists, fanatic, bound fiend, a revenant | Cult Fanatic + summon / Wrong-Come-Back | rite-traps, false comfort, the breaking |
| **Salt / desiccation ruin** | salt-mummies, salt-stalker, mirage-spirit | desiccated-dead set-piece | heat, thirst, glare, salt-collapse |
| **Volcanic / ash works** | ash-bound dead, fire mephits, ash-fiend | Caldera Guardian (bound) | heat, gas, lava, ashfall |
| **City undercity / criminal warren** | syndicate muscle, oozes, urban dead | Sunken Wards apex / a lieutenant | flooded dark, traps, the watch |
| **Living-faith grove (Sunmark)** | grove-spirits, benign fey, plant guardians | Grove-Warden (benign — a *test*, not a kill) | curse-of-trespass, plant snares (nonlethal) |

---

## Per-Site Adversary Cross-Reference (D1–D36)

*(Each site's full occupants are in its own file in `10_dungeons_and_ruins/`. This maps the primary adversary profile to use.)*

### Sundering Reach (Ring 0)
| Site | Primary adversary | Profile | Solo danger |
|---|---|---|---|
| The Peat Chapel (first delve) | weak Remembrance + fen beast | HORROR #1, BESTIARY beasts | low |
| The Sunken Tollhouse | drowned dead + smugglers | STAGE_12 #1/#5 | low-mod |
| The Deep Adit | thin-touch hazard + Remembrance | HORROR curses + #1 | mod |
| The Whispering Cairn | memory-echo haunt (archive) | HORROR #2 | low |
| The Barrow of Nine Doors | barrow-shades + a Barrow-Wight | HORROR #4 | mod |
| The Ledger Vault (heist) | guards + spy + animated object | FACTION (Ledger) + constructs | mod |
| The Greyfens Deep | drowned dead + luring light + Fen-Thing | STAGE_12 #1/#6, HORROR #2/aberration | mod |
| The Basin Keystone Approach | Choir-Keeper + dread (gated below) | STAGE_12 #2 | high (bound) |
| **The Under-Shrine Approach (DM-only)** | **Custodians (apex, gated)** | STAGE_12 #8 | **endgame** |

### Ashgarden Vale (Ring 1 S)
| Site | Primary adversary | Profile | Solo danger |
|---|---|---|---|
| The Pellow Grange | Ledger crew + relic hazard | FACTION (Ledger) | low-mod |
| The Buried Cloister | Concord dead + lesser sentinel | STAGE_12 #1, constructs | mod |
| Saint Veddow's Tomb (Inner Shrine) | Choir-Keeper-tier dead (gated) | STAGE_12 #2 | mod-high (bound) |

### Tollwood (Ring 1 E)
| Site | Primary adversary | Profile | Solo danger |
|---|---|---|---|
| The Greenward Toll-Station | drowned road-dead + Tollmen | STAGE_12 #1, FACTION (Tollmen) | low-mod |
| The Hanging Oaks | Gravecaller cell + a revenant | FACTION (Gravecallers), HORROR #3 | mod |
| The Old Mast (gated) | Old-Wood Presence + Mast-Beast | HORROR fey-presence, BOSS B3 | high (gated) |

### Pale Coast (Ring 1 W)
| Site | Primary adversary | Profile | Solo danger |
|---|---|---|---|
| The Drowned Lamp | drowned mariner dead + node | HORROR #6, STAGE_12 #1 | mod |
| The Wreckers' Caves | wreckers + sea hag + drowned dead | FACTION (wreckers), HORROR #6/#9 | mod |
| The Skerry Shrine (gated) | Choir-Keeper-tier + sea hazards | STAGE_12 #2 | high (gated) |

### Caradril (city)
| Site | Primary adversary | Profile | Solo danger |
|---|---|---|---|
| The Sunken Wards Deep | constructs + Reclaimers + Syndicate + dead | STAGE_12 #1/#3/#4/#5 | mod-high (graded) |
| The Ashmarket Undercroft | Syndicate + relic-sludge ooze | STAGE_12 #5, BESTIARY oozes | mod |

### Far / mid-continent (Ring 2+)
| Site | Region | Primary adversary | Profile | Solo danger |
|---|---|---|---|---|
| The Nine Locks Sunken Stair | Verdance | drowned dead + lesser sentinel | STAGE_12 #1/#3 | mod |
| The Glassmere Reliquary Vaults | Glassmere | Reclaimers + construct + golem-like | STAGE_12 #3/#4, BOSS B10 | high |
| The Three Bridges Counting-Deep | Glassmere | Ledger guards + spy + vault construct | FACTION (Ledger), constructs | mod-high |
| The Marrowdowns Barrow Complex | Marrowdowns | barrow-wights + mass-undead set-piece | HORROR #4/#8 | high |
| The Sallowmarch Drowned Steps | Sallowmarch | drowned dead + tidal aberration | HORROR #6, DROWNED_STEPS | high |
| The Hollow Gulf Wreck-Reef | Hollow Gulf | drowned mariner dead + sea aberration | HORROR #6, aberration | high |
| The Wender Sky-Stones (non-Concord) | Wender | steppe spirits + outside-view echo | HORROR (echo), SUNMARK-style benign/strange | mod |
| The Sunhollow Great Grove (living-faith) | Sunmark | benign grove-guardian (a *test*) | SUNMARK, BESTIARY celestial/fey | low-mod (nonlethal) |
| The Highmark Frozen Works | Highmark | ice-locked construct + frost dead | STAGE_12 #3, HORROR | high |
| The Cindern Waste Buried Works | Emberfell | ash-bound dead + Cindern guardian | HORROR #7, STAGE_12 #7-style | high |
| The Saltmere Deep Towns | Saltmere | salt-mummies + drowned-town haunt | HORROR #5/#8 | high |
| The Hethewald Old Holds (gated) | Hethewald | deep-wood presence + Concord dead | HORROR fey-presence, STAGE_12 #1 | high (gated) |
| The Karran Old Iron Forts | Karran | warlord humanoids + ore-construct | FACTION (warlords), constructs | mod-high |
| The Old Concord Heartlands Ruin | Heartlands | apex Construct-Guardian + scavengers + Reclaimers | STAGE_12 #3 (apex), BOSS B14 | very high |
| The Emberfell Caldera Descent | Emberfell | Caldera Guardian + fire hazards | STAGE_12 #7 | very high |

---

## Dungeon Solo-Safety Constants

- **Bound guardians cannot pursue** past their chamber/site — retreat is always available.
- **Rest constraints** are per-site (in each dungeon file); when none, allow a short rest in a cleared, defensible room.
- **Most "dead" resolve by rite/parley/avoidance**; combat is optional in the great majority of rooms.
- **Wandering layer is single-foe/hazard** for a solo PC, used to pace and warn — never to swarm a wounded delver.
- **One signature boss per site**, with a non-combat out and a weakness the PC can scout (`BOSS_AND_APEX_THREATS.md`).
- **Update state** on delve milestones: clues to `KNOWN_CLUES.md`, site-state changes to `CONSEQUENCES.md`, faction reactions to `FACTION_STATE.md`.

## Related Files

- [`STAGE_12_ADVERSARIES.md`](STAGE_12_ADVERSARIES.md) (site adversary originals)
- [`BESTIARY_INDEX.md`](BESTIARY_INDEX.md) · [`BOSS_AND_APEX_THREATS.md`](BOSS_AND_APEX_THREATS.md)
- [`../10_dungeons_and_ruins/DUNGEON_INDEX.md`](../10_dungeons_and_ruins/DUNGEON_INDEX.md)
- [`SOLO_ENCOUNTER_SCALING.md`](SOLO_ENCOUNTER_SCALING.md)
