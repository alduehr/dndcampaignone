# BESTIARY_INDEX.md — Master Creature List

---
type: encounter
secrecy: mixed
status: static
region: Orrun
level_range: 1-20
related: [CREATURE_SOURCE_REFERENCE.md, ENCOUNTER_INDEX.md, BIOME_ENCOUNTER_MATRIX.md, HORROR_AND_CURSE_THREATS.md, BOSS_AND_APEX_THREATS.md, STAGE_12_ADVERSARIES.md]
tags: [type:encounter, secrecy:mixed, function:bestiary, master-index, creature-list]
---

## AI Use

The master list of **every creature category used across the campaign**, with type, CR band, where it appears, and whether it is an official source-reference (Track A) or a campaign-original (Track B). Use this to find a creature fast, confirm it has a home biome, and jump to its full notes. Source-handling conventions are defined in `CREATURE_SOURCE_REFERENCE.md`. Track-B originals are written out in `STAGE_12_ADVERSARIES.md`, `HORROR_AND_CURSE_THREATS.md`, `BOSS_AND_APEX_THREATS.md`, and the regional files.

**Secrecy:** the Hollow Court Custodians and the deep-harvest horror entries are **DM-only**; never surface them before their gates (REV_007 / endgame).

## How To Read This Index

- **Track:** A = official, source-referenced (DM pulls the stat block from the named book). B = campaign-original, abbreviated summary in-repo. R = reskin (official chassis + original behavior).
- **Source shorthand** (appended to the Track cell for Track-A rows, e.g. `A · 2024 MM`): the published book the AI DM pulls the stat block from — `2024 MM` (2024 Monster Manual, the default for any classic monster updated in 2024), `2014 MM` (2014 Monster Manual, for creatures not updated in 2024), `MotM` (Monsters of the Multiverse, 2022), `MToF` (Mordenkainen's Tome of Foes, 2018), `VGtM` (Volo's Guide to Monsters, 2016), `VRGtR` (Van Richten's Guide to Ravenloft, 2021 — the gothic-horror source), `RtHW` (Ravenloft: The Horrors Within, 2026 — **verified and integrated 2026-07-07**; largely VRGtR creatures updated to 2024 rules plus new cosmic-horror entries), `FToD` (Fizban's Treasury of Dragons, 2021), `XGtE` (Xanathar's Guide, 2017), `TCoE` (Tasha's Cauldron, 2020), `GoS` (Ghosts of Saltmarsh, 2019), `ToA` (Tomb of Annihilation, 2017). `see book` in the CR column means the AI DM confirms exact type/CR from the named book (Track-A entries never transcribe stats). All name-and-book attributions were re-verified in the 2026-07-07 pass. Track-A discipline applies to all of them: reference only, no copied stat blocks, no imported setting lore. See `CREATURE_SOURCE_REFERENCE.md`.
- **CR band** is approximate; scale to PC level per `SOLO_ENCOUNTER_SCALING.md`.
- **Full notes:** the file where the creature's tactics/solo notes live.
- **Arc context:** for which tier/region each creature type is most likely, see the Encounter Profile sections in `../15_campaign_arcs/REGIONAL_ARC_PACKS_LEVEL_5_TO_20.md`. Boss creatures (B1–B18) are integrated into `../15_campaign_arcs/VILLAIN_AND_APEX_THREAT_ESCALATION.md` and the Tier-4 endgame playbooks.

---

## A. Beasts (all regions)

