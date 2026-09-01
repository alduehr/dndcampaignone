# SOCIAL_SCENE_PROTOCOL.md

---
type: protocol
secrecy: dm-only
status: static
tags: [type:protocol, runtime, function:social]
related: [AI_DM_CORE_RULES.md, PLAYER_CHOICE_PROTOCOL.md, ../02_runtime_state/NPC_MEMORY.md, ../00_control/NPC_STANDARDS.md]
---

## Purpose

How the AI DM runs social encounters — conversation, negotiation, persuasion, deception, interrogation, and politics — while keeping NPCs consistent with their established personality, voice, attitude, and secrets.

## AI Use

Load for any social scene of consequence, especially with a major or secondary NPC. Pull the NPC's profile from `../08_npcs/MAJOR_NPCS.md` and their current standing from `../02_runtime_state/NPC_MEMORY.md`.

---

## Before the Scene

1. Load the NPC's profile (first impression, public role, voice, motivation, fear, leverage, what they want, what they'll offer, **secret**).
2. Load their current attitude and history from `NPC_MEMORY.md` and `../02_runtime_state/RELATIONSHIPS.md`.
3. Note their faction's current posture from `../02_runtime_state/FACTION_STATE.md` — it colors their goals.
4. Hold the secret in mind as subtext only. It shapes behavior; it is never narrated (see `SECRET_REVEAL_PROTOCOL.md`).

---

## Voicing NPCs

- Use the NPC's **voice note** verbatim as a guide. Examples from this campaign:
  - Sefra: rapid, charming, deflects with jokes, never quite answers the second question.
  - Wend: speaks in proverbs and half-songs; answers questions with older questions.
  - Reke: smooth, reasonable, frames the next step as obvious and modest.
  - Othetha: short, certain blessings; pauses before answering anything about the *cause* of the failures.
- Keep each NPC's verbal fingerprint distinct and consistent across sessions. If you improvise new phrasing, keep it within the note.

---

## Conveying Attitude Through Dialogue

Render attitude as behavior, not labels:

- **Hostile:** clipped, threatening, turns away, calls for others.
- **Suspicious / wary:** answers questions with questions, withholds, tests the player.
- **Neutral:** transactional, polite, gives only what's asked.
- **Friendly:** volunteers detail, offers help, warms over the scene.
- **Ally:** confides, defends the player to others, takes risks.

Move attitude in response to how the player treats the NPC and the dead (in this world, trust is earned by how one treats the dead). Update `NPC_MEMORY.md` at session end.

---

## When To Roll vs. Play It Out

- **Play it out** when the player's words and reasoning are doing the work and the NPC is movable. Good roleplay can succeed without a die.
- **Roll** (per `ROLL_AND_CHECK_PROTOCOL.md`) when the outcome is uncertain, failure is interesting, and the approach matters — e.g., pushing past a guarded secret, talking down a zealot, haggling under pressure.
- Use Persuasion / Deception / Intimidation against a flat DC from the NPC's relevant passive (10 + modifier); use Insight to read them. Don't roll repeatedly to "wear down" an NPC — one meaningful check per real attempt.
- **Never let a single failed social roll hard-block a required path.** Failure shifts the scene (suspicion, a closed door, a new condition), it doesn't end the mystery (three-clue rule still applies).

---

## What NPCs Reveal at Each Attitude Level

- NPCs guard their **secret** at all attitudes until the player earns it through clues, trust, leverage, or consequence (see `SECRET_REVEAL_PROTOCOL.md`).
- Higher attitude unlocks more **player-safe** information, favors, and access — not the secret.
- Example: a friendly Othetha will share rite knowledge and Warden safe-houses; only a late-arc, hard-earned trust crisis makes her break her oath and reveal the seal's purpose.

---

## NPC Lies

- Track every consequential lie in the DM hidden recap (`../16_ai_session_packs/DM_HIDDEN_RECAP_TEMPLATE.md`): the lie, the truth, and whether the player believes it.
- Keep lies internally consistent across sessions. An NPC who lied last week must remember the lie.
- Let Insight surface *that* something is off (a tell), without handing over the truth.
- Some NPCs lie without knowing it (Sefra genuinely doesn't know who hired her; Briss sincerely believes the Remnant is benign). Voice their sincerity honestly.

---

## Social Failure Handling

When a social scene goes wrong:

- The NPC becomes suspicious, ends the conversation, raises a price, or alerts others.
- A faction's attitude can sour (update `FACTION_STATE.md`); a clock may tick.
- Failure opens a new route (a different informant, leverage to find, a relationship to repair) rather than closing the mystery.

---

## Reading the Scene's Purpose

Identify what the scene is *for*, and run it accordingly:

- **Information delivery:** route clues fairly (`CLUE_DELIVERY_PROTOCOL.md`); don't dump.
- **Relationship building:** let warmth, conflict, or vulnerability land; update `RELATIONSHIPS.md`.
- **Quest advancement:** surface the hook through the NPC's wants; tie to `../02_runtime_state/ACTIVE_QUESTS.md`.

A scene can serve more than one; lead with the one that matters most now.

---

## Immovable vs. Movable

- An NPC should be **movable** when the player offers something real (a fitting argument, leverage, trust, payment).
- An NPC should be **immovable** when moving them would betray their established core (Wend won't share the old songs until the player honors the dead; Veyl wants agreement, not surrender). Honor these; don't let a high roll override character truth.

---

## Related Files

- [`AI_DM_CORE_RULES.md`](AI_DM_CORE_RULES.md)
- [`PLAYER_CHOICE_PROTOCOL.md`](PLAYER_CHOICE_PROTOCOL.md)
- [`SECRET_REVEAL_PROTOCOL.md`](SECRET_REVEAL_PROTOCOL.md)
- [`../02_runtime_state/NPC_MEMORY.md`](../02_runtime_state/NPC_MEMORY.md)
- [`../08_npcs/MAJOR_NPCS.md`](../08_npcs/MAJOR_NPCS.md)
- [`../00_control/NPC_STANDARDS.md`](../00_control/NPC_STANDARDS.md)
