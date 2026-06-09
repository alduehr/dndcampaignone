# WORLDBUILDING_STANDARDS.md

## Purpose

Use this file when creating or editing:
- World overview
- Maps
- Regions
- Settlements
- Wilderness zones
- Travel routes
- Landmarks
- Ruins
- Local cultures
- Geography
- Regional conflicts

The goal is a large predetermined world that an AI DM can run without inventing major geography during play.

---

## Worldbuilding Philosophy

The world should feel:
- Vast
- Authored
- Political
- Mysterious
- Dangerous
- Connected
- Full of secrets
- Playable from many directions

Avoid creating places that are only decorative. Every major place should have tension, secrets, and hooks.

---

## Region Standard

Every region should include:

```md
# Region Name

---
type: region
secrecy: mixed
status: static
region: Region Name
settlement:
factions:
level_range:
related:
tags:
---

## AI Use
When the AI DM should load this region.

## One-Sentence Identity
What makes this region distinct.

## Player-Facing Overview
What outsiders know or notice.

## DM-Only Truth
What is really going on.

## Geography
Terrain, climate, boundaries, natural features.

## Major Settlements
List and short summaries.

## Minor Settlements
List and short summaries.

## Wilderness Zones
Forests, swamps, mountains, plains, coasts, roads, etc.

## Travel Routes
Roads, rivers, passes, ferries, portals, dangerous routes.

## Factions Present
Who operates here and why.

## Regional Conflicts
Active pressures and tensions.

## Regional Secrets
Hidden truths and mysteries.

## Recurring Threats
Monsters, factions, disasters, curses, rival groups.

## Quest Hooks
Hooks tied to actual content.

## Encounter Themes
What kinds of challenges belong here.

## What Changes If Ignored
Faction advances, disasters, political shifts, monster spread, etc.

## Related Files
```

---

## Settlement Standard

Every settlement should include:

```md
# Settlement Name

---
type: settlement
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

## One-Sentence Identity

## First Impression
What the player notices first.

## Public Overview
What residents say about the place.

## DM-Only Truth
What is really going on.

## Districts / Notable Areas

## Local Leadership

## Important NPCs

## Factions Present

## Shops and Services

## Laws and Customs

## Current Tensions

## Secrets

## Rumors

## Quest Hooks

## Possible Scenes

## Consequences If Ignored

## Related Files
```

---

## Wilderness Location Standard

Every wilderness location should include:

```md
# Location Name

---
type: wilderness_location
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

## One-Sentence Identity

## What The Player Notices First

## What Is Actually Going On

## Hazards

## Creatures / Adversaries

## NPCs Present

## Factions Present

## Secrets

## Clues

## Hooks

## Treasure / Resources

## How It Changes After Interaction

## Consequences If Ignored

## Related Files
```

---

## Map Description Standard

Map notes should support later visual map creation.

Include:
- Continental shape
- Major regions
- Borders
- Mountains
- Rivers
- Coasts
- Seas
- Forests
- Deserts
- Swamps
- Roads
- Trade routes
- Magical routes
- Political boundaries
- Dangerous zones
- Hidden locations
- Scale assumptions
- Travel time assumptions
- Points of interest

Do not require exact coordinates at first. Use relative geography clearly.

---

## Travel Design

Travel should include:
- Route options
- Time cost
- Risk level
- Faction presence
- Environmental challenges
- Encounter themes
- Rumors encountered along the way
- Consequences of delay

Travel should not be empty filler. It should create decisions.

---

## Regional Hooks

Every region should support:
- Low-level hooks
- Mid-level hooks
- High-level hooks
- Faction hooks
- Mystery hooks
- Personal hooks
- Travel complications
- Rumors
- Dungeons or ruins
- Ignored consequences

---

## Settlement Density Guidelines

For major regions, aim over time for:
- 1 major city
- 2–4 towns
- 5–10 villages
- 10–20 wilderness locations
- 3–8 dungeons/ruins
- 20–50 named NPCs
- 20–50 hooks/rumors
- Multiple faction conflicts

These are long-term targets, not single-pass requirements.
