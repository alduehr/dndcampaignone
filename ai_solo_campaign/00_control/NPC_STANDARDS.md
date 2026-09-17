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
- Combat relevance tag (none / commoner-like / guard-like / specialist)
- Optional secret

---

## Mechanical Requirements

NPC mechanical completeness follows the tiers in `DND_MECHANICS_REQUIREMENTS.md`. Do not leave combat-relevant NPCs as narrative-only, and do not copy official stat blocks verbatim (see `RULESET_ASSUMPTIONS.md`).

| Tier | Mechanical requirement |
|---|---|
| Major (combat-relevant) | Full Tier 1 stat block or abbreviated/reference profile: CR/level role, type, size, AC, HP, speed, ability emphasis, saves, skills, senses, languages, actions, signature abilities, tactics, morale, solo danger rating, noncombat options, scaling notes |
| Major (noncombatant) / Secondary | Tier 2 profile: competence level, key abilities/skills, passive Insight/Perception if useful, whether dangerous in combat, named fallback stat profile, important spells/abilities if any |
| Minor | Tier 3: a `Combat Relevance` tag (none / commoner-like / guard-like / specialist) plus any notable proficiency. Full stats only if they become important |

Before marking an NPC file done, confirm its tier's mechanical fields are present and not TBD.

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

## Mechanical Profile
Required for any combat-relevant major NPC per `DND_MECHANICS_REQUIREMENTS.md` (Tier 1: villains, recurring adversaries, major allies/companions, rivals, faction champions, bosses, important spellcasters, anyone likely to fight/travel/oppose the player). Use a full custom stat block, a D&D-compatible abbreviated stat profile, or a "use a [baseline]-like profile, modified as follows" reference. Do not leave as TBD unless explicitly a placeholder. Include:
- Suggested level / CR-equivalent role; creature type; size
- AC; HP (or HP range); speed
- Ability emphasis; saving-throw proficiencies; skill proficiencies
- Senses (if relevant); languages; proficiency bonus / CR guidance
- Main attacks/actions; bonus actions, reactions, spellcasting (if relevant)
- Signature abilities; tactics; morale
- Solo-play danger rating; noncombat ways to handle them
- Scaling notes (up/down by tier)

If this major NPC is a noncombatant (Tier 2: leader, patron, priest, sage, merchant, quest-giver), give the lighter Tier 2 profile instead: approximate competence level, key ability strengths, relevant skills, passive Insight/Perception if useful, whether dangerous in combat, and a named fallback stat profile (e.g. "Noble-like, noncombatant unless cornered"; "Spy-like with stronger Insight/Deception"; "Priest-like with low-level divine magic").

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

## Combat Relevance
Per `DND_MECHANICS_REQUIREMENTS.md` Tier 2: state whether dangerous in combat, and give a named fallback stat profile if combat unexpectedly occurs (e.g. "Guard-like"; "Spy-like"; "Commoner, noncombatant"). Note any important spell, ability, or tool proficiency.

## Related Files
```

---

## Minor NPC Standard

```md
| Name | Location | Role | Personality Hook | Useful Detail | Combat Relevance | Optional Secret |
|---|---|---|---|---|---|---|
```

`Combat Relevance` (per `DND_MECHANICS_REQUIREMENTS.md` Tier 3): one of `none` / `commoner-like` / `guard-like` / `specialist`, plus any notable skill or tool proficiency. Minor NPCs do not need full stats unless they become important.

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
