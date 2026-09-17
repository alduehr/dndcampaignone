# TRAVEL_ENCOUNTERS.md — Travel Encounter Tables by Terrain and Level Band

---
type: encounter
secrecy: mixed
status: static
region: Orrun
factions: [all]
level_range: 1-20
related: [BIOME_ENCOUNTER_MATRIX.md, REGIONAL_ENCOUNTER_TABLES.md, SOLO_ENCOUNTER_SCALING.md, ../01_runner_protocol/TRAVEL_PROTOCOL.md]
tags: [type:encounter, secrecy:mixed, function:travel, all-tiers, solo-tuned]
---

## AI Use

Generic **travel encounter tables by terrain and level band**, for use when the PC is on the road/water/wild and a region-specific table isn't needed (or to supplement one). Organized by the five level bands (1–4, 5–8, 9–12, 13–16, 17–20) so the same terrain scales across the whole campaign. Travel encounters are **mostly non-combat** and should create *decisions*, not a movement tax (`TRAVEL_PROTOCOL.md`). Roll only when a result would add choice/risk/complication (`SOLO_ENCOUNTER_SCALING.md` Rule 6).

## How To Use

1. Pick **terrain** (road / wilderness / water / mountain / waste / forest).
2. Pick the **level band** matching the PC.
3. Roll d10 or pick to fit clocks/fiction.
4. Apply **travel-variant modifiers** (night/storm/fog/cold/heat/season) at the bottom.
5. For a specific region, prefer its `REGIONAL_ENCOUNTER_TABLES.md` / per-region file; use this for connective travel.

**Type legend:** [Combat] · [Social] · [Hazard] · [Dead]=Remembrance haunting · [Clue] · [Noncombat]=signs/tracks/dilemmas.

---

## ROAD / SETTLED TRAVEL

### Levels 1–4
| d10 | Encounter | Type | Solo Danger |
|---|---|---|---|
| 1 | A patrol checking travelers (Compact/local watch) | [Social] | none |
| 2 | A merchant caravan, wary, willing to trade gossip | [Social][Clue] | none |
| 3 | Toll-bandits demanding coin (morale-fragile) | [Social][Combat] | low |
| 4 | A grieving family with a dead they fear (M5) | [Social][Clue] | none |
| 5 | A lone Remembrance on the causeway, facing one way | [Dead][Clue] | low |
| 6 | A flooded/broken road stretch | [Hazard] | low |
| 7 | A wounded traveler or robbed pilgrim (aid dilemma) | [Noncombat][Social] | none |
| 8 | Fog/weather blurs the road | [Hazard] | low |
| 9 | A pack predator's signs (tracks, a carcass) | [Noncombat] | none |
| 10 | A faction agent with a job/warning | [Social][Clue] | none |

### Levels 5–8
| d10 | Encounter | Type | Solo Danger |
|---|---|---|---|
| 1 | A faction escort/reprisal (telegraphed) | [Social][Combat] | low-mod |
| 2 | A larger bandit/outlaw band at a chokepoint | [Combat] | mod |
| 3 | A merchant-prince's convoy + hired guards | [Social] | none |
| 4 | A wraith-tier Remembrance at a wayside shrine | [Dead] | mod |
| 5 | A bridge/ferry toll dispute | [Social] | low |
| 6 | A rival adventurer/agent racing the player | [Social][Clue] | low |
| 7 | A collapsed pass/washed-out crossing | [Hazard] | mod |
| 8 | Refugees fleeing a regional crisis (clock) | [Social][Clue] | none |
| 9 | A monstrous predator's hunting ground (warning) | [Noncombat] | none |
| 10 | A Concord ruin beside the road (optional delve) | [Clue][Noncombat] | varies |

### Levels 9–12
| d10 | Encounter | Type | Solo Danger |
|---|---|---|---|
| 1 | A petty-lord's toll-soldiers / hold-guard | [Social][Combat] | mod |
| 2 | A construct-guardian astride an old road-node | [Combat] | mod-high (bound) |
| 3 | A faction warband on the move (avoidable) | [Social][Combat] | high |
| 4 | A far-region official/legate with a proposition | [Social][Clue] | none |
| 5 | A relic-caravan worth a fortune (Ledger heartland) | [Social][Clue] | low |
| 6 | A banshee/grief-boss at a ruined hall | [Dead][Combat] | mod |
| 7 | A landslide/flood/fire across the route | [Hazard] | mod |
| 8 | A regional war's edge (pick a side, or pass) | [Social] | varies |
| 9 | A monstrosity raid on a hamlet (rescue) | [Combat][Social] | mod-high |
| 10 | A continental rumor that reframes a mystery (M6) | [Clue] | none |

