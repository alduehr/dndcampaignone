# Widdershin Cave — Party & Level Scaling

Non-canon, standalone — see [`../README.md`](../README.md) and
[`WIDDERSHIN_CAVE.md`](WIDDERSHIN_CAVE.md) for the base adventure this
converts.

Covers **any party from 1 to 6 characters at any average level from 1 to
4** — a solo level 1 PC, a full table of six level 4s, or anything between
(4 level 1s, 3 level 3s, 5 level 4s, a mixed-level group, etc.). Two
independent dials do the work, and you combine them:

- **Party SIZE** drives *how many* foes you're fighting (action economy).
- **Average party LEVEL** drives *how tough each one is* (chassis/numbers)
  — except when the party's levels are spread wide, see **Mixed-Level
  Parties** below.

Nothing else changes. DCs, puzzle logic, clue paths, NPC behavior, morale,
telegraphs, and retreat options are **identical at every scale** — that's
deliberate (see `WIDDERSHIN_CAVE.md`'s own Running Notes) and it's also
just correct: those things don't get harder because you brought friends.

---

## How To Use This

1. **Find your Size row** (count your characters, 1–6) in the **Foe Count
   Table** below. This tells you how many Reef Crabs and Skeletons appear
   in Zones 2 and 4.
2. **Find your Level row.** If every character is within 1 level of each
   other, use the (rounded) average. If the spread is wider than that, see
   **Mixed-Level Parties** instead — don't just average a level-1 and a
   level-4 together.
3. **Combine them.** Count comes from Size, stats come from Level. A party
   of 5 level-4 characters uses the Size-5 *count* with Level-4 *stats*; a
   party of 3 level-3s uses Size-3 counts with Level-3 stats.
4. **Apply the structural rules** (tunnel width, boss HP tier, Wailing
   Command, Tide Call pacing) from the section below.
5. **Scale treasure** using the short table at the end — mostly unchanged
   regardless of size or level.

---

## Foe Count Table (by Party Size)

Applies to **Zone 2 (Reef Crabs)** and **Zone 4 (Skeleton Crew)**. Stats for
each individual foe come from the Toughness Ladder below, not from this
table. Skeleton counts stay deliberately low — Zone 4 is a single-file
chokepoint fight, and a long queue of interchangeable mooks fought one at a
time just extends the fight without adding real challenge, so more bodies
past a certain point is worse design, not harder design.

| Party Size | Reef Crabs (Zone 2) | Skeletons (Zone 4) |
|---|---|---|
| 1 | 2 | 3 |
| 2 | 3 | 3 |
| 3 | 4 | 4 |
| 4 | 5 | 4 |
| 5 | 6 | 5 |
| 6 | 7 | 6 |

**At average level 3+, 1–2 of those skeletons are replaced by "Bosun's
Bones" elites instead of the standard line** — this reduces the standard
skeleton count, it does not add elites on top of it. Use **1 Bosun** for
party size 1–4, **2 Bosuns** for party size 5–6 (e.g., a size-4 party at
level 3 fights 3 standard skeletons + 1 Bosun, not 4 standard + 1 Bosun).

Reef Crabs stay a single, uniform tier at every level (see below) — Zone 2
is explicitly designed to be fully avoidable via the dry-spine Stealth
route regardless of size, so it's fine for it to look intimidating on paper
without needing elite variants.

---

## Toughness Ladder (by Average Level)

### Reef Crab
| Level | AC | HP | Attack | Notes |
|---|---|---|---|---|
| 1 | 15 | 6 | claw +3, 1d4+1 | as written in the base module |
| 2 | 15 | 8 | claw +4, 1d4+2 | — |
| 3 | 16 | 12 | claw +5, 1d6+2 | gains **Grab** (bonus action): a hit target is grappled (escape DC 12) |
| 4 | 16 | 20 | claw +6, 2d6+3 | single attack, no multiattack — tougher and harder-hitting instead of doubling actions; keeps Grab |

### Standard Skeleton (Skeleton Crew, Zone 4)
| Level | AC | HP | Melee (scimitar) | Ranged (shortbow) |
|---|---|---|---|---|
| 1 | 13 | 13 | +3, 1d6+1 | +3, 1d6 |
| 2 | 13 | 15 | +4, 1d6+2 | +4, 1d6+1 |
| 3 | 14 | 18 | +5, 1d6+3 | +5, 1d6+2 |
| 4 | 14 | 20 | +6, 1d6+4 | +6, 1d6+3 |

Vulnerable to bludgeoning, immune to poison damage and the
poisoned/exhausted conditions, resistant to cold damage — unchanged at
every level.

### Elite Skeleton — "Bosun's Bones" (swapped in at level 3+; see Foe Count Table)
| Level | AC | HP | Main Action | Shield Bash (bonus action) |
|---|---|---|---|---|
| 3 | 16 | 24 | scimitar +5, 1d6+3 | melee attack, +5 to hit, reach 5 ft, **1d4 bludgeoning**; on a hit, target makes a **DC 13 Strength save** or is pushed 5 ft directly away |
| 4 | 17 | 30 | Multiattack: 2× scimitar +6, 1d6+4 each | melee attack, +6 to hit, reach 5 ft, **1d4 bludgeoning**; on a hit, target makes a **DC 14 Strength save** or is pushed 5 ft directly away |

Shield Bash is a genuine bonus action a Bosun can use the same turn as its
main-action attack (or Multiattack, at level 4) — it's a real
action-economy threat, not flavor text, which is exactly why it's fully
worth defining precisely rather than leaving as a vague "knocks them back."

### Captain Perrin Locke, the Widdershin Warden
| Level | HP (before Size Tier bonus) | Attack (Cutlass of Drowning) | Notes |
|---|---|---|---|
| 1 | 35 | +4, 1d8+2 slashing + 1d6 cold | as written in the base module |
| 2 | 40 | +5, 1d8+3 slashing + 1d6 cold | — |
| 3 | 50 | +6, 1d8+4 slashing + 2d6 cold | Tide Call's prone effect now also deals 1d6 cold to anyone it knocks down |
| 4 | 60 | +7, 2d6+4 slashing + 1d6 cold | cutlass strike upgraded to a heavier two-handed swing; cold damage stays modest so the hit doesn't spike too hard against a squishier level-4 caster |

**Idol Resistance, morale, retreat, and the puzzle-first resolution are
identical at every level** — a smart table that returns the Fathom Eye
still ends this without a full fight, at any size or level. **Tide Call and
Wailing Command are defined once, in `WIDDERSHIN_CAVE.md` and the
Structural Scaling section below, and don't change per level** — only
*when* they're guaranteed to trigger shifts with party size (see below).

---

## Mixed-Level Parties: Same-Band vs. Wide-Gap

**If every character is within 1 level of another** (e.g., a mix of levels
2 and 3), just average and round to the nearest whole level, then use that
row normally. This adventure's math is forgiving enough that small spreads
don't need special handling.

**If the spread is wider than 1 level** (e.g., a level-1 and a level-4 in
the same party), do **not** average. A level-4-average attack line can
threaten to drop a level-1 character in a single hit — that's not a fair
fight, it's a coin flip on a PC's life. Instead:

1. **Use the lowest character's level** to set every foe's **AC and
   attack line** (to-hit and damage) from the Toughness Ladder above. This
   keeps the worst-case hit survivable for your most fragile character.
2. **Add HP instead of damage** to compensate for the party's actual
   strength: apply a flat **+10% HP to every foe** (crabs, skeletons,
   Locke) for each full level of spread beyond 1, on top of whatever the
   Structural Scaling Size Tier multiplier already adds. Round to the
   nearest whole number for individual foes and to the nearest 5 for
   Locke.
3. **Bosun swap-in and other level-3+/level-4+ features follow the lowest
   level too** — if your lowest character is level 1, don't swap in a
   Bosun's Bones even if your average would've qualified.

**Worked example — 1 level-1 character + 1 level-4 character** (size 2,
spread 3, so 2 levels of spread beyond 1 → **+20% HP**):
- Use **Level-1 stat lines** for AC/attack on everything (crabs, skeletons,
  Locke) — safe for the level-1 character.
- Crabs (size 2 → 3 of them): HP 6 × 1.2 = 7.2 → **7 HP** each, stats
  otherwise Level-1.
- Skeletons (size 2 → 3 of them): HP 13 × 1.2 = 15.6 → **16 HP** each,
  stats otherwise Level-1. No Bosun swap-in (lowest level is 1).
- Locke: Level-1 base 35 HP × Tier I (size 2 = ×1.0) × 1.2 = 42 → round to
  the nearest 5 → **40 HP**, Level-1 attack line, Tier I structural rules.
- The level-4 character will still feel the fight is easy in raw damage
  output — that's intentional. The point of this rule is protecting the
  level-1 character's survival, not giving the level-4 character a hard
  fight solo; if you want more challenge for the higher-level members
  specifically, lean on Locke's Tide Call and the Bosun swap-in (using
  their *individual* level where the fiction allows, e.g. a Bosun
  specifically targeting the tougher character) rather than raising damage
  against the whole party.

