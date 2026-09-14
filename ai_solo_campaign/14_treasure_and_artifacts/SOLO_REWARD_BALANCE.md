# SOLO_REWARD_BALANCE.md — Calibrating Rewards for One Player Character

---
type: index
secrecy: mixed
status: static
region: Orrun
level_range: 1-20
related: [TREASURE_INDEX.md, MAGIC_ITEM_INDEX.md, REGIONAL_TREASURE_TABLES.md, CONSUMABLES_AND_MINOR_MAGIC.md, ../13_encounters_and_bestiary/SOLO_ENCOUNTER_SCALING.md]
tags: [type:index, secrecy:mixed, treasure, reward-balance, solo-tuned]
---

## AI Use

Load whenever placing or awarding treasure. This file is the **pacing governor** for the whole Stage 14 library: it tells the AI DM how much, how often, and what kind of reward a single PC should get so the campaign stays both survivable and dangerous. When any other treasure file says "level-appropriate," this file defines what that means for one character.

## Core Problem

Standard 5e treasure assumes a four-PC party. A solo PC:
- Takes a larger share of every hoard (good), but also
- Has no party to cover gaps (no backup healer, no backup tank, no second set of skills), so
- Needs **slightly more recovery and utility support** than a single party member would,
- But must **not** be handed a stack of combat-boost items that trivialize the telegraphed-danger design in `../13_encounters_and_bestiary/`.

The answer is **breadth over spikes**: many small advantages (consumables, utility, mobility, information, social leverage) rather than a few big numerical boosts.

---

## The Five Balance Principles

1. **Recovery first.** A solo PC's biggest weakness is the death spiral. Prioritize healing potions, stabilization charms, rests, and "second-chance" items over raw damage. A solo PC should rarely be more than one tier behind on healing access.
2. **Utility over numbers.** Information tools, mobility, stealth, light/warmth/water, and social leverage are worth more to a solo player than +X items. Weight rewards toward these.
3. **No early power spikes.** No flat numerical weapon/armor bonus (+1 or better) before **Rare tier is earned** (≈ level 5–6). Before that, use situational items (a weapon that works *only* against the restless dead; armor that helps *only* vs a hazard).
4. **No single "solve-everything" item.** Every powerful item has a cost, a charge limit, a downside, or a faction that wants it. The player should never own an item that removes a whole pillar of play.
5. **Danger is preserved.** Rewards make hard things *possible*, not *easy*. After a big reward, the next region/tier escalates to match (see `../13_encounters_and_bestiary/SOLO_ENCOUNTER_SCALING.md`).

---

## Permanent-Item Pacing (the safe baseline)

This is the **target rhythm** of permanent magic items for a solo PC. Treat as a guide, not a quota — the player can find more if they take risks, or fewer if they avoid danger (the world rewards engagement, not entitlement).

| Level | Recommended permanent items by now | Rarity ceiling earned |
|---|---|---|
| 1 | 0 (starting gear only) | — |
| 2 | 1 Common or 1 situational Uncommon | Common |
| 4 | 1–2 Uncommon | Uncommon |
| 6 | 2–3 Uncommon + 1 Rare | Rare |
| 8 | 3–4 Uncommon + 1–2 Rare | Rare |
| 10 | + first Very Rare in reach | Very Rare (lower) |
| 12 | 1–2 Very Rare | Very Rare |
| 14 | 2–3 Very Rare; first Legendary possible | Legendary (lower) |
| 16 | 1 Legendary | Legendary |
| 18 | 1–2 Legendary | Legendary |
| 20 | 2+ Legendary + endgame artifact access | Artifact |

**Attunement ceiling:** standard 5e cap of 3 attuned items applies. Because a solo PC has fewer hands, lean on this: 3 well-chosen attuned items is a complete late-game kit. Don't flood the player with attunement-hungry rewards they can't use.

---

## Consumable Pacing (the real solo lifeline)

Consumables do not cause power creep and are the safest way to keep a solo PC alive. Be **generous** here relative to permanent items.

| Level band | Healing potions on hand (typical) | Other consumables |
|---|---|---|
| 1–4 | 2–4 *Potion of Healing* equivalents available to buy/find | antitoxin, oil, a charm or two |
| 5–8 | 3–6 healing (incl. *Greater* by ~6) | scrolls of 1st–2nd, escape/utility tokens |
| 9–12 | several *Greater*/*Superior* | scrolls of 3rd–4th, situational relics |
| 13–16 | *Superior*/*Supreme* available | scrolls of 5th, powerful one-use relics |
| 17–20 | always topped up | high scrolls, endgame one-use items |

See `CONSUMABLES_AND_MINOR_MAGIC.md` for the menu. **Rule of thumb:** a solo PC entering a dungeon should be able to carry roughly 1.5× the healing a party member would.

---

## Currency Pacing (rough lifetime totals)

