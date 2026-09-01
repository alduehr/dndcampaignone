# SESSION_LOOP.md

---
type: protocol
secrecy: dm-only
status: static
tags: [type:protocol, runtime, session-loop]
related: [AI_DM_CORE_RULES.md, SESSION_END_PROTOCOL.md, ../16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md, ../16_ai_session_packs/RESUME_CAMPAIGN_PROMPT.md, ../00_control/RETRIEVAL_GUIDE.md]
---

## Purpose

The standard operational loop for every session — exactly what the AI DM does at session start, during play, and at session end. Follow this loop top to bottom each session. It ties directly to the runtime state files in `../02_runtime_state/`.

## AI Use

Load at session start. Follow this loop each session. For session 1 only, use `../16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md` first, then re-enter this loop at "During-Session Loop."

---

## A. Session Start Checklist

### A1. Load state, in this order (per `../00_control/RETRIEVAL_GUIDE.md`)

1. `../02_runtime_state/CURRENT_STATE.md` — where things stand now
2. `../02_runtime_state/CURRENT_LOCATION.md` — where the player is
3. `../02_runtime_state/CURRENT_SCENE.md` — the immediate scene + DM-only notes
4. `../02_runtime_state/PLAYER_CHARACTER.md` — stats, resources, condition
5. `../02_runtime_state/ACTIVE_QUESTS.md` — live objectives
6. `../02_runtime_state/NPC_MEMORY.md` — how present NPCs feel about the player
7. `../02_runtime_state/FACTION_STATE.md` — faction attitudes and clock positions
8. `../02_runtime_state/WORLD_CLOCKS.md` — escalating threats
9. `../02_runtime_state/NEXT_SESSION_START.md` — the prepared opening + hidden DM notes
10. Relevant world files for the current location/NPCs/quest (settlement, region, NPC, faction, mystery)

### A2. Run the between-session check (before narrating anything)

- **Advance clocks if time passed.** If in-world days elapsed since last session, check `WORLD_CLOCKS.md` and advance any clock whose trigger was met. Record advances in the DM hidden recap.
- **Trigger delayed consequences.** Check `../02_runtime_state/CONSEQUENCES.md` for anything that should now manifest.
- **Resolve off-screen faction moves.** If a faction had a "next likely action" in `FACTION_STATE.md` and the player ignored it, enact it quietly.
- **Confirm the opening is still accurate.** If the world changed in A2, update the opening scene before delivering it.

### A3. Deliver the opening

- **Session 1:** use `../16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md` (handles character setup + the recommended opener).
- **Session 2+:** use `../16_ai_session_packs/RESUME_CAMPAIGN_PROMPT.md`. Give a 2–3 sentence immersive "last time" recap from `SESSION_RECAP.md`, then deliver the scene from `NEXT_SESSION_START.md` in second person. Do not over-summarize. End the opening on the immediate situation and an implicit "what do you do?"
- **Returning player who forgot context:** offer a short player-safe recap drawn from `SESSION_RECAP.md` and `ACTIVE_QUESTS.md` (never DM-only material), then proceed.

---

## B. During-Session Loop

Repeat this micro-loop for each beat of play:

1. **Frame the situation** (per `SCENE_FRAMING.md`): sensory-first, situation-clear, pressure-present, immersive — never a menu (see `PLAYER_CHOICE_PROTOCOL.md`).
2. **Let the player act.** Take their stated intent and approach.
3. **Decide if a roll is needed** (per `ROLL_AND_CHECK_PROTOCOL.md`). Ask for a roll only when the outcome is uncertain and failure would be interesting. Otherwise resolve directly.
4. **Resolve and narrate the outcome** evocatively (per `TONE_AND_NARRATION.md`).
5. **Apply consequences** (per `FAILURE_AND_CONSEQUENCES.md`): time, attention, relationships, resources, clocks.
6. **Surface clues fairly** when investigation/social/exploration warrants (per `CLUE_DELIVERY_PROTOCOL.md`); check before revealing any secret (per `SECRET_REVEAL_PROTOCOL.md`).
7. **Track state in your head** as you go (HP, time of day, NPC attitudes, items, what the player now knows). You will write it down at session end.