---

## Structural Scaling

### Zone 4 tunnel width
**Stays 1 square wide for any level-1 party, regardless of size** — the
Foe Count Table already keeps skeleton counts low at every size, so a
single-file fight stays snappy even with six level-1 characters queued up.
**For level 2+ parties of size 4 or more,** widen it to **2 squares** so
the fight doesn't bench most of the table behind one front-liner. Size 1–3
at any level, or any size at level 1, keeps the 1-square chokepoint as
written.

### Locke's boss HP (Size Tier multiplier)
Applied on top of the Toughness Ladder's base HP for Locke's level (and on
top of the Mixed-Level Parties bonus, if that rule applies instead).

| Size Tier | Party Size | Multiplier |
|---|---|---|
| I | 1–2 | ×1.0 |
| II | 3–4 | ×1.15 |
| III | 5–6 | ×1.3 |

Round to the nearest 5 (e.g., Level 3 base 50 × Tier II's ×1.15 = 57.5 →
**60**).

### Wailing Command
**Unchanged at every size and level.** Locke can call surviving Zone-4
skeletons to Zone 6 (2-round travel time, telegraphed) — and only
surviving skeletons. If the player cleared Zone 4 entirely, Wailing Command
does nothing but a mournful, echoing shout. **Never manufacture new
skeletons out of nowhere at any party size** — a bigger table just means a
bigger fight in Zone 4 up front, which is where that pressure belongs.

