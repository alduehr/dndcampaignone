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
  dm.campaign.json          ← DungeonMaster app campaign-onboarding manifest (machine-read; see ONBOARDING.md)
  .gitignore
  .claude/
    agents/                ← Specialist subagent definitions (tracked; see below)
  ai_solo_campaign/         ← THE campaign engine — authoritative, secret-bearing, wired to play. See below.
  locations/
    vael/
      orrun/                ← Spoiler-free world-reference library, addressed by canonical key. See below.
  one_shots/                ← Standalone non-canon one-shot adventures, deliberately disconnected. See below.
```

---

## The Three Content Trees

This repo holds **three separate content trees** with different purposes, different authority levels, and different secrecy rules. Knowing which one you're in changes what you're allowed to assume.

| Tree | Purpose | Canon authority | Secrets | Onboarded to DungeonMaster app? |
|---|---|---|---|---|
| `ai_solo_campaign/` | Runs "The Long Remembering," the one predetermined solo campaign this repo exists for | **Authoritative** — the source of truth for everything campaign-related | Contains DM-only truths, hidden faction agendas, mystery answers | Yes — `dm.campaign.json`'s `contentRoot`, as a campaign unit |
| `locations/vael/orrun/` | General-purpose, spoiler-free reference library for the world of Orrun/Vael — geography, settlements, culture, generic bestiary — reusable outside the campaign | Derived/curated from campaign canon; **not** a second source of truth. If it ever disagrees with `ai_solo_campaign` on a plain geography/culture fact, `ai_solo_campaign` wins | None — deliberately contains no hidden-truth material, no faction secrets, no campaign quest hooks | Yes — onboarded separately as a **location** unit (`dm.location.json`), then mounted into the campaign's namespace via `dm.campaign.json`'s `locations` entry |
| `one_shots/` | Standalone, non-canon one-shot adventures set in the world of Orrun but deliberately disconnected from the campaign's canon, factions, mystery web, and NPCs | Not campaign canon at all; invents its own disposable cast, never uses registered campaign names | N/A — nothing here is a secret because nothing here is real to the campaign | No — outside `contentRoot`, not referenced by any campaign index |

**Practical rule of thumb:** if you're running or writing *the campaign*, you're in `ai_solo_campaign/`. If you need a spoiler-free fact about the world for a one-shot, an NPC walk-on, or a different game entirely, go to `locations/vael/orrun/`. If you want a fun, disposable session with no continuity obligations, go to `one_shots/`.

---

## Canonical Location Keys

Places in `locations/vael/orrun/` are addressed by a **canonical key**, not a file path: `<world>/<continent>/<kind>/<slug>`. World is `vael`, continent is `orrun`, kind is one of `regions`, `wilderness`, `settlements`, `sites`, `culture`, `bestiary`, `timelines`, `travel`. Ashgarden Vale is `vael/orrun/regions/ashgarden-vale`, on disk at `locations/vael/orrun/regions/ashgarden-vale.md`.

`ai_solo_campaign/` files cite these keys directly, in backticks, rather than linking to a relative path (e.g. a settlement file's First Impression section reads "Full sensory description: `` `vael/orrun/settlements/hollowmere` ``." instead of a markdown link). A campaign file that overlays one specific place carries a `location_ref:` front-matter field equal to that place's key; every location file itself carries a matching `location_key:` field. This means the DungeonMaster app can mount `locations/vael/orrun/` as an independent location unit and resolve every campaign cross-reference by key, without caring where either tree physically sits on disk.

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
  skills/                   ← DungeonMaster app skills overlay (mandatory DM-procedure files: canon-and-gaps, combat, procedures)
```

Note: `ai_solo_campaign/maps/` no longer exists — the map manifest and image assets moved to `locations/vael/orrun/maps/` (maps are geography, not campaign-runtime material, and the two copies were always byte-identical). `dm.campaign.json`'s `contentRoot` still points at `ai_solo_campaign` for the campaign's own content.

Read order for most work: `CLAUDE.md` → `00_control/PROJECT_RULES.md` → `00_control/CANON_AUTHORITY.md` → `00_control/GENERATION_GUARDRAILS.md` → the relevant specialist standards file (`WORLDBUILDING_STANDARDS.md`, `NPC_STANDARDS.md`, `QUEST_STANDARDS.md`, etc.) → `00_control/RETRIEVAL_GUIDE.md` for what to load for the task at hand.

---

## `locations/vael/orrun/` — World Reference Library

Full detail lives in [`locations/vael/orrun/README.md`](locations/vael/orrun/README.md) (relationship to the campaign, canonical-key scheme, maintenance rules) and [`locations/vael/orrun/GAZETTEER_INDEX.md`](locations/vael/orrun/GAZETTEER_INDEX.md) (every file, indexed). Summary:

