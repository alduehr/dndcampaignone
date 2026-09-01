---
visibility: dm-only
title: Combat
---
# Combat

Read this file before adjudicating any combat turn: when a fight starts, when
a new participant joins an ongoing fight, and again at the start of each
combat if the encounter was interrupted by a long gap in play. This overlays
the shared combat procedure — its mechanical backbone (surprise, initiative,
turn structure, when to roll what, adjudicating via `update_character`/
`set_state`, ending combat) holds exactly as written and is not repeated in
full here. `rules-reference/SKILL.md` still covers precise mechanical
definitions. What this file adds is **this campaign's own encounter design
discipline**, which every authored encounter in this campaign already
follows and which this app session (single player) is the primary target
for.

## This campaign is solo-tuned by default

This app session is bound to exactly one character — this campaign was
authored **for exactly that**: every encounter table, dungeon, and boss in
the content tree is already tuned for a lone PC (never balanced for a
four-person party). Read `13_encounters_and_bestiary/
SOLO_ENCOUNTER_SCALING.md` once, early, and keep its rules active for the
rest of the campaign:

- **Never scale a printed encounter up "for challenge."** If a table result
  or dungeon entry lists one foe, or a small group with morale, that count is
  already the intended solo-appropriate shape — don't multiply it.
  Difficulty comes from raising a single foe's tier, not from adding bodies
  (see `SOLO_ENCOUNTER_SCALING.md` Rule 3 for the adjustment dials).
- **Bosses are already reduced for solo play** — signature mechanics, add
  waves, and phase pressure are deliberately trimmed from what a party-tuned
  boss would carry, per `SOLO_ENCOUNTER_SCALING.md` Rule 7 and
  `13_encounters_and_bestiary/BOSS_AND_APEX_THREATS.md`. Don't restore
  party-scale pressure.
- **A non-combat resolution exists for nearly every encounter** in this
  campaign by design (a true rite, a parley, a watchword, a weakness) — check
  the specific encounter/dungeon entry for it before assuming a fight is the
  only path.

> If this campaign is ever run outside this app for a full tabletop group
> instead of a solo player, use `13_encounters_and_bestiary/
> PARTY_SCALING_6_PLAYERS.md` instead of `SOLO_ENCOUNTER_SCALING.md` — that
> conversion layer does not apply to a normal single-character app session
> and should not be consulted here.

## Solo-play safety net (non-negotiable for this campaign)

On top of the shared procedure's mechanics, this campaign requires:

- **Telegraph before anything lethal.** No encounter should be able to kill
  or seriously threaten the PC before they've had a meaningful chance to
  notice danger and choose how to engage it. Authored encounters already
  include warning signs — narrate them.
- **Use morale actively, not just at 0 HP.** Foes flee, surrender, or parley
  at roughly half HP or when their actual goal fails, per the authored
  encounter's own morale notes — very few fights in this campaign are meant
  to end in a fight to the death.
- **Retreat is always an option** unless the specific site explicitly says
  otherwise (a sealed vault, a bound guardian that can't leave its chamber is
  the opposite case — it can't pursue). Don't let a solo PC get cornered with
  no way out that the fiction hasn't set up.
- **A wounded PC (below roughly ⅓ HP) gets extra caution**, per
  `SOLO_ENCOUNTER_SCALING.md` Rule 5 — lean on enemy morale/goals, keep an
  escape route live, and let failure convert to a costly consequence (per
  `FAILURE_AND_CONSEQUENCES.md`) rather than a cheap death.

## Adjudicating outcomes, this campaign's addition

On top of the shared procedure's `update_character`/`set_state` discipline:
if a fight's outcome changes anything about the world beyond the immediate
combatants (an NPC's fate, a faction's posture, a site now damaged or
changed), record it via `record_canon` — see `canon-and-gaps/SKILL.md`.

## Related campaign files

- `13_encounters_and_bestiary/SOLO_ENCOUNTER_SCALING.md` — the master solo
  encounter-budget ruleset
- `13_encounters_and_bestiary/BOSS_AND_APEX_THREATS.md`
- `01_runner_protocol/COMBAT_PROTOCOL.md` · `01_runner_protocol/
  FAILURE_AND_CONSEQUENCES.md`
