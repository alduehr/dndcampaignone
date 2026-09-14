# FACTION_STANDARDS.md

## Purpose

Use this file when creating or editing:
- Factions
- Guilds
- Churches
- Cults
- Noble houses
- Criminal networks
- Armies
- Rival adventuring groups
- Political movements
- Secret societies
- Faction clocks
- Faction quests

Factions are engines of change. They should create pressure, opportunity, conflict, consequences, and movement.

---

## Faction Philosophy

Every faction needs:
- Public face
- True agenda
- Resources
- Methods
- Internal conflict
- Relationships
- Secrets
- Activity if ignored
- Hooks into play

Avoid static factions that exist only as lore.

---

## Faction File Standard

```md
# Faction Name

---
type: faction
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
When to load this faction.

## One-Sentence Identity

## Public Face
What most people believe.

## True Agenda
DM-only if hidden.

## Founding / History

## Leader

## Important Members

## Resources

## Methods

## Territory / Influence

## Internal Conflict

## Allies

## Enemies

## Secrets

## Current Activity

## Escalation Clock

## Quests Offered By This Faction

## Quests Against This Faction

## How They React To The Player

## What They Do If Ignored

## How They Can Help A Solo Player

## How They Can Threaten A Solo Player Without Cheap Death

## Combat Capability And Stat References
Per `DND_MECHANICS_REQUIREMENTS.md`: how dangerous the faction is in a fight, the typical adversary types/levels it can field (enforcers, soldiers, champions, spellcasters), and the stat references used (link to bestiary entries or named-NPC profiles; no narrative-only enforcers). Note the solo-PC danger of a confrontation and any scaling guidance for low- vs high-level play.

## Related NPCs

## Related Locations

## Related Mysteries

## Related Files
```

---

## Faction Clock Standard

```md
## Clock Name

### What Advances The Clock
- ...

### Stage 1
...

### Stage 2
...

### Stage 3
...

### Stage 4
...

### Final Consequence
...

### How The Player Can Slow, Stop, Redirect, Or Exploit It
- ...
```

---

## Faction Relationship Standard

Use a table like:

```md
| Faction | Relationship | Public Reason | Hidden Reason | Current Tension |
|---|---|---|---|---|
```

Relationships should include:
- Alliances
- Rivalries
- Trade dependencies
- Religious disputes
- Shared secrets
- Historical betrayals
- Proxy conflicts
- Blackmail
- Open war
- Cold war
- Personal leader relationships

---

## Faction Quest Chain Standard

Each major faction should eventually have:
- Introductory hook
- Trust-building task
- Moral complication
- Internal faction conflict
- Rival faction conflict
- Major faction decision point
- Consequence if helped
- Consequence if opposed
- Consequence if ignored

---

## Faction Agency Rules

Factions should act when:
- Time passes
- The player completes a related quest
- The player ignores a threat
- The player harms faction interests
- The player helps an enemy
- A world clock advances
- A secret becomes public
- A leader dies or disappears
- A major location changes hands

Record faction changes in:
- `/02_runtime_state/FACTION_STATE.md`
- `/02_runtime_state/WORLD_CLOCKS.md`
- Relevant faction files if static canon changes

---

## Mechanical Requirements

Factions that can confront the player must be mechanically usable per `DND_MECHANICS_REQUIREMENTS.md`. Before marking a faction file done, confirm:

- Faction leaders and champions likely to fight have Tier 1 stat blocks/profiles (full custom, abbreviated, or reference-style — never copied verbatim).
- Rank-and-file/enforcers reference an adversary stat profile (e.g. "Guard-like", "Cultist-like", "Veteran-like") or a bestiary entry.
- Each combat-capable faction has solo-PC danger notes and scaling guidance for the level tiers it appears in.
- Faction quests follow `QUEST_STANDARDS.md` mechanical fields (level range, DCs, combat/noncombat options, rewards, scaling).

Noncombatant factions (purely political/social) still need a fallback note for what happens if a confrontation turns violent.

---

## Faction Design Avoidances

Avoid:
- Factions that are purely good or purely evil
- Factions with no internal disagreement
- Factions that passively wait for the player
- Factions with no resources
- Factions with no named members
- Secret cults everywhere unless thematically justified
- All factions having the same methods
- Faction lore that creates no quests or conflicts
