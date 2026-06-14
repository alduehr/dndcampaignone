# FACTION_ENCOUNTERS.md — Faction-Linked Encounter Tables

---
type: encounter
secrecy: mixed
status: static
region: Orrun
factions: [all]
level_range: 1-20
related: [BESTIARY_INDEX.md, ENCOUNTER_INDEX.md, ../07_factions/, ../02_runtime_state/FACTION_STATE.md, ../02_runtime_state/WORLD_CLOCKS.md]
tags: [type:encounter, secrecy:mixed, function:faction, adversary-groups, solo-tuned]
---

## AI Use

Encounter tables for **faction-linked encounters** — patrols, agents, enforcers, reprisals, and offers — for all 7 major factions, the Caradril city factions, and the regional minor factions. Use these when a faction is *active* (a clock is running, the player crossed them, or a quest brings them on-scene). Faction encounters are **mostly social/intrigue** and escalate to violence only when telegraphed. Stat references are Track-A baselines or the Stage 12 originals; tune for solo per `SOLO_ENCOUNTER_SCALING.md`. Always offer a non-combat path and record outcomes in `FACTION_STATE.md`.

**Secrecy:** the Hollow Court is **DM-only/apex** — it does **not** field random patrols; it acts only through cutouts until the endgame. Never deploy the Court as a faction-encounter.

## Faction Adversary Stat Key (reusable)

| Type | Stat reference | Notes |
|---|---|---|
| Patrol / footman | Guard-like (AC 16, ~11 HP) | Compact, Tide-Watch, Protectorate, holds |
| Veteran / sergeant | Veteran-like (AC 17, ~58 HP) | leaders of a patrol |
| Captain / champion | Knight/Veteran-like (AC 18, ~90 HP, Leadership) | named; never a default fight |
| Enforcer / strong-arm | Thug-like (AC 11, ~30 HP) | Ledger, holds, ports |
| Agent / spy | Spy-like (AC 13, ~22 HP) | Hush, Reclaimers, Syndicate, Ledger |
| Assassin / lieutenant | Assassin-like (AC 15, ~55 HP) | Syndicate, rare |
| Cultist | Cultist-like (AC 11, ~9 HP) | Gravecallers, heresies |
| Cult fanatic / speaker | Cult Fanatic-like (AC 13, ~33 HP) | cell leaders |
| Acolyte / rite-keeper | Acolyte/Priest-like (AC 11–13, ~20–27 HP) | Mourners, Wardens, temples |
| Scholar-caster | Mage-like (AC 12, ~40 HP) + Remembrance one-off | Remnant/Reclaimers |
| Warden champion | Priest/Paladin-like (AC 16+, ~58+ HP) | Ashen Wardens, rare |

---

## 1. Ashen Wardens (rite-keeper order; unknowing seal-guardians)

- **Public face:** death-rite priests who "walk the dead home." **Tone:** earnest, weary, secretive without knowing why.
- **Where:** Reach, waystations (Ashwalk Rest), node-sites, coast/wood anchorites.

| d8 | Encounter | Type | Solo Danger |
|---|---|---|---|
| 1 | A Warden walking a dead soul home (rite-aid) | social/ally | none |
| 2 | A Warden quartermaster offering rite-supplies/lore | social | none |
| 3 | A Warden refusing access to a sealed node ("it's not for the living") | social/obstacle | none |
| 4 | A Warden-Confessor of conscience (Voss) hinting at doubt | clue | none |
| 5 | A Warden party performing a seal-rite the player can witness/aid | clue/social | none |
| 6 | A wandering anchorite who knows a gated truth (M5/M6) | clue | none |
| 7 | Wardens blocking a Gravecaller breaking-in-progress (ally vs cult) | combat-adjacent | low |
| 8 | A senior Warden testing the player before sharing (Othetha-tier) | social | none |

- **Combat:** only if the player desecrates a seal or sides with breakers; champions are Priest/Paladin-like — **never cheap**. **Non-combat:** earnest talk, faction standing, helping a rite. **If ignored:** they keep sealing; the player loses a lore-ally.

## 2. Cinder Ledger (merchant-bank monopoly)

- **Public face:** legitimate trade and banking. **True agenda:** monopolize relics ("quiet-coin") and the harvest's value. **Tone:** polite, ruthless, lawyered.
- **Where:** everywhere there's trade — Reach, Caradril (Ledger Keep), ports, far Glassmere heartland.

| d8 | Encounter | Type | Solo Danger |
|---|---|---|---|
| 1 | A Ledger factor offering a contract/loan with a hook | social/intrigue | none |
| 2 | A salt/relic caravan with hired guards | social | low |
| 3 | A collector-captain (Mauld Tallow) calling in a debt | social/threat | low |
| 4 | Ledger buyers outbidding the Remnant for a relic (bidding war) | intrigue/clue | low |
| 5 | Ledger enforcers "escorting" the player off a dig | threat | low-mod |
| 6 | A turnable clerk (Coll Riis-type) with damning ledgers (M3/M6) | clue/ally | none |
| 7 | A drainage/eviction crew + guards at a contested site | social/threat | low |
| 8 | A Ledger reprisal: hired thugs + a spy, telegraphed | threat→combat | mod |

