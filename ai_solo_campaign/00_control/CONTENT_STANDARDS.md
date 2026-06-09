# CONTENT_STANDARDS.md

## Purpose

This file defines shared standards for all content in the AI solo campaign repository.

Content should be:
- Predetermined
- Structured
- Tagged
- Indexed
- Cross-linked
- AI-retrievable
- Clear about secrecy level
- Useful in play

---

## Standard Metadata Block

Use this near the top of important files:

```md
---
type:
secrecy: player-safe | dm-only | mixed
status: static | runtime | active | template
region:
settlement:
factions:
level_range:
related:
tags:
---
```

Definitions:

- `type`: location, region, settlement, npc, faction, quest, mystery, clue, dungeon, encounter, artifact, state, protocol, index, template, etc.
- `secrecy`: whether the whole file is safe for the player, DM-only, or mixed.
- `status`: static lore, runtime state, active campaign state, or template.
- `region`: relevant region if applicable.
- `settlement`: relevant settlement if applicable.
- `factions`: relevant factions.
- `level_range`: level range if applicable.
- `related`: related file paths.
- `tags`: retrieval tags.

---

## Standard File Sections

Use these sections where appropriate:

```md
# File Title

## AI Use
When to load this file and how the AI DM should use it.

## Summary
Short, direct summary.

## Player-Facing
Information safe to tell the player if relevant.

## DM-Only
Hidden truth, secrets, mechanics, or future consequences.

## Related Files
- path/to/file.md
```

Not every file needs this exact structure, but every file must be easy for an AI DM to understand and use.

---

## Secrecy Rules

Always separate:

### Player-Facing Information

This includes:
- What the player sees
- What the player hears
- What the player knows
- What the player could reasonably infer
- Public rumors
- Local beliefs
- In-world claims that may or may not be true

Do not include hidden truth in player-facing sections unless it has been discovered.

### DM-Only Information

This includes:
- True causes
- Secrets
- Hidden NPC motives
- Faction agendas
- Mystery answers
- Future events
- Clue logic
- Villain plans
- Consequence clocks
- Actual supernatural/cosmological truth

If a file is player-safe, do not put DM-only information in it.

If a file is mixed, clearly mark player-facing and DM-only sections.

---

## Index Entry Standard

Index entries should include:

```md
| Name | Type | File | Secrecy | Tags | Summary | Related |
|---|---|---|---|---|---|---|
```

Every index entry should make it clear when an AI DM should load that file.

---

## Cross-Linking Rules

Whenever creating content, link it to related material.

A location should link to:
- NPCs there
- Factions present
- Quests available
- Secrets/clues located there
- Dungeons nearby
- Encounter tables
- Relevant region file

An NPC should link to:
- Location
- Faction
- Quests
- Secrets/clues they know
- Relationships
- Current attitude/memory if active

A quest should link to:
- Location
- NPCs
- Factions
- Clues
- Secrets
- Rewards
- Consequences
- Follow-up threads

A faction should link to:
- Leaders
- Members
- Locations
- Quests
- Clocks
- Secrets
- Enemy/allied factions

A mystery should link to:
- Clues
- Locations
- NPCs who know something
- Quests that reveal information
- Factions that hide or distort information

---

## Canon Rules

Every new established fact should be recorded where appropriate.

Use:
- `/03_canon/CANON.md` for authoritative world facts
- `/03_canon/PLAYER_SAFE_CANON.md` for player-known or player-safe world facts
- `/03_canon/DM_ONLY_CANON.md` for hidden truths
- `/02_runtime_state/*` for current campaign state

Do not leave important facts only inside a random quest or NPC file.

---

## Writing Style

Prefer:
- Dense, useful entries
- Concrete details
- Clear stakes
- Conflicting motives
- Usable secrets
- Clues with purpose
- Hooks that point to real content
- Short summaries
- Tables when useful

Avoid:
- Generic fantasy filler
- Long lore with no play function
- Repeated names or concepts
- Perfectly good or perfectly evil factions
- Villains who passively wait
- Quests with only one solution
- Mysteries with only one clue
- Player-facing spoilers
- Excessive boxed text

---

## Minimum Play Function Rule

Every major piece of content should answer at least two of these:

- What can the player do with this?
- Who wants this?
- Who is hurt by this?
- Who benefits from this?
- What secret does this hide?
- What clue does this reveal?
- What faction cares about this?
- What changes if ignored?
- What consequence can result?
- What future scene can this create?

If it cannot answer at least two, improve it or cut it.
