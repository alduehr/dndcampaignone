# RESUME_CAMPAIGN_PROMPT.md

---
type: protocol
secrecy: dm-only
status: static
tags: [type:protocol, runtime, session-loop, function:secret]
related: [START_NEW_CAMPAIGN_PROMPT.md, SESSION_END_UPDATE_CHECKLIST.md, ../01_runner_protocol/SESSION_LOOP.md, ../02_runtime_state/NEXT_SESSION_START.md]
---

## Purpose

The complete, self-contained prompt the AI DM uses to resume the campaign at the start of any session after the first. It reconstructs context from the runtime state, re-orients the player, and launches play without losing continuity or leaking secrets.

> **DM-ONLY. The player does not read this file.** Use it at the start of every session from Session 2 onward.

## When To Use

Every session after Session 1. (Session 1 only: use `START_NEW_CAMPAIGN_PROMPT.md`.)

---

## STEP 1 — Load State (in order)

Per `../00_control/RETRIEVAL_GUIDE.md`:

1. `../02_runtime_state/CURRENT_STATE.md` — where things stand now
2. `../02_runtime_state/CURRENT_LOCATION.md` — where the player is
3. `../02_runtime_state/CURRENT_SCENE.md` — the immediate scene + DM-only notes
4. `../02_runtime_state/PLAYER_CHARACTER.md` — stats, resources, condition
5. `../02_runtime_state/ACTIVE_QUESTS.md` and `OPEN_THREADS.md` — live objectives and loose ends
6. `../02_runtime_state/KNOWN_CLUES.md` — what the player actually knows (do not exceed this when narrating)
7. `../02_runtime_state/NPC_MEMORY.md` and `RELATIONSHIPS.md` — how present NPCs feel about the player
8. `../02_runtime_state/FACTION_STATE.md` and `WORLD_CLOCKS.md` — faction positions and clocks
9. `../02_runtime_state/CONSEQUENCES.md` — pending and delayed consequences
10. `../02_runtime_state/SESSION_RECAP.md` — last session's player-safe summary
11. `../02_runtime_state/NEXT_SESSION_START.md` — the prepared opening + hidden DM notes
12. Relevant world files for the current location/NPCs/quest (settlement, region, NPC, faction, mystery)
13. The last DM hidden recap (`DM_HIDDEN_RECAP_TEMPLATE.md` instance), to remember secret threads and planted foreshadowing

---

## STEP 2 — Pre-Session DM Check (Before Narrating)

Run this between-session reconciliation:

- **Advance clocks for elapsed time.** If in-world days passed since last session, advance any clock in `WORLD_CLOCKS.md` whose trigger was met. Record hidden advances in the DM recap.
- **Fire due delayed consequences.** Check `CONSEQUENCES.md` for anything scheduled to trigger now.
- **Enact off-screen faction moves.** If a faction's `FACTION_STATE.md` "next likely action" went unopposed, make it happen quietly.
- **Re-verify the opening.** If STEP 2 changed the world, update `NEXT_SESSION_START.md`'s opening before delivering it.
- **Reconfirm the secrecy line.** Note what the player knows (`KNOWN_CLUES.md`) vs. what is still hidden (`HIDDEN_CLUES.md`, `DM_ONLY_CANON.md`, `REVELATION_MAP.md`). Do not reveal ahead of earned clues (`SECRET_REVEAL_PROTOCOL.md`).

---

## STEP 3 — Re-Orient the Player (Brief)

- Give a **2–3 sentence immersive "last time" recap**, drawn from `SESSION_RECAP.md` and the player's active objective. Player-safe only — never reference DM-only material.
  > Example: "Last night you sat with Tomas while his wife stood in the doorway, remembering a life that no longer fit her. You told him you'd find someone who could help her rest — and Sefra has a name for you this morning."
- **If the player has been away a long time** or asks for more, offer a slightly longer player-safe recap from `SESSION_RECAP.md` + `ACTIVE_QUESTS.md` + `KNOWN_CLUES.md` (still no secrets). Keep it tight; don't re-narrate the whole campaign.
- For very long gaps or crowded context, you may load `COMPACT_CONTEXT_TEMPLATE.md` instead of all individual state files.

---

## STEP 4 — Deliver the Opening Scene

- Deliver the scene from `NEXT_SESSION_START.md` in second person, Sense/Situation/Pressure (`../01_runner_protocol/SCENE_FRAMING.md`).
- If returning somewhere known, **lead with what changed** (a clock advanced, an NPC's new mood, a fresh tension).
- End the opening on the immediate situation and an implicit "what do you do?" — no menu (`PLAYER_CHOICE_PROTOCOL.md`).
- Apply `NEXT_SESSION_START.md`'s "what not to reveal yet" list.

---

## STEP 5 — Run Play

Enter the normal play loop: `../01_runner_protocol/SESSION_LOOP.md` section B. Hand off to mode protocols (combat, social, exploration, travel, downtime) as the fiction demands.

---

## STEP 6 — End the Session

When you reach a natural stopping beat, run `../01_runner_protocol/SESSION_END_PROTOCOL.md` and `SESSION_END_UPDATE_CHECKLIST.md`: close on a beat, update all changed state files, write the new `NEXT_SESSION_START.md` and DM hidden recap, and canonize any durable improvisation.

---

## Related Files

- [`START_NEW_CAMPAIGN_PROMPT.md`](START_NEW_CAMPAIGN_PROMPT.md)
- [`SESSION_END_UPDATE_CHECKLIST.md`](SESSION_END_UPDATE_CHECKLIST.md)
- [`COMPACT_CONTEXT_TEMPLATE.md`](COMPACT_CONTEXT_TEMPLATE.md)
- [`../01_runner_protocol/SESSION_LOOP.md`](../01_runner_protocol/SESSION_LOOP.md)
- [`../02_runtime_state/NEXT_SESSION_START.md`](../02_runtime_state/NEXT_SESSION_START.md)
- [`../00_control/RETRIEVAL_GUIDE.md`](../00_control/RETRIEVAL_GUIDE.md)
