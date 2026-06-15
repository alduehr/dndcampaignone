# TREASURE_INDEX.md — Master Index of Treasure, Artifacts, and Rewards

---
type: index
secrecy: mixed
status: static
region: Orrun
level_range: 1-20
related: [MAGIC_ITEM_INDEX.md, ARTIFACT_INDEX.md, REGIONAL_TREASURE_TABLES.md, FACTION_REWARDS.md, DUNGEON_REWARD_INDEX.md, QUEST_REWARD_INDEX.md, CONSUMABLES_AND_MINOR_MAGIC.md, NONCOMBAT_REWARDS.md, CURSED_ITEMS.md, SENTIENT_ITEMS.md, ECONOMY_AND_PRICING_GUIDE.md, SOLO_REWARD_BALANCE.md, ../02_runtime_state/INVENTORY_AND_REWARDS.md]
tags: [type:index, secrecy:mixed, treasure, reward, master-index, solo-tuned]
---

## AI Use

**The Stage 14 master file.** Start here when the player finds, earns, buys, or sells anything. This index tells the AI DM which treasure file to load for a given need, summarizes the campaign's reward philosophy, and defines how official (Track A) vs custom (Track B) items are handled. Load alongside the runtime `../02_runtime_state/INVENTORY_AND_REWARDS.md`.

## Reward Philosophy (one screen)

- **Solo-first:** breadth over spikes; recovery and utility over flat bonuses; never a "solve-everything" item. Full rules: `SOLO_REWARD_BALANCE.md`.
- **Danger preserved:** rewards make hard things *possible*, not easy; the world escalates to match.
- **Noncombat parity:** clever/peaceful solutions earn rewards equal to combat ones.
- **Remembrance-bound:** items that touch death/the dead carry the harvest's fingerprints — clue, cost, or curse; never easy resurrection; apex truth never spelled out in an item.
- **Intentional placement:** no random artifact drops; every relic has an owner, history, and interested faction.

---

## File Map (what to load when)

| Need | File |
|---|---|
| Pace/amount of rewards for one PC | `SOLO_REWARD_BALANCE.md` |
| A custom magic item (Track B) | `MAGIC_ITEM_INDEX.md` |
| A major relic/artifact (12 named) | `ARTIFACT_INDEX.md` |
| Ambient loot by region/level | `REGIONAL_TREASURE_TABLES.md` |
| Potions/scrolls/charms/one-use | `CONSUMABLES_AND_MINOR_MAGIC.md` |
| What a faction gives (ranked) | `FACTION_REWARDS.md` |
| A specific dungeon's loot | `DUNGEON_REWARD_INDEX.md` |
| A quest category's reward palette | `QUEST_REWARD_INDEX.md` |
| Social/political/info/access rewards | `NONCOMBAT_REWARDS.md` |
| Cursed/dangerous rewards | `CURSED_ITEMS.md` |
| Sentient items (run as mini-NPCs) | `SENTIENT_ITEMS.md` |
| Prices, coin, gems, services | `ECONOMY_AND_PRICING_GUIDE.md` |
| Coverage/QA | `REWARD_PLACEMENT_AUDIT.md` |
| Runtime: what the player owns now | `../02_runtime_state/INVENTORY_AND_REWARDS.md` |

---

## Official vs Custom Items — Two-Track Handling

Mirrors the Stage 13 source-handling decision.

- **Track A — Official D&D items (reference only).** Named with a source shorthand (**2024 DMG**, **2024 MM**, **MotM**, **VRGtR**, etc.), rarity, type, fit-rationale, and placement note. **Never reproduce official item text, properties, or stat numbers.** The AI DM pulls exact mechanics from the cited book at the table. Used mainly for common consumables (`Potion of Healing`, spell scrolls, `Alchemist's Fire`) and a handful of generic utility items.
- **Track B — Custom campaign items (original).** Every item in `MAGIC_ITEM_INDEX.md`, `ARTIFACT_INDEX.md`, `CURSED_ITEMS.md`, `SENTIENT_ITEMS.md`, and the named consumables in `CONSUMABLES_AND_MINOR_MAGIC.md`. Each is tagged **ORIGINAL CAMPAIGN ITEM** with an abbreviated D&D-compatible prose effect (not a formatted stat block, not a copied one).

> When the player's reward could be either, prefer a **Track-B custom item** for anything signature/thematic and **Track-A reference** for routine consumables.

---

## Rarity Bands at a Glance

| Rarity | Level band | Role | Rough value |
|---|---|---|---|
| Common | 1–4 | minor utility | 50–100 gp |
| Uncommon | 1–8 | meaningful utility | 101–500 gp |
| Rare | 5–12 | significant power (earned) | 501–5,000 gp |
| Very Rare | 9–16 | major power | 5,001–50,000 gp |
| Legendary | 13–20 | campaign-defining | 50,000 gp+ |
| Artifact | level-independent | unique, plot-significant | cannot be bought |

Full pacing (items-by-level, consumable generosity, currency totals): `SOLO_REWARD_BALANCE.md`.

---

## The 12 Artifacts (quick roll-call)

Grief-Glass · Warden's Unlit Lantern · Ledger of Quiet Debts · Gravecaller's Knock · Compact Seal · Sealed Archive Key · Custodian's Compass · Quiet Country Vessel · Drowned Flame · Ash-Crown Fragment · Harvest Engine Shard · Last Voice. Detail + secrecy gates: `ARTIFACT_INDEX.md`. **Endgame (M6–M9 gated, DM-only true nature):** Quiet Country Vessel, Custodian's Compass, Harvest Engine Shard, Last Voice, Compact Seal trap.

## Counts (Stage 14 deliverables)

- Custom magic items: **38** (`MAGIC_ITEM_INDEX.md`; 48 originals counting artifacts) — target 30–50 ✓
- Named artifacts/relics: **12** — target 10–12 ✓
- Cursed items: **10** (+3 endgame cursed-class) — target 8+ ✓
- Sentient items: **6** — target 5+ ✓
- Faction reward tracks: **7 majors + 4 city blocs** ✓
- Regions with treasure flavor: **20/20** ✓
- Level bands with guidance: **5/5** ✓
- Dungeon reward hooks: **36 sites** ✓

---

## Secrecy Reminders (do not leak)

- **Hollow Court "rewards" are traps** — every Court-traced gift is a curse/leash (`FACTION_REWARDS.md` §7, `CURSED_ITEMS.md` #4/#9, `SENTIENT_ITEMS.md` #4).
- **No item description reveals the apex truth** (harvest, keystone, Hollow Court, Custodians) before it's earned. Endgame artifacts require M6–M9 to understand/use.
- **Remembrance relics are plot-before-power** and risk Thin-touch.
- DM-only blocks across these files are never surfaced to the player.

## Related Files

- [`SOLO_REWARD_BALANCE.md`](SOLO_REWARD_BALANCE.md)
- [`MAGIC_ITEM_INDEX.md`](MAGIC_ITEM_INDEX.md)
- [`ARTIFACT_INDEX.md`](ARTIFACT_INDEX.md)
- [`FACTION_REWARDS.md`](FACTION_REWARDS.md)
- [`DUNGEON_REWARD_INDEX.md`](DUNGEON_REWARD_INDEX.md)
- [`REWARD_PLACEMENT_AUDIT.md`](REWARD_PLACEMENT_AUDIT.md)
- [`../02_runtime_state/INVENTORY_AND_REWARDS.md`](../02_runtime_state/INVENTORY_AND_REWARDS.md)
