# EXPLORATION_PROTOCOL.md

---
type: protocol
secrecy: dm-only
status: static
tags: [type:protocol, runtime, function:exploration]
related: [AI_DM_CORE_RULES.md, ROLL_AND_CHECK_PROTOCOL.md, CLUE_DELIVERY_PROTOCOL.md, TRAVEL_PROTOCOL.md]
---

## Purpose

How the AI DM runs exploration — ruins, dungeons, wilderness sites, and any scene where the player moves through and examines an environment. Covers pacing, search resolution, clue placement, traps, navigation, and time tracking for a solo PC.

## AI Use

Load when the player enters an unexplored location or begins systematic investigation. Pair with `CLUE_DELIVERY_PROTOCOL.md` for clue-bearing sites and `TRAVEL_PROTOCOL.md` for getting there.

---

## Describing Environments

- Open with mood and the few details that matter (per `SCENE_FRAMING.md` / `TONE_AND_NARRATION.md`): the cold off the basin, the broken grey shapes under the water, the salt and star at a threshold.
- Give the player a **clear mental map of their options**: visible exits, obvious features, anything that draws the eye. Don't hide the navigable layout; hide the *secrets*.
- Reveal further detail in response to where the player looks. Don't pre-narrate everything in the room.

---

## Pacing Exploration

- **Slow down** for: first entry to a significant site, anything uncanny, the approach to a clue or danger, the threshold of the shrine.
- **Summarize** for: empty corridors, repetitive rooms, routine movement ("you work down the flooded stair until the water reaches your knees").
- Keep momentum. If a zone has nothing of consequence, say so and move the player to the next decision.

---

## Resolving "I Search the Room"

1. **Passive first.** What the player's passive Perception would fairly catch is already described — especially danger telegraphs and fair-to-notice clues. A solo PC must not miss a *required* detail because they didn't say the magic word (apply three-clue rule, `CLUE_DELIVERY_PROTOCOL.md`).
2. **Active search** (Investigation/Perception per `ROLL_AND_CHECK_PROTOCOL.md`) reveals **hidden or interpretive** layers: a concealed compartment, the meaning of a carving, a disturbed grave.
3. **Reveal vs. withhold:** give what they'd plausibly find for the effort and skill applied; withhold what's genuinely hidden behind a higher DC, a needed tool, or a needed key (e.g., reading Concord Script gates certain inscriptions — route around it for non-readers via the three-clue rule).
4. **Don't tax thoroughness.** Searching a room the player reasonably should search shouldn't cost a clock tick unless time pressure is established in the fiction.

---

## Environmental Clues

- Place clues as **perceivable details**, never as "you find a clue." (Bad: "you discover an important clue." Good: "the grave's soil is wrong — turned from beneath, not above.")
- Vary the sense: a sound, a smell, a temperature, a mark, a missing thing.
- Cross-check the mystery web (`../11_mysteries_and_secrets/MYSTERY_WEB.md`) for which conclusion the site supports and ensure ≥3 paths exist to it. If the player misses one path, the others remain (see `CLUE_DELIVERY_PROTOCOL.md` for the missed-clue procedure).

---

## Traps and Hazards

- **Telegraph by default** (solo PCs can't afford blind lethality): scorch marks, tripped dust, a too-clean floor, a guide's warning, Concord wardings that hum.
- Give DCs to detect and to disarm/avoid (5e/2024 scale, `ROLL_AND_CHECK_PROTOCOL.md`), plus a costly bypass (time, a resource, a longer route).
- A sprung trap should wound or complicate, not instantly kill a solo character without prior signs.
- The drowned shrine's deep danger is **telegraphed as lethal** (cold, dread, Concord wards, Sashe's refusal). Warn, then let consequences be real if the player presses anyway (`../16_ai_session_packs/SOLO_SAFETY_START.md`).

---

## Navigation and Tracking

- Track where the player has been in a simple zone list; remind them of known exits and unexplored directions when useful.
- For **dungeon/ruin** sites, navigate by named zones/landmarks rather than strict grids.
- For **wilderness**, navigate by landmarks and routes (the Concord roads, the holms, the Greyfens), not hexes. The Greyfens are lethal off-route without a guide and navigable with one (Old Sashe) — a fair, clear gate.

---

## Time and Attrition Tracking

- Track resources that matter: light, rations, spell slots, exhaustion — there is no party to share them (`SOLO_PLAY_PRINCIPLES.md`).
- Track in-world time; passing time can advance world clocks (`../02_runtime_state/WORLD_CLOCKS.md`) and wandering danger.
- Telegraph attrition so the player can decide to press on, rest, or withdraw. Always keep a retreat route available.

---

## Related Files

- [`AI_DM_CORE_RULES.md`](AI_DM_CORE_RULES.md)
- [`ROLL_AND_CHECK_PROTOCOL.md`](ROLL_AND_CHECK_PROTOCOL.md)
- [`CLUE_DELIVERY_PROTOCOL.md`](CLUE_DELIVERY_PROTOCOL.md)
- [`TRAVEL_PROTOCOL.md`](TRAVEL_PROTOCOL.md)
- [`SOLO_PLAY_PRINCIPLES.md`](SOLO_PLAY_PRINCIPLES.md)