```text
locations/vael/orrun/
  README.md                ← What this folder is, the canonical-key scheme, maintenance rules
  CONTINENT.md               ← Orrun at a glance (no location_key; an overview doc, not a place)
  GAZETTEER_INDEX.md          ← Full file index by category (no location_key)
  AUDIT_2026-08-01.md          ← Cohesion + secrecy audit (no location_key)
  dm.location.json            ← DungeonMaster app location-manifest contract
  regions/                  ← 16 region files, one per place, each carrying location_key: vael/orrun/regions/<slug>
  wilderness/                ← 7 wilderness zones: terrain, hazards, fauna, resources
  settlements/                ← 44 individual settlements/cities, one file per place, plus 5 no-key group indexes
  sites/                    ← 34 individual ruins/adventure sites, one file per place, plus 4 no-key group indexes + site-index.md
  culture/                   ← Calendar, cosmology (public), gods and faiths, languages, public world history
  bestiary/                  ← Generic wandering monsters and hazards by terrain — no campaign secrets
  timelines/                  ← The Unmade: alternate-timeline cosmology, including the Last Telling
  travel/                    ← Travel rates, routes, and hazards across the continent
  maps/                     ← Maps manifest + image assets — AUTHORITATIVE (moved from ai_solo_campaign/maps/)
```

Every content file here is `secrecy: player-safe`. If you're writing new content for this library, it must stay spoiler-free with respect to the campaign's central mystery — no hidden-truth material, no faction agendas, no campaign quest hooks, no current officeholders named (describe the office, not who holds it, so the library doesn't go stale as campaign play changes hands) — and it must carry a `location_key:` field if it represents an addressable place.

---

## `one_shots/` — Standalone Non-Canon Adventures

Full detail lives in [`one_shots/README.md`](one_shots/README.md). Each one-shot is its own subfolder (currently `widdershin_cave/`, `the_ell_at_marchwell/`) with its own self-contained files (premise, characters, room tables, DM screen, map spec, rewards). Deliberately outside `dm.campaign.json`'s `contentRoot` and outside every campaign index — nothing here is pulled into a live campaign session or checked against `NAMING_REGISTRY.md`. Not addressed by canonical key; out of scope for the location-key scheme.

---

## Root-Level Files

| File | Purpose |
|---|---|
| [`CLAUDE.md`](CLAUDE.md) | Claude Code's project instructions: prime directive, non-negotiable rules, hard constraints, core files to read first, specialist agent table |
| [`README.md`](README.md) | Public-facing overview: what this is, current status, development stages, key control files, recommended prompts |
| [`ONBOARDING.md`](ONBOARDING.md) | How this repo onboards into the separate DungeonMaster app (cloud AI DM server + phone app) |
| [`REPO_MAP.md`](REPO_MAP.md) | This file |
| [`dm.campaign.json`](dm.campaign.json) | Machine-read DungeonMaster campaign-onboarding manifest: `contentRoot`, `locations` (mounts `locations/vael/orrun`), player-safe path globs |

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
| Get a spoiler-free fact about Orrun's geography/culture for reuse elsewhere | `locations/vael/orrun/GAZETTEER_INDEX.md` |
| Resolve a canonical location key to a file | `locations/vael/orrun/<kind>/<slug>.md`, or start at `GAZETTEER_INDEX.md` |
| Run a quick, disposable session with no continuity obligations | `one_shots/README.md` |
| Understand how this repo plugs into the DungeonMaster app | `ONBOARDING.md` + `dm.campaign.json` + `locations/vael/orrun/dm.location.json` |
| Find the map assets and manifest | `locations/vael/orrun/maps/` (authoritative; each entry's `region` field is a canonical key) |
| Find a specialist subagent for a production pass | `.claude/agents/` (table also in `CLAUDE.md`) |

---

## Related Files

- [`CLAUDE.md`](CLAUDE.md) — Claude Code instructions and load order
- [`README.md`](README.md) — public overview and recommended prompts
- [`ai_solo_campaign/00_control/RETRIEVAL_GUIDE.md`](ai_solo_campaign/00_control/RETRIEVAL_GUIDE.md) — situational load guide for campaign play
- [`ai_solo_campaign/00_control/CONTENT_INDEX.md`](ai_solo_campaign/00_control/CONTENT_INDEX.md) — full campaign file inventory
- [`locations/vael/orrun/README.md`](locations/vael/orrun/README.md) — location library's own scope, key scheme, and rules
- [`locations/vael/orrun/GAZETTEER_INDEX.md`](locations/vael/orrun/GAZETTEER_INDEX.md) — full location-library file inventory
- [`one_shots/README.md`](one_shots/README.md) — one-shot catalog and rules
