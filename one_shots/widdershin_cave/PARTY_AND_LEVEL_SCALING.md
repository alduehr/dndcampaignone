# Widdershin Cave — Party & Level Scaling

Non-canon, standalone — see [`../README.md`](../README.md) and
[`WIDDERSHIN_CAVE.md`](WIDDERSHIN_CAVE.md) for the base adventure this
converts.

Covers **any party from 3 to 6 characters at any average level from 1 to 4.**
The base module is written for **four characters at level 1**; this file
covers every other combination. Two independent dials do the work:

- **Party SIZE** drives *how many* foes you fight, plus Locke's HP and action
  economy.
- **Average party LEVEL** drives *how tough each one is.*

Nothing else changes. DCs, puzzle logic, clue routes, NPC behavior, morale,
telegraphs, and retreat options are **identical at every scale** — that's
deliberate, and it's also just correct: those things don't get harder because
you brought friends.

> **This is a party adventure.** It is not built for one or two characters —
> a solo PC loses the Zone 6 fight on the math even in Phase 2. If you want to
> run it for one player, give them a sidekick or two and use the size-3 row.

---

## How To Use This

1. **Find your Size row** (3–6) in the **Foe Count Table**. That's how many
   Reef Crabs and Skeletons appear in Zones 2 and 4.
2. **Find your Level row.** If every character is within 1 level of another,
   use the rounded average. If the spread is wider, see **Mixed-Level
   Parties** — don't average a level 1 and a level 4 together.
3. **Combine them.** Count comes from Size, stats come from Level.
4. **Apply the Size Tier** (Locke's HP, Multiattack, lair action, Tide Call
   pacing).
5. **Scale treasure** using the table at the end.

---

## Size Tiers

| Tier | Party Size | Locke HP × | Locke gains |
|---|---|---|---|
| **A** | 3–4 | ×1.15 | — |
| **B** | 5–6 | ×1.6 | **Multiattack** and a **lair action** (below) |

Tier B exists because HP alone cannot make a single-actor boss threatening to
six characters. Locke with 200 HP and one attack per round is a long fight in
which nobody is ever in danger. He needs *actions*, not hit points.

**Multiattack (Tier B only):** Locke makes two Cutlass of Drowning attacks
instead of one.

**Lair action (Tier B only):** on initiative count 20 (losing ties), the tide
shifts under the party — one creature Locke can see in the open water makes a
**DC 13 Strength save** or is dragged 10 ft toward the sea-arch. No damage.
This does **not** count against the Tide Call cap and does not require his
action.

---

## Foe Count Table (by Party Size)

Applies to **Zone 2 (Reef Crabs)** and **Zone 4 (Skeleton Crew)**. Individual
stats come from the Toughness Ladder, not this table.

| Party Size | Reef Crabs (Zone 2) | Skeletons (Zone 4) |
|---|---|---|
| 3 | 4 | 4 |
| 4 | 5 | 4 |
| 5 | 6 | 5 |
| 6 | 7 | 6 |

