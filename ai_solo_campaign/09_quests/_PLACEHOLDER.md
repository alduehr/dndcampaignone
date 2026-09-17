# _PLACEHOLDER.md — /09_quests/

## Purpose

This folder will contain quest files, hook tables, rumor tables, and quest indexes.

## Current Status

**Populated.** This folder contains the quest indexes (`QUEST_INDEX.md`, `MAJOR_CAMPAIGN_QUESTS.md`, `DEVELOPED_QUESTS_INDEX.md`, `HOOKS_JOBS_RUMORS_INDEX.md`), hooks/rumors tables, and the developed quest files across subfolders (act_1_quests, regional_quests, city_quests, faction_quests, hooks_and_rumors). See `QUEST_INDEX.md` for the full inventory and `../00_control/RETRIEVAL_GUIDE.md` ("Resolving a quest") for load guidance.

## Actual File Layout (updated 2026-07-11 — the original scaffold named planned files that were built under different names)

- `QUEST_INDEX.md` — master table of all quests
- `RUMORS_TABLE.md` — regional and settlement rumors *(scaffold called this `RUMOR_TABLE.md`)*
- `HOOKS_TABLE.md` — session-ready hooks *(scaffold: `HOOK_TABLE.md`)*
- Jobs/bounties live in `HOOKS_JOBS_RUMORS_INDEX.md` and the `hooks_and_rumors/` files *(scaffold: `BOUNTY_BOARD.md` — never created as a separate file)*
- Faction quest chains live in `faction_quests/[FACTION]/_CHAIN_INDEX.md` *(scaffold: `FACTION_QUESTS.md` — superseded by per-faction folders)*
- Developed quests: `MAJOR_CAMPAIGN_QUESTS.md`, `act_1_quests/`, `regional_quests/`, `city_quests/`, `faction_quests/`, `by_region/` — indexed in `DEVELOPED_QUESTS_INDEX.md`, cross-cut by `by_level/`, `by_faction/`, `by_type/`

## Quest File Standards

See `00_control/QUEST_STANDARDS.md`.

## Related Files

- [`../00_control/QUEST_STANDARDS.md`](../00_control/QUEST_STANDARDS.md)
- [`../02_runtime_state/ACTIVE_QUESTS.md`](../02_runtime_state/ACTIVE_QUESTS.md)
- [`../00_control/CONTENT_INDEX.md`](../00_control/CONTENT_INDEX.md)
