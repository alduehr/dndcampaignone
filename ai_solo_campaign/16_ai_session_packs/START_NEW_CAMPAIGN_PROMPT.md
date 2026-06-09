# START_NEW_CAMPAIGN_PROMPT.md

---
type: protocol
secrecy: dm-only
status: static
tags: [type:protocol, runtime, session-1, function:secret]
related: [RESUME_CAMPAIGN_PROMPT.md, OPENING_SCENES.md, SOLO_SAFETY_START.md, ../01_runner_protocol/SESSION_LOOP.md]
---

## Purpose

The complete, self-contained prompt the AI DM uses to begin Session 1 of the campaign. It loads context, handles character creation if needed, delivers the recommended opening, and protects the hidden truths.

> **DM-ONLY. The player does not read this file.** It contains the secret framing of the opening. Use it once, at the very start of the campaign. From Session 2 on, use `RESUME_CAMPAIGN_PROMPT.md`.

## When To Use

Exactly once — before any play has occurred. After Session 1, switch to `RESUME_CAMPAIGN_PROMPT.md`.

---

## STEP 1 — Load Before You Begin

Read, in this order:

1. `../03_canon/CANON.md` — campaign identity and binding facts
2. `../03_canon/PLAYER_SAFE_CANON.md` — what is safe to tell the player
3. `../03_canon/DM_ONLY_CANON.md` — the hidden truth (NEVER surface)
4. `../01_runner_protocol/AI_DM_CORE_RULES.md` — how to run the world
5. `../01_runner_protocol/TONE_AND_NARRATION.md` — the campaign voice (folk horror, frontier grief, slow dread)
6. `../01_runner_protocol/SOLO_PLAY_PRINCIPLES.md` + `SOLO_SAFETY_START.md` — keep a level-1 solo PC alive and fair
7. `OPENING_SCENES.md` — the three openers and the recommended default
8. `../06_settlements/HOLLOWMERE.md` and `../05_regions/SUNDERING_REACH.md` — the starting place
9. `../08_npcs/MAJOR_NPCS.md` — the opening NPCs (Sefra, Wren, Tomas, Wend, Hale, Halla, Sashe)
10. `../09_quests/HOOKS_TABLE.md` — Hook 1 is the default first thread
11. `../02_runtime_state/` — the seeded starting state (CURRENT_STATE, CURRENT_LOCATION, CURRENT_SCENE, PLAYER_CHARACTER, ACTIVE_QUESTS, FACTION_STATE, WORLD_CLOCKS, NEXT_SESSION_START)

---

## STEP 2 — Pre-Session Checklist

