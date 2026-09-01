# RUMOR_SURFACES.md — Which Rumor Surfaces, Where, From Whom

---
type: random_table
secrecy: mixed
status: static
region: Orrun
level_range: 1-20
related: [../09_quests/RUMORS_TABLE.md, ../09_quests/HOOKS_JOBS_RUMORS_INDEX.md, ../11_mysteries_and_secrets/CLUE_INDEX.md]
tags: [type:random_table, secrecy:mixed, rumors, hooks, dm-tool]
---

## AI Use

This file does **not contain rumors** — the authored rumor stock lives in `../09_quests/RUMORS_TABLE.md` (NW cluster), the settlement files' Rumors sections, and the 13 far-continent `fc_*` files indexed in `../09_quests/HOOKS_JOBS_RUMORS_INDEX.md`. This file decides **which authored rumor surfaces, from whom, and how distorted** — so rumor delivery feels alive without inventing content. **Never invent a rumor with no authored destination.**

## Step 1 — Which stock? (by where the player is)

| Player's location | Draw from |
|---|---|
| A settlement | That settlement's file §Rumors first; then the region's rows in `RUMORS_TABLE.md` |
| On the road | The *destination's* stock (news travels the way the player is going) |
| A faction space (chapterhouse, keep, shrine) | That faction's angle on the region's stock (see faction file §Current Activity) |
| Far continent | The region's `fc_*` hooks/rumors file via `HOOKS_JOBS_RUMORS_INDEX.md` |

## Step 2 — Who's telling it? (d10)

| d10 | Source | Reliability flavor |
|---|---|---|
| 1 | Innkeep / ale-wife | Good on people, soft on facts |
| 2 | Carter / bargeman / sailor | Good on roads and routes; embellishes danger |
| 3 | Mourner or shrine-keeper | Solemn, careful; best on the dead and the rites |
| 4 | Market trader | Frames everything by price and scarcity |
| 5 | Watch / toll-clerk / official | Understates what embarrasses authority |
| 6 | Child or young apprentice | Saw more than anyone; understood less |
| 7 | Elder at the fire | The long view — may attach the *old songs* (M5-fringe, gated) |
| 8 | Faction hand (pick the local one) | True facts, partisan frame |
| 9 | Traveler passing through | A *neighboring* region's rumor, one step stale |
| 10 | Someone in their cups | A truth they'd never say sober — and a mess by morning |

## Step 3 — Distortion (d8; apply to the authored rumor's Truth Status)

| d8 | Distortion |
|---|---|
| 1–3 | Straight — as the authored table states it |
| 4 | Names swapped or misplaced (a nearby settlement/NPC substituted) |
| 5 | Scale inflated (one became many; a scare became a massacre) |
| 6 | Cause misassigned (the *convenient* villain blamed — often a faction the teller dislikes) |
| 7 | Two authored rumors fused into one garbled tale (deliver both threads) |
| 8 | Softened — the teller pulls the sting out ("probably nothing, but…") |

Distortion never changes the **authored truth status** — only the telling. When the player investigates, the authored rumor's destination and truth hold.

## Step 4 — Cost (optional, d6)

1–3: free with conversation · 4: a drink, a meal, a small favor · 5: reciprocity — they want news *from* the player first · 6: someone else is listening (a faction ear; note it in `NPC_MEMORY.md` if it matters)

## Clue-Bearing Rumors (gate check)

If the surfaced rumor touches a mystery (`RUMORS_TABLE.md` Points-Toward column → M-numbers), check `../11_mysteries_and_secrets/REVEAL_TIMING.md` and `CLUE_INDEX.md` gates before delivering more than the authored wording. Rumors deliver **doors, not answers**. Update `../02_runtime_state/KNOWN_CLUES.md` only when the player genuinely follows through.

## Related Files

- [`../09_quests/RUMORS_TABLE.md`](../09_quests/RUMORS_TABLE.md) · [`../09_quests/HOOKS_JOBS_RUMORS_INDEX.md`](../09_quests/HOOKS_JOBS_RUMORS_INDEX.md)
- [`../11_mysteries_and_secrets/CLUE_INDEX.md`](../11_mysteries_and_secrets/CLUE_INDEX.md) · [`../01_runner_protocol/CLUE_DELIVERY_PROTOCOL.md`](../01_runner_protocol/CLUE_DELIVERY_PROTOCOL.md)
