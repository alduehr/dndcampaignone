# STATE_UPDATE_TEMPLATE.md

## Purpose

A copy-paste template for updating all runtime state files at session end. Ensures consistent structure and prevents omissions. Use alongside `SESSION_END_UPDATE_CHECKLIST.md`.

## Current Status

**Ready (Stage 2).** Use this template at every session end alongside `SESSION_END_UPDATE_CHECKLIST.md` and `../01_runner_protocol/SESSION_END_PROTOCOL.md`. Keep DM-only content out of player-safe state files (`SESSION_RECAP.md`, `KNOWN_CLUES.md`, `PLAYER_CHARACTER.md`, etc.).

---

## How To Use

At session end, copy this template. Fill in each section based on what happened in the session. Then paste the relevant portions into the appropriate runtime state files.

---

## Session State Update Template

```md
## Session [N] State Update — [Date]

### CURRENT_STATE.md
- In-world date/time:
- Current location:
- Scene status:
- Player condition:
- Immediate danger:
- Current objective:
- Active companions:
- Last important action:
- Next likely scene:

### PLAYER_CHARACTER.md changes
- Level change: (yes/no — new level if yes)
- HP change:
- Spell slots/resources:
- Equipment gained/lost:
- Conditions:
- Exhaustion:
- Lingering injuries:

### CURRENT_LOCATION.md
- Location:
- Sub-location:
- Time of day:
- Weather:
- Who is present:
- Recent changes to location:

### ACTIVE_QUESTS.md changes
- Quest updated:
  - New status:
  - Completed objectives:
  - New information:
  - Next steps:
- Quest updated:
  - ...

### OPEN_THREADS.md additions
- New thread:
  - Type:
  - What the player knows:
  - How it could resolve:

### KNOWN_CLUES.md additions
- Clue discovered:
  - What the player found:
  - What they interpreted:
  - Mystery it feeds:

### HIDDEN_CLUES.md changes
- Clue missed (if applicable):
- Clue status changed:

### NPC_MEMORY.md updates
- NPC:
  - Attitude change:
  - Interaction summary:
  - Promises/debts/lies:

### FACTION_STATE.md updates
- Faction:
  - Attitude change:
  - Activity update:
  - Clock change:

### WORLD_CLOCKS.md updates
- Clock advanced:
  - New stage:
  - Trigger:

### INVENTORY_AND_REWARDS.md changes
- Items gained:
- Items lost:
- Currency change:
- Favors gained/spent:

### RELATIONSHIPS.md changes
- Relationship changed:
  - New quality:
  - Reason:

### CONSEQUENCES.md additions
- New consequence:
  - Type:
  - Origin:
  - Player knows: yes/no
  - When manifests:

### SESSION_RECAP.md entry
- What happened:
- What player learned:
- What changed:
- Choices that mattered:
- Unresolved:

### NEXT_SESSION_START.md
- Opening scene description:
- Files to load:
- Hidden DM notes:
- What not to reveal yet:

### Canon updates needed
- New fact for CANON.md:
- New player-safe fact for PLAYER_SAFE_CANON.md:
- New DM-only fact for DM_ONLY_CANON.md:

### Index updates needed
- New content to add to CONTENT_INDEX.md:
- New tags to add to TAG_INDEX.md:
```

---

## Related Files

- [`SESSION_END_UPDATE_CHECKLIST.md`](SESSION_END_UPDATE_CHECKLIST.md)
- [`../02_runtime_state/`](../02_runtime_state/)
