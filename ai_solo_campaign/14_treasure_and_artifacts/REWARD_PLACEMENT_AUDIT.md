# REWARD_PLACEMENT_AUDIT.md — Stage 14 Coverage and Safety Audit

---
type: audit
secrecy: mixed
status: static
region: Orrun
level_range: 1-20
related: [TREASURE_INDEX.md, ARTIFACT_INDEX.md, MAGIC_ITEM_INDEX.md, REGIONAL_TREASURE_TABLES.md, DUNGEON_REWARD_INDEX.md, FACTION_REWARDS.md, SOLO_REWARD_BALANCE.md]
tags: [type:audit, secrecy:mixed, reward-audit, coverage, solo-tuned]
---

## Purpose

Pre-completion audit for Stage 14. Confirms every required coverage axis is met and every safety rule (solo balance, secrecy, no copied official text) holds before the stage is marked complete.

## Summary

**Stage 14 PASS.** All coverage axes met; all safety rules upheld. 0 Critical, 0 High, 0 Medium findings. 3 Low/forward notes logged to `../17_generation_backlog/CONTENT_GAPS.md`.

---

## A. Region Coverage (20/20) ✓

Every region has treasure flavor in `REGIONAL_TREASURE_TABLES.md` + at least one dungeon reward hook in `DUNGEON_REWARD_INDEX.md`.

| Region | Treasure flavor | Dungeon hook | Signature magic |
|---|---|---|---|
| Sundering Reach | ✓ | ✓ (×10 sites) | Warden's Lantern, Restful Edge, relics |
| Ashgarden Vale | ✓ | ✓ (×3) | Dry-Boots, Wake-Garland |
| Tollwood | ✓ | ✓ (×3) | Bark-Charm, Toll-Keeper's Chain |
| Pale Coast | ✓ | ✓ (×3) | Drowned Flame, Diving-Mask, Held Breath |
| Caradril | ✓ | ✓ (×2) | Tally-Glass, Honest Coat, Quiet-Step Boots |
| Verdance Reaches | ✓ | ✓ (Nine Locks) | Bloom-Splint |
| Glassmere League | ✓ | ✓ (×2) | Clarity-Lens, Mirror-Shard |
| Marrowdowns | ✓ | ✓ | Ancestor-Ring |
| Sallowmarch | ✓ | ✓ | marsh-healer gear, Desiccant Case |
| Hollow Gulf | ✓ | ✓ | Reef-Charts |
| Wender Steppe | ✓ | ✓ | Wind-Chime Compass |
| Karran Marches | ✓ | ✓ | Border-Iron Brand |
| Emberfell/Ashfast | ✓ | ✓ | Emberglass Brand-Bottle |
| Saltmere Reaches | ✓ | ✓ | Desiccant Case |
| Concord Heartlands | ✓ | ✓ | Ash-Crown Fragment, Unforgotten Mail |
| Hethewald | ✓ | ✓ | wood-charms, amber-relic |
| Sunmark | ✓ | ✓ | Sun-Disk Pendant |
| Highmark Passes | ✓ | ✓ | Giant-Forged Maul |
| Cindern Waste | ✓ | ✓ | ash-glass relic |
| Drowned Steps | ✓ | ✓ | Drowned Crown-Arc |

## B. Level-Band Coverage (5/5) ✓

| Band | Reward guidance | Source |
|---|---|---|
| 1–4 | ✓ | `SOLO_REWARD_BALANCE.md`, `REGIONAL_TREASURE_TABLES.md` |
| 5–8 | ✓ | same + `FACTION_REWARDS.md` |
| 9–12 | ✓ | + `ARTIFACT_INDEX.md` (fragments/cursed surface) |
| 13–16 | ✓ | + Very Rare/Legendary, faction relics |
| 17–20 | ✓ | + endgame artifacts (M6–M9 gated) |

## C. Dungeon Reward Hooks (39/39) ✓

Every authored adventure site in `../10_dungeons_and_ruins/` has a signature reward, mundane band treasure, and (where present) a cursed/danger item in `DUNGEON_REWARD_INDEX.md`. The DM-only Under-Shrine Approach is flagged endgame-only.

## D. Faction Reward Tracks (7 majors + 4 city) ✓

