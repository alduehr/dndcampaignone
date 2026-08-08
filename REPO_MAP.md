# REPO_MAP.md

## Purpose

This is the **single authoritative map of this repository's structure** — every top-level folder and file, what it's for, and where to go next. It exists so nobody (human or AI) has to reverse-engineer the layout from scratch, and so the layout doesn't quietly drift as the project grows.

**Governance rule:** this file is the source of truth for top-level structure. Any commit that adds, removes, renames, or moves a top-level folder or file must update this file in the same commit. `CLAUDE.md`'s "Repository Shape" and `README.md`'s "Repository Structure" carry short summaries for their own audiences (Claude Code instructions; public-facing readme) but **defer to this file for the complete, current picture** — if they ever disagree with this file, this file wins and the others are stale.

---

## Top-Level Structure

```text
/dndcampaignone
  CLAUDE.md                ← Claude Code instructions, load order, non-negotiable rules (start here in-session)
  README.md                ← Public-facing project overview and recommended prompts
  ONBOARDING.md             ← How this repo onboards into the separate DungeonMaster app
  REPO_MAP.md              ← This file — the authoritative structure map
  dm.campaign.json          ← DungeonMaster app onboarding manifest (machine-read; see ONBOARDING.md)
  .gitignore
  .claude/
    agents/                ← Specialist subagent definitions (tracked; see below)
  ai_solo_campaign/         ← THE campaign engine — authoritative, secret-bearing, wired to play. See below.
  Locations/
    Orrun/                 ← Spoiler-free world-reference library, derived from the campaign. See below.
  one_shots/                ← Standalone non-canon one-shot adventures, deliberately disconnected. See below.
```

---

## The Three Content Trees

This repo holds **three separate content trees** with different purposes, different authority levels, and different secrecy rules. Knowing which one you're in changes what you're allowed to assume.

| Tree | Purpose | Canon authority | Secrets | Onboarded to DungeonMaster app? |
|---|---|---|---|---|
| `ai_solo_campaign/` | Runs "The Long Remembering," the one predetermined solo campaign this repo exists for | **Authoritative** — the source of truth for everything campaign-related | Contains DM-only truths, hidden faction agendas, mystery answers | Yes — `dm.campaign.json`'s `contentRoot` |
| `Locations/Orrun/` | General-purpose, spoiler-free reference library for the world of Orrun/Vael — geography, settlements, culture, generic bestiary — reusable outside the campaign | Derived/curated from campaign canon; **not** a second source of truth. If it ever disagrees with `ai_solo_campaign` on a plain geography/culture fact, `ai_solo_campaign` wins | None — deliberately contains no hidden-truth material, no faction secrets, no campaign quest hooks | No — outside `contentRoot` |
| `one_shots/` | Standalone, non-canon one-shot adventures set in the world of Orrun but deliberately disconnected from the campaign's canon, factions, mystery web, and NPCs | Not campaign canon at all; invents its own disposable cast, never uses registered campaign names | N/A — nothing here is a secret because nothing here is real to the campaign | No — outside `contentRoot`, not referenced by any campaign index |

**Practical rule of thumb:** if you're running or writing *the campaign*, you're in `ai_solo_campaign/`. If you need a spoiler-free fact about the world for a one-shot, an NPC walk-on, or a different game entirely, go to `Locations/Orrun/`. If you want a fun, disposable session with no continuity obligations, go to `one_shots/`.

---

## `ai_solo_campaign/` — The Campaign Engine

Full folder-by-folder detail lives in [`ai_solo_campaign/00_control/RETRIEVAL_GUIDE.md`](ai_solo_campaign/00_control/RETRIEVAL_GUIDE.md) (what to load for a given in-play situation) and [`ai_solo_campaign/00_control/CONTENT_INDEX.md`](ai_solo_campaign/00_control/CONTENT_INDEX.md) (every file, indexed). Summary:

