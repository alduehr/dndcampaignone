# _PLACEHOLDER.md — /15_random_tables/

## Purpose

This folder will contain random tables for travel events, weather, wilderness encounters, NPC personality generation, urban events, rumor surfacing, and other AI DM tools that add variety without requiring full content generation.

## Current Status

**Intentionally deferred — non-blocking for live play.** A consolidated random-table library here is an optional Stage 17+ enhancement. The play-critical tables already exist elsewhere: regional and travel encounter tables in `../13_encounters_and_bestiary/` (per-region `*_ENCOUNTERS.md`, `REGIONAL_ENCOUNTER_TABLES.md`, `TRAVEL_ENCOUNTERS.md`), treasure tables in `../14_treasure_and_artifacts/`, and hooks/rumors tables in `../09_quests/`. This folder does not block starting the campaign.

## Expected File Types

- `TRAVEL_EVENTS.md` — events keyed by region during overland travel
- `WEATHER.md` — weather tables by region and season
- `URBAN_EVENTS.md` — random street events, overheard conversations, etc.
- `NPC_PERSONALITY.md` — quick trait generator for minor NPCs
- `RUMOR_SURFACES.md` — tables for which rumors to surface in which locations
- Regional encounter tables (often housed in region files rather than here)

## Design Requirement

Tables should produce interesting situations, not just random noise. Every table result should potentially connect to existing content.

## Related Files

- [`../13_encounters_and_bestiary/`](../13_encounters_and_bestiary/)
- [`../01_runner_protocol/TRAVEL_PROTOCOL.md`](../01_runner_protocol/TRAVEL_PROTOCOL.md)
- [`../05_regions/`](../05_regions/)
