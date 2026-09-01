# QUEST_STANDARDS.md

## Purpose

Use this file when creating or editing:
- Main campaign quests
- Regional quests
- Faction quests
- Personal quests
- Side quests
- Hooks
- Rumors
- Bounties
- Jobs
- Failure states
- Consequences
- Open threads

The campaign must be open-world but deeply authored. The player should always have prepared opportunities available.

---

## Quest Philosophy

A good quest should:
- Connect to real people, places, factions, secrets, or consequences
- Support multiple approaches
- Include failure states
- Change if ignored
- Account for solo play
- Avoid single-solution design
- Avoid requiring one specific roll to proceed

Failure should usually change the situation, not end the campaign.

---

## Mechanical Requirements

Every developed quest must be mechanically complete per `DND_MECHANICS_REQUIREMENTS.md`. Before marking a quest file done, confirm it includes:

- Recommended character level / range
- Expected solo-PC danger level
- Likely checks and DC bands (DC 10/15/20/25/30)
- Possible combat encounters with solo danger notes and real stat references
- Possible noncombat solutions
- Rest opportunities and/or time pressure
- Rewards appropriate to level
- Failure consequences
- Scaling notes

Do not require a single successful roll to continue the story. Use D&D-style DCs throughout.

---

## Developed Quest Standard

```md
# Quest Name

---
type: quest
secrecy: mixed
status: static
region:
settlement:
factions:
level_range:
related:
tags:
---

## AI Use

## Quest Type
Main | Regional | Faction | Personal | Side | Dungeon | Mystery | Travel

## Level Range
Recommended character level/range AND expected danger level for a solo PC.

## Likely Checks And DCs
Per `DND_MECHANICS_REQUIREMENTS.md`: list the checks likely to come up and their DC band (DC 10 easy / 15 moderate / 20 hard / 25 very hard / 30 nearly impossible). Never gate story progress behind a single successful roll.

## Starting Hook

## Location

## Involved NPCs

## Involved Factions

## Surface Problem

## Hidden Truth

## Objectives

## Possible Approaches

## Obstacles

## Important Scenes

## Clues

## Combat Options
Include possible combat encounters with solo-PC danger notes and the enemy stat references used (link bestiary/NPC profiles; no narrative-only adversaries).

## Noncombat Options

## Solo-Play Safety Valves

## Rest And Time Pressure
Rest opportunities (short/long) available, and any time pressure or clock that limits resting. Per `DND_MECHANICS_REQUIREMENTS.md`.

## Rewards
Rewards appropriate to the recommended level/tier (currency, items, magic items, favors, information). Reference `REWARDS_BY_LEVEL.md` when it exists.

## Consequences

## Failure State

## Follow-Up Hooks

## Scaling Notes
How to scale the quest's encounters, DCs, and rewards up or down for the actual PC level. Per `DND_MECHANICS_REQUIREMENTS.md`.

## State Updates
What to update on success, failure, delay, or partial success.

## Related Files
```

---

## Hook Standard

```md
| Hook | Where It Appears | Who Knows It | Points Toward | Related File | Truth Status |
|---|---|---|---|---|---|
```

Truth status options:
- True
- False
- Partial
- Misleading
- Outdated
- Propaganda
- Supernatural distortion

---

## Rumor Standard

```md
| Rumor | Source | Region/Settlement | Truth Status | Points Toward | Notes |
|---|---|---|---|---|---|
```

Rumors should point to existing or planned content. Do not create rumors with no destination.

---

## Quest Consequence Standard

Consequences should cover:

```md
## If The Player Succeeds

## If The Player Fails

## If The Player Partially Succeeds

## If The Player Ignores It

## If The Player Betrays A Key NPC

## If The Player Solves It Nonviolently

## If The Player Uses Excessive Force
```

Not every quest needs every category, but major quests should include several.

---

## Solo-Play Safety Valves

Dangerous quests should include:
- Warning signs
- Scoutable information
- Negotiation route
- Stealth route
- Retreat route
- Possible ally
- Environmental advantage
- Alternate objective
- Partial success option

Do not make every problem solvable by combat.

---

## Level Range Guidance

For solo play:
- Low-level threats should be dangerous but telegraphed.
- Avoid ambushes that can kill the player before meaningful choice.
- High-danger areas should have visible warning signs.
- A single enemy can be more dangerous than expected.
- Multiple enemies can overwhelm a solo character quickly.
- Social, stealth, investigation, and preparation should matter.

---

## Quest Design Avoidances

Avoid:
- Disconnected fetch quests
- Single-path quests
- "You must fight these enemies to continue"
- Progress hidden behind one failed roll
- Lore dumps disguised as quests
- Quests that assume a party
- Rewards with no relevance
- Consequences that are never tracked
- Hooks that do not point to authored content