- **Combat:** enforcers are Thug/Spy-like; they **intimidate over kill** (a dead client pays no debts). **Non-combat:** pay, lawyer, expose, turn a clerk. **If ignored:** the monopoly clock advances; prices/relics tighten; rivals are crushed.

## 3. Mourners' Circle (folk grief-faith)

- **Public face:** grief-keepers and grave-singers. **Tone:** kind, old, keepers of half-remembered truths (M5/M6 seeds).
- **Where:** every settlement's grave-ground; eldest Mourners are lore-anchors.

| d6 | Encounter | Type | Solo Danger |
|---|---|---|---|
| 1 | A grave-singer performing a rite the player can aid | social/ally | none |
| 2 | An eldest Mourner holding a folk-memory clue (old songs) | clue | none |
| 3 | A grieving family fearing a dead won't rest (hook) | social/hook | none |
| 4 | A Mourner-apprentice bridging to the player (Iola-type) | social/ally | none |
| 5 | A Mourner quietly opposing a breaking/harvest (conscience) | clue/ally | none |
| 6 | A Mourner-keeper at a node who senses "something wrong" (M6) | clue | none |

- **Combat:** essentially never (noncombatant faith); if cornered, Acolyte/Commoner-like. **Non-combat:** respect, aid a rite, listen. **If ignored:** a lost ally and a closed clue-path; the dead still rise.

## 4. Reachward Compact (frontier government council; infiltrated)

- **Public face:** law and order on the frontier. **True nature:** infiltrated by a Court agent (Reke). **Tone:** bureaucratic, stretched thin, some honest, some compromised.
- **Where:** Reach roads/towns; circuit reeves; watch.

| d8 | Encounter | Type | Solo Danger |
|---|---|---|---|
| 1 | Wardmen checking travelers on the road | social | none |
| 2 | A circuit magister-reeve (honest; Sela Coalmont) with a job | social/hook | none |
| 3 | A watch sergeant needing help (under-resourced) | social/hook | none |
| 4 | A compromised councilor (Reke) steering the player wrong (M4) | intrigue/clue | low |
| 5 | A bailiff enforcing a Ledger-friendly ruling (corruption) | social/obstacle | low |
| 6 | A records-clerk (Pevin Oss) with a paper-trail clue | clue | none |
| 7 | The watch detaining the player over a misunderstanding | social/threat | low |
| 8 | A militia muster against a real threat (the player can join) | combat-adjacent | varies |

- **Combat:** the watch is Guard/Veteran-like; **arrest over kill** in settled areas. **Non-combat:** law, persuasion, exposing corruption. **If ignored:** corruption deepens; the Court's agent gains ground (DM clock).

## 5. Gravecallers (outlawed cult that speaks with the dead)

- **Public face (rumor):** dangerous grave-robbers/necromancers. **True nature:** desperate people who want the dead *back*, some sincere, some radical (Ashby). **Tone:** grief weaponized; the Knock; false comfort.
- **Where:** Greyfens cells, coast cells, deep wood; recruiting the bereaved.

| d8 | Encounter | Type | Solo Danger |
|---|---|---|---|
| 1 | A cell scout marking a door (the Knock) | clue/social | low |
| 2 | Sister Knell gently recruiting a grieving family | social/clue | none |
| 3 | A cell-mother (Mother Osset) leading a forbidden rite | clue/obstacle | low-mod |
| 4 | Cole Ashby's radicals moving to break a shrine | threat→combat | mod |
| 5 | A botched rite producing a Wrong-Come-Back (revenant) | horror/combat | mod-high |
| 6 | A cell offering the player "answers" (a recruiting trap) | intrigue | low |
| 7 | A cultist + imp/quasit familiar guarding a relic | combat | mod |
| 8 | A cell fleeing a Warden crackdown (the player chooses sides) | social/intrigue | low |

- **Combat:** Cultist/Cult Fanatic-like + rare bound fiend; **break on morale** when the rite fails. **Non-combat:** sympathy, exposing the radicals, the rite's truth. **If ignored:** the Breaking clock advances; more shrines shatter; more dead rise.

## 6. Concord Remnant / Reclaimers (scholar society; would-be heirs)