```text
ai_solo_campaign/
  00_control/               ← Standards, workflow, tracking, indexes, canon authority, naming registry — read first
  01_runner_protocol/        ← AI DM behavior rules: session loop, combat/social/travel protocols, roll policy
  02_runtime_state/          ← LIVE campaign state — updated every session (current location, quests, clues, NPC memory, clocks...)
  03_canon/                 ← Authoritative world facts, split player-safe / DM-only
  04_world_atlas/            ← World overview, map descriptions, full-world/full-continent cartography authority
  05_regions/                ← Region files (16) + wilderness/ subfolder (named sites, hazards, DCs)
  06_settlements/            ← Settlement files, caradril_districts/, settlement_map_packets/, city_map_packets/
  07_factions/               ← major_factions/, minor_factions/, relationship map, turn rules
  08_npcs/                  ← Major/secondary/minor NPC files, by_region/ rosters, indexes
  09_quests/                 ← Quest files, hooks_and_rumors/, by_region/ quest sets
  10_dungeons_and_ruins/      ← Adventure site files (dungeon mechanical standard: zones, hazards, boss mechanics)
  11_mysteries_and_secrets/   ← Mystery chains, clue index, revelation map, false leads
  12_campaign_arc/           ← Main arc overview, level 1-20 progression
  13_encounters_and_bestiary/ ← Encounter tables, adversary profiles, monster index
  14_treasure_and_artifacts/  ← Magic items, artifacts, reward-by-level tables
  15_campaign_arcs/           ← Level 5-20 arc: tier overviews, escalation, endgame, playable paths
  15_random_tables/           ← Random tables for travel, weather, events (shares the "15" prefix with 15_campaign_arcs on purpose — historical numbering, not a duplicate; see CLAUDE.md)
  16_ai_session_packs/        ← Session start/end prompts, state update checklist, resume templates
  17_generation_backlog/      ← Expansion plan, content gaps
  18_audits/                 ← Formal audit reports
  maps/                     ← Maps manifest + image assets — AUTHORITATIVE copy (wired into dm.campaign.json's contentRoot)
  skills/                   ← DungeonMaster app skills overlay (mandatory DM-procedure files: canon-and-gaps, combat, procedures)
```

Read order for most work: `CLAUDE.md` → `00_control/PROJECT_RULES.md` → `00_control/CANON_AUTHORITY.md` → `00_control/GENERATION_GUARDRAILS.md` → the relevant specialist standards file (`WORLDBUILDING_STANDARDS.md`, `NPC_STANDARDS.md`, `QUEST_STANDARDS.md`, etc.) → `00_control/RETRIEVAL_GUIDE.md` for what to load for the task at hand.

---

## `Locations/Orrun/` — World Reference Library

Full detail lives in [`Locations/Orrun/README.md`](Locations/Orrun/README.md) (relationship to the campaign, maintenance rules) and [`Locations/Orrun/00_overview/GAZETTEER_INDEX.md`](Locations/Orrun/00_overview/GAZETTEER_INDEX.md) (every file, indexed). Summary:

```text
Locations/Orrun/
  README.md                ← What this folder is, how it relates to ai_solo_campaign/, maintenance rules
  00_overview/               ← World summary, gazetteer index, audits — start here
  01_geography/              ← Continent overview, travel routes, regions/ (16 files), wilderness/ (7 zones)
  02_settlements/            ← Cities/towns/villages, grouped by region, public-facing only
  03_culture/                ← Calendar, cosmology (public), gods and faiths, languages, public world history
  04_bestiary/               ← Generic wandering monsters and hazards by terrain — no campaign secrets
  05_timelines/               ← The Unmade: alternate-timeline cosmology, including the Last Telling
  06_sites/                  ← 34 ruins/adventure sites as physical places (approach, layout, hazards, salvage) — no plot attached
  maps/                     ← MIRROR of ai_solo_campaign/maps/ — not authoritative, update the campaign copy first
```