| Faction | R1 | R2 | R3 | Opposition |
|---|---|---|---|---|
| Ashen Wardens | ✓ | ✓ | ✓ (Unlit Lantern) | ✓ |
| Cinder Ledger | ✓ | ✓ | ✓ (trade share) | ✓ |
| Mourners' Circle | ✓ | ✓ | ✓ (Grief-Glass) | ✓ |
| Reachward Compact | ✓ | ✓ | ✓ (Compact Seal) | ✓ + DM trap |
| Gravecallers | ✓ | ✓ | ✓ (the Knock) | ✓ |
| Concord Remnant | ✓ | ✓ | ✓ (Archive Key) | ✓ |
| Hollow Court | DM-only: **no open rewards; all gifts are traps** | — | — | endgame ally = price |
| Salt Syndicate / Hush / Charter Houses / Tide-Watch | ✓ | ✓ | ✓ | ✓ |

## E. Count Targets ✓

- Artifacts: **12** (≥10) ✓
- Custom magic items: **38** (30–50) ✓ — 48 originals incl. artifacts
- Cursed items: **10** (+3 endgame) (≥8) ✓
- Sentient items: **6** (≥5) ✓

## F. Safety Checks ✓

| Check | Result | Notes |
|---|---|---|
| No official item text copied (Track A reference-only) | **PASS** | only name/source/rarity/fit/placement given; no properties/numbers reproduced |
| No early apex-truth exposure | **PASS** | endgame artifacts gate to M6–M9; DM-only blocks separated; Court gifts = traps; no item names/locates the keystone/Court before earned |
| Solo balance safe | **PASS** | no flat +X before Rare; recovery/utility weighted up; insurance-floor defined; no solve-everything item |
| Cursed items telegraphed + recoverable | **PASS** | every curse has a warning sign and a discoverable lift; no campaign-ending/cheap-death curses |
| Sentient items don't overshadow PC | **PASS** | companion-not-co-pilot rule; agendas = hooks, not punishment |
| Noncombat reward parity | **PASS** | `NONCOMBAT_REWARDS.md` matches loot; quest index restates parity rule |
| Remembrance relics = plot before power | **PASS** | Thin-touch risk, faction heat, limited effect; no easy resurrection items |
| Cross-links present | **PASS** | all 14 files cross-linked; runtime INVENTORY linked |
| Indexed | **PASS** | CONTENT_INDEX + TAG_INDEX + NAMING_REGISTRY updated |
| No four-PC assumptions | **PASS** | all guidance single-PC |

## G. Secrecy Separation ✓

DM-only content is confined to clearly-marked **DM-Only blocks** in `ARTIFACT_INDEX.md` (#5, #7, #8, #10, #11, #12), `CURSED_ITEMS.md` (#4, #9), `SENTIENT_ITEMS.md` (#4), and `FACTION_REWARDS.md` (§7). No player-facing summary, index row, or item description leaks the harvest, the Hollow Court, the keystone, or the Custodians.

## Forward Notes (logged to CONTENT_GAPS, Low priority)

1. **RtHW (June 16 2026) horror-item supplement** could add 1–2 Track-A cursed/relic references once the book is verified; not blocking.
2. **Endgame artifact mechanics** (Harvest Engine Shard, Quiet Country Vessel) are intentionally light pending Stage 15 Act 4–5 builds — deepen alongside `ENDGAME_STATES.md`.
3. **Runtime ownership tracking:** `../02_runtime_state/INVENTORY_AND_REWARDS.md` should record which artifacts/relics the player holds as play begins; populated during Stage 17, not now.

> **Stage 15/15B update (2026-06-16):** Endgame artifact usage and mechanics are now handled by:
> - `../15_campaign_arcs/ENDGAME_STRUCTURE.md`
> - `../15_campaign_arcs/ENDGAME_STATES.md`
> - `../15_campaign_arcs/FINAL_REVELATION_AND_ENDING_PATHS.md`
> - `../15_campaign_arcs/ENDGAME_REGION_PLAYBOOK.md`
> - `ARTIFACT_INDEX.md`
>
> Forward Note 2 above is resolved: the endgame artifacts are no longer "pending Stage 15." Any remaining mechanical detail for artifact use-in-play is optional Stage 17+/19 polish, not a blocker.

## Recommended Next Step

Proceed to **Stage 15 — Level 5–20 Arc Expansion.** Pull reward placements from this folder; keep endgame artifacts M6–M9 gated.

## Related Files

- [`TREASURE_INDEX.md`](TREASURE_INDEX.md)
- [`SOLO_REWARD_BALANCE.md`](SOLO_REWARD_BALANCE.md)
- [`../17_generation_backlog/CONTENT_GAPS.md`](../17_generation_backlog/CONTENT_GAPS.md)
