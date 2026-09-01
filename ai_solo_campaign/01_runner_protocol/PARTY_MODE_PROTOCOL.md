# PARTY_MODE_PROTOCOL.md — Running the Campaign for a Group (Six Players)

---
type: protocol
secrecy: mixed
status: static
region: Orrun
level_range: 1-20
related: [AI_DM_CORE_RULES.md, SOLO_PLAY_PRINCIPLES.md, ../13_encounters_and_bestiary/PARTY_SCALING_6_PLAYERS.md, ../14_treasure_and_artifacts/PARTY_REWARDS_6_PLAYERS.md, ../16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md]
tags: [type:protocol, secrecy:mixed, party-mode, runtime, six-players]
---

## AI Use / DM Use

The campaign is authored **solo-first** and that remains the default mode. Load this file (once, at campaign start) **only when running the campaign for a party** — it defines party mode: what changes, what explicitly does not, and how to adapt the solo-specific systems. Written for **six players**; scale the noted numbers proportionally for 3–5. Everything here is an **overlay** — no authored file is superseded except where this file explicitly says so.

## Declaring The Mode

Party mode is declared once, at campaign start (or at a clean act boundary if converting mid-campaign — not recommended). In party mode, three files replace/extend their solo counterparts:

| Concern | Solo authority (default) | Party-mode authority |
|---|---|---|
| Encounter math | `../13_encounters_and_bestiary/SOLO_ENCOUNTER_SCALING.md` | `../13_encounters_and_bestiary/PARTY_SCALING_6_PLAYERS.md` |
| Rewards | `../14_treasure_and_artifacts/SOLO_REWARD_BALANCE.md` | `../14_treasure_and_artifacts/PARTY_REWARDS_6_PLAYERS.md` |
| Solo safety net | `../16_ai_session_packs/SOLO_SAFETY_START.md` | §Companions And Allies below |

Everything else — canon, secrecy, clocks, mysteries, quests, sites, NPCs — is used **as written**.

## Session 1 For Six (adapting Opener A)

The Failed Funeral works even better with a crowd, with two adjustments:

- **Arrival:** the PCs arrive together (a caravan, a barge, a hired escort disbanding) or in 2–3 clumps the funeral gathers into one scene. Each PC still has their "own reasons" for coming to Hollowmere — collect one per player during character creation and weave them in.
- **Sefra recruits the group:** her line becomes plural — she was paid to find *capable newcomers*, and six is better than one (DM: her hidden patron's instruction was "capable hands," so nothing breaks — the steering now steers a party).
- **Distribute the doors:** Act 1 has **seven doors** (`../12_campaign_arc/ACT_1_LEVELS_1_4.md`) — with six players, seed a different door's hook toward each PC in the first two sessions (Wren's crisis, the Reeve, the Ledger job, the fens, the knock at night, the Mourners, the scholar). The doors all converge on the basin, so the party can split its curiosity and still arrive at the same story. This is the single biggest gift party mode gives this campaign: the door structure becomes a spotlight structure.

## Companions And Allies (the biggest inversion)

Solo mode's ally network (Hale as companion, Old Sashe as fen-guide, Brann in the Tollwood, hirelings, the safety net) exists to give one PC a second pair of hands. Six players ARE the second pair of hands.