Skeleton counts stay deliberately low. Zone 4's participation problem is
solved by **deployment**, not by numbers — one skeleton holds the tunnel, two
push out into Zone 3 to fight in the open, the rest use shortbows down the
tunnel (see the base module's Zone 4 entry). Adding bodies to a single-file
queue makes the fight longer, not harder.

**At average level 3+, some skeletons are replaced by "Bosun's Bones" elites**
— this *replaces* standard skeletons, it does not add elites on top. Use
**1 Bosun** at size 3–4, **2 Bosuns** at size 5–6. A size-4 party at level 3
fights 3 standard + 1 Bosun, not 4 + 1.

Reef Crabs stay a single tier per level at every size — Zone 2 is fully
avoidable via the dry-spine Stealth route, so it can look intimidating on
paper without needing elite variants.

---

## Toughness Ladder (by Average Level)

Ability modifiers, vulnerabilities, and conditions are unchanged from the base
module at every level; only the numbers below move.

### Reef Crab
| Level | CR | AC | HP | Attack | Notes |
|---|---|---|---|---|---|
| 1 | 1/8 | 15 | 6 | claw +3, 1d4+1 | grapple escape DC 11 |
| 2 | 1/8 | 15 | 8 | claw +4, 1d4+2 | escape DC 11 |
| 3 | 1/4 | 16 | 12 | claw +5, 1d6+2 | escape DC 12 |
| 4 | 1/4 | 16 | 20 | claw +6, 2d6+3 | escape DC 12; single attack, no multiattack — tougher and harder-hitting rather than doubling actions |

**Str +1, Dex +0, Con +1, Int −4, Wis +0, Cha −3** at every level. A grappling
crab always drags its catch toward deep water; that's a comedy beat, not a
drowning mechanic.

### Standard Skeleton (Zone 4)
| Level | CR | AC | HP | Melee (scimitar) | Ranged (shortbow) |
|---|---|---|---|---|---|
| 1 | 1/4 | 13 | 13 | +3, 1d6+1 | +3, 1d6 |
| 2 | 1/4 | 13 | 15 | +4, 1d6+2 | +4, 1d6+1 |
| 3 | 1/2 | 14 | 18 | +5, 1d6+3 | +5, 1d6+2 |
| 4 | 1/2 | 14 | 20 | +6, 1d6+4 | +6, 1d6+3 |

**Str +0, Dex +2, Con +1, Int −2, Wis −1, Cha −3.** Vulnerable to
bludgeoning; immune to poison damage and the poisoned and exhaustion
conditions; resistant to cold damage. Unchanged at every level. Turned
normally, no special ruling.

### Elite Skeleton — "Bosun's Bones" (level 3+ only)
| Level | CR | AC | HP | Main Action | Shield Bash (bonus action) |
|---|---|---|---|---|---|
| 3 | 1 | 16 | 24 | scimitar +5, 1d6+3 | +5 to hit, reach 5 ft, **1d4 bludgeoning**; on a hit, **DC 13 Strength save** or pushed 5 ft away |
| 4 | 2 | 17 | 30 | Multiattack: 2× scimitar +6, 1d6+4 | +6 to hit, reach 5 ft, **1d4 bludgeoning**; on a hit, **DC 14 Strength save** or pushed 5 ft away |

**Str +3, Dex +1, Con +2, Int −2, Wis +0, Cha −2.** Same
vulnerability/immunities as the standard line. Shield Bash is a real bonus
action usable the same turn as its main action — a genuine action-economy
threat, which is why it's specified precisely rather than left as a vague
"knocks them back." The Bosun is also the one holding the tunnel; if you want
the chokepoint to matter, put it there.

### Captain Perrin Locke, the Widdershin Warden
Base HP before the Size Tier multiplier, then the tiered results:

| Level | CR | Base HP | **Tier A HP** (size 3–4) | **Tier B HP** (size 5–6) | Cutlass of Drowning |
|---|---|---|---|---|---|
| 1 | 2 | 35 | **40** | **55** | +4, 1d8+2 slashing + 1d6 cold |
| 2 | 3 | 40 | **45** | **65** | +5, 1d8+3 slashing + 1d6 cold |
| 3 | 3 | 50 | **60** | **80** | +6, 1d8+4 slashing + 2d6 cold |
| 4 | 4 | 60 | **70** | **95** | +7, 2d6+4 slashing + 1d6 cold |

At level 3, Tide Call's prone effect also deals 1d6 cold to anyone it knocks
down. At level 4 the cutlass becomes a heavier two-handed swing and the cold
rider stays modest, so a single hit doesn't spike too hard against a squishier
caster. AC stays 13 at every level — he's slow and solid, not evasive, and
lowering the miss rate keeps the fight moving.

**Everything else about Locke is identical at every level and size:** the black
thread, Idol Resistance, **the half-HP gate**, the ways to get the idol off him
once that gate opens, Phase 2, **the three-round altar rite**, the always-open
parley window (which gives information, never peace), Tam's distraction, the
Turn Undead ruling, his refusal to target Tam, and his refusal to follow a
retreat past the vault door.

**The fight is never skippable at any size or level.** The idol cannot come off
Locke while he is at or above half HP, and returning it always costs three
held rounds afterward. Scaling changes how long that takes and how much it
hurts — it never changes whether it happens. The only size-and-level
concession: a **party of three at level 1** may reduce the altar rite to
**two rounds** if the fight is already running long. Never reduce the half-HP
gate.

**Half-HP thresholds, for quick reference** (Locke's tiered HP ÷ 2 — the point
at which the thread goes slack and every removal route opens):

| Level | Tier A (size 3–4) | Tier B (size 5–6) |
|---|---|---|
| 1 | 40 → **20** | 55 → **28** |
| 2 | 45 → **23** | 65 → **33** |
| 3 | 60 → **30** | 80 → **40** |
| 4 | 70 → **35** | 95 → **48** |

At every combination that's roughly **2–3 rounds of party damage** to reach the
gate, then a round to take the idol, then the three-round rite — a **6–7 round
climax** whatever the table size, which is what you want from a one-shot boss.

**Tide Call is hard capped at twice per fight, always.** Only the *timing*
shifts:

| Tier | First use | Second use |
|---|---|---|
| A (size 3–4) | Guaranteed by round 3 if it hasn't recharged naturally | Whenever it next recharges |
| B (size 5–6) | Guaranteed by round 2 | Guaranteed by round 5 if it hasn't recharged naturally |

**Wailing Command is unchanged at every size and level** — surviving Zone-4
skeletons only, 2 rounds of travel, telegraphed. If the party cleared Zone 4,
it does nothing but a mournful shout. **Never manufacture new skeletons at any
party size.** A bigger table gets a bigger fight in Zone 4 up front, which is
where that pressure belongs, and a boss with more actions in Zone 6.

---

## Mixed-Level Parties

**If every character is within 1 level of another** (e.g. a mix of 2s and
3s), average, round to the nearest whole level, and use that row normally.
The math is forgiving enough that small spreads need no special handling.

**If the spread is wider than 1 level** (e.g. a level 1 and a level 4 in the
same party), do **not** average — a level-4 attack line can drop a level-1
character in one hit, which isn't a fight, it's a coin flip on a PC's life.
Instead:

1. **Use the lowest character's level** for every foe's **AC and attack
   line** from the Toughness Ladder. This keeps the worst-case hit survivable
   for your most fragile character.
2. **Add HP instead of damage:** a flat **+10% HP to every foe** for each full
   level of spread beyond 1, applied on top of the Size Tier multiplier. Round
   individual foes to the nearest whole number and Locke to the nearest 5.
3. **Level-3+ features follow the lowest level too** — if your lowest
   character is level 1, no Bosun's Bones even if the average would qualify.

**Worked example — a party of 4 containing a level 1 and a level 4** (size 4,
spread 3, so 2 levels beyond 1 → **+20% HP**):
- **Level-1 stat lines** for AC and attacks on everything.
- Crabs (size 4 → 5 of them): 6 × 1.2 = 7.2 → **7 HP** each.
- Skeletons (size 4 → 4 of them): 13 × 1.2 = 15.6 → **16 HP** each. No Bosun.
- Locke: base 35 × 1.15 (Tier A) × 1.2 = 48.3 → **50 HP**, Level-1 attack
  line, Tier A rules.
- The level-4 character will find the raw numbers easy. That's intentional —
  this rule protects the fragile character's survival. If you want more
  challenge for the higher-level members specifically, lean on Tide Call
  positioning and let the Bosun (at its *individual* level, where the fiction
  allows) target the tougher character, rather than raising damage against
  everyone.

---

## Treasure Scaling

Keep individual finds **unchanged at every scale** — the 22 gp strongbox and
Scrimshaw #1 in Zone 2, the 35 gp strongbox, silver flask, knucklebone and
Scrimshaw #2 in Zones 3–4, and the tide-chart disc. They're flavor and clue
delivery, not a per-PC budget line.

Scale the Zone 6 payout and the consumables:

| Party Size | Sea-chest coin | Widdershin Coins | Potions of healing (Zone 4) |
|---|---|---|---|
| 3–4 | 300 gp | 2 | 2 |
| 5–6 | 650 gp | 3 | 4 |

That lands at roughly 100–110 gp per character at every size, which is a real
reward for one session at these tiers without distorting anything.

**At size 5–6 only,** add **2 potions of water breathing** to the smuggler's
medicine chest — smugglers would have them, they're useful on the exit swim,
and they give a big party a second interesting consumable to fight over.

**Fixed at every size and level:**
- **The boarding cutlass:** exactly **one**, always. Unique collectible, not
  a per-character reward.
- **Tam's Knucklebone:** exactly **one**, and only if the party earns it.
- **Widdershin Coins and the Knucklebone recharge once per adventure at every
  level.** Don't bump the rate for higher-level parties; they're trinkets, not
  build-arounds, and a flat rule is easy to track when several characters are
  carrying one.

---

## Worked Examples

**4 level-1 characters** — the base module as printed. Size 4 → 5 Crabs /
4 Skeletons, all Level-1 stats (no Bosun; that's level 3+). Locke: **40 HP**,
half-HP gate at **20**, Level-1 line, **Tier A** — no Multiattack, no lair
action, Tide Call guaranteed by round 3, cap 2. Altar rite: 3 rounds. Loot:
300 gp, 2 Widdershin Coins, 1 cutlass, 2 potions of healing.

**3 level-3 characters.** Size 3 → 4 Crabs (AC 16 / HP 12 / escape DC 12) and
4 Skeletons, **1 swapped for a Bosun** → 3 standard (Level-3 line) + 1 Bosun
(AC 16 / HP 24, scimitar +5 1d6+3, Shield Bash +5 for 1d4 bludgeoning, DC 13
push). Put the Bosun in the tunnel mouth. Locke: **60 HP**, half-HP gate at
**30**, Level-3 line (+6, 1d8+4 + 2d6 cold; Tide Call adds 1d6 cold to anyone
it knocks down), **Tier A**. Altar rite: 3 rounds — with only three characters
this is the tightest version of the climax in the whole range, and the most
exciting. Loot: 300 gp, 2 Coins, 1 cutlass, 2 potions of healing.

**5 level-4 characters.** Size 5 → 6 Crabs (AC 16 / HP 20, claw +6 2d6+3,
escape DC 12) and 5 Skeletons, **2 swapped for Bosuns** → 3 standard (Level-4
line) + 2 Bosuns (AC 17 / HP 30, Multiattack 2× scimitar +6 1d6+4, Shield Bash
+6 for 1d4 bludgeoning, DC 14 push). Locke: **95 HP** (Level-4 base 60 × 1.6),
half-HP gate at **48**, Level-4 line (+7, 2d6+4 + 1d6 cold), **Tier B** —
Multiattack, lair action on initiative 20, Tide Call guaranteed by round 2 with
the second by round 5, cap 2. Altar rite: 3 rounds, and with five characters
someone can afford to stand still and hold it. Loot: 650 gp, 3 Coins, 1
cutlass, 4 potions of healing, 2 potions of water breathing. Budget **~4 hours.**

**6 level-4 characters** — the top of the range. Size 6 → 7 Crabs (AC 16 /
HP 20, claw +6 2d6+3, escape DC 12) and 6 Skeletons, **2 swapped for Bosuns**
→ 4 standard (Level-4 line) + 2 Bosuns (AC 17 / HP 30, Multiattack 2×
scimitar +6 1d6+4, Shield Bash +6 for 1d4 bludgeoning, DC 14 push). Locke:
**95 HP**, Level-4 line (+7, 2d6+4 + 1d6 cold), **Tier B** — **Multiattack
(two cutlass strikes per round)**, **lair action on initiative 20**, Tide Call
guaranteed by round 2 with the second by round 5, still capped at 2. Wailing
Command calls survivors only; no manufactured reinforcements even here. Loot:
650 gp, 3 Coins, 1 cutlass, 4 potions of healing, 2 potions of water
breathing. Budget **~4–4.5 hours** for this table, not 3.

**Anything else** (5 level-2s, a same-band 2/3/3/3 group, etc.): read your
Size row for counts and the Size Tier, your Level row for stats — or the
Mixed-Level rule if the spread is wide. There is no combination of 3–6
characters at levels 1–4 this system doesn't cover.
