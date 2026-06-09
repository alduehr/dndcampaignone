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
