# NPC_STANDARDS.md

## Purpose

Use this file when creating or editing:
- Major NPCs
- Secondary NPCs
- Minor NPCs
- NPC indexes
- Relationship webs
- NPC memories
- Voice guides
- NPC secret ledgers

The campaign should contain hundreds of predetermined NPCs so the AI DM does not need to invent important people during play.

---

## NPC Tiers

### Major NPC

Full campaign-relevant character.

Requires:
- Full profile
- Secret
- Motivation
- Fear
- Leverage
- Relationships
- Voice
- Possible evolution
- Quest/mystery/faction links

### Secondary NPC

Useful recurring or local character.

Requires:
- Name
- Location
- Role
- Motive
- Secret or complication
- Relationship link
- What they know
- How they enter play

### Minor NPC

Named local color with utility.

Requires:
- Name
- Location
- Role
- Personality hook
- Useful detail
- Optional secret

---

## Major NPC Standard

```md
# NPC Name

---
type: npc
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

## Name

## Tier
Major

## Location

## Faction Ties

## Role

## First Impression

## Appearance

## Voice

## Personality

## Motivation

## Fear

## Secret

## Leverage

## What They Know

## What They Want From The Player

## What They Can Offer

## How They Can Harm The Player

## Relationship Links

## Current Attitude Toward The Player

## Possible Evolution

## DM-Only Notes

## Related Quests

## Related Mysteries

## Related Locations

## Related Files
```

---

## Secondary NPC Standard

```md
# NPC Name

---
type: npc
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

## Tier
Secondary

## Location

## Role

## First Impression

## Motivation

## Secret Or Complication

## Relationship Link

## What They Know

## How They Enter Play

## Related Files
```

---

## Minor NPC Standard

```md
| Name | Location | Role | Personality Hook | Useful Detail | Optional Secret |
|---|---|---|---|---|---|
```

---

## NPC Memory

When an NPC meaningfully interacts with the player, update:

`/02_runtime_state/NPC_MEMORY.md`

Track:
- NPC name
- Date/session
- Interaction summary
- Attitude toward player
- Promises made
- Debts owed
- Secrets revealed
- Lies told
- Favors requested
- Threats made
- Next likely action

---

## NPC Relationship Web

NPC relationships should include:
- Family
- Mentors
- Rivals
- Debtors
- Patrons
- Blackmailers
- Secret lovers
- Former allies
- Political dependencies
- Religious ties
- Criminal ties
- Old betrayals
- Shared secrets

Use relationship links to create quests and consequences.

---

## NPC Voice Notes

Voice notes should be short and usable.

Good:
- "Speaks like every sentence is a contract."
- "Never answers the first question directly."
- "Uses affectionate insults when nervous."
- "Pauses before names, as if checking whether they are safe to say."

Bad:
- "Charismatic and mysterious."
- "Talks normally."
- "Has an accent."

---

## NPC Design Avoidances

Avoid:
- NPCs with no use in play
- Ten NPCs filling the same role in the same location
- Every NPC having a tragic secret
- Every NPC being secretly powerful
- NPCs who know everything
- NPCs who solve the player's problems
- NPCs who exist only to dump lore
- Player-facing descriptions that reveal hidden motives
