# SOLO_ENCOUNTER_SCALING.md — Adjusting Encounters for One PC

---
type: encounter
secrecy: player-safe
status: static
region: Orrun
level_range: 1-20
related: [ENCOUNTER_INDEX.md, BOSS_AND_APEX_THREATS.md, ../01_runner_protocol/COMBAT_PROTOCOL.md, ../01_runner_protocol/SOLO_PLAY_PRINCIPLES.md, ../00_control/DND_MECHANICS_REQUIREMENTS.md]
tags: [type:encounter, secrecy:player-safe, function:solo-safety, scaling, combat-budget]
---

## AI Use

Load this **whenever you roll or build an encounter**. Every encounter table in this folder is already solo-tuned, but this file is the master ruleset for *how* to read those tables for one player character, how to convert a standard CR/XP budget to a solo budget, and when to soften, harden, or skip an encounter. This is the safety spine of Stage 13.

## The Core Problem

The published encounter math assumes a **four-PC party**. A lone PC:
- Has one action per round instead of four (action economy is the killer).
- Has one health pool, one set of saves, no one to revive them.
- Cannot split focus-fire, cover retreats, or tank-and-spank.
- Dies to "swarm" encounters that a party shrugs off.

So the campaign **never** runs party-balanced encounters straight. Use the rules below.

## Rule 1 — How To Read These Encounter Tables As A Solo Player

The regional and travel tables are **already written for one PC**. When you roll a result:
1. Default to the **non-combat reading** first ([Dead], [Folk], [Hazard], [Clue], social). Most rows are not fights.
2. If it is a combat row, the stat reference given is **already the solo-appropriate count** (usually 1 foe, or a small group with morale and escape).
3. Never multiply the listed enemies for "challenge." If you want more danger, raise the *single* foe's tier, not the *number*.
4. If the PC is travelling with an ally/companion/hireling, you may add one extra standard foe — never more.

## Rule 2 — The Solo Encounter Budget (CR / XP method)

When building a fresh encounter not on a table, use this:

- **Take the PC's level. Find the "Hard" single-PC XP threshold** (one quarter of the party-of-four "Hard" number; the published per-character thresholds give this directly).
- **A single foe is the safest shape.** A lone enemy of CR ≈ PC level is a *Hard* fight for a careful PC and a *deadly* one for a reckless or wounded PC. That is the campaign's standard "real fight."
- **Solo multiplier for groups:** a lone PC feels the action-economy penalty hard. When facing **2+ foes**, treat the encounter as if it were worth **~×2 to ×3 its raw XP**. Two CR-1 foes against a lone L2 PC play like a deadly encounter, not a medium one. Budget accordingly — i.e. use *fewer* bodies than the raw math suggests.
- **Practical caps for a lone PC with no allies:**
  - L1–4: 1 real threat + maybe 1–2 mooks who break morale fast.
  - L5–10: 1 elite, or 1 leader + 2–3 mooks, or 3–4 mooks.
  - L11–16: 1 boss-tier, or a leader + a handful of supports.
  - L17–20: 1 apex (with lair/legendary effects standing in for "a party's worth" of pressure) — this is how the campaign delivers boss feel to a solo PC: one big legendary creature, not a mob.

## Rule 3 — Adjustment Factors (the solo dials)

When an encounter looks too hard, pull these dials **before** the fight, not mid-combat:
- **Remove 1–2 standard enemies** from any group. This is the single most reliable fix.
- **Drop the foe a tier:** Veteran-like → Guard-like; Wraith-like → Specter-like.
- **Use morale aggressively:** solo foes and groups break, flee, or parley at half HP or when their *goal* fails — they are not suicidal (`COMBAT_PROTOCOL.md`).
- **Telegraph harder:** more warning, more time to prepare, scout, or avoid. A solo PC's main defense is information.
- **Stagger arrivals:** foes trickle in over rounds so the PC fights them in sequence, not all at once.
- **Add terrain the PC can exploit:** chokepoints, high ground, cover, a door to bar, water/fire to use.

When an encounter looks too easy, **raise the single foe's tier** or add lair/environment pressure — do not just pile on bodies (that spikes lethality unpredictably for a solo PC).

## Rule 4 — When To Give Advantage Or Extra Resources

