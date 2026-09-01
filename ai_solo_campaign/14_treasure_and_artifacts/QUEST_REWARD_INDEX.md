# QUEST_REWARD_INDEX.md — Reward Hooks by Quest Category

---
type: index
secrecy: mixed
status: static
region: Orrun
level_range: 1-20
related: [FACTION_REWARDS.md, NONCOMBAT_REWARDS.md, MAGIC_ITEM_INDEX.md, ARTIFACT_INDEX.md, ../09_quests/QUEST_INDEX.md, ../09_quests/MAJOR_CAMPAIGN_QUESTS.md, ../09_quests/DEVELOPED_QUESTS_INDEX.md]
tags: [type:index, secrecy:mixed, quest-reward, hooks, solo-tuned]
---

## AI Use

Reward **hooks** keyed to quest *categories*, so the AI DM can attach a level-appropriate, theme-appropriate reward to any quest without inventing it cold. This file does not re-list every quest (see `../09_quests/`); it gives each category a reward palette + worked examples. Apply pacing from `SOLO_REWARD_BALANCE.md`. Always offer a reward for **noncombat resolution** equal to the combat one (project rule).

## Reward Palette by Category

> For each: **default palette** (what fits) + **example** (a concrete hook tied to existing content).

---

### Main / Campaign Quests (Q_MAJOR_001–028)

- **Palette:** mystery-linked relics (`ARTIFACT_INDEX.md`), Concord Script/archive access, faction standing leaps, major information unlocks, endgame artifact *fragments* (gated). Coin is secondary; **revelation and leverage** are the real rewards.
- **Solo tilt:** main-quest rewards should make the *next* stage survivable (a node-detector before delving toward nodes; a Thin-touch ward before relic-heavy beats).
- **Examples:**
  - Resolving Wren's rite (Act 1) → the **Warden's Unlit Lantern** path opens (Warden trust) + an M1 clue confirmed.
  - Reaching the Sealed Archive (Act 3) → **The Sealed Archive Key** + C-M6/M9 truth-cache.
  - Late convergence → **Custodian's Compass** / endgame relics, M6–M9 gated.

### Faction Quests (Stage 8 chains, `faction_quests/`)

- **Palette:** the ranked tracks in `FACTION_REWARDS.md` — tokens → tools → relics + titles. Standing changes (up with one faction, often down with a rival).
- **Solo tilt:** access and allies over loot; a faction quest is a great place to grant a recurring ally or a safe-house.
- **Example:** Mourners' chain Rank 3 → **The Grief-Glass** entrusted + grief-truth (M6 gated) + *Keeper of the Quiet* standing.

### Regional Quests (`regional_quests/`, `by_region/`)

- **Palette:** the region's signature minor-magic + consumables (`REGIONAL_TREASURE_TABLES.md`), local standing/reputation, regional access (a guide, a route, a sanctuary), region-flavored coin/gems.
- **Solo tilt:** regional rewards build the **reputation** web that opens the region for repeat play.
- **Example:** Coast "Lost Crew"/"Drowned-Bell" quests → **Wrackmouth Diving-Mask** or **Lantern of the Held Breath** + Coast standing + a tide-reader ally (Mabon Crale).

### Personal Quests

- **Palette:** relationship rewards (confidant, debt owed, companion), a keepsake item (often a *sentient* or minor-magic item with meaning — e.g. **Brightneedle**), and emotional/thematic payoff (a soul laid to rest).
- **Solo tilt:** for a lone PC, a personal quest's *relationship* reward is often the most valuable thing in the campaign.
- **Example:** Helping Brightneedle finish the cobbler's last work → he passes on peacefully; the awl becomes a treasured keepsake; a quiet hopeful M5 demonstration.

### Side Quests / Jobs / Bounties (`hooks_and_rumors/`, `HOOKS_TABLE.md`)

- **Palette:** coin (band-appropriate), consumables, minor favors, a single piece of information, a faction token. Quick, clean, level-scaled.
- **Solo tilt:** the consumable-and-coin layer that keeps a solo PC stocked between big beats (`SOLO_REWARD_BALANCE.md` § Consumable Pacing).
- **Example:** a Hartfell bounty on a Mast-Beast → coin + a **Tollwood Bark-Charm** + Hartfell goodwill.

### Dungeon Quests (`../10_dungeons_and_ruins/`)

- **Palette:** the dungeon's signature reward (`DUNGEON_REWARD_INDEX.md`) + band-appropriate hoard + any site-specific cursed/relic item.
- **Solo tilt:** a notable reward per major site; not every room is loot; retreat-with-partial-reward is always possible.
- **Example:** `THE_DEEP_ADIT` → "old glass" relic samples (M3 proof) + Heights gems + a Thin-touch danger (telegraphed).

### Mystery Quests (`../11_mysteries_and_secrets/`)

- **Palette:** **information is the reward** — a confirmed clue, a decoded record, a witness's testimony, archive/Script access. Sometimes a relic that *is* a clue (Grief-Glass, Ledger of Quiet Debts).
- **Solo tilt:** mystery rewards must respect the three-clue rule and the secret-protection matrix — never a single reward that resolves the apex.
- **Example:** decoding a Star-Stone relay → confirms M2 (the network is continental) + a **Whisper-Stone of Candlewick**.

### Travel / Exploration Quests

- **Palette:** maps, routes, mobility items (`MAGIC_ITEM_INDEX.md` mobility entries), region discoveries, salvage.
- **Example:** charting a safe Coast passage → **Hollow Gulf Reef-Charts** (if far) or Coast route-access + salvage.

---

## Reward-Sizing Quick Reference (by quest tier)

| Quest tier | Coin (typical) | Item reward | Plus |
|---|---|---|---|
| Minor job (L1–4) | 1–50 gp | a consumable or Common | a favor/token |
| Side quest (L1–8) | 25–500 gp | a Common/Uncommon | local standing |
| Regional quest (L1–12) | scaling to band | region's signature magic | reputation + access |
| Faction quest (any) | stipend | rank track item | standing (± rivals) |
| Dungeon quest | band hoard | signature reward | site relic/curse |
| Main quest | secondary | mystery relic | **revelation + leverage** |

## Noncombat-Parity Rule (restate)

For every quest, define **at least one nonviolent path that yields the full reward.** If the player talks down the Reedwarden instead of killing him, they still get the route/standing/loot. A clever solution is *more* impressive solo and should never pay less.

## State Updates

On quest reward, update `INVENTORY_AND_REWARDS.md`, `FACTION_STATE.md` (standing), `RELATIONSHIPS.md` (allies/debts), `CONSEQUENCES.md` (who noticed), and `KNOWN_CLUES.md` (information rewards). Mirror major relics into `ARTIFACT_INDEX.md` ownership notes if persistent.

## Related Files

- [`FACTION_REWARDS.md`](FACTION_REWARDS.md)
- [`DUNGEON_REWARD_INDEX.md`](DUNGEON_REWARD_INDEX.md)
- [`NONCOMBAT_REWARDS.md`](NONCOMBAT_REWARDS.md)
- [`../09_quests/QUEST_INDEX.md`](../09_quests/QUEST_INDEX.md)
- [`../09_quests/MAJOR_CAMPAIGN_QUESTS.md`](../09_quests/MAJOR_CAMPAIGN_QUESTS.md)
