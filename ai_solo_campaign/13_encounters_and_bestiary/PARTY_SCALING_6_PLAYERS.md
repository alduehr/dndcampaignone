# PARTY_SCALING_6_PLAYERS.md — Converting the Solo-Tuned Campaign for a Six-Player Party

---
type: encounter
secrecy: player-safe
status: static
region: Orrun
level_range: 1-20
related: [SOLO_ENCOUNTER_SCALING.md, ENCOUNTER_INDEX.md, BOSS_AND_APEX_THREATS.md, BESTIARY_INDEX.md, ../01_runner_protocol/PARTY_MODE_PROTOCOL.md, ../14_treasure_and_artifacts/PARTY_REWARDS_6_PLAYERS.md]
tags: [type:encounter, secrecy:player-safe, party-mode, scaling, combat-budget, six-players]
---

## AI Use / DM Use

Load this **instead of applying `SOLO_ENCOUNTER_SCALING.md`'s budgets** when the campaign is being run in **party mode** (see `../01_runner_protocol/PARTY_MODE_PROTOCOL.md`). Every encounter table, dungeon, quest, and adversary profile in this campaign is authored **solo-first** — this file is the master conversion ruleset that scales that authored content up to a **six-player party** without editing any authored file. The authored content stays the single source of truth for *who/where/why/tactics/morale/outs*; this file converts only the *math*.

**Design intent:** preserve the authored encounter's fictional stakes. A fight written as "solo danger: moderate" should feel *moderate to six players* after conversion — same dread, same outs, bigger numbers.

## The Core Problem (Inverted)

`SOLO_ENCOUNTER_SCALING.md` protects one PC from action economy. Six PCs have the opposite profile:

- **Six actions per round** (plus bonus actions, reactions, and usually a familiar or pet) versus a solo encounter's one or two foes — an unconverted solo encounter dies before it acts twice.
- **Six health pools, healers, and revival magic** — attrition that threatens one PC is noise to six.
- **Area-of-effect spells** — the "small group with morale" that scares a solo PC evaporates to one fireball.
- **Six skill sets** — locked doors, hazards, and social gates that gate a solo PC rarely gate a party.
- And note: six is **more** than the published four-PC baseline — even "deadly for 4" math plays about one difficulty step lower for 6.

So in party mode, **never run a combat row as printed.** Convert first.

## Rule 1 — How To Read The Solo Tables At Six Players

1. **Non-combat rows are unchanged.** [Clue], [Folk], [Hazard], and social rows work at any party size (see Rule 4). Most rows are not fights — that stays true.
2. **Combat rows list the solo count.** Convert with the multiplier ladder (Rule 3). Never treat the printed count as party-ready.
3. **Keep the row's role, morale, telegraphs, and outs exactly as written.** Conversion changes bodies and tiers, never behavior.
4. **Some "overwhelming" solo encounters are already party-sized.** Where the fiction fields a real gang (e.g. the Tollmen's 6–10 bandits, a Gravecaller cell, a wreckers' crew), the *count* may already fit — but it was balanced to *overwhelm* (i.e., to force the social/stealth solution). To preserve that intent for six players, upgrade the leaders and add reinforcements so the fight remains the *worst* option, or accept that the party can now win it and let the consequences (law, faction heat, the vacuum it creates) carry the weight instead.

## Rule 2 — The Six-Player Encounter Budget

When building or converting an encounter:

- **Baseline:** use the published per-character XP thresholds × 6. Because six PCs exceed the four-PC baseline, treat a computed "Hard" as playing one step easier — to *feel* Hard, budget into the published Deadly band; to feel Deadly, budget ~1.5× Deadly.
- **Bodies are now good design** (the inverse of solo): multiple foes keep six players engaged and give AoE something to do. Prefer **N foes ≈ party size ± 2** for a standard fight.
- **Single foes are now the weak shape.** A lone monster of any CR gets action-starved by six PCs. Never run a lone foe as a real fight unless it has legendary-style pressure (Rule 5).
- **Practical shapes for a real six-player fight:**
  - L1–4: 1 leader + 4–8 mooks, or 6–10 mooks in waves.
  - L5–10: 1 elite + 4–6 standards, or 2 elites + mooks, or ~8–12 mooks with terrain.
  - L11–16: 1 boss-tier (with legendary pressure) + 3–5 supports, or 2–3 elites + mooks.
  - L17–20: 1 apex **with** legendary actions/lair effects **and** meaningful adds — never naked.

## Rule 3 — The Conversion Ladder (apply per authored encounter)

Convert the authored solo encounter by role:

| Authored solo shape | Six-player conversion |
|---|---|
| 1 weak foe / "a warning, not a threat" | Keep as color, or ×4–6 of it as a real skirmish |
| 2–3 mooks (a "real solo fight") | ×3 count, **or** ×2 count + upgrade one to a leader chassis |
| 1 standard foe ≈ PC level (the solo "Hard") | Keep it + add 4–6 mooks, **or** upgrade one chassis step and add 2–3 supports |
| 1 elite / "a scare" (solo Deadly) | Upgrade one chassis step **and** add escorts, e.g. Specter→Wraith + 2–3 specters; Wight→Wight + skeleton pack; Bandit captain→Veteran + gang |
| Leader + handful | Double the handful, upgrade the leader one step |
| Boss / apex | Rule 5 |
| Swarm/environmental ("mass" rows like the Drift-Line) | Unchanged in nature; widen the area/saves to touch everyone (Rule 4) |

