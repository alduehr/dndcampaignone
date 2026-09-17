# NONCOMBAT_REWARDS.md — Social, Political, Information, and Access Rewards

---
type: index
secrecy: mixed
status: static
region: Orrun
level_range: 1-20
related: [FACTION_REWARDS.md, ECONOMY_AND_PRICING_GUIDE.md, QUEST_REWARD_INDEX.md, SOLO_REWARD_BALANCE.md, ../08_npcs/NPC_INDEX.md, ../07_factions/FACTION_INDEX.md]
tags: [type:index, secrecy:mixed, noncombat-reward, social, political, access, information, relationship, solo-tuned]
---

## AI Use

For a solo player, **noncombat rewards are often more valuable than loot** — they solve the problems a lone PC can't muscle through (locked doors, hostile authorities, missing knowledge, no backup). This file makes them **as detailed and trackable as combat loot.** Load when rewarding diplomacy, investigation, stealth, faction work, or a clever nonviolent solution. Track granted rewards in `RELATIONSHIPS.md`, `INVENTORY_AND_REWARDS.md`, `FACTION_STATE.md`, and `CONSEQUENCES.md`.

**Core principle (project rule):** a nonviolent or clever solution must be rewarded *as richly* as a fight. Never let combat be the only path to the good loot.

## Reward Categories

---

## 1. Political Rewards

| Reward | What it grants | Typical source | Tier |
|---|---|---|---|
| **Title / Office** | recognized authority (reeve, commissioner, factor, magistrate) — command of watch, gate access, requisition | Reachward Compact, Charter Houses | 5–12 |
| **Land grant / property deed** | a holding, farm, town-house, or keep (a base; income; status) | Compact, Charter Houses, grateful lord | 9–16 |
| **Civic medal / honor** | public standing; advantage on social checks with that polity | any city/region government | 1–12 |
| **Legal protection / pardon** | charges dropped; immunity from a specific authority | Compact, Tide-Watch, a magister | any |
| **Charter rights** | license to trade/operate (the basis of Caradril power) | Charter Houses, Tidewater Council | 9–16 |
| **A vote's ear** | a council member owes you / heeds you (sway policy) | Magister Brail, Sefa Dann | 9–16 |

## 2. Social / Standing Rewards

| Reward | What it grants | Source | Tier |
|---|---|---|---|
| **Faction standing rank** | the ranked tracks in `FACTION_REWARDS.md` | all factions | any |
| **Guild / order membership** | services, contacts, a hall to use | Lampwrights' Collegium, Crucible guilds, Wardens | 5–12 |
| **Temple blessing** | rites, sanctuary, lodging, a divine boon-flavor | Three Thresholds, Mourners | any |
| **NPC loyalty** | a named NPC becomes a reliable friend/contact | quest NPCs | any |
| **Reputation (regional)** | known as friend/legend in a region; doors open, prices drop | accumulated deeds | scaling |

## 3. Information Rewards (gold for a solo investigator)

| Reward | What it grants | Source | Tier |
|---|---|---|---|
| **Map** | safe routes, hidden sites, node-locations (DM-gated for harvest sites) | Remnant, guides, salvagers | any |
| **Archive access** | reading rights to a records-vault (the Sealed Archive is the prize) | Concord Remnant, Compact records | 5–12 |
| **Language: Concord Script** | unlocks Script-gated clues campaign-wide — a *major* access reward | Concord Remnant (Sub-Lector Tamsin Orr) | 5–10 |
| **Confession / testimony** | a witness's sworn account (leverage, evidence, a mystery beat) | turned NPCs, the dead (via rites) | any |
| **A bought secret** | one true fact from the Hush | the Bellman | 5–12 |
| **Lore unlock** | grief-songs (M5), Gravecaller fragments (M6), Warden truths (M1) | Mourners, Gravecallers, Wardens | gated |

> **Information as treasure is mystery-gated.** Never hand the player a "map to the keystone" or "the Hollow Court's location" as a reward — the apex stays earned through converging clues (`../11_mysteries_and_secrets/SECRET_PROTECTION_MATRIX.md`).

## 4. Access Rewards (open the doors a lone PC can't force)

