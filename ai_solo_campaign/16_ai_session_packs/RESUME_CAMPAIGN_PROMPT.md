# RESUME_CAMPAIGN_PROMPT.md

## Purpose

The standard prompt the AI DM uses to resume the campaign at the start of any session after the first. Loads current state, recaps recent events, re-establishes scene, and launches play without losing continuity.

## Current Status

**PLACEHOLDER — Not yet populated.** To be created during Stage 2.

---

## When To Use

Use at the start of every session after session 1. Replace `START_NEW_CAMPAIGN_PROMPT.md` after the campaign has begun.

---

## Standard Resume Procedure

When this prompt is complete, it will instruct the AI DM to:

1. Load files in the order defined in `RETRIEVAL_GUIDE.md`
2. Read `NEXT_SESSION_START.md` for the prepared opening
3. Read `SESSION_RECAP.md` for previous session summary
4. Deliver a brief, immersive re-orientation (not a long summary)
5. Present the immediate scene
6. Let the player act

---

## Expected Contents

### Required Files To Load
- `02_runtime_state/CURRENT_STATE.md`
- `02_runtime_state/CURRENT_LOCATION.md`
- `02_runtime_state/CURRENT_SCENE.md`
- `02_runtime_state/PLAYER_CHARACTER.md`
- `02_runtime_state/ACTIVE_QUESTS.md`
- `02_runtime_state/NPC_MEMORY.md`
- `02_runtime_state/FACTION_STATE.md`
- `02_runtime_state/WORLD_CLOCKS.md`
- `02_runtime_state/NEXT_SESSION_START.md`
- Relevant location, NPC, and faction files for the current scene

### Pre-Session DM Check
- Are there any clocks that should have advanced since last session?
- Have any delayed consequences triggered?
- Have any faction actions occurred off-screen?
- Is the opening scene still accurate, or did something change?

### Opening Delivery
- Brief immersive recap: "Last time you..." (2–3 sentences max)
- Immediate sensory scene-setting
- Jump to action; do not over-summarize

### What Not To Reveal At Session Open
- Per `NEXT_SESSION_START.md` hidden DM notes

---

## Related Files

- [`START_NEW_CAMPAIGN_PROMPT.md`](START_NEW_CAMPAIGN_PROMPT.md)
- [`SESSION_END_UPDATE_CHECKLIST.md`](SESSION_END_UPDATE_CHECKLIST.md)
- [`../02_runtime_state/NEXT_SESSION_START.md`](../02_runtime_state/NEXT_SESSION_START.md)
- [`../00_control/RETRIEVAL_GUIDE.md`](../00_control/RETRIEVAL_GUIDE.md)
