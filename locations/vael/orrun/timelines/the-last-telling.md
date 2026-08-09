# THE_LAST_TELLING.md

---
type: wilderness_location
secrecy: player-safe
status: static
location_key: vael/orrun/timelines/the-last-telling
region: (exists parallel to all of Orrun; not a fixed location in the Kept Telling)
level_range: 8-16 (scalable; see Scaling Notes)
tags: [timelines, last-telling, the-unmade, dark-mirror, high-danger]
related: [THE_UNMADE_OVERVIEW.md, THE_RITE_OF_THE_BROKEN_THRESHOLD.md, UNMADE_ENCOUNTERS.md, NPCS_OF_THE_UNMADE.md]
---

## AI Use

Load this file when a party has committed to the Rite of the Broken Threshold and successfully reached the Last Telling, or when planning a Last Telling excursion in advance. This is a **self-contained, campaign-agnostic danger site** — it does not reference or depend on any single campaign's hidden villains or central mystery, and it should not be conflated with one. See "DM Guidance: Keeping It Separate" at the end of this file.

## One-Sentence Identity

The Last Telling is the world where the Last Door never reopened: nothing has been allowed to rest in over a thousand years, and everything that should have died is still — grimly, exhaustedly — here.

---

## What It's Called

"The Last Telling" is the neutral, scholarly name — what a loremaster, a Fray-Walker, or this document calls it when precision matters. Almost nobody who has actually been there uses it. Ordinary people across Orrun call it by a regional folk-name instead, the same way different cultures name the same afterlife differently. **Use the local name in play; save "the Last Telling" for narration, rules text, and scholars.**

| Regional Name | Where It's Used | Why That Name |
|---|---|---|
| **The Pall** | Sundering Reach, Tollwood, Pale Coast, Sallowmarch Protectorate, Saltmere Reaches (grief-and-funerary cultures, and places that live close to their own dead) | A pall is a funeral cloth — fitting for cultures organized around the Last Door and death-rites. Evokes something laid *over* the world rather than a place beside it. |
| **The Waning** | Ashgarden Vale, Sunmark, Hethewald Free Holds, Marrowdowns, Wender Steppe (agrarian, pastoral, seasonal cultures) | These are places that measure the world in light, seasons, and grazing. To them the horror isn't death exactly — it's things that stopped waxing and never finished waning. |
| **The Ashlands** | Emberfell Theocracy, Karran Marches (fire-and-ash cultures) | Self-explanatory to anyone who's seen the Last Telling's grey overcast firsthand and already lives somewhere that burned. |
| **The Echo Realm** | Caradril, Glassmere League, Concord Heartlands, Verdance Reaches, Hollow Gulf Ports (scholarly, urban, mercantile, archive-and-ruin cultures) | Fits the layered, repeating-ruin character of the place (see Geography below) and the "everything happened before, badly" tone that appeals to historians and archivists. |

Every region file in [`../01_geography/regions/`](../regions/) carries its own local name under a "Local Name For The Last Telling" heading, so the right word is available wherever play happens to be.

**Extending the pattern:** for a new region, pick whichever of the four fits its dominant culture (grief/funerary → the Pall; agrarian/seasonal → the Waning; volcanic/fire → the Ashlands; scholarly/urban → the Echo Realm) rather than coining a fifth name by default. A new regional name is fair game if a specific culture genuinely calls for it — just register it, and keep it distinct from **the Unmade**, which names the cosmology of *all* Tellings collectively, not this one specifically (see `THE_UNMADE_OVERVIEW.md`).

---

## What Travelers Notice First

- The sky is the wrong color: a flat, ash-grey overcast that never fully clears and never fully rains, day or night, everywhere.
- Sound carries strangely — too far, or not at all. Silence in the Last Telling has a pressure to it, like a held breath.
- Cold that isn't quite winter. It settles in joints and old wounds rather than skin.
- The living are rare, tired, and instantly recognizable to each other. A living stranger draws attention within minutes — some of it hopeful, most of it hungry.
- Familiar geography, wrong in the details: a traveler from the Kept Telling will recognize the *shape* of rivers, coastlines, and hills, but roads run to ruins that should be towns, towns stand where the map says wilderness, and nothing is named quite the way it should be. Use this to let players feel the wrongness through places they already know, without needing a literal second gazetteer — improvise the specific "wrongness" of any Kept Telling location on the fly.

