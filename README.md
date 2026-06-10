# dndcampaignone

A large, predetermined, AI-run solo D&D campaign built in Claude Code. The goal is a deeply authored world — regions, factions, NPCs, quests, mysteries, dungeons — that an AI DM can run for one player from level 1 to level 20 without inventing major content on the fly.

## What This Is

This repository is a campaign engine, not a sourcebook. It has two layers:

- **Predetermined world layer** — authored regions, settlements, factions, NPCs, quests, dungeons, mysteries, and history
- **AI runtime layer** — rules, state files, session protocols, and indexes that let an AI DM run that world reliably across many sessions

The AI DM uses prepared content first and improvises only as much as a skilled human DM would.

## Repository Structure

```text
CLAUDE.md                        ← Claude Code instructions and load order
ai_solo_campaign/
  00_control/                    ← Standards, workflow, tracking, indexes
  01_runner_protocol/            ← AI DM behavior rules and session protocols
  02_runtime_state/              ← Live campaign state (updated every session)
  03_canon/                      ← Authoritative world facts, DM-only and player-safe
  04_world_atlas/                ← World overview and maps
  05_regions/                    ← Region files
  06_settlements/                ← Settlement files
  07_factions/                   ← Faction files and clocks
  08_npcs/                       ← NPC files and indexes
  09_quests/                     ← Quest files, hooks, and rumors
  10_dungeons_and_ruins/         ← Adventure site files
  11_mysteries_and_secrets/      ← Mystery chains, clues, and revelation maps
  12_campaign_arc/               ← Level 1–20 arc and act files
  13_encounters_and_bestiary/    ← Encounter tables and adversary profiles
  14_treasure_and_artifacts/     ← Magic items and reward tables
  15_random_tables/              ← Random tables for travel, weather, events
  16_ai_session_packs/           ← Session start/end prompts and checklists
  17_generation_backlog/         ← Expansion plan and content gaps
  18_audits/                     ← Audit reports
```

## Current Status

Stage 0 (repository setup) is in progress. The instruction and standards layer is complete. World content has not been generated yet.

See [`00_control/PROGRESS_LOG.md`](ai_solo_campaign/00_control/PROGRESS_LOG.md) for current status and [`00_control/TODO.md`](ai_solo_campaign/00_control/TODO.md) for the active work queue once those files exist.

## Development Stages

Defined in [`00_control/DEVELOPMENT_STAGES.md`](ai_solo_campaign/00_control/DEVELOPMENT_STAGES.md).

| Stage | Name | Goal |
|---|---|---|
| 0 | Repository Setup | Folder structure, control files, index placeholders |
| 1 | Campaign Foundation | Premise, factions, NPCs, secrets, starting hooks |
| 2 | AI Runtime Foundation | Session protocols, state files, start/end prompts |
| 3 | Starting Region | Deep region content for 10–20 sessions |
| 4 | First Major City | Political hub with factions, NPCs, quests |
| 5 | Level 1–4 Arc | Fully developed early campaign arc |
| 6 | First Full Audit | AI-readiness and continuity check |
| 7+ | Ongoing Expansion | Regions, factions, quests, mysteries, dungeons |

## Key Control Files

| File | Purpose |
|---|---|
| [`CLAUDE.md`](CLAUDE.md) | Claude Code instructions, load order, non-negotiable rules |
| [`00_control/PROJECT_RULES.md`](ai_solo_campaign/00_control/PROJECT_RULES.md) | Core design philosophy and content scale targets |
| [`00_control/PRODUCTION_WORKFLOW.md`](ai_solo_campaign/00_control/PRODUCTION_WORKFLOW.md) | Per-pass workflow loop |
| [`00_control/DEVELOPMENT_STAGES.md`](ai_solo_campaign/00_control/DEVELOPMENT_STAGES.md) | Full stage-by-stage roadmap |
| [`00_control/TRACKING_SYSTEM.md`](ai_solo_campaign/00_control/TRACKING_SYSTEM.md) | How to use tracking files (TODO, progress log, indexes) |
| [`00_control/CONTENT_STANDARDS.md`](ai_solo_campaign/00_control/CONTENT_STANDARDS.md) | File format and metadata standards |
| [`01_runner_protocol/AI_DM_CORE_RULES.md`](ai_solo_campaign/01_runner_protocol/AI_DM_CORE_RULES.md) | How the AI DM should behave during play |
| [`16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md`](ai_solo_campaign/16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md) | End-of-session state update checklist |

## Recommended Prompts

### Complete Stage 0 (create the folder and file structure)

```
Read CLAUDE.md and the imported project rules. Create the full ai_solo_campaign folder structure and all Stage 0 placeholder files as defined in DEVELOPMENT_STAGES.md and PRODUCTION_WORKFLOW.md. Do not generate world content yet. Update PROGRESS_LOG.md and TODO.md when done.
```

### Complete Stage 1 (generate campaign foundation)

```
Read CLAUDE.md, PROJECT_RULES.md, PRODUCTION_WORKFLOW.md, and DEVELOPMENT_STAGES.md Stage 1. Generate the campaign foundation: original premise, central conflict, hidden truth, level 1–20 escalation model, starting region and settlement, 5–8 major factions, 20 major NPCs, 20 major secrets, 10 campaign clocks, three opening scenes, first 10 hooks, and first 20 rumors. Update canon, indexes, PROGRESS_LOG.md, and TODO.md when done.
```

