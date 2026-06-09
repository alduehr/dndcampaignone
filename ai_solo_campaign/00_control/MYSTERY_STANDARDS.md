# MYSTERY_STANDARDS.md

## Purpose

Use this file when creating or editing:
- Mysteries
- Secrets
- Clues
- Revelation maps
- Puzzle chains
- False leads
- Omens
- Prophecies
- Hidden truths
- Investigation arcs

The campaign should be mystery-rich, but mysteries must be fair and solvable.

---

## Mystery Philosophy

Mysteries should feel deep, but not arbitrary.

A mystery is good when:
- The truth is known to the DM layer
- The player has multiple ways to discover it
- Clues are concrete enough to reason from
- False leads are fair
- Important progress does not depend on one roll
- Discovery changes the world
- The AI DM knows what the player actually knows

---

## Mystery Standard

```md
# Mystery Name

---
type: mystery
secrecy: dm-only
status: static
region:
settlement:
factions:
level_range:
related:
tags:
---

## AI Use

## Central Question

## True Answer

## Surface Explanation

## False Explanations

## Why The Truth Matters

## Required Clues

## Optional Clues

## Red Herrings

## NPCs Who Know Part Of The Truth

## Locations Where Clues Can Be Found

## Quests That Expose Clues

## Factions That Obscure Or Reveal Clues

## How The Player Can Discover The Answer Without Railroading

## What Changes When Discovered

## What Happens If Misunderstood

## Related Files
```

---

## Clue Standard

```md
# Clue Name

---
type: clue
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

## Clue Text / Description

## What It Points To

## Where It Can Be Found

## Who Can Interpret It

## Clue Type
Direct | Indirect | Symbolic | Damaged | Misleading | Partial

## What Player Question It Helps Answer

## Mystery / Revelation Supported

## Current Discovery Status
Hidden | Discovered | Misinterpreted | Confirmed

## Related Files
```

---

## Three-Clue Rule

Every important conclusion should have at least three clue paths.

Clues should vary by approach:
- Investigation
- Social interaction
- Exploration
- Research
- Magic
- Combat aftermath
- Faction contact
- Environmental observation
- Dreams/omens
- Documents
- NPC confession
- Physical evidence

---

## False Lead Rules

False leads are allowed, but they must be fair.

A fair false lead:
- Has a reason to exist
- Can be disproven
- Teaches something useful
- Points toward real content
- Does not punish the player for reasonable thinking

Bad false leads:
- Waste time without payoff
- Exist only to trick the player
- Require author knowledge to avoid
- Block progress
- Contradict the real answer without explanation

---

## Puzzle Rules

Puzzles must be runnable by an AI DM.

Every puzzle should include:
- Setup
- What the player sees
- Required information
- Intended solution
- Alternate valid solutions
- Failure consequence
- Costly bypass option
- Clues available nearby
- What not to reveal too early

The AI DM should present puzzles, not solve them unprompted.

If the player gives a clever valid solution, accept it even if it is not the intended answer.

---

## Known vs Hidden Clues

When a clue is discovered, update:

`/02_runtime_state/KNOWN_CLUES.md`

When a clue exists but is not discovered, store or reference it in:

`/02_runtime_state/HIDDEN_CLUES.md`
`/11_mysteries_and_secrets/CLUE_INDEX.md`

Track what the player actually knows. Do not assume the player has connected the dots unless they have.

---

## Mystery Design Avoidances

Avoid:
- One-clue mysteries
- Vague prophecy as the only clue
- All clues requiring successful rolls
- Secrets hidden only behind combat
- Reveals that invalidate player choices
- Mysteries that depend on the AI improvising the truth later
- Player-facing files that spoil hidden answers
