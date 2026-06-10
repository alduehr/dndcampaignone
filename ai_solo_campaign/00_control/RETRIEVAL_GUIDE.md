# RETRIEVAL_GUIDE.md

## Purpose

Tells the AI DM which files to load, when to load them, and how to use them. This is the navigation layer for the campaign repository.

## Current Status

Stages 1, 2, and 3 complete. Session load order, contextual load rules, pre-content-generation checks, and secrecy enforcement are operational. Sundering Reach world content load entries are live below.

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

## Stage 3 World Content Load Entries (Sundering Reach)

These files exist and are loadable as of Stage 3. Always load the minimum needed for the current scene.

### Region
- `05_regions/SUNDERING_REACH.md` — full region overview; load when entering a new zone or for travel context

### Settlements
- `06_settlements/HOLLOWMERE.md` — starting town; load every session set here
- `06_settlements/KETTLE_BRIDGE.md` — eastern toll-town
- `06_settlements/SALTMARGIN.md` — western salt-trade town
- `06_settlements/CANDLEWICK.md` — southern village; Concord Script clue gate
- `06_settlements/GREYWATER_HOLM.md` — fen-edge village; cult spread
- `06_settlements/HARROWGAST.md` — heights mining village; Deep Adit entrance
- `06_settlements/REEDFORD.md` — central ford hamlet; low-danger waypoint
- `06_settlements/THE_ASHWALK_REST.md` — Warden waystation; solo-safety sanctuary

### Wilderness Zones
- `05_regions/wilderness/GREYFENS_SITES.md` — fen sites; Gravecaller activity
- `05_regions/wilderness/SUNDER_HEIGHTS_SITES.md` — highlands; old glass; Remnant race
- `05_regions/wilderness/MIREWEND_AND_ROADS_SITES.md` — river and Concord road sites; travel layer
- `05_regions/wilderness/BASIN_SHORE_AND_HOLMS_SITES.md` — basin shore; deep basin gated to endgame

### Dungeons / Ruins
- `10_dungeons_and_ruins/THE_PEAT_CHAPEL.md` — intended first delve; level 1–2
- `10_dungeons_and_ruins/THE_SUNKEN_TOLLHOUSE.md` — river node; level 2–3
- `10_dungeons_and_ruins/THE_WHISPERING_CAIRN.md` — Concord Script gate; level 2–3
- `10_dungeons_and_ruins/THE_LEDGER_VAULT.md` — social/stealth heist in Hollowmere; level 2–4
- `10_dungeons_and_ruins/THE_BARROW_OF_NINE_DOORS.md` — parley-boss barrow; level 3–5
- `10_dungeons_and_ruins/THE_DEEP_ADIT.md` — harvest node; level 4–6; thin-touch risk

### NPCs
- `08_npcs/MAJOR_NPCS.md` — 20 full-profile major NPCs; load when relevant NPC is present
- `08_npcs/SECONDARY_NPCS.md` — ~21 secondary NPCs; load by location
- `08_npcs/MINOR_NPCS.md` — ~35 minor NPCs; load by settlement
- `08_npcs/NPC_INDEX.md` — master lookup table

### Quests
- `09_quests/HOOKS_TABLE.md` — first 10 hooks (Hook 1 = default opener)
- `09_quests/RUMORS_TABLE.md` — first 20 rumors
- `09_quests/hooks_and_rumors/SUNDERING_REACH_HOOKS.md` — hooks H11–H39
- `09_quests/hooks_and_rumors/SUNDERING_REACH_RUMORS.md` — rumors R21–R50
- `09_quests/regional_quests/Q_*.md` — 14 developed quests; load when quest is active

### Encounters
- `13_encounters_and_bestiary/SUNDERING_REACH_ENCOUNTERS.md` — 4 solo-tuned zone tables; load during travel or wilderness scenes

### Clues / Mysteries
- `11_mysteries_and_secrets/CLUE_INDEX.md` — all authored clues with locations and methods (DM-only)
- `02_runtime_state/HIDDEN_CLUES.md` — runtime mirror; tracks discovery status (DM-only)
- `11_mysteries_and_secrets/MYSTERY_WEB.md` — full mystery network (DM-only)

### Factions
- `07_factions/major_factions/` — load relevant faction file when faction is active in current scene
- `07_factions/FACTION_INDEX.md` — master table and relationship map

---

## Related Files

- [`CONTENT_INDEX.md`](CONTENT_INDEX.md)
- [`TAG_INDEX.md`](TAG_INDEX.md)
- [`01_runner_protocol/AI_DM_CORE_RULES.md`](../01_runner_protocol/AI_DM_CORE_RULES.md)
