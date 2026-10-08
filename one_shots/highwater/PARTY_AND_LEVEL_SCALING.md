# Highwater — Party & Level Scaling

Non-canon, standalone — see [`../README.md`](../README.md) and
[`HIGHWATER.md`](HIGHWATER.md) for the adventure this converts.

Covers **any party from 3 to 6 characters at level 5.** The base module is
written for **four characters at level 5**; this file gives every other size.
Nothing about the *puzzle logic, clue routes, DCs, NPC behavior, Gauge Marks,
or timer* changes with party size — those things don't get harder because
you brought friends. Only three dials move:

1. **How many foes** (and how tough the boss is).
2. **How many successes** the group checks need.
3. **Whether Ivo fights.**

> **This is a party adventure.** A single character cannot do the Great Wheel,
> the Gate 2 jam, and a boss fight in three hours on the math. For one or two
> players, run the size-3 row and add one or two sidekicks (use the stat
> profile in the main file for Ivo, and the Veteran-lite profile for others).

---

## How To Use This

1. Find your **Size** column (3, 4, 5, 6).
2. Replace the baseline foe counts in each encounter with the table below.
3. Apply the **Success Requirements** table to the group checks.
4. Apply **Ivo's role** and the **Boss dial**.
5. Check the **Pace Hints** for your size.

The XP budgets below use the 2024 "XP budget per character" bands for
level 5 (Low 500 / Moderate 750 / High 1,100 per character).

| Size | Low | Moderate | High |
|---|---|---|---|
| 3 | 1,500 | 2,250 | 3,300 |
| **4 (baseline)** | **2,000** | **3,000** | **4,400** |
| 5 | 2,500 | 3,750 | 5,500 |
| 6 | 3,000 | 4,500 | 6,600 |

---

## Foe Count Table (by Party Size)

Individual stats come from the Stat Profiles in the main file and do not
change with party size (except the Silt Elemental's HP, below).

| Encounter | Size 3 | **Size 4** | Size 5 | Size 6 |
|---|---|---|---|---|
| **E1 — Crest** (mere-claws) | 4 | **5** | 6 | 8 |
| **E2 — Gear Hall** | Greaves + 1 thug + 1 cutter | **Greaves + 2 thugs + 1 cutter** | Greaves + 3 thugs + 1 cutter | Greaves + 3 thugs + 2 cutters |
| **E3 — Forge** (ore-borers + mother) | 2 + mother | **3 + mother** | 4 + mother | 5 + mother |
| **E4 — Shaft** | weird + 1 quipper swarm | **weird + 2 swarms** | weird + 3 swarms | 2 weirds + 2 swarms |
| **E5 — Tailrace** (giant pike) | 2 | **3** | 4 | 5 |
| **E6 — Cache** | Varrow + Stoke + 2 thugs | **Varrow + Stoke + 3 thugs + 1 cutter** | Varrow + Stoke + 4 thugs + 2 cutters | Varrow + Stoke + 5 thugs + 2 cutters |
| **E7 — Crest finale** | elemental (HP 90), no spawn | **elemental (HP 114)** | elemental (HP 140) + 1 silt-spawn at round 3 | elemental (HP 170) + 2 silt-spawn (round 2 and round 4) |

**XP check at each size** (approximate; the fights are timer-bound, so these
are intentionally on the low side of each band):

| Encounter | Size 3 | **Size 4** | Size 5 | Size 6 |
|---|---|---|---|---|
| E1 | 800 | 1,000 | 1,200 | 1,600 |
| E2 | 650 | 750 | 850 | 950 |
| E3 | 650 | 750 | 850 | 950 |
| E4 | 900 | 1,100 | 1,300 | 1,800 |
| E5 | 200 | 300 | 400 | 500 |
| E6 | 1,750 | 1,950 | 2,350 | 2,550 |
| E7 | 1,800 | 1,800 | 2,000 | 2,200 |

### Tier rules for the boss (Silt Elemental) and Varrow

| Tier | Size | Silt elemental | Varrow |
|---|---|---|---|
| **A** | 3 | HP 90; Engulf recharge **6** only | HP 70; no Parry |
| **A** | 4 | HP 114; Engulf recharge 5–6 | HP 85; Parry |
| **B** | 5–6 | HP 140 (size 5) / 170 (size 6); add **Tidal Shove** (bonus action, 10 ft push, DC 15 Str) | HP 100; Rallying Call also grants an ally **Temp HP 5** |

**Draining stays the same at every size:** the elemental loses 10 HP at the
end of each round starting at round 3. This is how the fight is tuned to the
clock, not to the party.

---

## Success Requirements (by Party Size)

Group checks scale by **plus or minus one success**, never by DC.

| Check | Size 3 | **Size 4** | Size 5 | Size 6 |
|---|---|---|---|---|
| **Install Master Gear** (3 successes before 2 failures; DC 14) | 2 | **3** | 3 | 4 |
| **Clear the Diversion Mouth** (small job; DC 14) | 2 | **2** | 3 | 3 |
| **Clear the whole plug** (big job; DC 14) | 4 | **5** | 6 | 7 |
| **Great Wheel** (before 3 failures; DC 15) | 4 | **5** | 5 | 6 |
| **Hand-crank a gate** (before 2 failures; DC 15) | 2 | **3** | 3 | 4 |
| **Characters at the wheel per round** | 2 | **3** | 3 | 4 |

(The "Characters at the wheel per round" cap exists so every table gets a
spread of action economy; a six-character party can use four at the wheel
while the others hold the cache door.)

---

## Ivo's Role (by Party Size)

| Size | Ivo |
|---|---|
| **3** | **Fights.** AC 14, HP 35, Multiattack (two shortswords, +5, 1d6+3). He is a fighting companion; he will not run ahead and he will not leave the party. |
| **4** | **Guide.** Stat profile in the main file (AC 12, HP 22). He doesn't fight unless cornered. |
| **5–6** | **Optional.** Treat him as an NPC reference: the party can ask him questions, but he stays at the Keeper's House (too frail). The log and the clue paths still work. |

---

## Pace Hints (by Party Size)

| Size | Pace behavior | DM adjustment |
|---|---|---|
| **3** | Fewer attacks per round → fights run **more rounds**, but fewer decisions per round. | Open with the **negotiation** options on E2 and E6; trim E1 to 3 crayfish if the table is behind schedule. |
| **4** | Baseline. | Use the Pacing Sheet as written. |
| **5–6** | More voices, **slower decisions**, more splintering. | **Cut G2 and G3** (Cistern and Pump Room) entirely unless players ask; use the **Compressed Forge** (2 borers only); ask the table to **name one spokesperson per room** for plans. |

---

## Level Notes (Level 5 Baseline)

The module is tuned for **level 5**. If the table is off by a level:

| Party level | Adjustment |
|---|---|
| **4** | Use the size-3 foe counts at size 4 (one step down); reduce all save DCs by 1; remove the Silt Elemental's Engulf; Varrow loses Parry. |
| **5** | As written. |
| **6** | Use the next-size-up foe counts; +1 to DCs on hazards; Silt Elemental gains +10 HP and its slam becomes 2d8+6; Varrow's AC 18. |

Do **not** change timer length for level. If the table is behind, use the
elastic dials in [`PACING_SHEET.md`](PACING_SHEET.md).

---

## Treasure & Rewards (by Party Size)

| Size | Adjust |
|---|---|
| **3** | Maren's offer: **1,500 gp** (×1). |
| **4** | As written. |
| **5** | Maren's offer: **×1.25**. |
| **6** | Maren's offer: **×1.5**. |

Magic items and potions are fixed and do not scale.
