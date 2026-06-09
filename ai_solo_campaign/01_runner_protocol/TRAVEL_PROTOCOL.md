# TRAVEL_PROTOCOL.md

---
type: protocol
secrecy: dm-only
status: static
tags: [type:protocol, runtime, function:travel]
related: [AI_DM_CORE_RULES.md, EXPLORATION_PROTOCOL.md, ../04_world_atlas/MAP_DESCRIPTION.md, ../02_runtime_state/WORLD_CLOCKS.md]
---

## Purpose

How the AI DM handles overland and regional travel — pacing, meaningful events, faction activity en route, terrain and weather, and arrival. Travel should create decisions and advance the world, not be empty filler.

## AI Use

Load when the player begins a significant journey between locations. Pull distances/routes from `../04_world_atlas/MAP_DESCRIPTION.md` and region detail from `../05_regions/SUNDERING_REACH.md`.

---

## Travel Time and Routes

- Use the travel table in `../04_world_atlas/MAP_DESCRIPTION.md`. In-region rule of thumb (from the region file): Concord roads are safer, ~0.5–2 days between sites; off-road fen travel is double time, hazardous, and needs a guide.
- Present route choices as fiction, not menus (per `PLAYER_CHOICE_PROTOCOL.md`): the safe causeway vs. the faster, lethal fen shortcut; with a guide vs. alone.
- The Greyfens are the clearest travel gate: navigable with Old Sashe, lethal without (`../16_ai_session_packs/SOLO_SAFETY_START.md`).

---

## Play in Detail vs. Summarize

- **Summarize** routine, low-stakes travel: "You reach the holm by dusk without trouble." Then advance any clocks for the time passed.
- **Play through** when the journey holds a real choice, danger, or character beat (a route decision, a telegraphed hazard, an NPC to meet, a rumor to hear).
- Never narrate a long uneventful trek beat by beat. Cut to the next decision.

---

## Purposeful Travel Events

Travel events should do work, not be random noise. Each event should advance at least one of: a quest, a clue, an NPC relationship, a rumor pointing to authored content, a faction's pressure, or atmosphere that sets up a later beat.

Good sources of en-route events in this region:

- **Faction presence:** a Compact watch checkpoint, a Ledger relic-caravan, an Ashen Warden walking to a failed rite, a Mourners' procession, a hidden Gravecaller signal (the Knock).
- **The uncanny:** Remembrances drifting toward the water (telegraphed, usually avoidable — a clue, not necessarily a fight; see `../16_ai_session_packs/OPENING_SCENES.md` Opener C).
- **Rumors:** surface entries from `../09_quests/RUMORS_TABLE.md` via a fellow traveler or a wayside hamlet.
- **Hooks:** a stranded peat-cutter, a stolen salt shipment, an archive-cairn ahead — tie to `../09_quests/HOOKS_TABLE.md`.

Until Stage 13/15 build full encounter tables, draw events from the above authored sources; improvise only minor connective detail (`WHEN_TO_IMPROVISE.md`).

---

## Weather and Terrain as Complication

- Use the region's defining conditions: cold, wet, fog, sinking ground, flood-prone river banks. Greyfall (late autumn) is the starting season — brutal weather is on the way.
- Make weather a *decision*, not just flavor: fog that hides the route (and the dead), a flood that closes a causeway, cold that forces a rest or a shelter choice.

---

## Solo Travel Dangers and Outs

- Telegraph route hazards before they commit (per `SOLO_PLAY_PRINCIPLES.md`). A lone traveler in the fens must be able to read the danger and turn back.
- Always provide a retreat or a guide option. Don't strand a solo PC with no safe exit.
- Faction patrols/checkpoints should default to social/legal friction, not lethal ambush.

---

## What the Player Can Do While Traveling

- Forage, scout ahead, set a careful pace (stealth/Survival; with a guide, advantage or auto-success on routing).
- Take a long rest if the fiction allows a safe camp.
- Talk with a companion (Hale, Sashe) — a chance for relationship beats and player-safe lore.

---

## Time Passing and Clocks

- Every journey passes in-world time. At the end of travel, check `../02_runtime_state/WORLD_CLOCKS.md` and advance any clock whose trigger was met (e.g., the basin scheme proceeding while the player is away). Record hidden advances in the DM recap.
- Ignored threats progress during travel — the world does not pause for the road.

---

## Arrival

- Frame arrival as a fresh scene (Sense / Situation / Pressure, per `SCENE_FRAMING.md`): the first impression of the place, who's present, what's changed since last visit.
- If returning somewhere known, lead with what's *different* (a clock advanced, a new tension, an NPC's changed mood).

---

## "You Get There Without Incident"

- Use it freely for safe, established routes the player has run before, or when no event would add anything.
- Do **not** use it to skip a journey that should contain a telegraphed danger, an awaited consequence, or a choice the player would want.

---

## Related Files

- [`AI_DM_CORE_RULES.md`](AI_DM_CORE_RULES.md)
- [`EXPLORATION_PROTOCOL.md`](EXPLORATION_PROTOCOL.md)
- [`../04_world_atlas/MAP_DESCRIPTION.md`](../04_world_atlas/MAP_DESCRIPTION.md)
- [`../05_regions/SUNDERING_REACH.md`](../05_regions/SUNDERING_REACH.md)
- [`../09_quests/RUMORS_TABLE.md`](../09_quests/RUMORS_TABLE.md)
- [`../02_runtime_state/WORLD_CLOCKS.md`](../02_runtime_state/WORLD_CLOCKS.md)