**Chassis-step ladder** (use the anchors in `BESTIARY_INDEX.md` §Track-B Official-Chassis Anchors): Bandit→Thug→Bandit Captain→Veteran→Gladiator-tier; Cultist→Cult Fanatic→Priest-tier; Specter→Wraith; Skeleton/Zombie→Wight→Wraith; Guard→Veteran→Knight. One step ≈ one tier of threat; never jump two steps and multiply count at the same time.

**Stagger and waves:** the solo rule staggers arrivals to *soften*; the party version staggers to *sustain* — a second wave on round 2–3 keeps a six-player fight from ending at initiative.

## Rule 4 — What Does NOT Change

- **DCs.** Bounded accuracy holds; a DC 15 is a DC 15. Six players succeed more often because six people roll — that's correct, not a problem. Use group checks where the whole party acts (climb, sneak, march), individual checks where one person acts.
- **Morale, goals, telegraphs, retreat routes, and non-combat outs.** These are good design at any size. Foes still break at half strength; bound guardians still can't pursue; every dangerous site still warns first.
- **Hazard/trap DCs and effects** — but hazards now threaten whoever triggers them, not the whole campaign; you may widen area-effects so a hazard touches 2–3 PCs instead of one.
- **Clue delivery, mystery gating, reveal caps, secrecy.** Untouched. The three-clue rule was party-proof from the start.
- **The authored who/why/where.** Conversion never adds new named foes, factions, or sites — only bodies and tiers from the same stat references.

## Rule 5 — Converting Solo Bosses To Party Bosses (inverse of the solo Rule 7)

The campaign's bosses were *reduced* for solo play. For six players, restore and extend:

- **Restore HP:** the solo profiles cut ~25–40% — add that back, then add ~25% more (six players out-damage four).
- **Give 2–3 legendary-style actions per round** (move, one attack/signature, one control effect at end of others' turns) and a lair-style beat on initiative 20 where the site supports it (the node's cold pulse, the caldera's vent, the vault's wards). Build these from the boss's existing signature abilities — do not invent new powers foreign to the profile.
- **Adds every phase, not once:** the solo rule's "summon once when pressed" becomes waves — and the adds-stopping lever (the totem, the relay, the rite) stays, now as the party's tactical objective.
- **Keep every weakness and non-combat resolution.** A six-player table splitting between "hold the line" and "complete the rite" is the intended climax shape.
- **Phase transitions escalate** (the solo version's breathers become turns of the screw).

**Apex note (DM):** the endgame Custodians (`STAGE_12_ADVERSARIES.md` #8) were tuned as a solo moral climax. For six players run the Court as a true court — all present Custodians active, guardian-constructs as adds, the Under-Shrine's own effects as the lair — and keep the argument: it must remain winnable by *decision* as well as by force.

## Rule 6 — Six-Player Pacing Dials

- **Parties clear more per day.** Expect 2–3 real fights plus exploration per adventuring day where the solo PC managed 1. Rest constraints in dungeon files hold as written; time pressure and wandering checks now do the balancing work the fights alone did for one PC.
- **When a converted fight looks too easy mid-combat**, don't inflate HP on the fly — trigger the authored reinforcements/morale logic (more of the same foes exist in the fiction almost everywhere).
- **When too hard,** the solo dials still work: morale break, staggered retreat, the environment, the out.
- **Cheap-death protection relaxes to standard fairness.** Six players with a healer accept normal 5e lethality; keep telegraphs, drop the solo insurance reflexes (`SOLO_ENCOUNTER_SCALING.md` Rule 5 is solo-only).

## Quick Six-Player Cheat Sheet

| Party level | "A real fight" (feels Hard) | "A set-piece" (feels Deadly) |
|---|---|---|
| 1–2 | leader (CR 1) + 4–6 mooks | 2× CR 1 + mook wave |
| 3–4 | CR 3–4 elite + 4–5 mooks | CR 5 + supports, or 10+ mooks w/ terrain |
| 5–8 | CR 6–8 + 4–6 standards | CR 9–10 w/ legendary beats + adds |
| 9–12 | CR 10–12 + supports | CR 13–14 boss (Rule 5) + waves |
| 13–16 | CR 14–16 boss + 3–5 elites | CR 17–18 apex + lair + adds |
| 17–20 | CR 18–20 + elite escort | full apex court: legendary + lair + waves |

The constant rule, unchanged from solo: **information, terrain, morale, escape, and a non-combat out** make an encounter fair — the math only sets the volume.

## Related Files

- [`SOLO_ENCOUNTER_SCALING.md`](SOLO_ENCOUNTER_SCALING.md) — the solo math this file converts *from*
- [`../01_runner_protocol/PARTY_MODE_PROTOCOL.md`](../01_runner_protocol/PARTY_MODE_PROTOCOL.md) — everything non-combat about party mode
- [`../14_treasure_and_artifacts/PARTY_REWARDS_6_PLAYERS.md`](../14_treasure_and_artifacts/PARTY_REWARDS_6_PLAYERS.md) — reward conversion
- [`BOSS_AND_APEX_THREATS.md`](BOSS_AND_APEX_THREATS.md) · [`BESTIARY_INDEX.md`](BESTIARY_INDEX.md) (chassis anchors) · [`ENCOUNTER_INDEX.md`](ENCOUNTER_INDEX.md)