Coin should track the regional economy (`ECONOMY_AND_PRICING_GUIDE.md`), not a national average. The Reach is poor; Caradril and Glassmere are rich. Totals below are *campaign-cumulative ballpark* for a solo PC who engages with the world.

| Level band | Loose-coin order of magnitude (cumulative) | Notes |
|---|---|---|
| 1–4 | tens to low hundreds of gp | frontier poverty; a single gp matters |
| 5–8 | hundreds to ~2,000 gp | faction stipends, city work, first hoards |
| 9–12 | thousands to ~15,000 gp | letters of credit, trade shares, noble pay |
| 13–16 | tens of thousands | imperial hoards, ancient Concord caches |
| 17–20 | massive historical hoards | money stops being the point; access/legacy do |

Money is a means (services, hirelings, property, bribes, leverage), not a win condition. See `NONCOMBAT_REWARDS.md`.

---

## What to Weight UP for a Solo PC

- Healing, stabilization, and "don't-die" items.
- Escape/mobility (short teleport, climb, water-breathing, fly-for-a-round).
- Information (maps, identify-equivalents, lore tools, detect tools).
- Stealth and avoidance (the solo player's best survival tactic).
- Social leverage (an item or favor that turns a fight into a conversation).
- Light, warmth, water, food, navigation (the Reach and far-north are harsh).

## What to Weight DOWN / Gate

- Flat +X weapons/armor before Rare tier.
- Items that grant at-will hard crowd-control (a solo PC abusing CC trivializes telegraphed danger; cap to charges).
- Anything that removes a pillar of play (at-will invisibility before mid-tier; at-will flight before high-tier; unlimited free resurrection — the Remembrance cosmology makes this *especially* off-limits, see below).
- Duplicated power (don't give a second item that does what an owned item already does).

---

## Remembrance Cosmology Balance Rules (campaign-specific)

The setting's central conceit constrains rewards in three hard ways:

1. **No easy resurrection items.** Resurrection is dangerous in the Reach (see `../03_canon/MAGIC_RULES.md`: DC check, wrong-come-back risk). Do **not** hand the player a *Revivify*-on-a-stick. Items that touch death/the dead always carry the harvest's fingerprints — a clue, a cost, or a curse.
2. **Remembrance relics are plot before power.** "Old glass" / "quiet-coin" / "saint's-bones" relics primarily deliver clues, trigger **Thin-touch** (disadvantage on Death saves until a true rite/shrine long-rest) on careless contact, and attract faction interest. Their mechanical effect is secondary and always limited. They are never a clean upgrade.
3. **Apex truth is never in an item description.** No item the player can acquire spells out the harvest, the Hollow Court, or the keystone before those are earned through play. Endgame artifacts (`ARTIFACT_INDEX.md`: Harvest Engine Shard, Quiet Country Vessel, Last Voice) require M6–M9 revelations to *understand and use*, even if held earlier.

---

## Reward Cadence by Source

- **Dungeons:** each major site gives one notable reward + level-appropriate mundane treasure (`DUNGEON_REWARD_INDEX.md`). Not every room is loot.
- **Quests:** rewards scale to quest tier; noncombat resolutions are rewarded as richly as combat ones (`QUEST_REWARD_INDEX.md`, `NONCOMBAT_REWARDS.md`).
- **Factions:** ranked tracks; advancement, not loot-piñatas (`FACTION_REWARDS.md`). The Hollow Court's "gifts" are always traps.
- **Regional ambient:** mundane flavor, minor magic, gems/art per region (`REGIONAL_TREASURE_TABLES.md`).
- **Selling/recovery:** a poor frontier means *selling* relics is itself a choice with consequences (Ledger interest, Mourner disapproval, Gravecaller attention).

---

## Solo "Insurance" Floor

To avoid cheap death (a core project rule), ensure the player always has access to **at least one** of these per tier, even on a stingy run:
- A reliable healing source (potion supply, a temple, a Mourner rite).
- One escape/retreat option (item, ally, or known route).
- One way to gain advantage before a telegraphed boss (scouting tool, weakness clue, recruitable help).

If a player has burned all three, the DM should surface a fair opportunity to restock before the next lethal beat. This is a floor, not a handout.

---

## Related Files

- [`TREASURE_INDEX.md`](TREASURE_INDEX.md)
- [`REGIONAL_TREASURE_TABLES.md`](REGIONAL_TREASURE_TABLES.md)
- [`CONSUMABLES_AND_MINOR_MAGIC.md`](CONSUMABLES_AND_MINOR_MAGIC.md)
- [`../13_encounters_and_bestiary/SOLO_ENCOUNTER_SCALING.md`](../13_encounters_and_bestiary/SOLO_ENCOUNTER_SCALING.md)
- [`../03_canon/MAGIC_RULES.md`](../03_canon/MAGIC_RULES.md)
