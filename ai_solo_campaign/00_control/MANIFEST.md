# MANIFEST.md

## Purpose

Master inventory of what this repository is, what it contains, and how it is structured. Updated whenever the project's identity or structure changes materially.

## Current Status

**Stages 0–15B complete. Stage 16 (Pre-Play Readiness Audit + correction pass) complete. Stage 17 (Live Campaign Operation) is next.**

The repository contains full authored systems ready for live solo play:
- **Canon** with player-safe / DM-only separation (Stage 1).
- **AI runtime** protocols and a full runtime-state file set (Stage 2).
- **Starting region** (Sundering Reach, Stage 3) and **first major city** (Caradril, Stage 4).
- **Three Ring 1 adjacent regions** + the **full continent of Orrun** (5 built + 13 placeholder far regions).
- **Seven major factions**, operational with clocks, relationship map, turn rules, and quest chains (Stage 8).
- **NPC codex** — 50 majors plus secondary, minor, and far-continent rosters (Stage 9).
- **Quest library**, **mystery/clue/secret web**, **dungeons and adventure sites** (Stages 10–12.5).
- **Encounter/bestiary** and **treasure/reward/artifact** libraries (Stages 13–14).
- **Level 5–20 arc** — Tiers 2–4, endgame, region/faction escalation, off-route and ignore-arc guides (Stage 15/15B).

**Live play begins via `../16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md`.** For load order during play, see `RETRIEVAL_GUIDE.md`. For the readiness verdict, see `../18_audits/PRE_PLAY_READINESS_AUDIT.md`.

---

## Project Identity

| Field | Value |
|---|---|
| Project type | Large, predetermined, AI-run solo D&D campaign |
| System | D&D 5e / 2024 compatible |
| Play format | One player character, level 1–20 |
| AI DM mode | Predetermined-first, improvise-second |
| World | Original (no copyrighted settings) |
| Current stage | Stages 0–16 complete / Stage 17 (Live Campaign Operation) next |

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
  /12_campaign_arc     — Campaign arc files: Act 1 (L1–4), main arc overview, level 1–20 progression outline. Legacy folder; the current level 5–20 arc authority is /15_campaign_arcs.
  /13_encounters_and_bestiary — Encounter tables and adversary profiles
  /14_treasure_and_artifacts  — Magic items and reward tables
  /15_campaign_arcs    — Level 5–20 arc framework; full-world playability layer; tier paths (Tier 2/3/4); region-to-region transition guide; player-goes-anywhere and ignore-main-arc guides; final revelation and endgame playbooks. Current authority for the level 5–20 arc.
  /15_random_tables    — Random tables for travel, weather, events
  /16_ai_session_packs — Session start/end prompts and checklists
  /17_generation_backlog — Expansion plan and content gaps
  /18_audits           — Audit reports
```

---

## Campaign Identity

> Established and locked in Stage 1. See `../03_canon/CAMPAIGN_IDENTITY_LOCK.md` (DM-only) and `../03_canon/CANON.md`.

- **Campaign name:** The Long Remembering
- **World / continent:** Vael / Orrun
- **Premise:** A century after the order that "kept the dead at peace" fell, death-rites are failing across the ruin-haunted Sundering Reach, and a newcomer is drawn into why the dead will not rest.
- **Central conflict:** Multiple powers race to control the Remembrance — the lingering of the dead as preservable memory.
- **Hidden truth:** DM-only. See `../03_canon/DM_ONLY_CANON.md`. (Do not surface to the player.)
- **Starting region:** The Sundering Reach
- **Starting settlement:** Hollowmere
- **Tone:** Grounded folk-horror frontier fantasy; eerie, moral, hopeful.
- **Themes:** Memory vs. truth; grief and letting go; who owns the dead; renewal after collapse.

---

## Stage Status Summary

See `/00_control/STAGE_STATUS.md` for full status table.

| Stage | Name | Status |
|---|---|---|
| 0 | Repository Setup | complete |
| 1 | Campaign Foundation | complete |
| 2 | AI Runtime Foundation | complete |
| 3 | Starting Region (Sundering Reach) | complete |
| 4 | First Major City (Caradril) | complete |
| 5 | Level 1–4 Play Arc | complete |
| 6 | First Full Audit | complete |
| 7 / 7.5 | Ring 1 + full-continent cartography | complete |
| 8 | Faction Deepening | complete |
| 9 / 9.5 | NPC Codex + far-continent NPCs | complete |
| 10 | Quest Library | complete |
| 11 | Mystery/Clue Expansion | complete |
| 12 / 12.5 | Dungeons + continental sites | complete |
| 13 | Encounter/Bestiary | complete |
| 14 | Treasure/Artifacts | complete |
| 15 / 15B | Level 5–20 Arc + playability fill | complete |
| 16 | Pre-Play Readiness Audit + correction pass | complete |
| 17 | Live Campaign Operation | next |

---

## Related Files

- [`STAGE_STATUS.md`](STAGE_STATUS.md)
- [`PROGRESS_LOG.md`](PROGRESS_LOG.md)
- [`TODO.md`](TODO.md)
- [`DEVELOPMENT_STAGES.md`](DEVELOPMENT_STAGES.md)
- [`TRACKING_SYSTEM.md`](TRACKING_SYSTEM.md)
