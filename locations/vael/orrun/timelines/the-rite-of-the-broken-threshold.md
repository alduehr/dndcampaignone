# THE_RITE_OF_THE_BROKEN_THRESHOLD.md

---
type: mechanics
secrecy: player-safe
status: static
location_key: vael/orrun/timelines/the-rite-of-the-broken-threshold
region: (world-level, not location-bound)
level_range: usable at any level; recommended 5+ for the Last Telling specifically (see Danger Notes)
tags: [timelines, rite, ritual, DCs, unmade-glass, exhaustion, mechanics]
related: [THE_UNMADE_OVERVIEW.md, THE_LAST_TELLING.md, TELLING_TIERS_AND_RANDOM_TABLES.md]
---

## AI Use

Load this file whenever a player wants to attempt crossing into another Telling, wants to return from one, or asks how the mechanics work. This is D&D 5e/2024-compatible: no new subsystem, just a costly ritual with clear DCs, material costs, and consequences, per `../../../ai_solo_campaign/00_control/RULESET_ASSUMPTIONS.md`.

## Design Intent

The Rite must be:
- **Achievable from anywhere.** No fixed shrine, no gate, no single location gatekeeps it. Any quiet, undisturbed space works.
- **Difficult and expensive enough that it is never a default option.** Material cost, time cost, and a permanent personal cost every time.
- **Riskier and costlier the darker the destination.** Reaching the Last Telling should feel like a genuine campaign event, not a spell you prepare.
- **Returning should be meaningfully easier than leaving, but never free or guaranteed.** See "The Return Rite" below.
- **Never a source of cheap death.** Failure produces complications, exhaustion, and stranding — not instant character loss.

---

## What The Rite Requires (All Tiers)

1. **A working space.** Any location where the caster can mark a threshold — a doorway, a drawn circle, a natural arch, a grave-line — and remain undisturbed for the ritual's full duration. This can be improvised anywhere in the world; it does not require a shrine, a leyline, or a specific settlement.
2. **Unmade glass.** A rare, dark, faintly warm crystalline material that forms only where a Telling has recently "torn" nearby — old battlefields, sites of catastrophic unresolved choice, or (rarely) natural formations in old ruins. Traded on the black market and by a handful of specialist brokers (see `NPCS_OF_THE_UNMADE.md`). Base price **500 gp per shard**; the Last Telling requires a **matched/paired shard** ("a Broken Shard," effectively two shards fused, priced and sourced as such — typically 2,000+ gp or a dedicated quest to obtain). Shards are consumed by the rite.
3. **Time.** The ritual itself, uninterrupted (see table below). Interruption ruins the attempt and wastes the material component; it does not trigger a mishap.
4. **A caster or a guide.** Anyone can attempt the Rite — it does not require spellcasting. A character with **spellcasting ability** or **proficiency in Arcana or Religion** may use the relevant ability score for the check. A character with **neither** may still attempt it using a memorized ritual-script (learnable from any Fray-Walker or scholar, requiring no special class feature), rolling with disadvantage unless guided by someone who is proficient. This keeps the Rite available to any solo PC build, not just casters.
5. **The personal cost.** Paid every time, win or lose, once the ritual is completed to the point of the check (see below). This is what makes the Rite expensive in a way gold cannot bypass.

---

## Tiers, Costs, and DCs

| Tier | Material Cost | Ritual Time | Personal Cost | Check DC | Timing Requirement |
|---|---|---|---|---|---|
| **Near Telling** | 1 shard (500 gp) | 1 hour | 1 level of exhaustion | DC 15 | None |
| **Far Telling** | 3 shards (1,500 gp) | 8 hours | 1 level of exhaustion + one specific memory (player/DM choose something minor and roleplay-usable — never a mechanical ability) | DC 20 | None |
| **The Last Telling** | 1 Broken Shard (2,000+ gp or quest-sourced) | 24 hours, unbroken | 2 levels of exhaustion + one significant memory (roleplay-defined; the DM may offer a minor mechanical option instead — see Note below) | DC 25 | Must be performed during **a Between-Hour** (see below) |

**Check:** Religion, Arcana, or Survival (traveler's choice of the most fitting to their approach and background), or spellcasting ability check if using a prepared ritual spell-like framework. Advantage is granted if the traveler possesses a relevant Remembrance relic, is guided by an experienced Fray-Walker, or has crossed successfully before (they know what it costs).

**Exhaustion from the Rite** cannot be removed by a normal long rest while the traveler remains in the destination Telling — it represents being unanchored from home, not simple fatigue. It clears immediately upon a successful return.

**Note on the Last Telling's memory cost:** because this is meant to be usable in actual play without derailing a character, the DM may offer the player a lesser mechanical alternative to a story-significant memory loss — e.g., the character permanently forgets one non-critical piece of information (a contact's face, a route, a name) rather than losing a spell known or a proficiency. Never take away something that breaks the character's core concept. The point is weight, not punishment.

