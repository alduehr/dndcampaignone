# Stage 16 — Full-Arc Playability Audit

---
type: audit
secrecy: dm-only
status: static
date: 2026-06-15
tags: [audit, stage-16, full-arc, levels-1-20, tiers, endgame]
related: [STAGE_16_PRE_PLAY_READINESS_AUDIT.md, ../15_campaign_arcs/LEVEL_5_TO_20_OVERVIEW.md, ../12_campaign_arc/MAIN_ARC_OVERVIEW.md]
---

## Scope

Verify levels 1–20 are supported, findable, and linked, with open-world resilience (off-route travel, ignored-arc consequences, region transitions, multiple endings, failure/partial-victory states).

## Verdict

**PASS — the full L1–20 arc is runnable and findable.** One navigability gap (legacy overview not pointing to `15_campaign_arcs/`) was fixed during this audit.

## Tier Coverage

| Tier | Levels | Acts | Spine file | Playable detail |
|---|---|---|---|---|
| 1 | 1–4 | Act 1 | `12_campaign_arc/ACT_1_LEVELS_1_4.md` | 6 faction quests + 14 regional quests + threats/clue-trails/failure/milestone/NPC guides. |
| 2 | 5–10 | Acts 2–3 lower | `15_campaign_arcs/TIER_2_LEVELS_5_10.md` | `TIER_2_PLAYABLE_PATHS_LEVELS_5_10.md` (5 paths) + regional arc packs. |
| 3 | 11–16 | Acts 3 upper–4 | `15_campaign_arcs/TIER_3_LEVELS_11_16.md` | `TIER_3_PLAYABLE_PATHS_LEVELS_11_16.md` (6 paths); REV_007 apex gate opens (L13+). |
| 4 | 17–20 | Act 5 | `15_campaign_arcs/TIER_4_LEVELS_17_20.md` | `TIER_4_PLAYABLE_PATHS_LEVELS_17_20.md` (9 endgame playbooks). |

## Open-World Resilience

| Capability | File | Status |
|---|---|---|
| Off-route / "go anywhere" arrivals (too early/late, skipping Caradril/Ring 1) | `15_campaign_arcs/PLAYER_GOES_ANYWHERE_GUIDE.md` | ✓ |
| Player ignores the main arc (per-tier world-states; reintroduction) | `15_campaign_arcs/PLAYER_IGNORES_MAIN_ARC_GUIDE.md` | ✓ |
| Region-to-region transitions (level/type/time/hook/complication/en-route clue) | `15_campaign_arcs/REGION_TO_REGION_TRANSITION_GUIDE.md` | ✓ |
| World moves without the player (16+ named pressure events) | `15_campaign_arcs/CONTINENTAL_PRESSURE_TIMELINE.md`, `CAMPAIGN_ESCALATION_TIMELINE.md` | ✓ |
| Final-revelation paths (REV_001–010 × 3 route-independent paths each) | `15_campaign_arcs/FINAL_REVELATION_AND_ENDING_PATHS.md`, `MAIN_ARC_REVELATION_SEQUENCE.md` | ✓ |
| Multiple endgame paths (9 approaches × 5 outcomes: seal/restart/seize/destroy/transform) | `15_campaign_arcs/ENDGAME_STRUCTURE.md`, `ENDGAME_REGION_PLAYBOOK.md` | ✓ |
| Failure / partial-victory states by tier | `15_campaign_arcs/FAILURE_STATES_AND_WORLD_CONSEQUENCES.md` | ✓ |
| Solo balance + milestone leveling across all tiers | `15_campaign_arcs/SOLO_CAMPAIGN_BALANCE_GUIDE.md`, `LEVELING_AND_MILESTONE_GUIDE.md`, `OPEN_WORLD_CONTINUITY_GUIDE.md` | ✓ |

## Stage 15A/15B Linkage

- The legacy `12_campaign_arc/MAIN_ARC_OVERVIEW.md` now carries a forwarding pointer to the `15_campaign_arcs/` runnable arc (fixed this audit).
- The `15_campaign_arcs/` forwarding stubs (`ACT_2`–`ACT_5`, `VILLAIN_ESCALATION`, `ENDGAME_STATES`) correctly route old references into the tier/playbook set.
- `LEVEL_5_TO_20_OVERVIEW.md` provides the tier↔act crosswalk so act-language and tier-language references reconcile.
- Apex protection holds across all tiers: REV_007/Hollow Court gated L13+; far sources never deliver it; endgame vertical under Hollowmere.

## Result

A solo campaign can run continuously from level 1 to level 20 across multiple branching paths and endings without the AI DM inventing major structure. **No blockers.**
