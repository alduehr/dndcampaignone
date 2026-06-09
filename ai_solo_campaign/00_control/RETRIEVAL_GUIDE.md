# RETRIEVAL_GUIDE.md

## Purpose

Tells the AI DM which files to load, when to load them, and how to use them. This is the navigation layer for the campaign repository.

## Current Status

Stage 0 scaffold. Load priorities for world content will be added as content is created. Runtime and control file priorities are established here.

---

## Core Principle

**Load only what you need.** Loading everything at once wastes context. Use this guide to load the minimum necessary files for the current scene, then expand if needed.

---

## Session Start Load Order

When starting or resuming a session, load in this order:

1. `02_runtime_state/CURRENT_STATE.md` — where things stand right now
2. `02_runtime_state/CURRENT_LOCATION.md` — where the player is
3. `02_runtime_state/CURRENT_SCENE.md` — what is happening
4. `02_runtime_state/PLAYER_CHARACTER.md` — player stats, resources, condition
5. `02_runtime_state/ACTIVE_QUESTS.md` — live quests
6. `02_runtime_state/NPC_MEMORY.md` — relevant NPC attitudes
7. `02_runtime_state/FACTION_STATE.md` — faction positions
8. `02_runtime_state/WORLD_CLOCKS.md` — escalating threats
9. `16_ai_session_packs/RESUME_CAMPAIGN_PROMPT.md` — session opening guidance

Then load relevant world files based on current location, active quests, and NPCs present.

---

## New Campaign Start Load Order

When beginning a brand-new campaign:

1. `03_canon/CANON.md`
2. `03_canon/PLAYER_SAFE_CANON.md`
3. `03_canon/DM_ONLY_CANON.md`
4. `12_campaign_arc/MAIN_ARC_OVERVIEW.md`
5. `02_runtime_state/PLAYER_CHARACTER.md`
6. Relevant starting region file
7. Relevant starting settlement file
8. `16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md`

---

## Contextual Load Rules

### When in a settlement
Load:
- Settlement file
- Region file (if not already loaded)
- NPCs present at current location
- Active quests relevant to this settlement
- Faction state for factions active here

### When in a dungeon or ruin
Load:
- Dungeon/ruin file
- Quest file(s) pointing here
- Any relevant clues or mysteries
- Encounter context for current zone

### When in wilderness or travel
Load:
- Region file
- Travel protocol: `01_runner_protocol/TRAVEL_PROTOCOL.md`
- Relevant encounter table
- Any travel events or faction activity in this zone

### When in a social scene
Load:
- NPC file(s) for present NPCs
- Faction file if faction politics are at stake
- Relevant quest file if the scene advances a quest
- `01_runner_protocol/SOCIAL_SCENE_PROTOCOL.md`

### When delivering a clue
Load:
- Relevant clue file
- Mystery file the clue feeds into
- `02_runtime_state/KNOWN_CLUES.md` to check what the player already knows
- `01_runner_protocol/CLUE_DELIVERY_PROTOCOL.md`

### When a secret is about to be revealed
Load:
- `03_canon/DM_ONLY_CANON.md` — check what is still hidden
- `02_runtime_state/KNOWN_CLUES.md` — check discovery trail
- `01_runner_protocol/SECRET_REVEAL_PROTOCOL.md`

### At session end
Load:
- `16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md`
- All runtime state files that changed this session

---

## Pre-Content-Generation Checks

Before creating any major new content (NPCs, factions, regions, quests, mysteries, monsters, artifacts), check these files first:

| File | What To Check |
|---|---|
| `00_control/CANON_AUTHORITY.md` | Which file wins if there's a contradiction |
| `00_control/GENERATION_GUARDRAILS.md` | Drift prevention — does this new content fit the project? |
| `00_control/NAMING_REGISTRY.md` | Is this name already taken or forbidden? |
| `00_control/RULESET_ASSUMPTIONS.md` | Are mechanics consistent with D&D 5e / 2024? |
| `00_control/DND_MECHANICS_REQUIREMENTS.md` | Does this content meet mechanical completeness requirements? |
| `03_canon/CANON.md` | Does this contradict established canon? |

These checks take seconds and prevent large-scale rework later.

---

## File Priority Levels

| Priority | Meaning | Examples |
|---|---|---|
| Always load | Required for any session | CURRENT_STATE, PLAYER_CHARACTER, CURRENT_LOCATION |
| Load on demand | Load when relevant | NPC files, quest files, dungeon files |
| Load for secrets | DM-only; never surface to player | DM_ONLY_CANON, HIDDEN_CLUES, mystery files |
| Reference only | Load to check standards, not during play | Standards files, AUDIT_STANDARDS |

---

## Secrecy Enforcement

**Never load DM-only files and then summarize their contents to the player.**

- `secrecy:dm-only` files are for AI DM reasoning only.
- `secrecy:player-safe` files can be paraphrased, quoted, or described to the player.
- `secrecy:mixed` files require care — read the individual sections before using.

---

## Files That Will Exist After Stage 1

*To be filled in after Stage 1 content generation.*

- Campaign overview: `03_canon/CANON.md`
- Hidden truth: `03_canon/DM_ONLY_CANON.md`
- Starting region: `05_regions/[name].md`
- Starting settlement: `06_settlements/[name].md`
- Major factions: `07_factions/major_factions/[name].md`
- Major NPCs: `08_npcs/[name].md`
- Main arc overview: `12_campaign_arc/MAIN_ARC_OVERVIEW.md`
- Mystery web: `11_mysteries_and_secrets/MYSTERY_WEB.md`

---

## Related Files

- [`CONTENT_INDEX.md`](CONTENT_INDEX.md)
- [`TAG_INDEX.md`](TAG_INDEX.md)
- [`01_runner_protocol/AI_DM_CORE_RULES.md`](../01_runner_protocol/AI_DM_CORE_RULES.md)
