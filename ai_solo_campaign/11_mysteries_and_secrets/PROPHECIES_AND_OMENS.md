---
type: mystery
secrecy: mixed
status: static
region:
factions:
level_range: 1-20
related: [CLUE_INDEX.md, MYSTERY_WEB.md, DISCOVERY_PATHS.md, REVEAL_TIMING.md, by_region/]
tags: [type:mystery, stage-11]
---

# PROPHECIES_AND_OMENS.md

## AI Use

Load this file when deciding how to handle in-world omens, prophetic fragments, or ominous signs during play. This file defines the campaign's omen policy — not a collection of vague prophecy text.

---

## Policy: Omens As Clues, Not Prophecy

This campaign deliberately avoids vague prophecy as a primary mystery-delivery mechanism.

**Why:** Vague prophecy:
- Can unintentionally spoil DM-only truths if not carefully worded
- Creates single-point-of-failure clue paths ("the prophecy said to go to the cairn")
- Tends toward railroading
- Is hard for an AI DM to control during improvisation

**Instead:** The campaign delivers mystery through *concrete echoes* — observable events, physical evidence, NPC behaviour, documents, rite failures, site observations, and rumors that suggest a pattern without stating it outright.

These are handled through the **clue trail system** (`CLUE_INDEX.md`, regional clue files). They function as omens without requiring a prophecy text.

---

## What "Omens" Look Like In This Campaign

Omens in this campaign are always one of the following forms:

| Omen type | Example form | Where tracked |
|---|---|---|
| Death-rite failure | A burial rite didn't settle the dead; the body walked | Regional clue trail files |
| Relic behavior | An old-glass relic hums or pulses near a shrine | `CLUE_INDEX.md` |
| Rumor echo | "Three fishing boats gone in a night" | Hook tables / regional clue trails |
| Environmental sign | Old road stones cracked inward, soil black | Wilderness location files |
| NPC dream/omen | An NPC reports a recurring dream about a door | `NPC_KNOWLEDGE_MAP.md` — NPC-carried clue |
| Faction warning | A Warden's warning carved into a post | Faction file / regional clue trail |

None of these require a written prophecy. The AI DM delivers them as atmospheric description or NPC dialogue, then records them as clues discovered (`MYSTERY_STATE_TRACKER_TEMPLATE.md`).

---

## When Prophecy Text Would Be Appropriate

Prophecy text is appropriate only when:
1. A specific authored document exists in the world (a carved tablet, a Concord fragment, a Mourner's old song)
2. The prophecy text is already authored and indexed in a dungeon/ruin or region file
3. The text is deliberately partial, ambiguous, and does not name the apex truth

If a situation calls for in-world prophecy text and none has been authored yet, **improvise sparingly**: use oblique symbolic language (thresholds, doors, emptiness, the weight of names) without explaining the mechanism. Then record the improvised text in the session notes and consider adding it to a canon file.

---

## Mourner Old-Songs (Special Case)

The Mourners' Circle carries fragments of old grief-songs that encode half-remembered truth about the Quietfall. These function as the campaign's closest equivalent to prophecy. They are:
- Player-safe (oblique, poetic)
- Phase-gated (deeper songs only available with faction trust or late-arc access)
- Cross-referenced in `NPC_KNOWLEDGE_MAP.md` (grief-keeper NPCs) and regional clue trail files

The AI DM should treat old-songs as thematic reinforcement, not as literal clues, until a player earns enough trust or context to make the connection.

---

## What NOT To Do

- Do not write a four-stanza prophecy that summarizes the campaign arc
- Do not have an NPC say "the prophecy foretells that the chosen one will..."
- Do not use omen text to explain the harvest mechanism, the Under-Shrine location, or the Hollow Court's identity
- Do not treat omens as mandatory quest triggers

---

## Related Files
- `CLUE_INDEX.md` — concrete clue delivery (DM-only)
- `by_region/` — regional omen/clue trail files
- `NPC_KNOWLEDGE_MAP.md` — NPC-carried omens
- `DISCOVERY_PATHS.md` — how religious/rite-focused play engages with omens
- `REVEAL_TIMING.md` — phase gates for deeper truths
