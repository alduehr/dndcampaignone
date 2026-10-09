# Highwater — Party & Level Scaling

Non-canon, standalone — see [`../README.md`](../README.md) and
[`HIGHWATER.md`](HIGHWATER.md) for the adventure this converts.

Covers **any party from 3 to 6 characters at level 5.** The base module is
written for **four characters at level 5**; this file gives every other size.
Nothing about the *puzzle logic, clue routes, DCs, NPC behavior, Gauge Marks,
time costs, or timer* changes with party size — those things don't get harder
because you brought friends. Only four dials move:

1. **How many foes**, and how tough the four bosses are.
2. **How many successes** the group checks need.
3. **Whether Ivo fights.**
4. **The town's payment.**

> **This is a party adventure.** One character cannot work the Great Wheel,
> dig the Outfall, and fight the finale inside three hours. For one or two
> players, run the size-3 rows and add one or two sidekicks (Ivo's size-3
> profile works for a second sidekick too).

---

## How To Use This

1. Find your **Size** column (3, 4, 5, 6).
2. Replace the baseline foe counts in each encounter with the table below.
3. Apply the **Boss** table (Greaves, Varrow, the Snapper, the elemental).
4. Apply the **Success Requirements** table to the group checks.
5. Apply **Ivo's role**, the **Pace Hints**, and the **Rewards** row.

Budgets use the 2024 XP budget per character at level 5 (Low 500 /
Moderate 750 / High 1,100):

| Size | Low | Moderate | High |
|---|---|---|---|
| 3 | 1,500 | 2,250 | 3,300 |
| **4 (baseline)** | **2,000** | **3,000** | **4,400** |
| 5 | 2,500 | 3,750 | 5,500 |
| 6 | 3,000 | 4,500 | 6,600 |

---

## Foe Count Table

Stat lines are in the main file's *Stat Profiles*; only the bosses change
(next section).

| Encounter | Size 3 | **Size 4** | Size 5 | Size 6 |
|---|---|---|---|---|
| **E1 — Crest** | 2 mere-claws + Snapper | **4 mere-claws + Snapper** | 6 mere-claws + Snapper | 8 mere-claws + Snapper |
| **E2 — Gear Hall** | Greaves + 2 thugs + 1 cutter | **Greaves + 3 thugs + 2 cutters** | Greaves + 4 thugs + 3 cutters | Greaves + 6 thugs + 3 cutters |
| **E3 — Forge** | mother + 2 borers | **mother + 3 borers** | mother + 5 borers | mother + 7 borers |
| **E4 — Shaft** (optional) | weird + 1 quipper swarm | **weird + 2 swarms** | weird + 4 swarms | 2 weirds + 3 swarms |
| **E5 — Outfall** | 2 giant pike | **3 giant pike** | 4 giant pike | 5 giant pike |
| **E6 — Cache** | Varrow + Stoke + 2 thugs | **Varrow + Stoke + 3 thugs + 2 cutters** | Varrow + Stoke + a second Stoke-like archer + 5 thugs + 3 cutters | Varrow + Stoke + a second Stoke-like archer + 8 thugs + 5 cutters |
| **E7 — Crest finale** | elemental (size-3 row) | **elemental (baseline)** | elemental (size-5 row) | elemental (size-6 row) |

**XP at each size** (the fights are tuned to the low side of each band on
purpose — the clock, the missing long rest, and the hazards are the rest of
the difficulty):

| Encounter | Size 3 | **Size 4** | Size 5 | Size 6 | Band |
|---|---|---|---|---|---|
| E1 | 1,100 | 1,500 | 1,900 | 2,300 | Low |
| E2 | 1,000 | 1,200 | 1,400 | 1,600 | Low |
| E3 | 650 | 750 | 950 | 1,150 | Low |
| E4 | 900 | 1,100 | 1,500 | 2,000 | Low |
| E5 | 400 | 600 | 800 | 1,000 | Low (played as Moderate underwater) |
| E6 | 2,450 | 2,750 | 3,500 | 4,000 | Moderate |
| E7 | 3,100 | 3,300 | 4,500 | 5,800 | Moderate–High |

---

## Boss Table