- **Public face:** antiquarian scholars (Lampwrights' Collegium). **True nature:** the Reclaimers want the Concord's power *for themselves*. **Tone:** brilliant, patronizing, dangerous when the truth is at stake.
- **Where:** Caradril (Lantern Reach, Sealed Archive), digs, far Reliquary/Heartlands.

| d8 | Encounter | Type | Solo Danger |
|---|---|---|---|
| 1 | A scholar offering to translate Concord Script (with strings) | social/clue | none |
| 2 | A Reclaimer salvage-crew guarding a dig (Veska Dunn) | social/rival | mod |
| 3 | An idealist Lector (Briss) leaking a conscience-clue | clue/ally | none |
| 4 | A Reclaimer agent warning the player off (turn-back protocol) | threat | mod |
| 5 | A bidding war vs the Ledger over a relic | intrigue | low |
| 6 | An Archive gatekeeper (Wessel Dree) blocking M6/M9 | obstacle | low |
| 7 | A Sentinel-Scholar + agent defending a secret works | combat | mod |
| 8 | An offer of alliance (the truth, on Remnant terms) | intrigue/choice | none |

- **Combat:** Spy + Mage-like w/ Remembrance one-offs (`STAGE_12_ADVERSARIES.md` #4); **warn → control → eject**, lethal only if cornered. **Non-combat:** ally, out-scholar, expose, help them. **If ignored:** they reach the truth first and act on it.

## 7. Hollow Court (apex hidden power) — **DM-ONLY**

- **Does NOT field encounters.** Acts only through **cutouts** (Reke, Sefra Quick as unwitting fixer, hired hands) until the endgame gate (REV_007). Any "Court encounter" before then is *a cutout*, never the Court. The Custodians appear only in the Under-Shrine (`BOSS_AND_APEX_THREATS.md` B18). **Never narrate the Court as a faction the player can bump into.**

---

## City Factions (Caradril) — quick tables

*(Full social tables in `CARADRIL_ENCOUNTERS.md`; this is the adversary-encounter summary.)*

| Faction | Typical encounter | Stat ref | Non-combat out |
|---|---|---|---|
| **Tidewater Council / Charter Houses** | political maneuver, hearing, charter leverage | Noble-like (noncombatant) | persuasion, alliance, exposure |
| **The Tide-Watch** | patrol, detain, escort, reprisal | Guard/Veteran/Captain Kade | law, bribe, talk |
| **The Salt Syndicate** | smuggling beat, catch-and-eject, blackmail | Bandit/Thug/Sorrel (Spy/Assassin) | bribe, rival-turn, the Hush |
| **The Hush** | surveillance, blackmail, an info-offer | Spy-like / the Bellman | trade info, leverage |
| **The Quay Charter (Ledger arm)** | trade-guild pressure, debt | Thug/Spy-like | pay, lawyer, expose |
| **Lampwrights' Collegium (Remnant front)** | scholarly gate, translation-with-strings | Mage/Acolyte-like | alliance, out-scholar |

## Regional Minor Factions — quick tables

| Faction | Region | Typical encounter | Stat ref | Non-combat out |
|---|---|---|---|---|
| **The Tollmen** | Tollwood | toll-demand at Tollstone Cross; turnable (Renn) vs murderous (Skell) | Bandit/Thug-like | pay toll, turn Renn, route around |
| **Wreckers** | Pale Coast | false-light wrecking, sea-cave ambush | Bandit/Thug-like + sea | expose, avoid the reef, Tide-Reader's aid |
| **Salt-clans** | Saltmere | feud, hold-toll, blood-debt | Tribal warrior/Veteran-like | single-combat, blood-price, mediation |
| **Petty warlords** | Karran | warband raid, hold-toll, champion challenge | Bandit/Veteran/Brask | tribute, faction-play, single combat |
| **Steppe clans** | Wender | raid, horse-toll, hospitality-test | Scout/Tribal warrior-like | guest-right, gift, single combat |
| **Hollow Gulf privateers/pirates** | Hollow Gulf | sea-toll, boarding, letter-of-marque | Bandit/Veteran + ship | parley, bribe, port-law |
| **Protectorate garrison** | Sallowmarch | checkpoint, conscription, crackdown | Guard/Veteran-like | papers, bribe, smuggler-route |
| **Emberfell theocracy** | Emberfell | pilgrim-toll, heresy-trial, fire-rite | Cultist/Priest/Pyre-Warden | piety, the heretic-sage, avoid the deep waste |

## Faction-Encounter Solo Rules

- Patrols and agents **prefer their job to a fight** (escort, detain, warn, extort, recruit) — combat is a last resort and always telegraphed.
- A lone PC vs a faction warband must have **allies, terrain, stealth, or an escape** — never a straight party-mob (`SOLO_ENCOUNTER_SCALING.md`).
- Named faction leaders are **recurring** — they don't die cheaply and have escape/return logic (`BOSS_AND_APEX_THREATS.md`).
- **Record every faction encounter outcome** in `FACTION_STATE.md` and advance/slow the relevant clock in `WORLD_CLOCKS.md`.

## Related Files

- [`BESTIARY_INDEX.md`](BESTIARY_INDEX.md) · [`STAGE_12_ADVERSARIES.md`](STAGE_12_ADVERSARIES.md)
- [`CARADRIL_ENCOUNTERS.md`](CARADRIL_ENCOUNTERS.md) · [`BOSS_AND_APEX_THREATS.md`](BOSS_AND_APEX_THREATS.md)
- [`../07_factions/`](../07_factions/) · [`../02_runtime_state/FACTION_STATE.md`](../02_runtime_state/FACTION_STATE.md) · [`../02_runtime_state/WORLD_CLOCKS.md`](../02_runtime_state/WORLD_CLOCKS.md)
