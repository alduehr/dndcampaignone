# SOLO_PLAY_PRINCIPLES.md

---
type: protocol
secrecy: player-safe
status: static
tags: [type:protocol, function:solo-safety, runtime]
related: [AI_DM_CORE_RULES.md, COMBAT_PROTOCOL.md, FAILURE_AND_CONSEQUENCES.md, ../16_ai_session_packs/SOLO_SAFETY_START.md]
---

## Purpose

Defines how the AI DM adjusts standard D&D assumptions for a single player character. One player cannot survive the same encounters, information loss, or resource drain as a four-character party. These principles are foundational to every session and override any prepared content that assumes a party.

## AI Use

Load alongside `AI_DM_CORE_RULES.md` at session start. These principles apply to every session and every encounter. When any prepared content seems tuned for a party, re-tune it here before running it. For the campaign's concrete level-1–4 safety net (home base, companion, fen-guide, patron), load `../16_ai_session_packs/SOLO_SAFETY_START.md`.

---

## The Solo Doctrine (Read First)

1. **One PC is fragile.** A solo character has no one to revive them, draw fire, or notice the thing they missed. Build every scene assuming the player is alone unless a companion is explicitly present.
2. **Danger is real; death is fair.** The player can be hurt, robbed, captured, or killed — but only after warning, meaningful choice, and the chance to retreat. Never cheap death (see `FAILURE_AND_CONSEQUENCES.md`).
3. **Cleverness is the main resource.** Stealth, negotiation, investigation, preparation, and terrain use must be as rewarding as combat — usually more so.
4. **The world is the pressure, not the encounter.** Pressure comes from the world clocks (`../02_runtime_state/WORLD_CLOCKS.md`) advancing, not from stacking lethal fights. Let time and factions create stakes.

---

## Core Solo-Play Adjustments

### Encounter Scaling

- **Default to one meaningful adversary, not a group.** A single telegraphed enemy with goals and morale is the baseline solo encounter. For "swarm" content, give the player tactical advantages: chokepoints, allies, stealth routes, or escape routes.
- **Budget by halving party assumptions.** Treat a "deadly" encounter for four PCs as a likely TPK for one. A solo PC's fair "hard" fight is roughly one creature of CR ≈ the PC's level, or two creatures of CR ≈ half the PC's level, with terrain or an ally in play.
- **Action economy is the killer.** Multiple enemies acting each round overwhelm one PC fast. If you must use multiple enemies, stagger their arrival, split them with terrain, or give them non-lethal goals (capture, drive off, delay).
- **This campaign's early threats come one at a time.** Restless dead ("Remembrances") arrive singly and can usually be laid to rest by a true rite rather than fought (see `../16_ai_session_packs/SOLO_SAFETY_START.md`).

### Resource Management Awareness

- There is no party to share healing, spells, or supplies. Assume the PC's resources are the only resources.
- Provide affordable healing access (in Hollowmere: Brother Hale, the Mourners, a hedge-healer) so the PC is not one bad roll from death.
- Allow short and long rests at fair intervals. Do not chain encounters so tightly that the PC can never recover.
- Telegraph attrition: if a dungeon will drain resources, signal it so the player can prepare or withdraw.

### Information Delivery

- A solo PC has no party members to notice different things or hold different skills. Do not gate critical information behind a skill the PC lacks.
- Apply the three-clue rule rigorously (see `CLUE_DELIVERY_PROTOCOL.md`): every important conclusion has at least three paths, varied by approach, so a single character can find it.
- When the player lacks an expert skill, route the needed information through an NPC, a document, or an environmental observation instead.

### Warning, Telegraphing, and Preparation Time

- Always show danger before it commits. Cold, dread, claw-marks, a guide's refusal, a too-quiet room — give signs the player can read and act on.
- Give the player time and means to prepare: scout, ask around, hire help, buy supplies, choose the ground.
- Never spring instant lethality. An ambush may surprise, but it must not kill before the player gets a meaningful choice.

### Value of Noncombat Solutions

- Every dangerous obstacle should have at least one of: a stealth route, a social route, an investigation route, a preparation route, or a retreat route.
- Reward avoidance and cleverness with full progress, not partial credit. Bypassing a fight is a win, not a missed encounter.

---

## Temporary Companion / Ally Rules

When to offer or introduce help (per `../16_ai_session_packs/SOLO_SAFETY_START.md`):

- **Offer a companion when the PC is heading into clear danger alone** and a fitting ally exists (e.g., Brother Hale for rite-related outings; Old Sashe for the Greyfens).
- **Companions support; they do not solve.** Keep them lower-powered than the PC, reluctant to take the spotlight, and unwilling to hand over mystery answers. They heal, warn, guard a flank, or open a door — they do not win the scene.
- **Companions can be hurt, killed, or lost.** This raises stakes honestly. Do not make them invulnerable plot armor, but do not kill them cheaply either.
- **Do not force companions.** If the player prefers to go alone, let them — but keep the telegraphing and retreat options open.
- For companion mechanics (AC, HP, actions, scaling), see `../00_control/DND_MECHANICS_REQUIREMENTS.md` and the NPC's profile in `../08_npcs/MAJOR_NPCS.md`.

---

## Rest and Recovery

- Honor 5e/2024 rest rules. A solo PC needs recovery windows more than a party does.
- Use the home base (the Drowned Lantern) as a guaranteed safe long-rest location in Hollowmere.
- In hostile territory, provide at least one defensible rest spot or allow a controlled retreat to recover before the climax.

---

## When To Let The Player Be Powerful vs. When To Challenge

- **Let them be powerful** when they prepared well, used the fiction cleverly, or earned an advantage. Reward good play with decisive success; do not roll to undercut a clearly-won situation.
- **Challenge them** through the world clocks, social complications, moral dilemmas, and consequences — not by inflating enemy numbers or hit points mid-fight.
- "Hard but fair" means the player could see the danger and had options. "Cheaply lethal" means the danger was hidden, the options absent, or the math impossible. Always aim for the former.

---

## Solo-Safe Failure States

Failure for a solo PC must keep the campaign running. Prefer these over death or dead ends (full menu in `FAILURE_AND_CONSEQUENCES.md`):

- Captured rather than killed (new scene: escape, ransom, interrogation).
- Driven off / forced to retreat (regroup, return better prepared).
- Wounded with a lingering injury (cost without ending play).
- Robbed of an item or clue (recoverable; reroutes the path).
- A clock advances (the world gets worse, but the player still acts).
- A relationship or faction standing sours (social consequence).

A solo failure should change the situation and open a new path — never block all progress.

---

## Related Files

- [`AI_DM_CORE_RULES.md`](AI_DM_CORE_RULES.md)
- [`COMBAT_PROTOCOL.md`](COMBAT_PROTOCOL.md)
- [`FAILURE_AND_CONSEQUENCES.md`](FAILURE_AND_CONSEQUENCES.md)
- [`../16_ai_session_packs/SOLO_SAFETY_START.md`](../16_ai_session_packs/SOLO_SAFETY_START.md)
- [`../00_control/DND_MECHANICS_REQUIREMENTS.md`](../00_control/DND_MECHANICS_REQUIREMENTS.md)
- [`../00_control/QUEST_STANDARDS.md`](../00_control/QUEST_STANDARDS.md)
