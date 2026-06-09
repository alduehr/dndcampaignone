# MANIFEST.md

## Purpose

Master inventory of what this repository is, what it contains, and how it is structured. Updated whenever the project's identity or structure changes materially.

## Current Status

**Stage 0 — Repository Setup.** Scaffold created. No campaign world content exists yet.

---

## Project Identity

| Field | Value |
|---|---|
| Project type | Large, predetermined, AI-run solo D&D campaign |
| System | D&D 5e / 2024 compatible |
| Play format | One player character, level 1–20 |
| AI DM mode | Predetermined-first, improvise-second |
| World | Original (no copyrighted settings) |
| Current stage | Stage 0 complete / Stage 1 not started |

---

## Repository Layers

### Layer 1 — Predetermined World
All authored content: regions, settlements, factions, NPCs, quests, dungeons, mysteries, history, cosmology.

### Layer 2 — AI Runtime
Rules, protocols, state tracking, session start/end procedures, indexes, and retrieval systems.

---

## Folder Map

```text
/ai_solo_campaign
  /00_control          — Standards, workflow, tracking, indexes, manifest
  /01_runner_protocol  — AI DM behavior rules and session protocols
  /02_runtime_state    — Live campaign state (updated each session)
  /03_canon            — Authoritative world facts, separated by secrecy
  /04_world_atlas      — World overview and map descriptions
  /05_regions          — Region files
  /06_settlements      — Settlement files
  /07_factions         — Faction files and clocks
  /08_npcs             — NPC files and indexes
  /09_quests           — Quest files, hooks, and rumors
  /10_dungeons_and_ruins    — Adventure site files
  /11_mysteries_and_secrets — Mystery chains, clues, revelation maps
  /12_campaign_arc     — Level 1–20 arc and act files
  /13_encounters_and_bestiary — Encounter tables and adversary profiles
  /14_treasure_and_artifacts  — Magic items and reward tables
  /15_random_tables    — Random tables for travel, weather, events
  /16_ai_session_packs — Session start/end prompts and checklists
  /17_generation_backlog — Expansion plan and content gaps
  /18_audits           — Audit reports
```

---

## Campaign Identity

> Not yet established. To be filled in during Stage 1.

- **Campaign name:** TBD
- **Premise:** TBD
- **Central conflict:** TBD
- **Hidden truth:** TBD (DM-only)
- **Starting region:** TBD
- **Starting settlement:** TBD
- **Tone:** TBD
- **Themes:** TBD

---

## Stage Status Summary

See `/00_control/STAGE_STATUS.md` for full status table.

| Stage | Name | Status |
|---|---|---|
| 0 | Repository Setup | complete (with Stage 0 cleanup pass 2026-06-09) |
| 1 | Campaign Foundation | not started |
| 2 | AI Runtime Foundation | not started |
| 3 | Starting Region | not started |
| 4+ | Expansion | not started |

---

## Related Files

- [`STAGE_STATUS.md`](STAGE_STATUS.md)
- [`PROGRESS_LOG.md`](PROGRESS_LOG.md)
- [`TODO.md`](TODO.md)
- [`DEVELOPMENT_STAGES.md`](DEVELOPMENT_STAGES.md)
- [`TRACKING_SYSTEM.md`](TRACKING_SYSTEM.md)