- **Companion NPCs become guides, patrons, and faces — not party members.** Hale still knows the rites; Sashe still knows the fens; they walk *with* the party at most to the site's edge, advise, and step back. They stop absorbing combat pressure entirely.
- **Never run an NPC as a seventh party member.** Seven-plus bodies per side turns every fight to sludge and steals player spotlight.
- **The solo safety net stands down:** no guaranteed rescue reflexes, no insurance interventions. Telegraphs and outs remain (they're design, not charity).
- Ally *factions* (watch support, Warden aid, faction muscle) still function — offscreen or as scene-framing, not as controlled units.

## Runtime State In Party Mode

- **`../02_runtime_state/PLAYER_CHARACTER.md` becomes the party roster:** duplicate the character block once per PC under `## PC 1..6` headers; keep the shared Notes section for party-level facts (base, funds, reputation).
- **`NPC_MEMORY.md` and `RELATIONSHIPS.md` track per-PC where it matters** (who promised what to whom; which PC Sister Knell approached) — attribute entries to a named PC, not "the player."
- **`KNOWN_CLUES.md` is party-level:** a clue found by one PC is found (assume table-talk); never gate the mystery on which PC learned what.
- Everything else in `/02_runtime_state/` (clocks, faction state, quests, consequences) is party-level already and unchanged.

## Social Scenes, Checks, And Spotlight

- **DCs unchanged** (bounded accuracy). One PC talks; others assist, observe (Insight), or work a different NPC in the same scene — Caradril's districts and the moot-scenes are written with multiple simultaneous levers, which now get used in parallel.
- **Group checks** for whole-party activities (stealth, travel, climbing): standard half-succeed rule.
- **Spotlight discipline:** rotate the "face" by faction — six players naturally adopt one faction contact each (this maps onto the seven-faction structure almost perfectly, and faction-vs-faction party debates are a feature, not a problem).
- **Solo-play prompts in the protocols** ("the player has no one to confer with," lone-PC framing in `SOLO_PLAY_PRINCIPLES.md`, `SCENE_FRAMING.md`) are read as party-plural; no other change.

## Pacing, Rests, Milestones, Death

- **Milestones are shared and unchanged** — they're story-keyed (`ACT_1_MILESTONES.md`, `../15_campaign_arcs/LEVELING_AND_MILESTONE_GUIDE.md`); the party levels together when the story-beat lands. Expect the party to hit beats **faster** (six minds, parallel threads): let the clocks and the doors absorb the speed rather than padding.
- **Adventuring-day shape:** the party handles 2–3 real fights/day (see `PARTY_SCALING_6_PLAYERS.md` Rule 6); rest constraints in dungeon files are unchanged and now do real balancing work.
- **Death:** standard 5e lethality with fair telegraphing. The solo cheap-death prohibitions relax to normal good practice; revival, where the party earns it, follows `../03_canon/MAGIC_RULES.md` — and in *this* world, what resurrection risks meddling with is a campaign theme. Use that gravity.

## What Never Changes In Party Mode

- **Secrecy and reveal gates.** R1 cap in Act 1; REV gating; the apex stays DM-only. Six players triangulate faster — gate by *evidence earned*, exactly as written, not by pace.
- **Faction clocks, world consequences, canon, naming.**
- **The mystery web.** Three-clue redundancy was party-proof by design.
- **Telegraphs, morale, retreat, non-combat outs.**
- **The prime directive:** predetermined-first; improvise connective tissue only; record what matters.

## Table Realities (six chairs)

- Initiative: use side-based or popcorn variants if turns drag; the campaign doesn't care which.
- The Hollowmere hub scenes (inn, funeral, market) comfortably stage six; small interiors (the Brevin cottage, Sefra's corner table) — send 2–3 and let the rest work another thread that session.
- Handouts: the player-safe layer (maps, `PLAYER_SAFE_CANON.md`, rumor text) prints cleanly for the table; everything `mixed`/`dm-only` stays behind the screen.

## Related Files

- [`../13_encounters_and_bestiary/PARTY_SCALING_6_PLAYERS.md`](../13_encounters_and_bestiary/PARTY_SCALING_6_PLAYERS.md)
- [`../14_treasure_and_artifacts/PARTY_REWARDS_6_PLAYERS.md`](../14_treasure_and_artifacts/PARTY_REWARDS_6_PLAYERS.md)
- [`AI_DM_CORE_RULES.md`](AI_DM_CORE_RULES.md) · [`SOLO_PLAY_PRINCIPLES.md`](SOLO_PLAY_PRINCIPLES.md) (superseded pieces noted above)
- [`../12_campaign_arc/ACT_1_LEVELS_1_4.md`](../12_campaign_arc/ACT_1_LEVELS_1_4.md) (the seven doors → spotlight structure)
- [`../16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md`](../16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md) (run Step 3 once per player)