Tip the scales toward the PC when:
- The PC scouted, prepared, set an ambush, or used the environment (reward it with advantage, surprise, or a free round).
- The PC recruited an ally, bought help, or leveraged a faction (an ally absorbs 1 foe's worth of pressure).
- The PC is badly wounded and the fiction allows a found potion, a defensible position, or an NPC intervention.
- A clever, valid plan would trivialize the fight — let it (`AI_DM_CORE_RULES.md`: let clever ideas bypass content).

## Rule 5 — Handling A Badly-Wounded PC

A solo PC has no healer. When the PC is below ~⅓ HP:
- **Lean on enemy morale and goals** — most foes do not chase a fleeing PC to the death; they have a job to do.
- **Offer a clear escape route** in the fiction (always pre-placed in dangerous zones).
- **Let damage convert to consequence, not death:** capture, robbery, a lingering injury, lost time, a worsened clock — per `FAILURE_AND_CONSEQUENCES.md`. Cheap death is bad design.
- **Bound guardians cannot pursue** beyond their site — retreat is always an out in dungeons.
- Never spring a *new* encounter on a sub-⅓ HP PC without a meaningful warning and an avoidance option.

## Rule 6 — When NOT To Roll For An Encounter

Skip the encounter roll when:
- The PC is travelling a safe, patrolled road in daylight in a settled region (narrate color instead).
- The PC just finished a hard fight and is limping to safety (don't double-tap; let them reach rest).
- An encounter would only stall the story without adding choice or stakes (`ROLL_AND_CHECK_PROTOCOL.md`).
- The party has cleverly avoided the danger already (don't undo good play with a random roll).
- The session is wrapping and a fresh combat would not resolve cleanly.

Roll for encounters when the result would create a **decision, a risk, or a meaningful complication** — not as a tax on movement.

## Rule 7 — Converting A Party Boss To A Solo Boss

For boss-tier creatures (see `BOSS_AND_APEX_THREATS.md`):
- **Lower HP ~25–40%** from a party-balanced version so the solo PC can actually end it before resources run out.
- **Keep 1 signature mechanic, not three** — a solo PC can't split attention across a multi-phase, multi-add, legendary-action-heavy gauntlet.
- **Replace "summon adds every round" with "summon once when pressed,"** or make the adds the PC's *escape lever* (kill the totem, the summons stop).
- **Always include a non-combat resolution** (rite, parley, watchword, weakness exploit) so the boss is a *problem*, not just a sponge.
- **Phase transitions become breathers, not escalations:** give the solo PC a beat to reposition or use the environment between phases.

## Quick Solo-Budget Cheat Sheet

| PC Level | "A real fight" (Hard) | "A scare" (Deadly, escape-able) | Max bodies (no allies) |
|---|---|---|---|
| 1–2 | 1× CR ½–1 | 1× CR 2, or 2× CR ½ | 2 (+ fragile mooks) |
| 3–4 | 1× CR 2–3 | 1× CR 4, or 3× CR 1 | 3 |
| 5–8 | 1× CR 4–6 | 1× CR 7–8, or leader+2 | 4 |
| 9–12 | 1× CR 8–11 | 1× CR 12, or leader+3 | 5 |
| 13–16 | 1× CR 12–15 | 1× CR 16, or boss+supports | small group |
| 17–20 | 1× CR 16–19 | 1× apex/legendary | 1 apex + lair |

These are *guidance*, not hard caps. The constant rule: **information, terrain, morale, escape, and a non-combat out** make a solo encounter fair — not careful XP math alone.

## Related Files

- [`ENCOUNTER_INDEX.md`](ENCOUNTER_INDEX.md)
- [`BOSS_AND_APEX_THREATS.md`](BOSS_AND_APEX_THREATS.md)
- [`../01_runner_protocol/COMBAT_PROTOCOL.md`](../01_runner_protocol/COMBAT_PROTOCOL.md)
- [`../01_runner_protocol/SOLO_PLAY_PRINCIPLES.md`](../01_runner_protocol/SOLO_PLAY_PRINCIPLES.md)
- [`../01_runner_protocol/FAILURE_AND_CONSEQUENCES.md`](../01_runner_protocol/FAILURE_AND_CONSEQUENCES.md)
- [`../00_control/DND_MECHANICS_REQUIREMENTS.md`](../00_control/DND_MECHANICS_REQUIREMENTS.md)
