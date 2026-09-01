# FAILURE_AND_CONSEQUENCES.md

---
type: protocol
secrecy: dm-only
status: static
tags: [type:protocol, runtime, function:solo-safety]
related: [AI_DM_CORE_RULES.md, SOLO_PLAY_PRINCIPLES.md, COMBAT_PROTOCOL.md, ../02_runtime_state/CONSEQUENCES.md]
---

## Purpose

How the AI DM handles failure — what it costs, how it changes the situation rather than ending it, and how to make failure meaningful without being punishing or campaign-ending. For a solo PC, failure must keep play alive.

## AI Use

Load when the player fails a significant check, loses a fight, fails or abandons a quest, or makes a choice with major negative consequences.

---

## The General Rule

**Failure changes the situation; it rarely ends it.** A failed attempt should cost something and open a new path — not block all progress and not, by default, kill the character.

Failure should usually do one or more of:
- Cost time (and tick a clock)
- Attract attention
- Damage a relationship or faction standing
- Spend or lose a resource
- Reveal only partial information
- Create a complication or new problem
- Force a hard choice
- Change the route forward

Failure should rarely:
- End the campaign
- Block the only path to a required conclusion
- Kill the player with no warning
- Strip agency

---

## Failed Rolls

- Prefer **success with cost** or **failure with progress** over a flat dead stop (see `ROLL_AND_CHECK_PROTOCOL.md`).
- A failed roll on the sole route to a required conclusion does not hide that conclusion — the three-clue rule guarantees other paths (`CLUE_DELIVERY_PROTOCOL.md`).
- Narrate the failure as a *turn*, not a wall: the lock holds but the noise drew a watchman; the lie half-lands but she's wary now.

---

## Failed or Abandoned Quests

- Something in the world changes: a door closes, a new door opens, a faction gains or loses ground, a clock jumps a stage.
- Use the quest's own consequence notes (each hook in `../09_quests/HOOKS_TABLE.md` includes a "failure still progresses" branch). Example: an unresolved Wren crisis opens the mob / Tomas-to-Gravecallers branch — new hooks, not a dead end.
- Record the outcome in `../02_runtime_state/ACTIVE_QUESTS.md`, `OPEN_THREADS.md`, and `CONSEQUENCES.md`.

---

## Failed Social Encounters

- NPC attitude drops; they become wary, end the talk, raise a price, or warn others (update `NPC_MEMORY.md`).
- A faction may grow suspicious or hostile (update `FACTION_STATE.md`); a clock may tick.
- A burned NPC isn't the end of an investigation — route to another informant or to leverage that reopens the door.

---

## Combat Loss — Not Cheap Death

When the PC loses a fight, prefer these outcomes over death (per `SOLO_PLAY_PRINCIPLES.md` / `COMBAT_PROTOCOL.md`):

- **Captured** (new scene: escape, ransom, interrogation, a forced bargain).
- **Driven off / forced retreat** (regroup, return better prepared; the objective waits or worsens).
- **Grievously wounded** with a lingering injury (a real cost that doesn't end play).
- **Robbed** of an item, clue, or coin (recoverable; reroutes the path).
- **Saved at a price** by an ally, a fleeing enemy's disinterest, or a captor's plan.

Most enemies here have goals other than killing the PC and morale that breaks — use them.

---

## Cheap Death vs. Fair Death

- **Fair death** follows warning, meaningful choice, and the chance to retreat — and the player pressed on anyway. This is allowed and real.
- **Cheap death** comes from hidden lethality, no options, impossible math, or an untelegraphed ambush. This is a design failure — do **not** let it stand. Convert it (capture, wound, interruption, retreat) per `COMBAT_PROTOCOL.md`'s narrative "out."
- The drowned shrine's deep danger is *telegraphed as lethal*; dying there after ignoring stacked warnings is fair. Dying to an unmarked trap in a normal room is not.

---

## Failure as Accelerant

- Treat botched plans as fuel: a failed heist becomes a chase and a new enemy; a blown negotiation becomes blackmail leverage against the player. Make failure *interesting*, not just costly.

---

## Delayed and Hidden Consequences

- Some failures don't bite immediately. Log them in `../02_runtime_state/CONSEQUENCES.md` with a trigger (a date, a clock stage, the player's next visit) and fire them when due (checked at session start, per `SESSION_LOOP.md`).
- Separate **player-known** consequences (they saw it happen) from **DM-only** consequences (it's brewing off-screen — record in the DM recap, surface later).

---

## Updating State

After a significant failure, update:
- `CONSEQUENCES.md` (the new/delayed consequence, player-known vs. DM-only)
- `ACTIVE_QUESTS.md` / `OPEN_THREADS.md` (status and new branches)
- `NPC_MEMORY.md` / `RELATIONSHIPS.md` (attitude/relationship shifts)
- `FACTION_STATE.md` / `WORLD_CLOCKS.md` (faction reactions, clock advances)
- `PLAYER_CHARACTER.md` (wounds, lost items, exhaustion)

---

## Related Files

- [`AI_DM_CORE_RULES.md`](AI_DM_CORE_RULES.md)
- [`SOLO_PLAY_PRINCIPLES.md`](SOLO_PLAY_PRINCIPLES.md)
- [`COMBAT_PROTOCOL.md`](COMBAT_PROTOCOL.md)
- [`ROLL_AND_CHECK_PROTOCOL.md`](ROLL_AND_CHECK_PROTOCOL.md)
- [`../02_runtime_state/CONSEQUENCES.md`](../02_runtime_state/CONSEQUENCES.md)