### Run a continuity and AI-readiness audit

```
Read AUDIT_STANDARDS.md, DEVELOPMENT_STAGES.md, and all relevant content files. Run a full continuity and AI-readiness audit. Do not rewrite major canon. Produce a prioritized gap report in /18_audits and update CONSISTENCY_AUDIT.md, TODO.md, and CONTENT_GAPS.md.
```

### Check project status

```
Read TRACKING_SYSTEM.md, DEVELOPMENT_STAGES.md, PROGRESS_LOG.md, TODO.md, CONTENT_INDEX.md, CONTENT_GAPS.md, and CONSISTENCY_AUDIT.md. Produce a current project status report: current stage, what is complete, what is incomplete, what is blocked, and what to do next. Do not create new campaign content.
```

## Design Principles

- **Predetermined-first.** The AI DM uses authored content before improvising.
- **Original world.** No Forgotten Realms, Eberron, or other copyrighted settings.
- **Solo-play design.** Every encounter, quest, and system is built for one player character.
- **Secrets separated.** DM-only information is never in player-facing files.
- **Everything indexed.** Content that cannot be retrieved is not AI-ready.
- **Factions with agency.** Factions act even when the player ignores them.
- **Mysteries with multiple clue paths.** No one-clue mysteries.

## Build Stages

### Stage 0 — Repository Setup

Create the project structure, placeholder files, control docs, tracking docs, indexes, canon files, and runtime state files. No real campaign creation yet. This is scaffolding.

### Stage 1 — Campaign Foundation

Create the core campaign identity: premise, tone, central conflict, hidden truth, starting region, starting settlement, major factions, major NPCs, secrets, clocks, opening scenes, hooks, rumors, and the first mystery web.

### Stage 2 — AI Runtime Foundation

Make the campaign runnable by an AI DM. This means session loop, state files, start/resume prompts, clue tracking, NPC memory, faction state, world clocks, solo-play rules, and end-of-session update process.

### Stage 3 — Starting Region Deep Build

Expand the starting region so it can support many sessions. Add settlements, wilderness locations, dungeons, NPCs, hooks, quests, local mysteries, faction clocks, rumors, and encounter tables.

### Stage 4 — First Major City Deep Build

Create the first big hub city with districts, politics, shops, temples, guilds, crime, factions, secrets, NPCs, rumors, quests, social scenes, and long-term consequences.

### Stage 5 — Level 1–4 Play Arc

Fully develop the early campaign. This is where the first real playable arc gets built: early main quests, side quests, first dungeon, early villain, first major mystery, faction choices, rewards, and level-up path.

### Stage 6 — First Full Audit

Stop expanding and audit everything so far. Check canon, secrets, mechanics, AI readiness, indexing, solo-play safety, clue paths, faction agency, and state tracking.

### Stage 7 — Regional Expansion Ring 1

Build the regions surrounding the starting area so the player can leave the starting region and still hit prepared content in multiple directions.

### Stage 8 — Faction Deepening

Fully develop the major factions: leaders, members, resources, agendas, clocks, quest chains, secrets, allies, enemies, and reactions to the player.

### Stage 9 — NPC Codex Expansion

Build out the large predetermined NPC library: major NPCs, secondary NPCs, minor NPCs, relationship webs, voice notes, secrets, and locations.

### Stage 10 — Quest Library Expansion

Build the huge quest/hook library: main quests, regional quests, faction quests, personal quests, rumors, jobs, bounties, complications, and travel events.

### Stage 11 — Mystery, Secret, and Clue Expansion

Deepen the mystery structure: secrets, clue index, revelation map, false leads, prophecies, puzzle chains, and multiple clue paths for major truths.

### Stage 12 — Dungeons, Ruins, and Adventure Sites

Create a large library of explorable locations with history, rooms/zones, hazards, puzzles, secrets, treasure, bosses, solo-play options, and consequences.

### Stage 13 — Encounter and Bestiary Expansion

Create solo-friendly threats: monsters, adversary groups, recurring villains, bosses, hazards, random encounters, and noncombat obstacles.

### Stage 14 — Treasure, Artifacts, and Rewards

Create rewards that support solo play and progression: magic items, artifacts, treasure tables, level-appropriate rewards, favors, tools, and survivability options.

### Stage 15 — Level 5–20 Arc Expansion

Fully develop the midgame, high-level, and endgame arcs. This is where Acts 2–5 become playable across levels 5–20.

### Stage 16 — Pre-Play Readiness Audit

Final check before starting actual solo play. Make sure the first 10–20 sessions are ready, secrets are protected, state is initialized, clues work, mechanics are usable, and there are no critical issues.

### Stage 17 — Live Campaign Operation

Actually run the campaign. After each session, update state, clues, NPC memory, factions, consequences, inventory, relationships, and next-session start.

### Stage 18 — Periodic Live Audits

Every few sessions or after major events, audit the live campaign to prevent drift and restore forgotten threads.

### Stage 19 — Campaign Completion and Epilogues

Resolve the endgame, faction outcomes, NPC fates, mysteries, world state, player character epilogue, unresolved threads, and sequel hooks.

### Summary

In practical terms: Stages 0–2 make the machine, Stages 3–5 make the first playable campaign chunk, Stage 6 checks it, and Stages 7–15 scale it into a massive world.