### Levels 13–16
| d10 | Encounter | Type | Solo Danger |
|---|---|---|---|
| 1 | An apex construct/golem guarding a great ruin | [Combat] | high (bound) |
| 2 | A theocracy/protectorate crackdown checkpoint | [Social][Combat] | mod |
| 3 | A giant or wyvern's road-claim (toll-in-blood) | [Combat][Social] | high |
| 4 | A high-tier Remembrance/banshee set-piece | [Dead] | high |
| 5 | A continental power's envoy (alliance/threat) | [Social][Clue] | none |
| 6 | A cataclysm-edge hazard (eruption/quake/flood) | [Hazard] | high |
| 7 | A Reclaimer/Remnant grand-expedition crossing | [Social][Combat][Clue] | mod |
| 8 | A drowned-causeway/aberration lurking near a ford | [Combat][Hazard] | high |
| 9 | A fallen-realm ruin-field to cross (Heartlands) | [Hazard][Clue] | high |
| 10 | A clear far-proof of the harvest's reach (M6) | [Clue] | none |

### Levels 17–20
| d10 | Encounter | Type | Solo Danger |
|---|---|---|---|
| 1 | An apex creature claims the route (dragon/giant lord) | [Combat][Social] | very high |
| 2 | A faction's final-act army/blockade | [Social][Combat] | very high |
| 3 | A world-clock disaster in progress (the harvest leaking wide) | [Hazard][Clue] | high |
| 4 | An endgame ally racing to the same place | [Social] | none |
| 5 | A mass-haunt / continental drift-line (M5 climax-scale) | [Dead][Clue] | high |
| 6 | A deep-horror aberration far from its lair (very rare) | [Combat] | very high |
| 7 | A collapsing Concord work (the network failing) | [Hazard][Clue] | high |
| 8 | A Court cutout's last gambit (DM-gated) | [Social][Intrigue] | varies |
| 9 | A region's fate hangs on the player passing through | [Social] | varies |
| 10 | The road to Hollowmere/the keystone itself (endgame) | [Clue] | — |

---

## WILDERNESS / OFF-ROAD

| Band | Common (d6 sample) |
|---|---|
| **1–4** | 1 mundane predator-sign · 2 a fen/forest beast · 3 a Remembrance · 4 a hazard (mire/rockfall/cold) · 5 a hermit/forager (social) · 6 a smuggler/outlaw cache (clue) |
| **5–8** | 1 a monstrosity's range (warning) · 2 a wraith-tier dead · 3 a rival expedition · 4 a worse hazard · 5 a hidden ruin · 6 a beast fighting a beast (bypass chance) |
| **9–12** | 1 a giant/ogre's ground · 2 a construct at a node · 3 a hag's grief-bargain · 4 a flood/fire/storm · 5 a far-ruin clue · 6 a wounded apex (dilemma) |
| **13–16** | 1 a dragon/giant's hunting range · 2 a high-tier dead · 3 a fallen-realm hazard-field · 4 an aberration's strange ground · 5 an apex predator clash · 6 a continental-proof clue |
| **17–20** | 1 an apex creature's lair-edge · 2 a world-clock disaster · 3 a deep-horror sign · 4 a collapsing great-work · 5 an endgame omen · 6 a region's tipping point |

## WATER / SEA / RIVER

| Band | Common (d6 sample) |
|---|---|
| **1–4** | 1 a nervous ferry/bargeman (social) · 2 a flooded crossing · 3 a drowned Remembrance by a landing · 4 fog on the water · 5 smugglers · 6 a fishing-family in trouble (rescue) |
| **5–8** | 1 wreckers/false lights · 2 drowned mariner dead · 3 a sea/river predator (shark/croc) · 4 a storm · 5 a privateer toll · 6 a wreck worth salvaging (clue) |
| **9–12** | 1 a privateer boarding · 2 a water elemental/wave-spirit · 3 a great-river toll-war · 4 a delta fever-zone · 5 a drowned-town/causeway (clue) · 6 a sea-storm set-piece |
| **13–16** | 1 a deep-water aberration · 2 a tidal causeway hazard (Drowned Steps) · 3 a pirate fleet · 4 a drowned-tide mass-haunt · 5 a foreign ship (world-horizon) · 6 a submerged great-work |
| **17–20** | 1 a sea apex (kraken-spawn-tier) · 2 the Drowned Steps' deep horror · 3 a continental shipping crisis · 4 an endgame sea-omen · 5 a drowned-keystone echo (gated) · 6 a final crossing |