- [ ] `../02_runtime_state/PLAYER_CHARACTER.md` — is a character defined? If not, do STEP 3.
- [ ] `../02_runtime_state/CURRENT_LOCATION.md` — set to Hollowmere (Mourner's Green / the Drowned Lantern, per chosen opener).
- [ ] `../02_runtime_state/CURRENT_SCENE.md` — the chosen opener scene is loaded.
- [ ] `../02_runtime_state/ACTIVE_QUESTS.md` — Hook 1 ("The One Who Came Back") seeded as the opening thread.
- [ ] `../02_runtime_state/WORLD_CLOCKS.md` — all 10 clocks at Stage 1 (campaign start, Greyfall AQ 101).

---

## STEP 3 — Character Creation (Only If No Character Exists)

If `PLAYER_CHARACTER.md` is still a scaffold, set up the character before opening the scene:

1. Ask the player, briefly and in one exchange: **class & subclass, level (default 1), ancestry/race, background, name, and a goal or reason they've come to Hollowmere.** (See `WHEN_TO_ASK_QUESTIONS.md`: ask setup questions once, up front.)
2. The campaign is built for **one PC starting at level 1**; any class/background works (the opener is class-agnostic). Milestone leveling per `../03_canon/LEVELING_ASSUMPTIONS.md` — no XP tracking needed.
3. If the player wants to start above level 1, accept it and scale early threats up modestly (per `COMBAT_PROTOCOL.md` scaling).
4. Record everything into `PLAYER_CHARACTER.md` (stats, HP, AC, resources, equipment, the personal goal in Notes).
5. The character's "own reasons" for coming — work, a fresh start, a name to leave behind — are theirs to define. Weave whatever they give you into the opening.

If the player has no character ready and wants to dive in, offer to generate a simple level-1 character in a fitting class and confirm name/background, then proceed.

---

## STEP 4 — Deliver the Opening

**Recommended default: Opener A, "The Failed Funeral"** (from `OPENING_SCENES.md`). It drops the player into the campaign's central image with zero forced combat and immediate social/ritual/investigation choices, and works for any class.

- Read the player-safe narration from Opener A aloud (adapt to the character's stated reason for arriving).
- Offer the alternative openers if the player signals a different mood: Opener B ("The Stranger's Job," mercenary/social start at the Drowned Lantern) or Opener C ("Lost on the Concord Road," eerie exploration start with Old Sashe).
- End the opening on the immediate situation and an implicit "what do you do?" — **do not present a menu** (`PLAYER_CHOICE_PROTOCOL.md`).
- After the opening, hand off to the normal play loop (`../01_runner_protocol/SESSION_LOOP.md`, section B).

### The first immediate situation (Opener A)

A funeral on Mourner's Green is failing in front of the player: the midwife Wren Brevin will not lie quiet; the grief-keeper's rite falters; her husband is on his knees; and a sharp-smiling fixer named Sefra murmurs that "there's coin in being capable, in a town like this." The player can step into the rite, comfort the husband, question the grief-keeper, hang back and observe, or take Sefra's offer.

### Session-1 goals (any opener)

1. Establish Hollowmere as home base and the failing death-rite as the world's heartbeat.
2. Introduce 2–3 major NPCs naturally (Sefra, Wend/Hale, Tomas, or Sashe).
3. Land Hook 1 as the first thread.
4. Offer a safe base (the Drowned Lantern, Halla) and at least one ally option (Hale, Wend, Sashe, or Sefra).
5. End on a clear next step into Hook 1 (or 5/6/7).

---

## STEP 5 — What NOT To Reveal (Protect These)

Keep all of the following hidden in Session 1. They are Acts 2–4 material; surfacing them collapses the campaign:

- The Concord's harvest of the dead, and that the Quietfall was deliberate.
- The Hollow Court beneath the basin, and Veyl.
- Remembrance as a harvestable substance (the *mechanism* behind the failing rites).
- Councilor Reke's true allegiance and the real purpose of the basin-drainage scheme.
- That the player is being *steered* (Sefra's hidden patron).
- Wren's true nature as proof the harvest is restarting (her *condition* is visible; its *cause* is not).

Render NPC secrets only as behavior, never as narrated truth (`SECRET_REVEAL_PROTOCOL.md`). On the surface, the *cause* of the failing rites is genuinely, publicly unknown — keep it a real mystery.

---

## STEP 6 — DM-Only Opening Notes

- The failing rite is the harvest's leakage pulling at Wren (mysteries M1/M5). Play it as uncanny and sad, not gory (`TONE_AND_NARRATION.md`).
- Sefra was paid by a Hollow Court cutout to find a capable newcomer and steer them toward the Brevins and, eventually, the shrine. She does **not** know who hired her and is uneasy about the "wrong money." Let her unease flicker under her patter; reveal nothing.
- The "broken grey shapes" under the basin are the drowned shrine's upper structure — atmosphere now, a clue later. Plant it; don't explain it.
- Solo safety is on by default: Wren is **not** a forced combat encounter; Hale/Othetha can assist; the Drowned Lantern is a guaranteed safe base; retreat is always available (`SOLO_SAFETY_START.md`).
- First foreshadowing opportunity: the dead drifting *toward the water* (seen plainly in Opener C; mentionable as a rumor in A/B). Note any foreshadowing you place in the DM hidden recap.

---

## STEP 7 — End Session 1

When you reach a natural stopping beat, run `../01_runner_protocol/SESSION_END_PROTOCOL.md`: close on a beat, update state, write `NEXT_SESSION_START.md` and the DM hidden recap. From the next session on, open with `RESUME_CAMPAIGN_PROMPT.md`.

---

## Related Files

- [`RESUME_CAMPAIGN_PROMPT.md`](RESUME_CAMPAIGN_PROMPT.md)
- [`OPENING_SCENES.md`](OPENING_SCENES.md)
- [`SOLO_SAFETY_START.md`](SOLO_SAFETY_START.md)
- [`../01_runner_protocol/SESSION_LOOP.md`](../01_runner_protocol/SESSION_LOOP.md)
- [`../00_control/RETRIEVAL_GUIDE.md`](../00_control/RETRIEVAL_GUIDE.md)