## What Is Actually Going On

In the Last Telling, the Last Door shut and never opened again. Something — no one there agrees what, and the Last Telling has no shortage of theories, cults, and liars — sealed the way onward more than a thousand years ago by their reckoning, and the dead have been piling up on this side of it ever since. They simply never got to leave. They are not raging undead in the classic sense; most are exhausted, layered, half-forgotten things that have been *going through the motions of being alive* for so long that they have mostly forgotten how to want anything else. The truly dangerous ones are the rare few who remember exactly what they lost, and want it back.

This is a standalone cosmological fact of the Unmade — it is not secretly the same conspiracy as any specific campaign's central mystery, even one built on similar Remembrance/afterlife themes. Different Tellings can independently arrive at similar horrors; that's the point of the concept.

## Geography and Environment

- **No fixed map.** The Last Telling mirrors the Kept Telling's landmasses in rough outline but is not identical in detail. Improvise regional flavor from whatever part of Orrun the party is thematically near when they cross, twisted per the table below.
- **Layered ruin.** Because nothing has ever finished falling, settlements in the Last Telling tend to be built on top of, through, and around older versions of themselves — a thousand years of "towns" stacked like sediment, still half-inhabited by whoever was living (or not-quite-living) there in each layer.
- **No true wilderness.** Even far "empty" country is quietly occupied — grey fields tended by grey hands, forests walked by things that used to be foresters. Nowhere is truly abandoned; everywhere is under-populated by people going through very old motions.

### Quick Wrongness Table (d6) — What A Familiar Kept Telling Location Looks Like Here

| d6 | Wrongness |
|---|---|
| 1 | The place is intact but empty — everyone left generations ago, mid-task, and nothing has moved since. |
| 2 | The place is ruled by a "keeper" — a dead layer-holder who has run it, gently and terribly, for centuries. |
| 3 | The place has folded in on itself: several eras of the same location overlap visibly, and travelers can walk between them. |
| 4 | The place is a mass grave-city: the dead here vastly outnumber any living population that ever existed, layered in from elsewhere. |
| 5 | The place is actively, quietly hostile: whatever went wrong here is still going wrong, on a loop, and travelers can get caught in it. |
| 6 | The place is, disturbingly, almost fine — a pocket where the dead mostly did move on, and the few living residents are desperate to keep outsiders from finding out why this spot is different (a good hook seed). |

## Who/What Is In Charge

There is no single ruler, and deliberately so — a unified hidden power behind the Last Telling would turn it into somebody's specific plot rather than a general cosmological horror. Instead, it has many **Keepers**: individual dead who accumulated enough will and memory over the centuries to organize a layer, a town, or a stretch of road under their own rule. Some are tyrants. Some are, in their own exhausted way, trying to protect the living who remain. None of them can leave, and most of them have stopped wanting to.

## Native Threats

See `UNMADE_ENCOUNTERS.md` for full statlines. Common encounters:

- **The Unkept** (most common) — the ordinary dead of the Last Telling, going through old routines. Not usually hostile unless disturbed, provoked, or encountered en masse.
- **A Keeper** — a named, powerful dead ruler of a layer or settlement. Tier 1-equivalent adversary; see `UNMADE_ENCOUNTERS.md`.
- **A Hollow Hound** — predator-things that hunt anything with living warmth. The Last Telling's most common combat threat.
- **Fray-sickness** — environmental hazard, not a creature; see Hazards below.

## Hazards

| Hazard | DC | Effect |
|---|---|---|
| Fray-sickness (extended exposure, 24+ hours without shelter) | DC 15 Constitution save | 1 level of exhaustion on failure; repeats every 24 hours of continued exposure |
| A layer-fold (wrong-era overlap; see Wrongness Table result 3) | DC 15 Wisdom (Perception) to notice before stepping through; DC 15 Intelligence save if caught in one | On failed save, disoriented for 1d4 rounds and unsure which "era" of the location they're now in — narrative complication, not damage |
| A Keeper's domain (entering a ruled layer uninvited) | Varies by Keeper | See individual Keeper writeups; always telegraphed (a boundary marker, a change in the grey light, silence) before triggered |

## Rest and Time Pressure

