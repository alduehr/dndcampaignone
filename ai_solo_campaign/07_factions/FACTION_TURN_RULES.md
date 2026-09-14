# FACTION_TURN_RULES.md

---
type: protocol
secrecy: mixed
status: static
factions: [Ashen Wardens, Cinder Ledger, Mourners' Circle, Reachward Compact, Gravecallers, Concord Remnant, Hollow Court]
related: [FACTION_INDEX.md, FACTION_RELATIONSHIP_MAP.md, ../02_runtime_state/FACTION_STATE.md, ../02_runtime_state/WORLD_CLOCKS.md, ../01_runner_protocol/AI_DM_CORE_RULES.md]
tags: [protocol, factions, faction-turn, clocks, runtime, ai-dm]
---

## AI Use

Load between sessions (or at any meaningful time-skip) to make the world move while the player is not watching. This file tells the AI DM **when** a faction turn happens, **how** to decide what each faction does, **how** those actions become rumors and consequences the player can encounter, and **which state files to update afterward.** Use it together with `FACTION_STATE.md`, `WORLD_CLOCKS.md`, and `FACTION_RELATIONSHIP_MAP.md`.

Core principle (from `PROJECT_RULES.md` and `FACTION_STANDARDS.md`): **factions are engines of change. They act even when ignored.** The world should never feel paused waiting for the player.

---

## When A Faction Turn Happens

Run a faction turn at any of these triggers:

1. **Time passes meaningfully** — a long rest stretched into days, a multi-day journey, downtime, or a session-end/session-start gap.
2. **The player completes a faction-relevant quest** — the affected factions and their rivals react.
3. **The player ignores a standing threat or hook** — the clock advances and the driving faction acts.
4. **The player harms a faction's interests** — that faction retaliates per its methods.
5. **The player helps a faction's enemy** — the harmed faction notices and adjusts.
6. **A world clock advances a stage** (`WORLD_CLOCKS.md`) — the driving faction takes the next concrete action that stage implies.
7. **A secret becomes public** — every faction touched by it repositions.
8. **A leader or key member dies, vanishes, or is exposed** — the faction's internal conflict resolves or escalates.
9. **A major location changes hands** (e.g., the basin works reach a new stage) — territory-driven reactions.

If none of these have occurred and no real time has passed, **do not force a turn** — idle churn is as bad as a frozen world.

---

## What Advances A Faction Clock

A clock advances one stage when **any** of the following accumulates (see each clock in `WORLD_CLOCKS.md` for its specific drivers):

- **Pure inaction:** the player ignores the clock's driving thread across a stretch of time (the default "ticking" — typically advance one stage per extended period of neglect; the Master clock #1 advances chiefly *through* the Basin clock #2, not on its own).
- **Player action that feeds it:** e.g., selling relics to the Ledger (#6), feeding the Remnant knowledge (#7), helping the basin works (#2).
- **A linked clock advancing:** the Basin clock (#2) reaching a stage pushes the Master clock (#1); the Wardens-Break clock (#3) advancing accelerates #1; regional clocks (V/T/C-PC) feed #6/#1/#10.
- **An NPC succeeding off-screen:** Reke winning a vote, the Vyre–Quorrin deal maturing, Cole Ashby acquiring tools.

A clock **slows, stalls, or steps back** when the player uses one of its listed levers (each clock lists "Player levers"). Record both advances and slowdowns.

**Rate guidance (solo pacing):** advance at most one stage per faction per turn unless the player did something dramatic (e.g., handed the Remnant the shrine's location). Never jump a clock to its Final Consequence without the player having had reachable chances to intervene. The Master clock must always remain telegraphed and beatable.

---

## How To Decide What A Faction Does

For each faction with a trigger, resolve a turn in five quick steps:

1. **Read its goal and methods** (the faction file's True Agenda + Methods). The Ledger buys and leverages; the Mourners protest and refuse; the Gravecallers recruit and probe; the Compact legislates; the Remnant researches and acquires; the Wardens labor and strain; the Court works through cutouts.
2. **Read its current clock stage** (`WORLD_CLOCKS.md`). Take the **next concrete action that stage implies**, not an abstract one. ("Stage 2: work begins; water drops" → the works visibly start; a Reed Holms family is served eviction.)
3. **Check the relationship map** (`FACTION_RELATIONSHIP_MAP.md`). If the player recently helped a rival, the faction reacts to that too (cooling, suspicion, a counter-move).
4. **Apply attitude toward the player** (`FACTION_STATE.md`): ally/friendly factions offer aid or warnings; suspicious/hostile factions surveil, pressure, or obstruct; unaware factions simply pursue their goal and may *become* aware.
5. **Choose ONE visible action and ONE optional hidden action.** The visible action can surface as a rumor, a changed scene, or a new hook. The hidden action advances a DM-only thread (the deal, the steering, the Court's reach) and is recorded but not narrated.

Prefer actions that **create opportunities and pressure for the player**, not actions that simply win the game off-screen. A faction that "already succeeded while you slept" is bad solo design; a faction that "took a step you can still see and counter" is good.

---

## How Faction Actions Become Rumors

Every visible faction action should be **learnable** before it is a fait accompli. Convert each turn's visible action into one or more of:

- **A rumor** at an inn, market, or road (use `RUMORS_TABLE.md` style; point it at the real action). Example: "They say the drainage crews started cutting the dyke past Reedford."
- **A changed scene** the player walks into (a blocked caravan, a new watch checkpoint, a fresh grave-mark on a door).
- **A new or escalated hook** (a Mourner asks for help against the buyers; a Warden begs aid for an un-tended town).
- **An NPC's changed behavior** (Domic Sael pushes a loan harder; Hale looks more hollow; Sefra grows uneasy).

Rule of thumb: **the player should be able to hear about a clock's advance before its Final Consequence lands.** Telegraph through rumor first, scene second, consequence third.

---

## How Conflicts Escalate Or De-escalate

Use the relationship map's blocs and tensions:

- **Escalate** when the player (or time) tips a tension: e.g., the player feeds the Ledger relics → the Circle's anti-buyer fury rises → mobs block a caravan → a buyer is beaten (Circle clock advances; Ledger reacts with hired pressure).
- **De-escalate** when the player mediates or removes a driver: e.g., the player wins a Compact vote against the basin scheme → the Circle's fury cools → the Wardens breathe → the Master clock stalls.
- **Cross-faction ripple:** when one faction acts, check its allies and enemies. The Ledger funding the works (ally: Compact) angers the Mourners (enemy) and quietly pleases the Court (hidden). Record the ripple even if only one strand surfaces this turn.
- **Keep "right from their own view":** no faction should act cartoonishly. Even retaliation has a logic the player could have predicted.

---

## Solo-Play Guardrails For Faction Turns

- **No off-screen lethality.** A faction turn never kills the player or an essential NPC without an on-screen, telegraphed, reachable sequence. Surveillance, pressure, framing, and proxy threats come first.
- **Always leave a lever.** Every advance must leave at least one of the clock's listed player levers still usable.
- **Never resolve the Master clock off-screen.** #1 (The Harvest Restarts) only reaches Stage 3+ through visible events (the basin draining, the shrine breaching) the player had chances to oppose.
- **Multiple clue paths survive.** A faction turn must not remove the last route to a needed clue (three-clue rule). If a turn would, route the clue elsewhere instead.
- **Protect the secrets.** Hidden actions (the deal, the steering, the Court's hand) are recorded in DM-only state, surfaced only as the player earns them.

---

## What To Update After A Faction Turn

After resolving faction turns, update these runtime files (per `SESSION_END_UPDATE_CHECKLIST.md`):

| File | What to record |
|---|---|
| `../02_runtime_state/WORLD_CLOCKS.md` | New clock stages; what advanced/slowed them; "last advanced" notes |
| `../02_runtime_state/FACTION_STATE.md` | Each faction's new attitude, activity, and "next likely action"; player reputation changes |
| `../02_runtime_state/CONSEQUENCES.md` | Concrete results (visible and hidden) of each faction action |
| `../02_runtime_state/OPEN_THREADS.md` | New or escalated hooks the turn created |
| `../02_runtime_state/NPC_MEMORY.md` | Any NPC whose behavior/attitude changed |
| `../02_runtime_state/RELATIONSHIPS.md` | Shifts in the player's standing with factions/NPCs |
| `../02_runtime_state/KNOWN_CLUES.md` / `HIDDEN_CLUES.md` | Clues the turn exposed or moved (keep secrecy separation) |

Record the **DM-only hidden action** in `CONSEQUENCES.md` (DM section) and `HIDDEN_CLUES.md` as appropriate — never in player-facing summaries.

---

## Quick Per-Faction Turn Cheat-Sheet

| Faction | Default visible move when it acts | Default hidden move (DM) | Surfaces as |
|---|---|---|---|
| Ashen Wardens | Triage a failing town; ask the player for help; warn of danger | Othetha's alarm deepens; the seal weakens unnoticed | A begging hook; a road-side rite; Hale's fatigue |
| Cinder Ledger | Out-buy salvage; press a loan; offer paid work | The Vyre–Quorrin deal matures; vault relic grows in value | A job offer; a debt called; a market rumor |
| Mourners' Circle | Protest/refuse cooperation; block a caravan; tend a backlog | Radicals stockpile tools; Iola's Gravecaller contact deepens | A blocked road; a furious vigil; a plea |
| Reachward Compact | Advance a vote; hire the player; field panic petitions | Reke pushes the basin scheme via procedure | A council scene; a watch checkpoint; a job |
| Gravecallers | Recruit the grieving; probe a ruin; mark a door | Cole Ashby nears the shrine with tools | A whispered offer; a found Knock-mark; a missing griever |
| Concord Remnant | Buy/translate relics; send agents to a ruin | The Reclaimers close on the shrine's location | A scholar's request; a relic shipment; a Caradril rumor |
| Hollow Court (DM) | (Never acts openly) — acts only through Reke and the steering | Master clock turns; the Court's reach grows as the basin drains | Only as the *effects* of Reke/the basin/leakage — never as the Court |

## Related Files

- [`FACTION_INDEX.md`](FACTION_INDEX.md)
- [`FACTION_RELATIONSHIP_MAP.md`](FACTION_RELATIONSHIP_MAP.md)
- [`../02_runtime_state/FACTION_STATE.md`](../02_runtime_state/FACTION_STATE.md)
- [`../02_runtime_state/WORLD_CLOCKS.md`](../02_runtime_state/WORLD_CLOCKS.md)
- [`../01_runner_protocol/AI_DM_CORE_RULES.md`](../01_runner_protocol/AI_DM_CORE_RULES.md)
- [`../16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md`](../16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md)