| Creature | Track | Type | CR band | Where | Full notes |
|---|---|---|---|---|---|
| Wolf / Dire wolf | A · 2024 MM | Beast | 1/4 – 1 | Tollwood, Hethewald, Wender, Highmark, Sunder Heights | BIOME_ENCOUNTER_MATRIX, regional |
| Giant constrictor / Giant snake | A · 2024 MM | Beast | 1/4 – 2 | Greyfens, Sallowmarch, Sunmark | regional |
| Giant frog / Giant toad | A · 2024 MM | Beast | 1/4 – 1 | Greyfens, Sallowmarch, Sallowmarch delta | regional |
| Boar / Giant boar | A · 2024 MM | Beast | 1/4 – 2 | Vale, Marrowdowns, Hethewald | regional |
| Giant eagle / Giant vulture | A · 2024 MM | Beast | 1 – 1 | Sunder Heights, Highmark, Wender, Karran | regional |
| Bear (black/brown; cave bear: 2014 MM) | A · 2024 MM | Beast | 1/2 – 2 | Tollwood, Hethewald, Highmark, Karran | regional |
| Giant spider / Swarm of spiders | A · 2024 MM | Beast | 1/4 – 1 | ruins, Hethewald deep wood, caves | DUNGEON_ENCOUNTER_SUPPORT |
| Wild horse / Riding horse herds | A · 2024 MM | Beast | 1/4 | Wender Steppe, Sunmark roads | regional |
| Panther / Lion | A · 2024 MM | Beast | 1/4 – 1 | Sunmark, Sallowmarch | regional |
| Crocodile / Giant crocodile | A · 2024 MM | Beast | 1/2 – 5 | Sallowmarch, Hollow Gulf, Sunmark rivers | regional |
| Reef shark / Hunter shark | A · 2024 MM | Beast | 1/2 – 2 | Pale Coast, Hollow Gulf, Drowned Steps | regional |
| Mire-Hound (custom dire predator) | B | Beast | 2 | Greyfens, Mirewend Sinks | regional (Sundering Reach) |

## B. Monstrosities (wilderness, ruins, mountains)

