# PARTY_REWARDS_6_PLAYERS.md — Reward Conversion for a Six-Player Party

---
type: treasure
secrecy: mixed
status: static
region: Orrun
level_range: 1-20
related: [SOLO_REWARD_BALANCE.md, REWARDS_BY_LEVEL.md, TREASURE_INDEX.md, ARTIFACT_INDEX.md, ../01_runner_protocol/PARTY_MODE_PROTOCOL.md, ../13_encounters_and_bestiary/PARTY_SCALING_6_PLAYERS.md]
tags: [type:treasure, secrecy:mixed, party-mode, rewards, six-players]
---

## AI Use / DM Use

Load in **party mode** (see `../01_runner_protocol/PARTY_MODE_PROTOCOL.md`) in place of `SOLO_REWARD_BALANCE.md`'s pacing rules. All authored reward *placements* (`REGIONAL_TREASURE_TABLES.md`, `DUNGEON_REWARD_INDEX.md`, `QUEST_REWARD_INDEX.md`, `FACTION_REWARDS.md`) stay canonical — this file converts quantity and pacing, never what exists or where.

## The Inversion

Solo reward balance was built on: **breadth over spikes** (one PC must cover every role), a generous **consumable lifeline** (no healer), an **insurance floor** (no one to carry a downed PC), and slow attunement pacing. Six players invert every premise: roles are covered, healers exist, and the same item stream split six ways is famine.

## Rule 1 — Currency And Mundane Treasure

- **Multiply coin, trade goods, and gem/art values ×4–5** at every authored placement (not ×6 — parties also pool costs, and the frontier economy in `ECONOMY_AND_PRICING_GUIDE.md` should stay tight enough to make faction pay and patronage matter).
- Quest *payments* are renegotiated in-fiction: a patron who offered one capable hand 25 gp offers a six-blade company 100–150 gp — and now expects company-sized results. Let patrons say so.

## Rule 2 — Consumables

- **Multiply authored consumable drops ×3–4** (potions, scrolls, charms from `CONSUMABLES_AND_MINOR_MAGIC.md`), biased toward party-utility (healing for the frontline, a scroll the caster can actually use).
- **Delete the solo insurance floor.** The always-within-reach emergency potion reflex is solo-only; a party carries its own floor.

## Rule 3 — Magic Items (the pacing rule)

- **Solo pacing ≈ one meaningful item per tier for one PC. Party pacing: roughly one meaningful item per PC per tier**, arriving unevenly (hoards of 1–3, not six-packs).
- Convert authored placements by **adding items from the same authored pools**: when a dungeon's reward index places one signature item + minor magic, keep the signature item singular and add 1–2 more picks from the same region/tier row of `REGIONAL_TREASURE_TABLES.md` / `MAGIC_ITEM_INDEX.md`. Never invent outside the pools; never duplicate a signature/named item.
- **Attunement is unchanged per PC** — six players means up to 18 attunement slots; the pacing above deliberately never fills them.
- **Breadth-over-spikes relaxes:** role-focused items (the fighter's blade, the wizard's focus) are now correct picks; the solo rule against solve-everything items **stays** (no item that trivializes pillars for six people at once).

## Rule 4 — Relics, Artifacts, And Plot Items

- **All 12 named relics/artifacts (`ARTIFACT_INDEX.md`) remain singular and mystery-gated exactly as written.** They are plot, not loot; party mode changes who *carries* them, not how many exist.
- Remembrance relics keep their Thin-touch cost per *handler* — a party that passes one around shares the risk, which is a scene, not a bug.
- Endgame artifacts (M6–M9 gated) and the Hollow Court's poisoned gifts are unchanged — one court, one set of traps, six people to disagree about them.

## Rule 5 — Faction Rewards And Standing

- **Standing is earned party-wide by default** (the Wardens trust *the company*), but **ranked rewards from `FACTION_REWARDS.md` are per-PC** where they are personal (initiation, title, a Warden's lantern) — expect different PCs to climb different factions, which is the intended six-player texture.
- Faction *pay* follows Rule 1; faction *access/information* rewards are naturally party-shared and need no multiplication.

## Rule 6 — Non-Combat And Downtime Rewards

`NONCOMBAT_REWARDS.md` (access, favors, property, reputation) converts cleanly: property and safehouses simply house six; favors are per-PC or party-level as the fiction says. A six-player company accumulates *political* weight faster than one adventurer — let reputation rewards arrive a beat earlier than the solo pacing suggests.

## Quick Conversion Card

| Reward type | Conversion |
|---|---|
| Coin / goods / gems | ×4–5 at every placement |
| Consumables | ×3–4, party-utility bias; **no** insurance floor |
| Minor/medium magic items | +1–2 extra picks per hoard from the same authored pool; ~1 meaningful item per PC per tier |
| Signature / named items | Singular, as written |
| The 12 relics/artifacts | Untouched — plot, gated, singular |
| Faction pay | ×4–5; ranked personal rewards per-PC |
| Access / info / property / reputation | As written (naturally shared); reputation lands a beat earlier |

## Related Files

- [`SOLO_REWARD_BALANCE.md`](SOLO_REWARD_BALANCE.md) — the solo pacing this file converts from
- [`REWARDS_BY_LEVEL.md`](REWARDS_BY_LEVEL.md) · [`REGIONAL_TREASURE_TABLES.md`](REGIONAL_TREASURE_TABLES.md) · [`MAGIC_ITEM_INDEX.md`](MAGIC_ITEM_INDEX.md) · [`ARTIFACT_INDEX.md`](ARTIFACT_INDEX.md)
- [`../01_runner_protocol/PARTY_MODE_PROTOCOL.md`](../01_runner_protocol/PARTY_MODE_PROTOCOL.md) · [`../13_encounters_and_bestiary/PARTY_SCALING_6_PLAYERS.md`](../13_encounters_and_bestiary/PARTY_SCALING_6_PLAYERS.md)