Every content file here is `secrecy: player-safe`. If you're writing new Orrun content, it must stay spoiler-free with respect to the campaign's central mystery — no hidden-truth material, no faction agendas, no campaign quest hooks, no current officeholders named (describe the office, not who holds it, so the library doesn't go stale as campaign play changes hands).

---

## `one_shots/` — Standalone Non-Canon Adventures

Full detail lives in [`one_shots/README.md`](one_shots/README.md). Each one-shot is its own subfolder (currently `widdershin_cave/`, `the_ell_at_marchwell/`) with its own self-contained files (premise, characters, room tables, DM screen, map spec, rewards). Deliberately outside `dm.campaign.json`'s `contentRoot` and outside every campaign index — nothing here is pulled into a live campaign session or checked against `NAMING_REGISTRY.md`.

---

## Root-Level Files

| File | Purpose |
|---|---|
| [`CLAUDE.md`](CLAUDE.md) | Claude Code's project instructions: prime directive, non-negotiable rules, hard constraints, core files to read first, specialist agent table |
| [`README.md`](README.md) | Public-facing overview: what this is, current status, development stages, key control files, recommended prompts |
| [`ONBOARDING.md`](ONBOARDING.md) | How this repo onboards into the separate DungeonMaster app (cloud AI DM server + phone app) |
| [`REPO_MAP.md`](REPO_MAP.md) | This file |
| [`dm.campaign.json`](dm.campaign.json) | Machine-read DungeonMaster onboarding manifest: `contentRoot`, player-safe path globs |

## `.claude/agents/`

Eleven specialist subagent definitions, tracked in version control (everything else under `.claude/` is local session data and gitignored). One agent per content domain: `campaign-architect`, `ai-dm-runtime-engineer`, `canon-continuity-auditor`, `world-atlas-builder`, `faction-weaver`, `npc-codex-builder`, `quest-arc-designer`, `mystery-clue-engineer`, `encounter-bestiary-designer`, `indexer-librarian`, `player-experience-reviewer`. Full descriptions in `CLAUDE.md`'s Specialist Agents table.

---

## Find It Fast

| I want to... | Go to |
|---|---|
| Start or resume a play session | `ai_solo_campaign/16_ai_session_packs/` |
| Check what state the campaign is in right now | `ai_solo_campaign/02_runtime_state/CURRENT_STATE.md` |
| Find a rule for how the AI DM should behave | `ai_solo_campaign/01_runner_protocol/` |
| Look up a region, settlement, dungeon, NPC, faction, or quest | `ai_solo_campaign/00_control/CONTENT_INDEX.md` or `RETRIEVAL_GUIDE.md` |
| Check what canon says about something | `ai_solo_campaign/03_canon/CANON.md` (or `PLAYER_SAFE_CANON.md` / `DM_ONLY_CANON.md`) |
| See the campaign's current production status / stage | `ai_solo_campaign/00_control/STAGE_STATUS.md`, `PROGRESS_LOG.md`, `TODO.md` |
| Check a proper noun for naming collisions before creating content | `ai_solo_campaign/00_control/NAMING_REGISTRY.md` |
| Resolve a contradiction between files | `ai_solo_campaign/00_control/CANON_AUTHORITY.md` |
| Get a spoiler-free fact about Orrun's geography/culture for reuse elsewhere | `Locations/Orrun/00_overview/GAZETTEER_INDEX.md` |
| Run a quick, disposable session with no continuity obligations | `one_shots/README.md` |
| Understand how this repo plugs into the DungeonMaster app | `ONBOARDING.md` + `dm.campaign.json` |
| Find the map assets and manifest | `ai_solo_campaign/maps/` (authoritative) — `Locations/Orrun/maps/` is a read-only mirror |
| Find a specialist subagent for a production pass | `.claude/agents/` (table also in `CLAUDE.md`) |

---

## Related Files

- [`CLAUDE.md`](CLAUDE.md) — Claude Code instructions and load order
- [`README.md`](README.md) — public overview and recommended prompts
- [`ai_solo_campaign/00_control/RETRIEVAL_GUIDE.md`](ai_solo_campaign/00_control/RETRIEVAL_GUIDE.md) — situational load guide for campaign play
- [`ai_solo_campaign/00_control/CONTENT_INDEX.md`](ai_solo_campaign/00_control/CONTENT_INDEX.md) — full campaign file inventory
- [`Locations/Orrun/README.md`](Locations/Orrun/README.md) — Orrun library's own scope and rules
- [`Locations/Orrun/00_overview/GAZETTEER_INDEX.md`](Locations/Orrun/00_overview/GAZETTEER_INDEX.md) — full Orrun file inventory
- [`one_shots/README.md`](one_shots/README.md) — one-shot catalog and rules