- **Short rests** are possible almost anywhere, though never fully comfortable — the Last Telling does not restore the spirit the way home does. No mechanical penalty; this is flavor.
- **Long rests** require genuine shelter: a defensible, warded, or Keeper-sanctioned space. Resting in the open risks Fray-sickness (see Hazards) and wandering Hollow Hounds.
- **Time pressure:** the party's exhaustion from the Rite itself (see `THE_RITE_OF_THE_BROKEN_THRESHOLD.md`) does not clear here — it's a standing clock encouraging travelers not to linger. There is no other hard deadline by default; add one (a Keeper's patience, a hunted anchor-thread, a dying NPC) as the adventure calls for it.

## Treasure and Resources

- **Unmade glass** can occasionally be found here, freshly formed at active layer-folds — a reason beyond curiosity to come. A short expedition might net 1-3 shards.
- **Remembrance-heavy relics**: objects the dead here have kept far too long sometimes carry genuine magic (treat as a normal magic item appropriate to level, reflavored as "something a dead person refused to let go of").
- **Information**: the Last Telling's dead remember things the Kept Telling forgot — a legitimate reason for scholarly or personal expeditions (a specific historical fact, a version of a lost person, a warning).

## Boss/Climax Option: A Keeper Confrontation

When an adventure into the Last Telling needs a climax, the natural shape is a confrontation with a **Keeper** who controls whatever the party needs (a person, an object, passage, information). See `UNMADE_ENCOUNTERS.md` for the Keeper's mechanical profile. Keepers should always have:

- A **reason** they became what they are (a specific unfinished thing).
- A **noncombat resolution**: nearly every Keeper can be bargained with, reminded of who they were, or offered a way to finally finish what they're holding onto. Combat should be one option among several, not the default.
- **Morale**: most Keepers do not fight to the death. Losing control of their layer is often worse to them than losing a fight.

## Retreat Options

- The Return Rite (see `THE_RITE_OF_THE_BROKEN_THRESHOLD.md`) works from anywhere in the Last Telling that qualifies as a **Hollow Mark** — a place where the seam runs thin. Hollow Marks are rare but not unique; every explored region should have at least one within a day's travel, often guarded or contested (a good scene generator).
- Short of a Hollow Mark, there is no other way home. This is the primary source of tension on a Last Telling excursion: always know, or be actively searching for, the nearest Hollow Mark.

## Level Range and Solo Danger

- **Recommended level: 8-16.** Below level 8, the Rite's own cost (a Between-Hour, a Broken Shard, permanent exhaustion/memory cost) should function as a hard gate — a low-level party simply cannot afford to go yet, which is the intended balance lever rather than in-Telling combat difficulty alone.
- **Solo-PC danger: high but survivable with preparation.** Individual Unkept are low threat; Hollow Hounds are dangerous in numbers; Keepers are boss-tier and should always be telegraphed and avoidable. Never place a Keeper-tier threat between a solo party and their only known Hollow Mark without warning.

## Scaling Notes

- **Lower levels (if the party arrives via mishap, not choice — see failure results in `THE_RITE_OF_THE_BROKEN_THRESHOLD.md`):** favor the Wrongness Table's gentler results (1, 6), keep Unkept passive, and place a Hollow Mark within easy reach.
- **Higher levels:** favor active Keepers, layer-folds, and Hollow Hound packs; make Hollow Marks contested or temporarily sealed to force real engagement with the place.

---

## DM Guidance: Keeping It Separate

If your campaign has its own hidden explanation for why the dead linger in the Kept Telling, the Last Telling is intentionally **not** a reflection of it. Do not let players treat the two as connected — the Last Telling's dead-that-never-left is a parallel, independently-arising horror in a different Telling, and nothing found here is evidence about the Kept Telling. If a player draws the comparison out loud, that's a fair and interesting in-fiction observation for a character to make ("this looks like what we're afraid of at home") — just don't let it become a real clue.

Nothing in this file, or anywhere in `/locations/vael/orrun`, states or hints at what is actually behind the Kept Telling's restless dead. That answer belongs to whatever specific campaign is being run, and lives in that campaign's own DM-only files — never here.

## Related Files

- [`THE_UNMADE_OVERVIEW.md`](the-unmade-overview.md)
- [`THE_RITE_OF_THE_BROKEN_THRESHOLD.md`](the-rite-of-the-broken-threshold.md)
- [`UNMADE_ENCOUNTERS.md`](unmade-encounters.md)
- [`NPCS_OF_THE_UNMADE.md`](npcs-of-the-unmade.md)
