# Stage 16 — Player-Safe Start Readiness Audit

---
type: audit
secrecy: dm-only
status: static
date: 2026-06-15
tags: [audit, stage-16, starting-play, session-1, player-safe]
related: [STAGE_16_PRE_PLAY_READINESS_AUDIT.md, ../16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md]
---

## Scope

Can level-1 solo play begin immediately, cleanly, and safely from the prepared materials, without the AI DM inventing opening structure or asking "where does the campaign begin?"

## Verdict

**PASS — opening play is immediately runnable.**

## Checklist

| Requirement | Status | Evidence |
|---|---|---|
| Clean, self-contained Session-1 prompt | ✓ | `START_NEW_CAMPAIGN_PROMPT.md` — 7 steps, loads canon + protocols + state, handles character creation, delivers opener, lists what-not-to-reveal. All referenced load files exist. |
| Clear opening situation + recommended default | ✓ | Opener A "The Failed Funeral" recommended; Openers B/C as alternates. `OPENING_SCENES.md` present. |
| Starting region material | ✓ | `05_regions/SUNDERING_REACH.md` deep-built (8 settlements, 4 wilderness zones, 6 dungeons). |
| Starting settlement material | ✓ | `06_settlements/HOLLOWMERE.md` — home base (the Drowned Lantern), Mourner's Green opening site. |
| First NPCs | ✓ | Sefra, Wren, Tomas, Wend, Hale, Halla, Sashe in `08_npcs/MAJOR_NPCS.md`; named in the START prompt. |
| First hooks | ✓ | Hook 1 staged as opening thread; Hooks 5–7 pre-loaded; Act 1 faction + regional quests listed — all in `ACTIVE_QUESTS.md`. |
| First rumors | ✓ | `09_quests/RUMORS_TABLE.md` + Act 1 surface in `PLAYER_SAFE_CANON.md` ("The Reach at Campaign Start"). |
| First quests | ✓ | 6 Act 1 faction quests (`act_1_quests/`, all files present) + 14 Act-1-appropriate regional quests, seeded as available. |
| First dungeons/sites | ✓ | Six Stage 3 Concord sites serve Act 1 (Peat Chapel, Sunken Tollhouse, Whispering Cairn, Ledger Vault, Barrow, Deep Adit); keystone upper-works gated. |
| First clues | ✓ | REV_001 reachable via 5 independent sources (Wren, Sashe's drift-map, Warden rite-observation, grave-soil, Ring 1 windows). |
| First faction pressure | ✓ | All 7 factions stirring at start (`PLAYER_SAFE_CANON.md` Act 1 situation); clocks at Stage 1 in `WORLD_CLOCKS.md`. |
| First travel options | ✓ | Three directions out of the Reach + Caradril; `TRAVEL_ROUTES_RING1.md` (6 routes). |
| First-session state seeded | ✓ | All 16 `02_runtime_state/` files present; CURRENT_STATE/LOCATION/SCENE/ACTIVE_QUESTS/WORLD_CLOCKS seeded to campaign-start baseline; PLAYER_CHARACTER scaffold ready for creation. |
| Solo-safety net at start | ✓ | `SOLO_SAFETY_START.md` — safe base (Halla/the Lantern), optional companion (Hale), fen-guide (Sashe), paid-work patron (Sefra/Compact/Ledger); Wren is not forced combat; retreat always available. |
| No apex leak in opening | ✓ | START prompt STEP 5 enumerates the protected truths; openers carry them only in DM-Only sections. |
| Character creation handled | ✓ | START prompt STEP 3 — one-exchange setup, class-agnostic opener, milestone leveling, above-level-1 accepted with modest scaling. |

## Player-Safe Surface Integrity

The player-facing Act 1 surface (`PLAYER_SAFE_CANON.md` "The Reach at Campaign Start") correctly presents the *cause* of the failing rites as genuinely unknown ("a real mystery, not a withheld fact"), seeds the basin tell ("the dead walk the wrong way... toward the water") without explaining it, and frames all 7 factions by public face only. No mechanism, Court, or harvest language appears.

## Result

A new AI DM can open the file `START_NEW_CAMPAIGN_PROMPT.md` and run Session 1 end to end with zero invented major structure. **No blockers.**
