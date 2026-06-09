# ROLL_AND_CHECK_PROTOCOL.md

---
type: protocol
secrecy: dm-only
status: static
tags: [type:protocol, runtime, rules, dnd-5e]
related: [AI_DM_CORE_RULES.md, FAILURE_AND_CONSEQUENCES.md, COMBAT_PROTOCOL.md, ../00_control/RULESET_ASSUMPTIONS.md]
---

## Purpose

When and how the AI DM calls for dice rolls. Covers when uncertainty matters, how to set DCs, how to describe outcomes across the spectrum, and how to keep failure interesting rather than story-stalling. D&D 5e / 2024-compatible (see `../00_control/RULESET_ASSUMPTIONS.md`).

## AI Use

Load when about to call for a check, or when unsure whether a roll is warranted.

---

## The Three Conditions for a Roll

Call for a check only when ALL of these hold:

1. **The outcome is uncertain** — success and failure are both genuinely possible.
2. **Failure would be interesting** — it creates a complication, cost, or new direction (not just "nothing happens" or "you're stuck").
3. **The player's approach matters** — what they're attempting, and how, affects the result.

If any condition fails, resolve narratively instead of rolling.

---

## Never Roll For

- **Trivial tasks** the character would obviously succeed at (climbing a ladder, recalling their own name, buying bread).
- **Lore the character would simply know** — give it to them.
- **Player reasoning that already solved the problem** — if they out-thought the obstacle, let it work; do not roll to undo good play.
- **Outcomes already fixed by established facts** — don't roll against canon.
- **Pure stalling** — if a failed roll would only block progress with no interesting alternative, skip the roll and find another cost (see "Failure with progress").

---

## Setting DCs (5e/2024 scale)

| DC | Difficulty |
|---|---|
| 10 | Easy |
| 15 | Moderate |
| 20 | Hard |
| 25 | Very hard |
| 30 | Nearly impossible |

- Pick the DC from the fiction before the roll, not after.
- Account for the **solo PC's** likely lack of a missing skill — don't gate critical paths behind a DC the lone character almost can't hit. If a path is vital, lower the DC, route it through another approach, or apply the three-clue rule (`CLUE_DELIVERY_PROTOCOL.md`).
- Reward a strong approach with advantage or a lower effective DC; penalize a poor one with disadvantage or a higher DC — make the player's method matter.

---

## Contested Checks Without a Party

- For social/stealth contests, roll the PC against a flat DC derived from the NPC's relevant passive value (e.g., 10 + the NPC's modifier), rather than rolling both sides every time. This keeps a solo scene moving.
- Use the NPC profiles in `../08_npcs/MAJOR_NPCS.md` for relevant strengths (e.g., Sefra's Deception/Insight, Sashe's Survival, Reke's social skill).

---

## Outcome Spectrum

Resolve in four bands, not just pass/fail:

- **Critical / strong success:** the player gets what they wanted, plus an edge (information, position, goodwill).
- **Success:** they get what they wanted.
- **Success with cost** (use on near-misses or to keep tension): they get it, but pay — time, noise, a resource, a worse position, attention from a clock. Prefer this over flat failure when the story needs the player to advance.
- **Failure:** they don't get it this way, and the situation changes (see `FAILURE_AND_CONSEQUENCES.md`). Failure should never be a hard stop on the only path.

### Failure with progress

When a failed roll would block the sole route forward, instead grant the goal with a complication, or reveal partial information plus a new obstacle. The three-clue rule means no single failed roll can hide a required conclusion.

---

## Advantage / Disadvantage

- Grant **advantage** for clever preparation, fitting tools, a helpful ally, surprise, or strong positioning.
- Impose **disadvantage** for poor conditions, haste, injury, fear, or working against the fiction.
- Prefer adjusting advantage/DC over inventing new subsystems.

---

## Passive vs. Active Checks

- Use **passive Perception/Insight** to decide what the player notices without searching — especially for telegraphing danger and surfacing environmental clues to a solo PC who can't "have the rogue check."
- Call for **active checks** when the player deliberately searches, studies, or presses. Don't punish a player for not announcing a search of the obvious — passive scores should already have surfaced the important, fair-to-notice details.

---

## Describing Outcomes

Narrate results in the fiction, never as raw mechanics (per `TONE_AND_NARRATION.md`).

- Bad: "You succeed the DC 15 Insight check."
- Good: "She answers smoothly, but her hand stills on the cup for half a beat too long. Whatever she just told you, she doesn't believe it herself."

Tie the *degree* of success/failure to the *texture* of the description.

---

## Related Files

- [`AI_DM_CORE_RULES.md`](AI_DM_CORE_RULES.md)
- [`FAILURE_AND_CONSEQUENCES.md`](FAILURE_AND_CONSEQUENCES.md)
- [`COMBAT_PROTOCOL.md`](COMBAT_PROTOCOL.md)
- [`CLUE_DELIVERY_PROTOCOL.md`](CLUE_DELIVERY_PROTOCOL.md)
- [`../00_control/RULESET_ASSUMPTIONS.md`](../00_control/RULESET_ASSUMPTIONS.md)
