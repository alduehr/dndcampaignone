# DOWNTIME_PROTOCOL.md

---
type: protocol
secrecy: dm-only
status: static
tags: [type:protocol, runtime, function:downtime]
related: [AI_DM_CORE_RULES.md, SESSION_LOOP.md, ../02_runtime_state/WORLD_CLOCKS.md, ../02_runtime_state/NPC_MEMORY.md]
---

## Purpose

How the AI DM handles downtime — rest, training, research, crafting, faction work, and relationship maintenance between adventures. Downtime keeps the campaign breathing without becoming dead air, and it always passes in-world time, which advances the world.

## AI Use

Load when the player wants time between adventures, or when a natural downtime window arrives (recovering from injury, waiting on an NPC, a quiet stretch in Hollowmere).

---

## Downtime vs. In-Town Interlude

- **In-town interlude:** a few hours to a day — shopping, one conversation, gathering a rumor. Run it as normal scenes; minimal clock movement.
- **Downtime:** several days to weeks of declared activity. Resolve it in summary, advance clocks, and surface what changed. Use this protocol for downtime.

---

## Standard Downtime Activities (5e/2024 + campaign options)

- **Rest and recover:** heal lingering injuries, clear exhaustion, recover from a hard arc.
- **Research:** dig into a mystery via documents, sages, or archives. In this world, learning **Concord Script** (from Lector Briss) is a key research gate that unlocks later clues (`../11_mysteries_and_secrets/MYSTERY_WEB.md`).
- **Train / practice:** justify a feat or skill focus narratively; tie to milestone leveling (`../03_canon/LEVELING_ASSUMPTIONS.md`), not XP grinding.
- **Crafting / commerce:** repair gear, commission an item, sell salvage to the Cinder Ledger.
- **Faction work:** run errands or build standing with a faction (Wardens, Mourners, Compact, Ledger) — moves attitude in `../02_runtime_state/FACTION_STATE.md`.
- **Relationship maintenance:** spend time with an ally or contact (Halla, Hale, Sashe, Sefra, Wend) — moves `../02_runtime_state/RELATIONSHIPS.md` and `NPC_MEMORY.md`.
- **Earn coin:** take low-danger paid work (Sefra's jobs, Compact errands, Ledger odd jobs) — the starting income safety net (`../16_ai_session_packs/SOLO_SAFETY_START.md`).

---

## Time Passes — Advance the World

Downtime is the strongest clock-advancer in the game. When the player spends days or weeks:

1. Determine elapsed in-world time.
2. Open `../02_runtime_state/WORLD_CLOCKS.md` and advance every clock whose trigger is met. The basin scheme proceeds, the Wardens strain, the Gravecallers recruit, the steering tightens — even while the player rests.
3. Enact any faction "next likely action" the player didn't prevent (`FACTION_STATE.md`).
4. Trigger due delayed consequences (`../02_runtime_state/CONSEQUENCES.md`).
5. Record hidden advances in the DM recap (`../16_ai_session_packs/DM_HIDDEN_RECAP_TEMPLATE.md`).

Make this visible on return: the world is a little worse, or different, because time moved.

---

## Make a "Week Off" Meaningful, Not Punishing

- Reward the declared activity with a concrete result (a lead, a repaired relationship, recovered HP, standing gained).
- Don't ambush a resting player with disaster *purely* to punish downtime — but do let the consequences of clocks they're ignoring become visible. The cost of rest is the world moving, not a random gotcha.
- If something urgent would genuinely interrupt the rest (a mob forms over Wren; a clock hits a hard stage), surface it as a choice: continue resting and accept the cost, or cut downtime short to act.

---

## What To Surface During Downtime

On returning from downtime, present (through fiction, not a menu):

- Any clock consequence the player can now see.
- An NPC who wants to talk (a worried Halla, a guilt-ridden Sefra, a grieving Tomas) — pulled from `NPC_MEMORY.md` "next likely action."
- A new or sharpened hook/rumor from `../09_quests/HOOKS_TABLE.md` / `RUMORS_TABLE.md`.
- The result of their downtime activity.

---

## Companion and Contact Development

- Downtime is the natural window for ally relationships to deepen or fray. Use it to develop Hale's doubts, Sashe's trust, Sefra's unease, or a faction contact's loyalty — feeding later arc beats. Record in `RELATIONSHIPS.md` and `NPC_MEMORY.md`.

---

## Related Files

- [`AI_DM_CORE_RULES.md`](AI_DM_CORE_RULES.md)
- [`SESSION_LOOP.md`](SESSION_LOOP.md)
- [`../02_runtime_state/WORLD_CLOCKS.md`](../02_runtime_state/WORLD_CLOCKS.md)
- [`../02_runtime_state/FACTION_STATE.md`](../02_runtime_state/FACTION_STATE.md)
- [`../03_canon/LEVELING_ASSUMPTIONS.md`](../03_canon/LEVELING_ASSUMPTIONS.md)