### Tide Call
**Hard capped at twice per fight, at every size and level** — see
`WIDDERSHIN_CAVE.md`'s boss writeup for the base ability (uses his action,
recharges on a 5–6). Larger parties only pull the *timing* of that first
use earlier; they never grant extra uses beyond the cap.

| Size Tier | First use | Second use |
|---|---|---|
| I (size 1–2) | Whenever it naturally recharges — no guarantee | Whenever it next naturally recharges after the first |
| II (size 3–4) | Guaranteed by round 3 if it hasn't recharged naturally yet | Whenever it next naturally recharges after the first |
| III (size 5–6) | Guaranteed by round 2 | Guaranteed by round 5 if it hasn't recharged naturally yet |

Everything else about the boss — Idol Resistance, the morale/parley window
below ⅓ HP, Tam's one-round distraction, targeting restrictions, retreat
behavior — is **unchanged at every Size Tier.** Bigger tables get more
pressure and more bodies, never a meaner or less fair version of the fight.

---

## Treasure Scaling

Keep individual finds (the 22 gp strongbox in Zone 2, the 35 gp strongbox
and flask in Zone 4, Log Fragments, the tide-chart disc) **unchanged at
every scale** — they're flavor and clue delivery, not a per-PC budget line.

Scale only the **Zone 6 sea-chest coin**, since that's the adventure's
actual payout:

