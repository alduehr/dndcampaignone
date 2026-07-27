---
visibility: dm-only
title: Downtime
---
# Downtime

Read this whenever a player asks to spend time between adventures on
something other than advancing the next scene. This overlays the shared
downtime procedure — its activity list and mechanics (recuperation,
profession, crafting, research, training, carousing, running a business) all
hold exactly as written and are not repeated here. What this file adds is
this campaign's own downtime texture and its faction-turn consequence, which
the shared procedure has no way to know about.

## Downtime moves the world, not just the character

This campaign's major factions act between sessions whether or not the
player is present — downtime is one of the main triggers for that. Before
resolving a downtime request:

- **Check whether time passing should advance a faction clock.**
  `07_factions/FACTION_TURN_RULES.md` defines when/how factions act
  off-screen; `02_runtime_state/WORLD_CLOCKS.md` lists the active clocks.
  Several days of downtime is exactly the kind of gap that clock advancement
  is meant to fill — apply it via `set_state`, and if a faction's move should
  be visible to the player on their return, narrate it as a change to the
  world rather than silently updating state.
- **Use `15_random_tables/URBAN_EVENTS.md`'s "Downtime Day" table** for quick
  texture on an otherwise uneventful stretch of downtime, rather than
  narrating a content-free skip — a downtime day can surface a rumor, a
  faction development, or a follow-up from a past scene without inventing new
  named content (that table routes to existing authored material only).

## Judgment calls

Same guidance as the shared procedure: extrapolate from the closest listed
activity rather than inventing a new subsystem, and `log_gap` anything that
comes up often enough to deserve real authored guidance.

## Related campaign files

- `07_factions/FACTION_TURN_RULES.md` · `02_runtime_state/WORLD_CLOCKS.md`
- `15_random_tables/URBAN_EVENTS.md`