| Creature | Track | Type | CR band | Where | Full notes |
|---|---|---|---|---|---|
| Giant scorpion / Ankheg | A · 2024 MM | Monstrosity | 3 – 2 | Cindern Waste, Bonepan, Saltmere | regional |
| Owlbear | A · 2024 MM | Monstrosity | 3 | Hethewald, Tollwood deep wood | regional |
| Harpy | A · 2024 MM | Monstrosity | 1 | Pale Coast skerries, Highmark, Karran | regional |
| Carrion Stalker — charnel predator | A · VRGtR / RtHW | Monstrosity | see book | Marrowdowns barrows, Saltmere drowned towns | HORROR #H12 note, regional |
| Gremishka — anti-magic pest | A · VRGtR / RtHW | Monstrosity | see book | deep wilderness color (sparing use) | CREATURE_SOURCE_REFERENCE |
| Chimera / Manticore | A · 2024 MM | Monstrosity | 3 – 6 | Highmark, Karran, Greatspine passes | BOSS_AND_APEX_THREATS |
| Roper / Piercer (cave ambusher) | A · 2024 MM | Monstrosity | 5 – 1/2 | Karran mines, deep ruins, Drowned Steps | DUNGEON_ENCOUNTER_SUPPORT |
| Salt-Stalker (custom desiccation hunter) | B | Monstrosity | 5 | Saltmere, Bonepan Flats | SALTMERE_REACHES_ENCOUNTERS |
| Mast-Beast (custom Tollwood deep-wood apex) | B | Monstrosity | 4 | Tollwood (Mast-Beasts' Range) | TOLLWOOD_ENCOUNTERS |

## C. Undead (burial sites, cursed land, fen, battlefield, Remembrance-scarred)

| Creature | Track | Type | CR band | Where | Full notes |
|---|---|---|---|---|---|
| Drowned / Drifting Remembrance | R/B | Undead (incorp.) | 1 – 3 | nodes, fen, basin, all Concord sites | STAGE_12_ADVERSARIES #1, HORROR |
| Ward/Choir-Keeper Remembrance | R/B | Undead (incorp.) | 5 – 8 | node climaxes | STAGE_12_ADVERSARIES #2, HORROR |
| Specter / Ghost / Wraith | A · 2024 MM | Undead | 1 – 5 | hauntings, ruins, barrows | HORROR_AND_CURSE_THREATS |
| Wight | A · 2024 MM | Undead | 3 | Marrowdowns barrows, Greyfens drift, battlefields | HORROR, regional |
| Skeleton / Zombie (reanimate) | A · 2024 MM | Undead | 1/4 – 1/4 | broken graves, Gravecaller work, cursed sites | regional |
| Ghoul / Ghast | A · 2024 MM | Undead | 1 – 2 | crypts, plague-delta, ruined towns | regional |
| Barrow-Wight / Barrow-Shade (custom) | B | Undead | 4 | Marrowdowns, Barrow of Nine Doors | MARROWDOWNS_ENCOUNTERS, HORROR |
| Salt-Mummy / Desiccated Dead (custom) | B | Undead | 3 – 6 | Saltmere drowned towns, Bonepan | SALTMERE_REACHES_ENCOUNTERS, HORROR |
| Ash-Bound Dead (custom) | B | Undead | 4 – 7 | Cindern Waste, Emberfell | CINDERN_WASTE_ENCOUNTERS, HORROR |
| Drowned Mariner Dead (custom) | B | Undead | 2 – 5 | Pale Coast, Hollow Gulf, Drowned Steps | HORROR, regional |
| Wrong-Come-Back (revenant; custom) | B | Undead | 3 – 8 | leaked resurrections, anywhere harvest leaks | HORROR_AND_CURSE_THREATS |
| **Allip** — secret-maddened dead | A · MToF | Undead | 5 | deep nodes, Sealed Archive edge, Heartlands halls | HORROR #H2 |
| **Sorrowsworn** (the Lost / the Wretched / the Lonely / the Hungry / the Angry) — grief made flesh | A · MToF | Monstrosity | 1/4 – 13 | worst drift-lines, drowned towns, Drowned Steps, pits | HORROR #H3 |
| **Soul Monger** — life/memory devourer **(DM-gated)** | A · MToF | Undead | 11 | deepest nodes, Concord Deep outer reach (high tier) | HORROR #H4 |
| **Bodak** — death-gaze drained dead | A · VGtM | Undead | 6 | deepest harvest-scarred sites, Drowned Steps | HORROR #H5 |
| **Deathlock / Deathlock Wight / Mastermind** | A · MToF | Undead | 3 – 8 | Concord caster-dead, Gravecaller deep-work | HORROR #H6 |
| **Vampiric Mist** — luring drain-fog | A · MToF | Undead | 3 | Greyfens, basin shallows, Sallowmarch, coast fog | HORROR #H7 |
| **Gallows Speaker** — the bound dead that speaks (gated clue-vector) | A · RtHW | Undead | see book | gibbet-crossroads, execution grounds, Heartlands halls | HORROR #H10, MYSTERY |
| **Necrichor** — death-fluid horror | A · VRGtR / RtHW | Undead | see book | harvest-leak sites, relic-vault spill, deep nodes | HORROR #H11 |
| **Jiangshi** — rigid preserved dead | A · VRGtR / RtHW | Undead | see book | Saltmere preserved dead, drowned towns | HORROR #H12 |
| **Boneless** — collapsed dead | A · VRGtR / RtHW | Undead | see book | drowned towns, plague-pits | HORROR #H12 |
| **Brain in a Jar** — preserved mind **(DM-gated)** | A · VRGtR / RtHW | Undead | see book | deep Concord vaults only | HORROR #H12 (gated) |
| **Death's Head** — death-omen flying skull | A · VRGtR / RtHW | Undead | 1/2 | deep nodes, barrow-fields | regional deep tables |
| Hollow Court Custodian **(DM-ONLY apex)** | B | Undead (preserved) | 16 – 20 | Under-Shrine only | STAGE_12_ADVERSARIES #8 (gated) |

## D. Fey (old forests, strange groves, ancient sites)

| Creature | Track | Type | CR band | Where | Full notes |
|---|---|---|---|---|---|
| Dryad / Tree-bound spirit | A · 2024 MM | Fey | 1 | Tollwood deep wood, Hethewald, Sunmark groves | regional |
| Pixie / Sprite / Will-cluster | A · 2024 MM | Fey | 1/4 – 0 | Hethewald, Sunmark | regional |
| Green Hag / Sea Hag | A · 2024 MM | Fey | 3 – 2 | Greyfens deep, Sallowmarch, Pale Coast caves | regional, HORROR |
| Blink dog / Displacer (paired fey predators) | A · 2024 MM | Fey/Monstrosity | 1/4 – 3 | Hethewald, Sunmark | regional |
| Fen-Echo / Old-Wood Presence (custom landmark-power) | B | Fey (presence) | varies | Tollwood Old Mast, Greyfens deep | TOLLWOOD_ENCOUNTERS, HORROR |
| Grove-Warden Spirit (custom; benign) | B | Fey | 4 | Sunmark Great Grove | SUNMARK_ENCOUNTERS |

## E. Fiends (cult territory, Gravecaller-linked, Emberfell)

| Creature | Track | Type | CR band | Where | Full notes |
|---|---|---|---|---|---|
| Imp / Quasit (cult familiar) | A · 2024 MM | Fiend | 1 | Gravecaller cells, dark cult sites | FACTION_ENCOUNTERS |
| Lesser summoned fiend (Bearded devil / Barlgura / Shadow demon) | A · 2024 MM | Fiend | 3 – 5 | botched Gravecaller / Emberfell heresy | HORROR, FACTION |
| Greater cult-bound fiend (Chain devil / Bone devil / Barbed devil) | A · 2024 MM | Fiend | 5 – 9 | rare; Emberfell heresy, deep cult | BOSS_AND_APEX_THREATS |
| Ash-Fiend / Cinder-Wretch (custom) | B | Fiend (fire) | 5 – 8 | Emberfell heresy, Cindern Waste | EMBERFELL_ENCOUNTERS, HORROR |

## F. Celestials (Sunmark, rare)

| Creature | Track | Type | CR band | Where | Full notes |
|---|---|---|---|---|---|
| Couatl (grove guardian) | A · 2024 MM | Celestial | 4 | Sunmark Great Grove (rare, benign-warden) | SUNMARK_ENCOUNTERS |
| Pegasus / celestial steed (omen) | A · 2024 MM | Celestial | 2 | Sunmark, high Highmark (very rare) | SUNMARK_ENCOUNTERS |
| Grove-Light / Living-Faith Echo (custom; benign) | B | Celestial (echo) | varies | Sunmark; the hope-mirror to the harvest dead | SUNMARK_ENCOUNTERS, HORROR (contrast) |

## G. Elementals (Emberfell, Cindern Waste, coastal, steppe)

| Creature | Track | Type | CR band | Where | Full notes |
|---|---|---|---|---|---|
| Fire elemental / Magma mephit | A · 2024 MM | Elemental | 5 – 1/2 | Emberfell, Cindern Waste | EMBERFELL_ENCOUNTERS |
| Air elemental / Dust mephit | A · 2024 MM | Elemental | 5 – 1/2 | Wender Steppe, Highmark, Bonepan | WENDER_STEPPE_ENCOUNTERS |
| Water elemental / Wave-spirit | A · 2024 MM | Elemental | 5 | Pale Coast, Hollow Gulf, Drowned Steps | regional |
| Earth elemental / Gargoyle | A · 2024 MM | Elemental | 5 – 2 | Karran, Highmark, ruins | regional |
| Caldera Guardian (custom fire-warder) | B | Elemental (fire) | 11 – 15 | Emberfell Caldera Descent | STAGE_12_ADVERSARIES #7 |
| Salt-Wind / Bonepan Mirage-Spirit (custom) | B | Elemental (air) | 4 | Bonepan Flats, Saltmere | SALTMERE_REACHES_ENCOUNTERS |

## H. Constructs (Concord ruins, Relay Vaults, Ledger vaults, arcane sites)

| Creature | Track | Type | CR band | Where | Full notes |
|---|---|---|---|---|---|
| Concord Construct-Guardian / Relay-Warden | B | Construct | 7 – 17 | Relay Vaults, Concord ruins, Heartlands | STAGE_12_ADVERSARIES #3 |
| Animated armor / Flying sword / Rug of smothering | A · 2024 MM | Construct | 1/4 – 2 | Ledger vaults, old halls, Reliquary | DUNGEON_ENCOUNTER_SUPPORT |
| Stone golem / Iron golem | A · 2024 MM | Construct | 10 – 16 | deep Concord vaults, Heartlands apex | BOSS_AND_APEX_THREATS |
| Carrionette — soul-trapping puppet | A · VRGtR / RtHW | Construct | 1 | Ashmarket relic-trade, Glassmere curiosity-vaults | HORROR #H12 |
| Shield/Watch-construct (lesser sentinel; custom) | B | Construct | 3 – 5 | node anterooms, Sunken Wards, Glassmere | DUNGEON_ENCOUNTER_SUPPORT |
| Relay-Choir Mote (custom swarm-construct) | B | Construct (swarm) | 4 | warming relays, deep nodes | DUNGEON_ENCOUNTER_SUPPORT |

## I. Aberrations (deep ruins, Drowned Steps, strange fen)

| Creature | Track | Type | CR band | Where | Full notes |
|---|---|---|---|---|---|
| Otyugh / Gibbering mouther | A · 2024 MM | Aberration | 5 – 2 | Sunken Wards, flooded deeps, plague-delta | DUNGEON_ENCOUNTER_SUPPORT |
| Chuul / Deep Scion / Morkoth (deep-water aberrations) | A · 2024 MM / VGtM | Aberration | 4 / 3 / 11 | Drowned Steps, Hollow Gulf deeps | DROWNED_STEPS_ENCOUNTERS |
| **Nightgaunt / Gug / Shoggoth / Greater Star Spawn Emissary** — deep cosmic terrors **(DM-gated, tier 3–4 only)** | A · RtHW | Aberration | see book (up to ~21) | Drowned Steps depths, Concord Deep outer reach, deepest Karran cuts | HORROR #H13 |
| Mind-fog Lurker / Memory-Eater (custom) | B | Aberration | 6 – 10 | Drowned Steps, deepest Concord nodes | DROWNED_STEPS, HORROR |
| Fen-Thing (custom strange-fen aberration) | B | Aberration | 4 | Greyfens deep, Sallowmarch fever channels | regional, HORROR |

## J. Dragons (Highmark, rare across continent)

| Creature | Track | Type | CR band | Where | Full notes |
|---|---|---|---|---|---|
| Wyvern (lesser drake) | A · 2024 MM | Dragon | 6 | Highmark, Karran Teeth, Greatspine | HIGHMARK_PASSES_ENCOUNTERS |
| White / chromatic dragon (young → ancient) | A · 2024 MM (also FToD) | Dragon | 8 – 20 | Highmark Passes (rare apex), Emberfell (red) | BOSS_AND_APEX_THREATS |
| Pseudodragon / drake (minor) | A · 2024 MM | Dragon | 1/4 – 2 | scattered; Highmark, Karran | regional |

## K. Giants (Karran Marches, Highmark, Sunder Heights)

| Creature | Track | Type | CR band | Where | Full notes |
|---|---|---|---|---|---|
| Hill giant / Stone giant | A · 2024 MM | Giant | 5 – 7 | Karran, Highmark foothills, Sunder Heights | KARRAN_MARCHES_ENCOUNTERS |
| Frost giant | A · 2024 MM | Giant | 8 | Highmark Passes, far north | HIGHMARK_PASSES_ENCOUNTERS, BOSS |
| Ogre (Half-ogre: 2014 MM) | A · 2024 MM | Giant | 2 – 1 | Karran, Hethewald, frontier wilds | regional |
| Ettin | A · 2024 MM | Giant | 4 | Karran Marches, Greatspine | KARRAN_MARCHES_ENCOUNTERS |

## L. Humanoid Adversaries (all regions — faction agents, bandits, cultists)

| Creature | Track | Type | CR band | Where | Full notes |
|---|---|---|---|---|---|
| Bandit / Thug / Bandit captain | A · 2024 MM | Humanoid | 1/8 – 2 | all roads, Tollmen, wreckers, raiders | FACTION_ENCOUNTERS, regional |
| Guard / Veteran / Knight | A · 2024 MM | Humanoid | 1/8 – 3 | Compact, Tide-Watch, Protectorate, holds | FACTION_ENCOUNTERS |
| Spy / Assassin | A · 2024 MM | Humanoid | 1 – 8 | Ledger, Hush, Salt Syndicate, Reclaimers | FACTION_ENCOUNTERS |
| Cultist / Cult fanatic / Priest | A · 2024 MM | Humanoid | 1/8 – 2 | Gravecallers, Emberfell, heresies | FACTION_ENCOUNTERS, MYSTERY |
| Mage / Acolyte | A · 2024 MM | Humanoid | 1/2 – 6 | Remnant, temples, hedge-casters | FACTION_ENCOUNTERS |
| Scout / Berserker (Tribal Warrior: 2014 MM) | A · 2024 MM | Humanoid | 1/2 – 2 | Wender, Karran, Sunmark, wilds | regional |
| Gravecaller cell-speaker (custom-tuned) | R | Humanoid | 1 – 4 | Greyfens, coast cells, deep wood | FACTION_ENCOUNTERS, MYSTERY |
| Reclaimer Agent (Remnant) | B | Humanoid | 3 – 6 | Concord-contested sites | STAGE_12_ADVERSARIES #4 |
| Salt Syndicate muscle | B | Humanoid | 1/2 – 3 | Caradril, Sunken Wards, ports | STAGE_12_ADVERSARIES #5 |

## M. Oozes (underground, Sunken Wards, flooded dungeons)

| Creature | Track | Type | CR band | Where | Full notes |
|---|---|---|---|---|---|
| Gray ooze / Ochre jelly / Black pudding | A · 2024 MM | Ooze | 1/2 – 4 | Sunken Wards, flooded nodes, deep ruins | DUNGEON_ENCOUNTER_SUPPORT |
| Gelatinous cube | A · 2024 MM | Ooze | 2 | corridor ruins, Relay Vaults | DUNGEON_ENCOUNTER_SUPPORT |
| **Oblex (Spawn & Adult)** — **memory-absorbing ooze**; the harvest's mirror | A · MToF (reprinted MotM) | Ooze | 1/4 – 5 | Remembrance-leak ruins, Concord nodes, memory-scarred fen, relic-vaults | HORROR #H1, MYSTERY_ENCOUNTERS |
| Relic-Sludge (custom Remembrance-tainted ooze) | B | Ooze | 3 | leaking relic vaults, Ashmarket undercroft | DUNGEON_ENCOUNTER_SUPPORT |

## N. Plants (Sunmark, Hethewald, Sallowmarch)

| Creature | Track | Type | CR band | Where | Full notes |
|---|---|---|---|---|---|
| Awakened tree / Shambling mound | A · 2024 MM | Plant | 2 – 5 | Hethewald, Sunmark, Sallowmarch | regional |
| Twig/Needle/Vine blight | A · 2024 MM | Plant | 1/8 – 1/2 | cursed groves, Tollwood, Sunmark | regional |
| Assassin vine ("strangle-reed" reskin) | A · ToA | Plant | 3 | Sallowmarch, Greyfens, Sunmark | regional |
| Bodytaker Plant & Podling — body-snatcher flora | A · RtHW | Plant | see book | Hethewald deep wood, the Old Holds | HORROR #H12 |
| Grave-Bloom (custom Remembrance-fed flora) | B | Plant | 2 | cursed graves, harvest-leak sites | HORROR, regional |

## O. Swarms (fen, cave, plague-touched, coastal)

| Creature | Track | Type | CR band | Where | Full notes |
|---|---|---|---|---|---|
| Swarm of rats / insects / bats | A · 2024 MM | Swarm | 1/4 – 1/2 | ruins, fen, plague-delta, caves | DUNGEON_ENCOUNTER_SUPPORT |
| Swarm of fever-flies (custom plague swarm) | B | Swarm | 1 | Sallowmarch fever channels | SALLOWMARCH_ENCOUNTERS |
| Swarm of quippers (reskin as crabs/eels, coastal) | A · 2024 MM | Swarm | 1 | Pale Coast, Hollow Gulf, Drowned Steps | regional |
| Carrion-Moth Swarm (custom; grave sites) | B | Swarm | 1 | barrows, Marrowdowns, harvest-leak | HORROR |

## P. Spirits / Hauntings (Marrowdowns, Drowned Steps, Concord ruins, Greyfens)

| Creature | Track | Type | CR band | Where | Full notes |
|---|---|---|---|---|---|
| Poltergeist (specter variant) | A · 2014 MM | Undead/spirit | 2 | ruins, barrows, drowned towns | HORROR_AND_CURSE_THREATS |
| Banshee | A · 2024 MM | Undead | 4 | old halls, Concord ruins, Heartlands | HORROR, regional |
| Dullahan — headless herald of death | A · VRGtR / RtHW | Undead | see book | Marrowdowns barrows, Heartlands roads (omen) | HORROR #H12 note |
| **Mist Horror** — predatory memory-mist | A · RtHW | see book | see book | Greyfens deep fog, Drowned Steps approaches | HORROR #H13 |
| Memory-Echo Haunt (custom; non-corporeal Remembrance scar) | B | Spirit (echo) | 1 – 6 | any harvest-touched site | HORROR_AND_CURSE_THREATS |
| Drift-Line Chorus (custom; mass-haunt phenomenon) | B | Spirit (mass) | environmental | Greyfens, basin, drowned towns | HORROR, MYSTERY |

## Q. Curses / Memory-Echo Threats (original Remembrance-linked)

| Threat | Track | Type | CR/band | Where | Full notes |
|---|---|---|---|---|---|
| Thin-touch (exposure condition) | B | hazard/condition | — | raw relics, Heights, nodes | HORROR, MAGIC_RULES |
| Remembrance-Drain Curse | B | curse | varies | botched rites, relic mishandling | HORROR_AND_CURSE_THREATS |
| The Forgetting (memory-loss affliction) | B | curse | varies | deep nodes, Drowned Steps, Custodian work | HORROR (DM-gated severity) |
| Hungering Grief (mass-mourning compulsion) | B | curse | environmental | drift-lines, failed funerals | HORROR, MYSTERY |

---

## Track-B Official-Chassis Anchors (2026-07-07)

Every campaign-original (Track B) and reskin (R) creature is mechanically **anchored to a real published D&D stat block** — the AI DM runs the anchor with the stated modifications. No creature in this campaign exists on invented mechanics alone. (Anchors restate what the full Track-B entries already describe; where a full entry gives abbreviated numbers, those override the anchor's.)

| Track-B / R creature | Official chassis anchor | Modification summary |
|---|---|---|
| Mire-Hound | **Dire wolf** (2024 MM, CR 1) | tougher (CR 2), fen-camouflage, drag-into-mire tactics |
| Salt-Stalker | **Bulette** (2024 MM, CR 5) | desiccating bite instead of leap; salt-flat ambusher |
| Mast-Beast | **Owlbear** (2024 MM, CR 3) | scaled to CR 4–6; deep-wood apex, antlered, territorial |
| Drowned / Drifting Remembrance | **Specter** (2024 MM, CR 1) | mournful not malicious; node-bound; laid by rite |
| Ward/Choir-Keeper Remembrance | **Wraith** (2024 MM, CR 5) | scaled to CR 5–8; node-climax guardian; rite-resolvable |
| Barrow-Wight / Barrow-Shade | **Wight** (2024 MM, CR 3) or **Wraith** (CR 5) | barrow-bound; stands down if the grave is respected |
| Salt-Mummy / Desiccated Dead | **Mummy** (2024 MM, CR 3) | desiccating-thirst curse replaces dreadful glare |
| Ash-Bound Dead | **Wight** (2024 MM) + Magma-Mephit-style heat aura; **Mummy** at high end | fire immunity, cold vulnerability |
| Drowned Mariner Dead | **Drowned Ascetic / Blade / Assassin / Master** (GoS) | mournful retune; tide-line-bound; settled by the salt-and-tide rite |
| Wrong-Come-Back | **Revenant** (2024 MM, CR 5) | scaled CR 3–8; purpose-driven, rite-resolvable |
| Memory-Echo Haunt | **Specter** (2024 MM, CR 1) | cannot leave its scar; resolved by laying the memory |
| Drift-Line Chorus | hazard — no chassis; focal manifestation: **Banshee / Ghost** (2024 MM) | environmental saves; mass-rite resolution |
| Fen-Echo / Old-Wood Presence | manifests via **Green Hag / Treant / Banshee** (2024 MM) by aspect | landmark-power; mostly environmental |
| Grove-Warden Spirit | **Dryad** (2024 MM, CR 1) elevated toward **Treant** (CR 9) | benign warden |
| Grove-Light / Living-Faith Echo | **Will-o'-wisp** (2024 MM, CR 2), benign retune | hope-mirror; non-hostile |
| Ash-Fiend / Cinder-Wretch | **Barbed devil** (2024 MM, CR 5) / **Salamander** (CR 5) | ash-and-cinder theme, CR 5–8 |
| Caldera Guardian | **Salamander** scaled toward **Efreeti** (2024 MM, CR 11) | site-bound fire-warder, CR 11–15 |
| Salt-Wind / Bonepan Mirage-Spirit | **Air elemental** (2024 MM, CR 5) weakened to CR 4 | mirage-lure behavior |
| Concord Construct-Guardian / Relay-Warden | **Shield guardian** (2024 MM, CR 7) scaled toward **Iron golem** (CR 16) | Concord protocols; parley/pass-phrase noncombat out |
| Shield/Watch-construct (lesser sentinel) | **Helmed horror** (2014 MM, CR 4) / **Animated armor** (CR 1) | node anteroom sentinel, CR 3–5 |
| Relay-Choir Mote (swarm-construct) | **Swarm of insects** (2024 MM) retyped construct | relay-defense swarm, CR 4 |
| Reclaimer Agent | **Mage / Veteran** (2024 MM) | Remnant field gear and doctrine |
| Salt Syndicate muscle | **Thug / Bandit captain** (2024 MM) | city-crime tactics |
| Gravecaller cell-speaker | **Cult fanatic** (2024 MM, CR 2) | rite-magic flavor; CR 1–4 band |
| Mind-fog Lurker / Memory-Eater | **Adult oblex** (MToF, CR 5) scaled to CR 6–10 | fog-form; memory-theft; pairs with **Mist Horror** (RtHW) |
| Fen-Thing | **Otyugh** (2024 MM, CR 5) reduced to CR 4 | strange-fen aberration |
| Relic-Sludge | **Gray ooze** (2024 MM, CR 1/2) scaled to CR 3 | Remembrance-tainted; memory-flash on touch |
| Grave-Bloom | **Vine blight** (2024 MM, CR 1/2) scaled to CR 2; mature form toward **Corpse flower** (MToF, CR 8) | grief-fed flora |
| Swarm of fever-flies | **Swarm of insects** (2024 MM, CR 1/2) | disease rider (marsh-fever DCs) |
| Carrion-Moth Swarm | **Swarm of insects** (2024 MM, CR 1/2) | grave-site swarm; unnerving, low harm |
| Hollow Court Custodian **(DM-only apex)** | **Mummy lord** (2024 MM, CR 15) / **Lich** (CR 21) frame, rebuilt per `STAGE_12_ADVERSARIES.md` #8 | preserved-not-rotted; an argument, not a monster |

## Creature-Type Coverage Confirmation

Every required creature category is represented with a biome-appropriate home:
Beasts ✓ · Monstrosities ✓ · Undead ✓ · Fey ✓ · Fiends ✓ · Celestials ✓ (Sunmark) · Elementals ✓ · Constructs ✓ · Aberrations ✓ · Dragons ✓ (Highmark/Emberfell) · Giants ✓ (Karran/Highmark/Heights) · Humanoid adversaries ✓ · Oozes ✓ · Plants ✓ · Swarms ✓ · Spirits/Hauntings ✓ · Curses/Memory-echo ✓.

## Related Files

- [`CREATURE_SOURCE_REFERENCE.md`](CREATURE_SOURCE_REFERENCE.md) — source-handling rules
- [`BIOME_ENCOUNTER_MATRIX.md`](BIOME_ENCOUNTER_MATRIX.md) — biome → creature cross-reference
- [`HORROR_AND_CURSE_THREATS.md`](HORROR_AND_CURSE_THREATS.md) — Remembrance/undead/curse originals
- [`BOSS_AND_APEX_THREATS.md`](BOSS_AND_APEX_THREATS.md) — elite/boss/apex
- [`STAGE_12_ADVERSARIES.md`](STAGE_12_ADVERSARIES.md) — dungeon adversary originals
- [`ENCOUNTER_INDEX.md`](ENCOUNTER_INDEX.md) — master encounter-file index