| Party Size | Sea-chest coin |
|---|---|
| 1 | 140 gp |
| 2 | 180 gp |
| 3–4 | 260 gp |
| 5–6 | 340 gp |

**Everything else in the vault stays fixed, regardless of party size or
level:**
- **Widdershin Coins:** 1 for party size 1–2, 2 for size 3–4, 2–3 for size
  5–6 — but every coin recharges **once per long rest, at every level.**
  Don't bump the recharge rate for higher-level parties; it's a nice
  trinket, not a build-around, and staying flat keeps it simple to track
  when multiple characters are carrying one.
- **The boarding cutlass:** exactly **one**, always — it's a unique
  collectible find, not a per-character reward. Don't duplicate it for
  larger parties.

---

## Worked Examples

**Solo, 1 level-1 character** (the base module, unchanged): 2 Crabs / 3
Skeletons, both Level-1 stats. Locke: 35 HP, Level-1 attack line, Tier I
structural rules — 1-square tunnel, Wailing Command survivors-only, Tide
Call on normal recharge (cap 2). Loot: 140 gp, 1 Widdershin Coin, 1
cutlass.

**4 level-1 characters:** Size 4 → 5 Crabs / 4 Skeletons, all Level-1
stats (no Bosun swap-in — that only triggers at level 3+). Locke: 35 HP ×
1.15 (Tier II) = 40.25 → **40 HP**, Level-1 attack line. **Tunnel stays
1 square wide** (level-1 party, regardless of size). Wailing Command calls
only whatever skeletons survived Zone 4. Tide Call: first use guaranteed by
round 3 if it hasn't recharged naturally, second use whenever it next
recharges — capped at 2 total. Loot: 260 gp, 2 Widdershin Coins (once per
long rest), 1 cutlass.

**3 level-3 characters:** Size 3 → 4 Crabs (Level-3 stats: AC16/HP12/Grab)
/ 4 Skeletons, **1 swapped for a Bosun's Bones** → 3 standard (Level-3
line) + 1 Bosun (AC16/HP24, scimitar +5 1d6+3, Shield Bash +5 to hit/1d4
bludgeoning/DC13 push). Locke: 50 HP × 1.15 (Tier II) = 57.5 → **60 HP**,
Level-3 attack line (+6, 1d8+4 slashing + 2d6 cold; Tide Call's prone
effect adds 1d6 cold). **Tunnel stays 1 square wide** — level 2+, but
party size is only 3, below the size-4 threshold. Wailing Command:
survivors-only. Tide Call: Tier II timing, capped at 2. Loot: 260 gp, 2
Widdershin Coins (once per long rest), 1 cutlass.

**5 level-4 characters:** Size 5 → 6 Crabs (Level-4 stats: AC16/HP20,
claw +6, 2d6+3, single attack, Grab) / 5 Skeletons, **2 swapped for
Bosun's Bones** → 3 standard (Level-4 line) + 2 Bosun (AC17/HP30,
Multiattack 2×scimitar +6 1d6+4, Shield Bash +6 to hit/1d4 bludgeoning/
DC14 push). Locke: 60 HP × 1.3 (Tier III) = 78 → **80 HP**, Level-4 attack
line (+7, 2d6+4 slashing + 1d6 cold). **Tunnel widens to 2 squares**
(level 2+ and size ≥4). Wailing Command: survivors-only, no manufactured
reinforcements even at this size. Tide Call: Tier III timing — first use
guaranteed by round 2, second guaranteed by round 5 if it hasn't recharged
naturally — hard capped at 2 total, never more. Loot: 340 gp, 3 Widdershin
Coins (once per long rest, same as every other size), **1 cutlass** (not
duplicated for the larger party).

**Anything else** (2 level-2s, 6 level-1s, a same-band mixed 2/3/3 group,
etc.): read your Size row for counts, your Level row for stats (or the
Mixed-Level Parties rule if the spread is wide), and the Structural Scaling
section for tunnel width, boss HP, and the two capped Tide Call uses. There
is no combination of 1–6 characters and levels 1–4 this system doesn't
already cover.