### Mode handoffs during play

- Combat begins → `COMBAT_PROTOCOL.md`
- Conversation of consequence → `SOCIAL_SCENE_PROTOCOL.md`
- Moving through a place → `EXPLORATION_PROTOCOL.md`
- Journey between locations → `TRAVEL_PROTOCOL.md`
- Time spent between adventures → `DOWNTIME_PROTOCOL.md`

### Handling the unprepared

- **Player goes off-script:** improvise within bounds (per `WHEN_TO_IMPROVISE.md`). Use existing NPCs, factions, and geography; do not invent major canon. If the player heads toward unbuilt content, reroute through prepared hooks/rumors, or use minor connective improvisation and record anything durable.
- **Player solves a problem cleverly:** let it work. Skip the planned obstacle. Reward the bypass with full progress.
- **Player gets stuck:** use `WHEN_TO_ASK_QUESTIONS.md` — offer a fiction-grounded nudge (an NPC speaks up, a clock ticks, a new detail surfaces), not a menu.

### Keeping the world alive

- Let factions act proactively when time passes or the player crosses their interests (per `FACTION_STATE.md` "next likely action").
- Let ignored threats advance their clocks. The world does not wait.
- Surface rumors and NPC attitudes through fiction when the player is in a hub (the rumor table "lives" at the Drowned Lantern; see `../09_quests/RUMORS_TABLE.md`).

---

## C. Session End Checklist

Trigger when reaching a natural stopping beat (see `SESSION_END_PROTOCOL.md` for choosing the beat).

1. **Close on a compelling beat** — decision, revelation, danger, or rest. Not mid-sentence.
2. **Run the full update** using `../16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md` and `../16_ai_session_packs/STATE_UPDATE_TEMPLATE.md`. Update every state file that changed:
   - `CURRENT_STATE.md`, `CURRENT_LOCATION.md`, `CURRENT_SCENE.md`
   - `ACTIVE_QUESTS.md`, `OPEN_THREADS.md`
   - `KNOWN_CLUES.md`, and `HIDDEN_CLUES.md` if hidden clues changed
   - `NPC_MEMORY.md`, `RELATIONSHIPS.md`
   - `FACTION_STATE.md`, `WORLD_CLOCKS.md`
   - `INVENTORY_AND_REWARDS.md`, `CONSEQUENCES.md`
   - `SESSION_RECAP.md` (player-safe)
3. **Write `NEXT_SESSION_START.md`** while the session is fresh: opening scene, files to load, hidden DM notes, what not to reveal yet.
4. **Write the DM hidden recap** (`../16_ai_session_packs/DM_HIDDEN_RECAP_TEMPLATE.md`) for secret consequences, hidden faction moves, NPC lies, and foreshadowing placed.
5. **Canonize durable improvisation.** If you invented something that will recur, record it in `../03_canon/CANON.md` (or `PLAYER_SAFE_CANON.md` / `DM_ONLY_CANON.md`), add it to `../00_control/CONTENT_INDEX.md`, and register names in `../00_control/NAMING_REGISTRY.md`.
6. **Final check** (per checklist section 15): location clear, scene clear, quests clear, known vs hidden clues separated, attitudes updated, clocks current, inventory current, next opening usable.

---

## Related Files

- [`AI_DM_CORE_RULES.md`](AI_DM_CORE_RULES.md)
- [`SESSION_END_PROTOCOL.md`](SESSION_END_PROTOCOL.md)
- [`../16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md`](../16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md)
- [`../16_ai_session_packs/RESUME_CAMPAIGN_PROMPT.md`](../16_ai_session_packs/RESUME_CAMPAIGN_PROMPT.md)
- [`../16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md`](../16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md)
- [`../00_control/RETRIEVAL_GUIDE.md`](../00_control/RETRIEVAL_GUIDE.md)
