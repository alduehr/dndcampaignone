# COMBAT_PROTOCOL.md

---
type: protocol
secrecy: dm-only
status: static
tags: [type:protocol, runtime, function:combat, function:solo-safety, dnd-5e]
related: [AI_DM_CORE_RULES.md, SOLO_PLAY_PRINCIPLES.md, ROLL_AND_CHECK_PROTOCOL.md, FAILURE_AND_CONSEQUENCES.md]
---

## Purpose

How the AI DM runs combat for a single player character — telegraphing, tracking initiative and enemy HP compactly, running enemies intelligently without making them unfairly lethal, handling retreat and morale, and preventing cheap death. This is solo combat first; all party assumptions are overridden by `SOLO_PLAY_PRINCIPLES.md`.

## AI Use

Load at the start of any combat. Always read this alongside `SOLO_PLAY_PRINCIPLES.md` — solo scaling is mandatory, not optional.

---

## Pre-Combat: Telegraph and Offer Outs

Before any fight commits:

- **Telegraph the threat.** Show signs the player can read — claw-marks, a cold that shouldn't be there, a guide's refusal, the dead drifting wrong. No instant lethality.
- **Give a beat to react.** Between seeing the danger and the first blow, the player gets a choice: prepare, position, parley, flee, or strike first.
- **Offer the noncombat route.** Most early threats (the restless dead) can be laid to rest by a true rite, talked past, avoided, or out-maneuvered (see `../16_ai_session_packs/SOLO_SAFETY_START.md`). Combat is one option, rarely the only one.
- **Frame the ground.** Name cover, exits, chokepoints, hazards, and distances. Terrain is the solo player's primary advantage.
- **Ambushes:** an ambush may grant surprise, but the player must still get a meaningful choice before dying. No hidden one-shot kills.

---

## Running Combat

### Tracking (compact)

- Roll initiative once; track order as a short list.
- Track enemy HP as a running number in your head/notes; describe wounds in fiction ("it's moving slower now, dragging one leg"), not as "12 HP left."
- Track the PC's HP from `../02_runtime_state/PLAYER_CHARACTER.md`; remind the player of their condition in-fiction when it changes meaningfully.

### Enemy behavior philosophy

- **Not suicidal, not omniscient.** Enemies act on believable goals and visible information, not metagame knowledge of the PC's HP or build.
- **Goals over death-wishes.** Most enemies want something other than the PC's corpse: to capture, drive off, delay, protect a site, or escape. Let those goals shape tactics and create non-lethal outcomes.
- **Intelligent vs. bestial:** intelligent foes use terrain, focus fire, feint, and negotiate; bestial/undriven things (a lone wrong-come-back Remembrance) act on simple instinct or compulsion and are often avoidable.

### Action economy (the real danger to a solo PC)

- Default to **one meaningful adversary.** If using more than one, stagger arrivals, split them with terrain, or give them limited/non-lethal goals so the PC isn't drowned by the action economy (per `SOLO_PLAY_PRINCIPLES.md`).
- Let the player's positioning and clever play reduce how many enemies can act on them each round.

### Morale

- Check morale when an enemy is bloodied, loses an ally, is outmaneuvered, or its goal becomes unreachable. On a morale break: it flees, surrenders, or parleys.
- This campaign's named adversaries do not fight to the death by default: the Tallow Man flees into the fens; Reke escapes rather than die cheaply; Cole Ashby is dangerous but can be talked down. Use their profiles in `../08_npcs/MAJOR_NPCS.md`.

### Environment and hazards

- Use terrain and hazards as both danger and tool: fog, sinking ground, water, cover, height, fire. The player should be able to weaponize the environment too.

---

## Solo-Safe Combat Design

- **No single encounter should be able to instantly kill the PC** without warning and a prior choice.
- **Death saves and stabilization** follow 5e/2024. A solo PC at 0 HP is in real peril — but allies (Hale), a fleeing enemy, or a captor can create a non-death outcome.
- **Last stand vs. retreat:** always keep a retreat route open. The player may choose a heroic stand, but they must have had the option to withdraw.
- **The narrative "out":** if the player is about to die from something that was *not* fairly telegraphed, do not kill them — convert it to capture, a grievous wound, a timely interruption, or a forced retreat. Cheap death is a design failure (see `FAILURE_AND_CONSEQUENCES.md`).
- **Healing access** exists by design (Hale, the Mourners, a hedge-healer). Don't strand the PC one bad roll from death.

---

## Bosses Alone

- Boss fights get **weaknesses, terrain options, and noncombat win conditions**, never pure HP walls. (Veyl, the final antagonist, is explicitly beatable by persuasion, sabotage, alliance with Maire, or combat — see `../08_npcs/MAJOR_NPCS.md` #14–15 and `../07_factions/major_factions/HOLLOW_COURT.md`.)
- Telegraph boss danger well in advance; let the player prepare, gather allies, and choose the ground.
- Phase bosses so the player can read progress and make tactical choices; allow disengagement points.

---

## Post-Combat

- Describe wounds, exhaustion, and the cost of the fight in fiction. Apply any lingering injury per `FAILURE_AND_CONSEQUENCES.md`.
- Resolve looting and information-gathering (a body, a tool, a map fragment can be a clue — route through `CLUE_DELIVERY_PROTOCOL.md`).
- Apply consequences of noise/visibility: who heard, who comes, which clock ticks (`../02_runtime_state/WORLD_CLOCKS.md`, `FACTION_STATE.md`).
- Allow a rest if the fiction permits (see `SOLO_PLAY_PRINCIPLES.md` rest rules).

---

## Encounter Scaling Quick Reference

- Treat any encounter labeled for four PCs as **roughly 4x too dangerous** for a solo PC; cut numbers, add terrain/ally, or convert to a non-combat challenge.
- Fair solo "hard" fight ≈ one creature of CR equal to the PC's level (with terrain/escape available), or two of CR ≈ half the PC's level.
- When in doubt, fewer enemies + smarter behavior + clearer outs.

---

## Related Files

- [`AI_DM_CORE_RULES.md`](AI_DM_CORE_RULES.md)
- [`SOLO_PLAY_PRINCIPLES.md`](SOLO_PLAY_PRINCIPLES.md)
- [`ROLL_AND_CHECK_PROTOCOL.md`](ROLL_AND_CHECK_PROTOCOL.md)
- [`FAILURE_AND_CONSEQUENCES.md`](FAILURE_AND_CONSEQUENCES.md)
- [`../16_ai_session_packs/SOLO_SAFETY_START.md`](../16_ai_session_packs/SOLO_SAFETY_START.md)