## MOUNTAIN / PASS (Highmark, Karran, Greatspine, Sunder Heights)

| Band | Common (d6 sample) |
|---|---|
| **1–4** | 1 cold/exposure · 2 a highland Remembrance (dead miner) · 3 claim-jumpers · 4 rockfall · 5 an eagle/wolf-pack · 6 a ruin/Concord Script (clue) |
| **5–8** | 1 a wolf-pack or bear · 2 an ogre/gargoyle · 3 a Remnant dig (rival) · 4 an avalanche/snapped aqueduct · 5 a wyvern's range (warning) · 6 a frozen Concord work (clue) |
| **9–12** | 1 a hill/stone giant · 2 a wyvern · 3 a warlord's pass-toll · 4 a blizzard · 5 a chimera/manticore · 6 an ice-locked ruin (M6 far-proof) |
| **13–16** | 1 a frost giant · 2 a young dragon's range · 3 an ettin/giant raid · 4 a killing blizzard/avalanche · 5 a giant-hold toll · 6 the clearest far-proof works (Highmark) |
| **17–20** | 1 an ancient dragon's domain · 2 a giant-lord's hold · 3 a continental-scale storm · 4 the oldest Concord works · 5 an endgame frontier-omen · 6 the far north's edge |

## WASTE / VOLCANIC / SALT (Cindern, Emberfell, Bonepan, Saltmere)

| Band | Common (d6 sample) |
|---|---|
| **9–12** | 1 heat/thirst/ashfall hazard · 2 ash-bound or salt-mummy dead · 3 a fire mephit/mirage-spirit · 4 a burrower (scorpion/ankheg-like) · 5 theocracy/salt-clan patrol · 6 a buried-works clue |
| **13–16** | 1 a fire elemental/ash-fiend · 2 a Caldera/Cindern guardian (bound) · 3 a deadly heat/lava/gas hazard · 4 a desiccated-dead set-piece · 5 a heresy-cult (fiend) · 6 a far-proof of the works (M6) |
| **17–20** | 1 a red dragon/fire apex · 2 a collapsing buried great-work · 3 a continental ash-storm · 4 a deep ash-horror · 5 an endgame fire-omen · 6 the deepest forbidden waste |

---

## Travel-Variant Modifiers (apply to any table)

| Variant | Effect |
|---|---|
| **Night** | +1 step danger on combat rows; Perception/Survival DCs +2; Remembrance dead more active; ambush risk up. Offer the choice to camp/wait. |
| **Storm / rain** | ranged & vision penalties; flood/lightning/cold hazards; navigation Survival DC +2–4; foes and PC both hampered. |
| **Fog** | vision <30 ft; ambush & getting-lost risk; Remembrance dead and luring lights thrive; great for *evasion* too. |
| **Cold / blizzard** | exhaustion via Con saves (DC 10→15 by severity); shelter becomes the goal; tracks easy but travel slow. |
| **Heat / drought** | exhaustion via Con saves; water becomes a resource; salt/ash undead amplified; midday glare hazard. |
| **Season** | spring floods (water/delta), summer heat (waste/salt), autumn storms (coast/sea), winter cold/short days (mountain/steppe). Shift the terrain table toward its seasonal hazard. |

**Solo rule:** a variant should *change the decision* (camp, reroute, push on at a cost), not just add damage. Always give the PC a way to read the conditions (Survival/Nature check) and choose.

## Related Files

- [`BIOME_ENCOUNTER_MATRIX.md`](BIOME_ENCOUNTER_MATRIX.md) · [`REGIONAL_ENCOUNTER_TABLES.md`](REGIONAL_ENCOUNTER_TABLES.md)
- [`SOLO_ENCOUNTER_SCALING.md`](SOLO_ENCOUNTER_SCALING.md)
- [`../01_runner_protocol/TRAVEL_PROTOCOL.md`](../01_runner_protocol/TRAVEL_PROTOCOL.md)