| Boss | Size 3 | **Size 4** | Size 5 | Size 6 |
|---|---|---|---|---|
| **Old Snapper** (E1) | HP 50; one grapple at a time | **HP 68; two grapples** | HP 85 | HP 100; Crush is 3d6 |
| **Pelham Greaves** (E2) | HP 70; no Parry | **HP 90; Parry** | HP 100 | HP 110 |
| **Sull Varrow** (E6) | HP 100; two longsword attacks; no Parry | **HP 130; three attacks; Parry; Dirty Fighting** | HP 150; Rallying Call also grants 5 temp HP | HP 170; Rallying Call reaches **two** allies |
| **Silt elemental** (E7) | HP 120; Engulf recharge **6** only; at most 1 silt-spawn split | **HP 152; Engulf 5–6; at most 2 splits** | HP 180 (≈ CR 8); at most 3 splits; gains **Tidal Shove** (bonus action: one creature within 10 ft, DC 16 Str save or pushed 10 ft toward the upstream parapet) | HP 210 (≈ CR 9); at most 4 splits; Tidal Shove; **Legendary Resistance (1/day)** |

**The elemental's Draining is the same at every size:** −15 HP at the end of
each round from round 4, collapse at the end of round 8. The fight is tuned
to the Draw-Down, not to the party, so a big party ends it sooner by damage
and a small party ends it by surviving.

---

## Success Requirements

Group checks scale by **one success**, never by DC.

| Check | Size 3 | **Size 4** | Size 5 | Size 6 |
|---|---|---|---|---|
| **Install Master Gear** (before 2 failures; DC 14) | 2 | **3** | 3 | 4 |
| **Diversion Mouth — small job** (before 2 failures; DC 14) | 2 | **2** | 3 | 3 |
| **Whole plug — big job** (DC 14) | 4 | **5** | 6 | 7 |
| **Great Wheel** (before 3 failures; DC 15) | 4 | **5** | 5 | 6 |
| **Hand-crank a gate** (before 2 failures; DC 15) | 2 | **3** | 3 | 4 |
| **Stoplogs** (before 2 failures; DC 13) | 2 | **3** | 3 | 3 |
| **Characters at the wheel per round** | 2 | **3** | 3 | 4 |

---

## Ivo's Role

| Size | Ivo |
|---|---|
| **3** | **Fights.** AC 14, HP 35, Multiattack (two shortswords, +5, 1d6+3). CR 1. Stays with the party; doesn't cost the 5-minute slow-down (he's spry with a purpose). |
| **4** | **Guide.** AC 12, HP 22 (main file). Doesn't fight unless cornered. Best used waiting at the levers. |
| **5–6** | **Guide, optional.** Same profile. With this many characters, suggest he stays at the levers from the start — the party has enough hands. |

---

## Pace Hints

| Size | What happens at the table | DM adjustment |
|---|---|---|
| **3** | Fewer attacks per round → fights run more rounds, but decisions are quick. | Lean on the social routes in E2 and E6. If behind, the E1 crayfish dive after the Snapper is bloodied. |
| **4** | Baseline. | Use the Pacing Sheet as written. |
| **5–6** | More voices, slower decisions, more splitting up. | Cut the Cistern and Pump Room to a sentence each unless asked; ask the table for **one spokesperson per room** for plans. Expect the party to split (some at the levers, some in the Cache) — that's fine and fast; run the Run separately per group. |

---

## Level Notes

The module is tuned for **level 5**. If the table is a level off:

| Party level | Adjustment |
|---|---|
| **4** | Use the next-smaller size's foe counts and boss rows (a 4-character level-4 party uses the size-3 column). A 3-character level-4 party uses the size-3 column and drops one standard foe (not a boss) from every fight. Hazard and trap DCs −1. |
| **5** | As written. |
| **6** | Use the next-larger size's foe counts and boss rows. A 6-character level-6 party uses the size-6 column and adds two standard foes to every fight. Hazard and trap DCs +1. The elemental's slams become 3d8+6. |

Do **not** change the timer, the time costs, or the success requirements for
level.

---

## Rewards

The town's payment scales with party size; items, potions, and found coin
don't.

| Size | Town payment multiplier |
|---|---|
| 3 | ×0.75 |
| **4** | **×1** |
| 5 | ×1.25 |
| 6 | ×1.5 |
