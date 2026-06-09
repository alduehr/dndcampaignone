# AUDIT_STANDARDS.md

## Purpose

Use this file when auditing the campaign for:
- Canon consistency
- Secret separation
- AI-readiness
- Retrieval quality
- Missing indexes
- Orphaned content
- Solo-play problems
- Mystery solvability
- Quest usability
- Faction agency
- State tracking gaps

Run audits regularly, especially before major expansion passes.

---

## Audit Categories

### 1. Canon Consistency
Check:
- Contradictory facts
- Duplicate names
- Conflicting timelines
- Conflicting geography
- Changed faction motives
- NPCs in two places at once
- Unrecorded canon

### 2. Secret Separation
Check:
- DM-only truth in player-safe files
- Future spoilers in player-facing summaries
- Hidden faction motives exposed incorrectly
- Mystery answers in player-facing indexes
- Resume prompts that reveal secrets

### 3. Retrieval Quality
Check:
- Missing metadata blocks
- Missing tags
- Weak summaries
- Missing “AI Use” sections
- Missing cross-links
- Unclear secrecy levels

### 4. NPC Connectivity
Check:
- NPCs with no location
- NPCs with no motive
- NPCs with no play function
- NPCs not in NPC_INDEX
- Major NPCs without secrets or relationships
- NPCs tied to missing factions/quests

### 5. Quest Usability
Check:
- Quests with no hook
- Quests with only one solution
- Quests with no consequence
- Quests with no failure state
- Quests not linked to locations/NPCs/factions
- Quests that assume a four-person party

### 6. Mystery Solvability
Check:
- Mysteries with fewer than three clue paths
- Clues with no discovery location
- Clues that are too vague
- False leads with no payoff
- Required clues hidden behind one failed roll
- Hidden truths invented but not indexed

### 7. Faction Agency
Check:
- Factions with no current activity
- Factions with no clock
- Factions with no named members
- Factions with no resources
- Factions that do nothing if ignored
- Faction relationships missing from relationship map

### 8. Solo-Play Safety
Check:
- Encounters assuming four PCs
- No retreat route
- No warning before overwhelming danger
- No noncombat approach
- Bosses with no foreshadowing
- Failure states that abruptly end the campaign

### 9. State Tracking
Check:
- State files missing fields
- Quests with no state update instructions
- NPC interactions not reflected in NPC_MEMORY
- Faction moves not reflected in FACTION_STATE
- Clues not reflected in KNOWN_CLUES or HIDDEN_CLUES
- Consequences not reflected in CONSEQUENCES

### 10. Index Completeness
Check:
- New files missing from CONTENT_INDEX
- Tags missing from TAG_INDEX
- NPCs missing from NPC_INDEX
- Quests missing from QUEST_INDEX
- Factions missing from FACTION_INDEX
- Clues missing from CLUE_INDEX
- Dungeons missing from DUNGEON_INDEX

---

## Severity Levels

Use these severity levels:

### Critical
Breaks campaign continuity, exposes major secrets, or makes the campaign impossible to run.

### High
Likely to confuse the AI DM or player, or seriously weaken a major arc.

### Medium
Weakens usability, retrieval, or play quality.

### Low
Polish issue.

---

## Audit Report Format

```md
# Audit Report: [Name]

## Scope
Files/folders reviewed.

## Summary
Short summary of overall health.

## Critical Findings
| Issue | File(s) | Why It Matters | Recommended Fix |
|---|---|---|---|

## High Findings
| Issue | File(s) | Why It Matters | Recommended Fix |
|---|---|---|---|

## Medium Findings
| Issue | File(s) | Why It Matters | Recommended Fix |
|---|---|---|---|

## Low Findings
| Issue | File(s) | Why It Matters | Recommended Fix |
|---|---|---|---|

## Orphaned Content

## Missing Index Entries

## Exposed Secrets

## Solo-Play Risks

## Mystery/Clue Risks

## Recommended Fix Order
1. ...
2. ...
3. ...
```

---

## Audit Rules

Do not silently rewrite major canon during an audit unless explicitly asked.

Small cleanup is fine if requested:
- Missing tags
- Broken links
- Index omissions
- Formatting issues

Major issues should be reported first:
- Canon contradictions
- Exposed secrets
- Broken mystery logic
- Major quest rewrites
- Faction motive conflicts

---

## Audit Timing

Run an audit:
- After Phase 1
- After any major region expansion
- After any major city expansion
- After any level-tier arc expansion
- Before beginning actual solo play
- After several play sessions
- Whenever canon feels unstable
