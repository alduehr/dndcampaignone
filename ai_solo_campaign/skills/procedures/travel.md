---
visibility: dm-only
title: Travel
---
# Travel

Read this whenever the party moves between locations rather than acting
within a single scene. This overlays the shared travel procedure — its pace
table, forced-march exhaustion rule, getting-lost, and foraging mechanics all
hold exactly as written and are not repeated here. What this file adds is
where to pull this campaign's own routes, hazards, and texture from, instead
of inventing them.

## Routes and hazards: use the authored geography, don't invent it

This campaign's regions each define their own real travel routes, distances,
and hazard DCs — don't estimate distance or danger generically when an
authored answer exists:

- **Route/travel-time data:** `04_world_atlas/TRAVEL_ROUTES_RING1.md` (the
  starting region and its three neighbors) or `04_world_atlas/
  FULL_WORLD_MAP_AUTHORITY.md` (the wider continent); each region's own file
  under `05_regions/` also states its Travel Routes and Level Range/Solo
  Danger sections with real distances and DCs.
- **Weather and season:** `15_random_tables/WEATHER.md` (season × climate
  zone). The campaign opens in Greyfall, mid-autumn — check the campaign's
  in-world clock via `get_state` for the current season before rolling.
- **Non-combat travel events:** `15_random_tables/TRAVEL_EVENTS.md` — a
  route-class table (Concord roads / wild country / river / sea) for texture
  beyond a bare encounter check. Route results back to existing authored
  content per that file's own rules; don't invent a new NPC or site to fill
  a result.

## Encounter checks: use the authored tables

Where the shared procedure says "make an encounter check... on a result
indicating an encounter, decide what's encountered from context" — for this
campaign, that context is authored. Use the specific region's encounter table
under `13_encounters_and_bestiary/[REGION]_ENCOUNTERS.md`, or
`13_encounters_and_bestiary/TRAVEL_ENCOUNTERS.md` for generic terrain lines,
rather than improvising a threat from nothing — and apply
`SOLO_ENCOUNTER_SCALING.md` to whatever the table produces (see
`combat/SKILL.md`, this overlay).

## Getting lost, foraging

The shared procedure's mechanics apply unchanged. Use the specific region's
stated terrain/navigation DCs from its `05_regions/` file where one is given,
rather than a generic default.

## Related campaign files

- `01_runner_protocol/TRAVEL_PROTOCOL.md`
- `04_world_atlas/TRAVEL_ROUTES_RING1.md` · `04_world_atlas/
  FULL_WORLD_MAP_AUTHORITY.md`
- `15_random_tables/TRAVEL_EVENTS.md` · `15_random_tables/WEATHER.md`
- `13_encounters_and_bestiary/TRAVEL_ENCOUNTERS.md`
