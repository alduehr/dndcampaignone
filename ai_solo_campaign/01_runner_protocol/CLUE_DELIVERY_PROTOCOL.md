# CLUE_DELIVERY_PROTOCOL.md

---
type: protocol
secrecy: dm-only
status: static
tags: [type:protocol, runtime, function:clue]
related: [AI_DM_CORE_RULES.md, SECRET_REVEAL_PROTOCOL.md, ../11_mysteries_and_secrets/MYSTERY_WEB.md, ../02_runtime_state/KNOWN_CLUES.md, ../02_runtime_state/HIDDEN_CLUES.md]
---

## Purpose

How the AI DM surfaces clues fairly, ensures every important conclusion is reachable, tracks what the player actually knows versus merely encountered, and never solves the mystery for the player. This protocol enforces the three-clue rule for a solo campaign.

## AI Use

Load before any scene where a significant clue might surface, or when the player is actively investigating a mystery. Always consult `../11_mysteries_and_secrets/MYSTERY_WEB.md` for which conclusion a clue supports and what the other paths are.

---

## The Three-Clue Rule (Enforced)

Every important conclusion in this campaign must have **at least three independent clue paths**, varied by approach, so a single character can reach it. The mystery web (`MYSTERY_WEB.md`, mysteries M0–M10) is already built this way; your job is to **honor it at the table**:

1. Before running an investigation scene, identify which mystery/conclusion it feeds and what the three+ paths to that conclusion are.
2. Never make a required conclusion depend on one clue, one location, one NPC, or one successful roll.
3. If the player misses one path, the others remain available. Track which paths are still open.

Vary clue approaches across: investigation, social, exploration, research, magic, combat aftermath, faction contact, environmental observation, dreams/omens, documents, NPC confession, physical evidence.

---

## How To Present a Clue

- **Never label it.** Don't say "you find an important clue" or "this seems significant." Present a concrete, perceivable detail and let the player weigh it (see `TONE_AND_NARRATION.md`).
  - Bad: "You find a crucial clue about the shrine."
  - Good: "The grave's soil is turned from beneath, not above. Whatever moved here, it came up."
- **Make it concrete enough to reason from.** A fair clue gives the player something to *do* or *connect*, not just atmosphere.

### Delivery by channel

- **Environmental (passive):** what the player perceives without searching — surfaced via passive Perception/Insight so a solo PC can't miss a fair, required detail (`ROLL_AND_CHECK_PROTOCOL.md`). Use for at least one path of every required conclusion.
- **Active investigation:** what they find when they search/study (Investigation/Perception, fair DC).
- **Social / NPC:** what an NPC tells, lets slip, or confirms — gated by attitude and trust (`SOCIAL_SCENE_PROTOCOL.md`). NPCs in this campaign each hold *part* of the truth (e.g., Sashe's drift-map, Wend's old songs, the Tallow Man's witness).
- **Documents / research:** ledgers, inscriptions, archive-cairns. Some are gated behind Concord Script — provide a non-reader path for the same conclusion elsewhere.

---

## Do Not Solve It For Them

- Deliver the clue; do **not** deliver the interpretation. The player connects the dots.
- If the player has a clue but hasn't connected it, that's fine — leave it. Do not editorialize ("this must mean the shrine is...").
- You may let an NPC *offer a theory* if that NPC would plausibly do so — but frame it as that NPC's opinion (possibly wrong), not as authorial truth.

---

## When the Player Has a Clue but Drew the Wrong Conclusion

- Allow it. Misinterpretation is fair and interesting. Track it in `KNOWN_CLUES.md` as a **misinterpreted** clue.
- Let the world respond to their wrong theory honestly (consequences, dead-end leads that aren't *blocking*, NPCs who react to the mistaken belief).
- Provide future clues that can correct the misread, but never force the correction.

---

## When the Player Misses All Paths

If the player has bypassed or failed every existing path to a *required* conclusion and is stalling:

1. **Confirm it's actually required.** Many conclusions are optional; only force-correct genuine blockers.
2. **Introduce a fourth path** through an active, fiction-grounded channel: a faction acts and exposes information, an NPC seeks the player out, a clock advances and surfaces evidence, a consequence reveals the truth (per the three-clue rule's "always add a path" principle).
3. **Never invent an answer that contradicts** `MYSTERY_WEB.md` or `../03_canon/DM_ONLY_CANON.md`. New paths point to the same authored truth.
4. Record the new path in `HIDDEN_CLUES.md` / the DM recap.

---

## Tracking What the Player Knows

At session end (and live, in your head):

- **Discovered and understood** → `../02_runtime_state/KNOWN_CLUES.md` (player-safe).
- **Discovered but misunderstood** → `KNOWN_CLUES.md`, flagged misinterpreted.
- **Exists but undiscovered / paths still open** → `../02_runtime_state/HIDDEN_CLUES.md` (DM-only).
- Do not assume the player has connected clues unless they've said or done so. Track the *connection*, not just the encounter.

---

## Foreshadowing That Becomes a Clue Later

- You may plant atmospheric details now that only resolve into clues after later context (the broken grey shapes under the basin, the dead facing the water, Sefra's "wrong money"). Note planted foreshadowing in the DM recap (`../16_ai_session_packs/DM_HIDDEN_RECAP_TEMPLATE.md`) so you can pay it off.

---

## Related Files

- [`AI_DM_CORE_RULES.md`](AI_DM_CORE_RULES.md)
- [`SECRET_REVEAL_PROTOCOL.md`](SECRET_REVEAL_PROTOCOL.md)
- [`../11_mysteries_and_secrets/MYSTERY_WEB.md`](../11_mysteries_and_secrets/MYSTERY_WEB.md)
- [`../02_runtime_state/KNOWN_CLUES.md`](../02_runtime_state/KNOWN_CLUES.md)
- [`../02_runtime_state/HIDDEN_CLUES.md`](../02_runtime_state/HIDDEN_CLUES.md)
- [`../00_control/MYSTERY_STANDARDS.md`](../00_control/MYSTERY_STANDARDS.md)
