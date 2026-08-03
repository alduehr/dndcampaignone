# one_shots/

## What this folder is

Standalone, **non-canon** one-shot adventures — fun, self-contained sessions
that live in the world of Orrun but are **deliberately disconnected** from
*The Long Remembering*'s campaign, canon, factions, mystery web, and NPCs.

This folder is a sibling to `ai_solo_campaign/`, not a subfolder of it, on
purpose:

- **It is outside `dm.campaign.json`'s `contentRoot`** (`"ai_solo_campaign"`),
  so it is automatically excluded from DungeonMaster onboarding — nothing
  here will ever be pulled into a live campaign session by that pipeline.
- **It is not referenced by any campaign index, canon file, or clue web** —
  not in `CONTENT_INDEX.md`, `NAMING_REGISTRY.md`, `DUNGEON_INDEX.md`, or
  `MYSTERY_WEB.md`. Names coined here are not checked against or added to
  `NAMING_REGISTRY.md`, since none of this is meant to ever appear in the
  main campaign.
- **It does not use any registered campaign NPC, faction, artifact, or
  location by name** — even when a one-shot is set near a real Orrun
  settlement for convenience, it invents its own disposable cast so it can
  be run with zero campaign lookups.

If a one-shot idea ever becomes good enough to fold into canon on purpose,
that's a deliberate, separate decision — move/rewrite it into
`ai_solo_campaign/` and register it properly at that point. Until then,
nothing in here is binding on campaign continuity.

## Contents

| One-Shot | Level | Party | Playtime | Setting | Summary |
|---|---|---|---|---|---|
| [`widdershin_cave/WIDDERSHIN_CAVE.md`](widdershin_cave/WIDDERSHIN_CAVE.md) | 1–4 | **3–6, tuned for four** (full scaling: [`PARTY_AND_LEVEL_SCALING.md`](widdershin_cave/PARTY_AND_LEVEL_SCALING.md)) | ~3–3.5 hrs at 3–4 characters; **~4–4.5 hrs at 5–6** | A sea-cave on Orrun's Pale Coast | A drowned smuggler captain who cannot let go of the idol he died trying to return — puzzle the tides, brave the wreck, and choose whether to fight him or free him. |
| [`the_ell_at_marchwell/THE_ELL_AT_MARCHWELL.md`](the_ell_at_marchwell/THE_ELL_AT_MARCHWELL.md) | **5 → 6** (milestone at the midpoint; scale by party size only) | **3–6, tuned for six** | **Four sessions**, 4–5 hrs each | A farmhouse in the Ashgarden Vale | A pantry door on an exterior wall, between two windows you can both lean out of at once, opens onto a corridor the house doesn't have. The party follows a fugitive clerk through it and has to find their way back out. |

### Session-zero pitch — *The Ell at Marchwell* (spoiler-free)

> You're carrying a warrant. Ferris Ambry, forty-one, under-clerk of the vale's
> tithe office, walked out of the counting room with the season's collection
> from three parishes — about eight hundred gold in coin and chapel plate, on a
> borrowed pony. He's soft, he's frightened, and he's not dangerous to anyone.
>
> He ran west, to the last farmhouse before the open downs, because his cousin
> lives there. It's cider country: hedged fields, drystone walls, whitewashed
> houses, apples going over in the yard. You'll be there by noon.
>
> Bring characters who'd take dull, well-paid work. **This is a horror
> campaign and it does not begin as one** — the first hour is an arrest at a
> farmhouse, and I'd like you to play it that way.
>
> Four sessions. Level five. Nothing you need to read beforehand.

*Everything in `the_ell_at_marchwell/` beyond this pitch is DM-facing.*

**Note on party size:** Widdershin Cave is a **party** adventure, not a solo
one — the Zone 6 boss is unwinnable for a single character on the math. It
does not serve the solo `ai_solo_campaign/` use case; it's built for a real
table. To run it for one player, give them a sidekick or two and use the
size-3 row in the scaling file.