### The Between-Hour

The Last Telling can only be reached during a **Between-Hour**: a stretch, usually a single night, when the seam between Tellings runs thin everywhere in the Kept Telling at once. Between-Hours are not fixed to the calendar and cannot be reliably predicted more than a few days out — but they are tracked, after a fashion, by hedge-astronomers, the Mourners' Circle's almanacs, and anyone who trades in Unmade glass. In practice: **a Between-Hour occurs roughly 4–6 times a year**, and any settlement with a temple, university, or active Fray-Walker can tell a determined traveler when the next one is expected, usually within a few days' warning. This is the primary "expensive in time" cost for the Last Telling specifically — a party cannot simply decide today to go tonight.

---

## What Failure Means

Failing the check does **not** kill the traveler and does **not** strand them permanently. On a failed check:

- **Near/Far Telling attempt:** The rite still opens a door — just not the intended one. The traveler arrives in a *nearby* Telling of the DM's choice (usually stranger or more inconvenient than intended, never instantly lethal). The personal cost is still paid. They may attempt the Return Rite normally once there.
- **Last Telling attempt:** The rite fails to fully open the Broken Door. The traveler suffers the personal cost but does not travel, and the Broken Shard is *not* consumed (it is famously hard to waste one this way) — they can try again at the next Between-Hour. On a **natural 1**, the door opens halfway: the traveler is shunted into a Far Telling adjacent to the Last Telling — dark, wrong, dangerous, but survivable — instead of the true destination. This is a mishap, not a death sentence.

---

## The Return Rite

Every traveler who crosses carries an **anchor-thread**: an unbreakable (under normal circumstances) tether of their own Remembrance, rooted in the Kept Telling. This is why the trip home is cheaper — the traveler is not forcing a door outward into the unknown, they are being pulled back toward something that already knows where they belong.

| Requirement | Value |
|---|---|
| Material cost | None |
| Ritual time | 1 hour |
| Personal cost | None beyond what was already paid to arrive |
| Check DC | 15 (any Telling, including the Last Telling) |
| Location requirement | Must be performed at a **thin place** — a naturally weak seam in the visited Telling. Common in Near/Far Tellings (any threshold-symbolic location: doorway, grave, crossroads). In the Last Telling specifically these are rare and called **Hollow Marks** — see `THE_LAST_TELLING.md`. |

**On a failed return check:** the traveler gains 1 level of exhaustion and may try again after a short rest. This can be repeated indefinitely — the Return Rite does not strand anyone by itself.

**The one way to get properly stranded:** if the anchor-thread is **severed** — by a hostile act in the visited Telling specifically targeting it (a rare and narratively significant threat, never a random encounter trait), by staying so long the traveler's own Remembrance destabilizes (DM discretion, only after extended in-Telling time on the order of months), or by choosing to burn it deliberately for a one-time major effect (DM's call, always a player choice, never forced) — the Return Rite stops working. The traveler must then perform the full outbound Rite in reverse: find or make Unmade glass *in that Telling*, and pay the full cost again. This is the campaign's built-in "we could actually be trapped here" lever — use it sparingly and only when it serves the story.

---

## Time Differential

Time in a Telling runs at its own pace, not perfectly locked to the Kept Telling. As a rule of thumb: **time passes at roughly the same rate**, within a margin of hours to a couple of days of drift per day spent away — close enough that a week-long expedition costs about a week at home, but never so exact that a party can rely on split-second timing across worlds. On rare, significant occasions (DM's discretion, reserved for dramatic effect) the drift can be much larger. Do not simulate this precisely; use it as a narrative dial, not a clock to track literally.

---

## Danger Notes (Per `DND_MECHANICS_REQUIREMENTS.md`-Style Guidance)

- **Near Tellings:** Low danger by design. Suitable for any level. A good way to introduce the concept without risking the party.
- **Far Tellings:** Moderate to high danger, varies by what the DM rolls or chooses (see `TELLING_TIERS_AND_RANDOM_TABLES.md`). Recommended for parties of level 5+.
- **The Last Telling:** High danger by design (see `THE_LAST_TELLING.md` for full encounter/hazard guidance). Recommended for parties of level 8+. Telegraph the cost and danger heavily before the party commits — the Rite's own cost structure (gold, time, a Between-Hour, permanent personal cost) is itself the telegraph. Never let a party wander into the Last Telling by accident.

---

## Related Files

- [`THE_UNMADE_OVERVIEW.md`](the-unmade-overview.md) — cosmology this rite operates within
- [`THE_LAST_TELLING.md`](the-last-telling.md) — full writeup of the destination
- [`TELLING_TIERS_AND_RANDOM_TABLES.md`](telling-tiers-and-random-tables.md) — generating Near/Far Tellings
- [`NPCS_OF_THE_UNMADE.md`](npcs-of-the-unmade.md) — where to find Unmade glass and Fray-Walkers
