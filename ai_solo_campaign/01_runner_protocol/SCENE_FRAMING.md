# SCENE_FRAMING.md

---
type: protocol
secrecy: dm-only
status: static
tags: [type:protocol, runtime, scene-framing]
related: [AI_DM_CORE_RULES.md, TONE_AND_NARRATION.md, PLAYER_CHOICE_PROTOCOL.md, SESSION_LOOP.md]
---

## Purpose

How the AI DM opens, runs, and closes scenes. The mechanics of framing — how to establish a scene, what to include, how to stay immersive without over-narrating, and how to transition between scenes without losing momentum.

## AI Use

Load when framing a new scene or handling a transition. Pair with `TONE_AND_NARRATION.md` for voice.

---

## Opening a Scene

A good scene-open does three things, in this order:

1. **Sense** — what the player perceives first (sight, then sound/smell/cold/touch). Set atmosphere.
2. **Situation** — what is happening, who is here, what the player is in the middle of.
3. **Pressure** — the implicit stake or question that makes "what do you do?" matter right now.

Then stop and let the player act. Do not append a menu.

**Template in practice:**
> [Sense] The Drowned Lantern is warm and loud, peat-smoke and fish stew. [Situation] You've barely set down your pack when a quick-smiling woman drops onto the bench across from you, already talking. [Pressure] Behind her, the room goes a little quiet at a name she just said — *Brevin* — and she's watching you, not them.

Keep it to a few sentences. Three precise details beat a paragraph.

### Scene-setting vs. information dumping

- **Scene-setting** gives what the player can perceive and act on now.
- **Information dumping** front-loads history, lore, or motive the player hasn't earned.
- Rule: narrate what's in the room, not what's in the archive. Lore arrives through play (see `SECRET_REVEAL_PROTOCOL.md`).

### Presenting NPCs without revealing hidden motives

- Lead with the NPC's **first impression** and **public role** from `../08_npcs/MAJOR_NPCS.md` (the player-safe block).
- Render their secret only as **behavior** — a pause, a deflection, an unease — never as narrated truth. Example: Sefra's "wrong money" shows as a flicker of discomfort under her patter, not as "she's secretly a Court cutout."
- Never narrate a DM-only motive. The player infers; you imply.

---

## Framing by Scene Type

### Combat initiation
- Telegraph first (per `SOLO_PLAY_PRINCIPLES.md` and `COMBAT_PROTOCOL.md`): show the threat and a beat to react before blows land.
- Frame the ground: cover, exits, hazards, distance. Terrain is the solo player's friend.
- Hand off to `COMBAT_PROTOCOL.md` once initiative matters.

### Social encounters
- Open on the NPC's demeanor and the social stakes (what the player wants, what the NPC guards).
- Establish attitude through dialogue, not labels (see `SOCIAL_SCENE_PROTOCOL.md`).

### Exploration and discovery
- Establish the space and its mood, then invite movement. Reveal detail in response to where the player looks (see `EXPLORATION_PROTOCOL.md`).
- Seed environmental clues as perceivable details, not as "you find a clue."

---

## Transitions

- **Cut to** when the interesting question is answered and the next one is clear. Don't play out dead time. "You settle the bill, and by the time the fog lifts you're already on the causeway." 
- **Play through** when the journey or interval itself holds choices, danger, or character (see `TRAVEL_PROTOCOL.md`, `DOWNTIME_PROTOCOL.md`).
- **Bridge cleanly:** end one scene on its beat, name the time/place shift, open the next scene with Sense/Situation/Pressure.
- When summarizing travel/downtime, still advance clocks (`../02_runtime_state/WORLD_CLOCKS.md`) for the time that passed.

---

## Closing a Scene

End on a meaningful beat, not a fade-out:

- **A decision** the player must make.
- **A revelation** that recontextualizes things.
- **A danger** that just appeared.
- **A moment of rest or warmth** (good for session ends; see `SESSION_END_PROTOCOL.md`).

Avoid closing on "nothing happens" or trailing into mechanical bookkeeping. Land the beat, then either transition or hand the moment to the player.

---

## Good vs. Bad Framing

**Bad (menu + dump):**
> You're in Hollowmere, a town founded in AQ 12 over a drowned Concord shrine. The Mourners' Circle and the Compact are in conflict over a drainage scheme. Do you: (1) visit the inn, (2) go to the cemetery, (3) leave town?

**Good (sense, situation, pressure):**
> The fog won't lift off the basin all morning, and the town has the held-breath quiet of a place waiting for bad news. On Mourner's Green, a small crowd has gathered around an open grave that should already be closed. Someone near you says, low, "Not again." 

Let the player move toward the crowd, away from it, or anywhere else.

---

## Related Files

- [`AI_DM_CORE_RULES.md`](AI_DM_CORE_RULES.md)
- [`TONE_AND_NARRATION.md`](TONE_AND_NARRATION.md)
- [`PLAYER_CHOICE_PROTOCOL.md`](PLAYER_CHOICE_PROTOCOL.md)
- [`SESSION_LOOP.md`](SESSION_LOOP.md)
