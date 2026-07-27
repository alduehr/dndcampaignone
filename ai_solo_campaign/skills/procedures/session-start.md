---
visibility: dm-only
title: Session Start
---
# Session Start

Read this at the start of every session, before the first player action is
resolved. This overlays the shared session-start procedure with **The Long
Remembering**'s own campaign-specific bootstrapping — the checklist below is
the authoritative version for this campaign; it retains every step of the
shared procedure and adds what a predetermined, index-first campaign needs on
top of it.

## 0. First session ever vs. a resume

Check `get_character` for the session's bound character. If it comes back as
an empty/default placeholder (no class, no name, level 1 with no background
set), this is the **first session** for this character — go to §1 below
before anything else. If a real character already exists, this is a
**resume** — skip to §2.

## 1. First session: character creation, then the opener

This campaign does not ship a pre-built character. Character creation is a
short, conversational exchange, run once, before the opening scene:

1. Ask the player, in one exchange: **class & subclass, ancestry, background,
   name, and a one-line reason they've come to Hollowmere** (work, a fresh
   start, a name to leave behind — theirs to define). Default level is 1;
   accept a higher starting level if the player wants one. See
   `16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md` Step 3 for the full
   framing and `03_canon/LEVELING_ASSUMPTIONS.md` for how leveling works in
   this campaign (milestone-based — no XP tracking needed).
2. Commit the result via `update_character` — full stats, HP, AC, starting
   equipment, and the stated personal reason recorded so it can be woven into
   the opening.
3. Read `16_ai_session_packs/OPENING_SCENES.md` and open with **Opener A —
   "The Failed Funeral"** by default (a public death-rite failing in
   Hollowmere; zero forced combat; works for any class). Offer Opener B (a
   mercenary/social start at the inn) or Opener C (an eerie exploration start
   on the Concord road) only if the player signals a different mood. Weave
   the player's stated reason for arriving into whichever opener is used.
4. Set the scene per `02_runtime_state/CURRENT_SCENE.md`'s starting shape via
   `set_state`, and seed the first quest thread ("Hook 1 — The One Who Came
   Back") via `set_state` (an `activeQuests` key) — see
   `09_quests/HOOKS_TABLE.md`.
5. **What NOT to reveal in session 1** — the Concord's harvest, the Hollow
   Court, Remembrance-as-substance, Councilor Reke's true allegiance, or that
   the player is being steered. These surface only much later, per the reveal
   gates in `11_mysteries_and_secrets/REVELATION_MAP.md` — see
   `canon-and-gaps/SKILL.md` (this campaign's overlay) for how those gates
   work.

Once the opener is delivered, proceed to the normal play loop — do not
separately re-run §2 below for the same session.

## 2. Every session (first or resumed): the retrieval-first checklist

1. **Consult the recap.** Read it before narrating anything, exactly as the
   shared procedure specifies — continuity comes from the recap and state,
   not from re-deriving the world from memory.
2. **Check current state.** `get_state` + `get_character` for location, active
   quest stage, faction clocks, and known clues before describing where the
   session opens.
3. **Check session canon.** Per `canon-and-gaps/SKILL.md`.
4. **Load this campaign's own retrieval index for the situation at hand.**
   This campaign is large (500+ files) and organized for **index-first
   navigation** — before improvising anything about a place, faction, or
   situation the party is walking into, check
   `00_control/RETRIEVAL_GUIDE.md`'s scenario table (e.g. "Entering a
   settlement," "Entering a region," "Handling a faction action," "Resolving
   a quest") for the exact set of files to load for that situation, rather
   than guessing which of the numbered folders (`04_world_atlas/` through
   `15_random_tables/`) to open. This is this campaign's equivalent of, and
   sits alongside, the shared skill-consultation discipline.
5. **Set the opening scene** and hand agency back to the player quickly, per
   the shared procedure's guidance.
6. **Do not re-roll or re-resolve anything already settled.**

## What NOT to do at session start

Everything the shared procedure already says (don't ask the player to
restate their character or goals — it's in state; don't front-load
exposition; don't silently invent facts without `record_canon`) applies
unchanged.

## Related campaign files

- `16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md` — full first-session
  framing (this file's §1 is the condensed, tool-based version of it)
- `16_ai_session_packs/RESUME_CAMPAIGN_PROMPT.md` — the fuller resume framing
- `16_ai_session_packs/OPENING_SCENES.md` — the three openers
- `00_control/RETRIEVAL_GUIDE.md` — the scenario-driven load map
