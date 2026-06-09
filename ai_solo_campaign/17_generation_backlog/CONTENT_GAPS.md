# CONTENT_GAPS.md

## Purpose

Track missing or underdeveloped content by category. Use this for category-level gaps. Use `TODO.md` for actionable tasks. Use `CONSISTENCY_AUDIT.md` for defects or contradictions.

## Current Status

Stage 0 scaffold. All gaps below reflect the complete absence of Stage 1+ world content.

---

## Regions

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| No regions exist | Critical | Campaign cannot be played | Generate starting region during Stage 3 | 3 |
| No adjacent regions | High | World feels bounded | Generate Ring 1 regions during Stage 7 | 7 |

---

## Settlements

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| No settlements exist | Critical | Player has nowhere to go | Generate starting settlement during Stage 1 | 1 |
| No major city | High | Mid-game hub missing | Generate first city during Stage 4 | 4 |

---

## Factions

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| No factions exist | Critical | No political tension or AI clock pressure | Generate 5–8 major factions during Stage 1 | 1 |
| No faction clocks | High | Factions are passive | Add clocks during Stages 1 and 8 | 1, 8 |

---

## NPCs

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| No NPCs exist | Critical | AI DM must invent everyone | Generate 20 major NPCs during Stage 1 | 1 |
| No secondary NPCs | High | Settlements feel empty | Generate 50–100 secondary NPCs during Stage 3 | 3, 9 |
| No minor NPC tables | Medium | Local color missing | Add minor NPCs during Stage 9 | 9 |

---

## Quests

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| No quests exist | Critical | Player has nothing to do | Generate 10 hooks during Stage 1 | 1 |
| No main campaign quests | Critical | Level 1–4 arc missing | Generate arc quests during Stage 5 | 5 |
| No failure states | High | Player choices have no teeth | Add failure states to all major quests | 5, 10 |

---

## Mysteries and Clues

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| No mysteries exist | Critical | Campaign lacks depth | Generate mystery web during Stage 1 | 1 |
| No clue trails | Critical | Mysteries unsolvable | Generate clue paths during Stage 11 | 1, 11 |
| No revelation map | High | AI DM doesn't know what to reveal when | Generate revelation map during Stage 1 | 1 |

---

## Dungeons and Ruins

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| No dungeons exist | High | No adventure sites | Generate 5–8 dungeons during Stage 3 | 3, 12 |
| No first major dungeon | High | Level 1–4 arc incomplete | Generate first dungeon during Stage 5 | 5 |

---

## AI Runtime

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| No session start prompt | Critical | AI DM has no entry point | Create `START_NEW_CAMPAIGN_PROMPT.md` during Stage 2 | 2 |
| No resume prompt | Critical | AI DM cannot resume cleanly | Create `RESUME_CAMPAIGN_PROMPT.md` during Stage 2 | 2 |
| Runtime state files are empty | Critical | AI DM has no current state | Populate after Stage 1 + character creation | 2 |
| No solo play protocols | High | AI DM may default to party-play assumptions | Fill all `01_runner_protocol/` files during Stage 2 | 2 |
| No compact context template | High | Long campaigns will overflow context | Create `COMPACT_CONTEXT_TEMPLATE.md` during Stage 2 | 2 |

---

## Campaign Arc

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| No main arc exists | Critical | No campaign direction | Generate arc overview during Stage 1 | 1 |
| No level 5–20 acts | High | Campaign ends at level 4 | Generate remaining acts during Stage 15 | 15 |
| No villain escalation | High | Antagonist pressure absent | Create villain escalation file during Stage 15 | 15 |
