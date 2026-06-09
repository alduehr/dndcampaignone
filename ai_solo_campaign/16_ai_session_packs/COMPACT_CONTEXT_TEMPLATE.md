# COMPACT_CONTEXT_TEMPLATE.md

## Purpose

A compressed single-document summary of all critical campaign state, designed for use when context windows are filling up during long campaigns. Instead of loading many state files, the AI DM loads this one compact summary, then supplements with specific files as needed.

## Current Status

**Ready (Stage 2).** Use this when context is crowded mid-campaign or after a long gap. Fill it at session end (overwrite each time) from the runtime state files. It is a DM-only snapshot — the "What not to reveal yet" section in particular must never be shown to the player.

---

## When To Use

Use this when:
- A session is running long and context is crowded
- Resuming a campaign after a very long gap
- The AI DM needs a fast orientation without loading many files

This is a summary, not a replacement. Load specific files when deep detail is needed.

---

## Compact Context Template

*Fill in at session end for next session use. Overwrite each time.*

```md
# COMPACT CONTEXT — Session [N] — [Date]

## Character
- Name | Class | Level | HP [current/max] | Conditions

## Location
- [Current location, sub-area, time of day]

## Scene
- [1–2 sentences on immediate situation]

## Active Quests (summary)
| Quest | Status | Next Step |
|---|---|---|

## Key NPC Attitudes (most relevant)
| NPC | Attitude | Key Memory |
|---|---|---|

## Faction Pressures
| Faction | Attitude to Player | Active Clock |
|---|---|---|

## Known Clues (active mysteries)
| Mystery | Clues Found | Player Understanding |
|---|---|---|

## Open Threads (top 5)
- ...

## Inventory highlights
- [Notable magic items, currency, important documents]

## Consequences pending
- [Key delayed consequences the AI DM must remember]

## What not to reveal yet
- [DM-only — top secrets still hidden]

## Next session hook
- [Opening scene description]
```

---

## Related Files

- [`RESUME_CAMPAIGN_PROMPT.md`](RESUME_CAMPAIGN_PROMPT.md)
- [`STATE_UPDATE_TEMPLATE.md`](STATE_UPDATE_TEMPLATE.md)
- [`../02_runtime_state/`](../02_runtime_state/)
