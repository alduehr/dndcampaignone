# SESSION_END_PROTOCOL.md

---
type: protocol
secrecy: dm-only
status: static
tags: [type:protocol, runtime, session-loop]
related: [SESSION_LOOP.md, ../16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md, ../16_ai_session_packs/STATE_UPDATE_TEMPLATE.md, ../02_runtime_state/NEXT_SESSION_START.md]
---

## Purpose

What the AI DM does at the end of every session — choosing the closing beat, running the state update, writing the next-session handoff, and recording durable improvisation. This is the single most important continuity step in the campaign. Skipping it causes drift.

## AI Use

Load at session end alongside `../16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md`. This is step C of `SESSION_LOOP.md`.

---

## 1. Choose the Closing Beat

End on a compelling beat, never mid-action or mid-sentence. Good session endings:

- **A moment of decision** — the player stands at a real choice for next time.
- **A moment of revelation** — something just recontextualized the situation.
- **A moment of danger** — a clean cliffhanger (telegraphed, fair).
- **A moment of rest or warmth** — a quiet beat at the Drowned Lantern; good for natural stopping points.

Signal the session is wrapping ("This feels like a place to pause"), then give the player a brief **in-character recap** — the player's recap of what *they* did and learned (player-safe only), not the DM's summary of hidden truths.

---

## 2. Run the State Update

Work through `../16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md` section by section, using `../16_ai_session_packs/STATE_UPDATE_TEMPLATE.md` to structure it. Update every state file that changed this session:

- `../02_runtime_state/CURRENT_STATE.md` — the new single-page snapshot
- `../02_runtime_state/CURRENT_LOCATION.md` — where the player now is and what changed there
- `../02_runtime_state/CURRENT_SCENE.md` — the immediate next scene + DM-only notes
- `../02_runtime_state/PLAYER_CHARACTER.md` — level, HP, resources, conditions, lingering injuries, items
- `../02_runtime_state/ACTIVE_QUESTS.md` / `OPEN_THREADS.md` — statuses, new info, new branches
- `../02_runtime_state/KNOWN_CLUES.md` (and `HIDDEN_CLUES.md` if hidden clues changed) — what the player actually knows now (separate discovered from undiscovered; flag misinterpretations)
- `../02_runtime_state/NPC_MEMORY.md` / `RELATIONSHIPS.md` — attitudes, promises, debts, lies, trust shifts
- `../02_runtime_state/FACTION_STATE.md` / `WORLD_CLOCKS.md` — faction reactions and clock positions
- `../02_runtime_state/INVENTORY_AND_REWARDS.md` — items, coin, favors, documents
- `../02_runtime_state/CONSEQUENCES.md` — immediate and delayed consequences (player-known vs. DM-only)
- `../02_runtime_state/SESSION_RECAP.md` — a player-safe summary of the session

### During the update, also:

- **Advance clocks** that should have moved during the session (time, ignored threats, faction triggers) — `WORLD_CLOCKS.md`.
- **Schedule delayed consequences** with a trigger, in `CONSEQUENCES.md`, so they fire at the right future session.
- **Separate secrecy** rigorously: nothing DM-only goes into `SESSION_RECAP.md` or any player-safe file.

---

## 3. Write the DM Hidden Recap

Fill `../16_ai_session_packs/DM_HIDDEN_RECAP_TEMPLATE.md` (DM-only): secret consequences, hidden faction reactions, NPC lies told (and whether believed), undiscovered clue implications, DM-only truths advanced, foreshadowing planted, and hidden clock advances. This is your private continuity layer; never surface it.

---

## 4. Write Next Session Start

Write `../02_runtime_state/NEXT_SESSION_START.md` while the session is fresh:

- The opening scene (immersive, second person, Sense/Situation/Pressure per `SCENE_FRAMING.md`).
- NPCs present, immediate pressure, current objective.
- Files to load at next session start.
- **Hidden DM notes** for the opening (what's really going on).
- **What not to reveal yet** (per `SECRET_REVEAL_PROTOCOL.md` and the revelation map).

A good `NEXT_SESSION_START.md` lets a future session begin cold without re-reading the whole campaign.

---

## 5. Canonize Durable Improvisation

If the session produced something that will recur (a named NPC, a place detail, a new rumor that points to authored content):

- Record it in `../03_canon/CANON.md` / `PLAYER_SAFE_CANON.md` / `DM_ONLY_CANON.md` as appropriate (per `WHEN_TO_IMPROVISE.md`).
- Register names in `../00_control/NAMING_REGISTRY.md`.
- Add to `../00_control/CONTENT_INDEX.md` (and `TAG_INDEX.md` if a new tag).
- Confirm it contradicts nothing in canon; resolve per `../00_control/CANON_AUTHORITY.md` if it does.

---

## 6. Final Check

Before ending, confirm (per checklist section 15):

- Current location and scene are clear.
- Active quests and open threads are clear.
- Known clues are separated from hidden clues; the player's actual knowledge is recorded.
- NPC attitudes and relationships are updated.
- Faction states and clocks are current.
- Inventory and player condition are current.
- `NEXT_SESSION_START.md` gives a usable opening with hidden notes and a "do not reveal" list.

If any item is unclear, fix it now. The next session depends entirely on this handoff.

---

## Related Files

- [`SESSION_LOOP.md`](SESSION_LOOP.md)
- [`../16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md`](../16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md)
- [`../16_ai_session_packs/STATE_UPDATE_TEMPLATE.md`](../16_ai_session_packs/STATE_UPDATE_TEMPLATE.md)
- [`../16_ai_session_packs/DM_HIDDEN_RECAP_TEMPLATE.md`](../16_ai_session_packs/DM_HIDDEN_RECAP_TEMPLATE.md)
- [`../02_runtime_state/NEXT_SESSION_START.md`](../02_runtime_state/NEXT_SESSION_START.md)