| Reward | What it grants | Source | Tier |
|---|---|---|---|
| **Safe-house key** | a secure rest/stash point in a settlement | Syndicate, Hush, allies | any |
| **Smuggler route** | a hidden path bypassing a checkpoint/hostile zone | Salt Syndicate, "Gull" Heddwyn | 3–12 |
| **Faction passage** | safe travel through dangerous faction territory | any faction you stand with | scaling |
| **Gate / district access** | entry to a locked district, vault, or restricted ruin | Compact, guilds, the relevant key | any |
| **Sanctuary right** | a place no enemy may pursue you (a temple, a Warden waystation) | temples, Wardens, Mourners | any |

## 5. Relationship Rewards (a companion for the lonely road)

| Reward | What it grants | Source | Tier |
|---|---|---|---|
| **Recurring ally** | a named NPC who helps when called (info, aid, a favor) | quest resolutions | any |
| **Confidant** | someone the PC can trust with secrets (a rare, valuable thing) | deep NPC bonds | any |
| **Hireling** | a paid specialist (guide, scribe, guard) — see `ECONOMY_AND_PRICING_GUIDE.md` | hiring | 3+ |
| **Companion** | a sidekick who travels with the PC (Brother Hale; see solo-companion rules) | faction/quest | 3+ |
| **A debt owed to you** | callable later (the strongest social currency) | saving/aiding an NPC | any |

> **Companion balance:** a companion supports, never solves (`../00_control/DND_MECHANICS_REQUIREMENTS.md` § Companions). Use the existing Brother Hale profile and the solo-companion rules; companions can be hurt/lost, raising stakes.

## 6. Economic Rewards (money that keeps paying)

| Reward | What it grants | Source | Tier |
|---|---|---|---|
| **Trade-route share** | recurring passive income (a cut of a caravan/barge line) | Cinder Ledger, Charter Houses | 9–16 |
| **Tax exemption** | keep more of what you earn in a region | Compact, a grateful lord | 9–16 |
| **Property / business** | an inn, shop, or workshop generating income + a base | various | 9–16 |
| **Letter of credit** | spend now, settle later (watch for the *gift* trap, `CURSED_ITEMS.md` #3) | Cinder Ledger | 5–12 |
| **Pension / stipend** | a regular sum for service | Compact, faction | 5+ |

## 7. Reputation Rewards (the world reacts to you)

Track in `CONSEQUENCES.md` and `RELATIONSHIPS.md`. Reputation is earned, regional, and *double-edged*:
- **Friend of [region/faction]:** better prices, free aid, doors open, NPCs seek you out.
- **Enemy of [faction]:** ambushes, closed markets, bounties (the factions act — `../07_factions/FACTION_TURN_RULES.md`).
- **Legend / Infamy:** at high tiers, your name precedes you — useful for intimidation/persuasion, dangerous for stealth.

---

## Granting & Tracking Checklist

When you award a noncombat reward, record:
1. **What** (the title/access/info/relationship).
2. **Who granted it** and **who knows** (for consequences).
3. **Standing change** (which faction up, which down — `FACTION_STATE.md`).
4. **Strings attached** (debts, expectations, hidden costs — esp. Compact/Court).
5. **State files:** `INVENTORY_AND_REWARDS.md` (favors/property/keys), `RELATIONSHIPS.md`, `NPC_MEMORY.md`, `CONSEQUENCES.md`.

## Solo-Value Reminder

When in doubt between handing a lone PC *another magic sword* or *a smuggler route + a loyal ally + a map*, prefer the latter. The solo campaign is carried as much by access and allies as by gear.

## Related Files

- [`FACTION_REWARDS.md`](FACTION_REWARDS.md)
- [`QUEST_REWARD_INDEX.md`](QUEST_REWARD_INDEX.md)
- [`ECONOMY_AND_PRICING_GUIDE.md`](ECONOMY_AND_PRICING_GUIDE.md)
- [`SOLO_REWARD_BALANCE.md`](SOLO_REWARD_BALANCE.md)
- [`../08_npcs/NPC_INDEX.md`](../08_npcs/NPC_INDEX.md)
