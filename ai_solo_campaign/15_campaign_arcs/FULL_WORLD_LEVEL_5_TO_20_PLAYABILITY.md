# FULL_WORLD_LEVEL_5_TO_20_PLAYABILITY.md — Master Playability Checklist (All Regions × Tiers)

---
type: campaign-arc
secrecy: mixed
status: static
region: Orrun
level_range: 5-20
factions: [Ashen Wardens, Cinder Ledger, Mourners' Circle, Reachward Compact, Gravecallers, Concord Remnant, Hollow Court]
related: [REGIONAL_ARC_PACKS_LEVEL_5_TO_20.md, TIER_2_PLAYABLE_PATHS_LEVELS_5_10.md, TIER_3_PLAYABLE_PATHS_LEVELS_11_16.md, TIER_4_PLAYABLE_PATHS_LEVELS_17_20.md, LEVEL_5_TO_20_OVERVIEW.md]
tags: [playability, checklist, stage-15b, regions, tiers, runnable]
---

## AI Use

**MIXED SECRECY — the Stage 15B master index.** Load this to answer one question fast: *"The player is in region X at level Y — what concrete prepared content can I run right now?"* This file is the routing table; the detail lives in the region arc packs and tier-path files. **Apex (REV_007/Hollow Court/Custodians/harvest/keystone) is DM-only and gated to L13+; never name it in player-facing narration.**

Stage 15B answers, for every region and tier: *what* is happening, *who* is involved, *where*, and *what changes*. If you ever find yourself about to invent a major faction move, NPC, dungeon, or consequence — stop and check the region's arc pack first.

---

## The Playability Test (apply on every arrival)

When the player arrives in a region at its intended tier, confirm the AI has, from prepared content:

1. **A named arrival situation** — what is visibly happening (arc pack → "Arrival Situation").
2. **Named NPCs** — from the Stage 9/9.5 codex (arc pack → "Key NPCs").
3. **Named factions and their current goals** (arc pack → "Active Factions").
4. **Named dungeons/sites** with levels and hooks (arc pack → "Relevant Dungeons").
5. **Named quest chains** to pick up (arc pack → "Relevant Quest Chains").
6. **Named clues/revelations** that can surface here (arc pack → "Clues/Revelations Possible").
7. **Named threats** with stat references (arc pack → "Encounter Profile").
8. **Named failure consequences** (arc pack → "If Player Ignores/Fails").

If any of the eight is missing for a given region+tier, that is a Stage 15B gap — log it in `../17_generation_backlog/CONTENT_GAPS.md`.

---

## Region × Tier Coverage Matrix

Primary = the region's intended level band. Available = playable earlier/later with the danger/partial-content handling in `PLAYER_GOES_ANYWHERE_GUIDE.md`. Each cell's concrete content is in `REGIONAL_ARC_PACKS_LEVEL_5_TO_20.md`.

| Region | Tier 2 (5–10) | Tier 3 (11–16) | Tier 4 (17–20) | Arc pack section |
|---|---|---|---|---|
| **Sundering Reach** | Primary (home board) | Primary (battleground) | **Primary (the descent)** | §1 |
| **Ashgarden Vale** | Primary | Available | Ally/fall resolution | §2 |
| **Tollwood** | Primary | Available (Old Mast gated) | Route-control | §3 |
| **Pale Coast** | Primary | Available (Skerry gated) | Ally/fall resolution | §4 |
| **Caradril** | Primary (mid-game hub) | Primary (war-front) | Asset/obstacle | §5 |
| **Verdance Reaches** | Available (corridor, L8+) | Primary (Ring 2) | Logistics spine | §6 |
| **Concord Heartlands** | — (too lethal) | **Primary (L13–17)** | Means-gathering (Ash-Crown) | §7 |
| **Glassmere League** | Available (L9+ edge) | Primary (L9–13) | Banking endgame | §8 |
| **Hethewald Free Holds** | Available (L7+) | Primary (L7–12) | Refuge/route | §9 |
| **Hollow Gulf Ports** | — | Primary (L10–15) | Maritime endgame | §10 |
| **Saltmere Reaches** | — | Primary (L11–15) | Older-fall corroboration | §11 |
| **Emberfell Theocracy** | — (very lethal) | Primary (L12–16) | Means-gathering (mirror) | §12 |
| **Cindern Waste** (Emberfell sub-region) | — | Available (L13–16, very lethal) | Artifact/relic source | §12b |
| **Sallowmarch Protectorate** | — | Primary (L10–14) | — | §13 |
| **Marrowdowns** | Available (L6–10) | Primary (L6–10/14) | — | §14 |
| **Wender Steppe** | Available (L8+) | Primary (L8–13) | REV_009 echo | §15 |
| **Karran Marches** | — | Primary (L9–14) | Turned-Reclaimer ally | §16 |
| **Sunmark** | Available (L8+) | Primary (L8–13) | **Synthesis model (REV_010)** | §17 |
| **Highmark Passes** | — | Primary (L12–16) | Cold-preserved proof | §18 |
| **The Vertical Descent** (Concord Deep / Under-Shrine; DM-only) | Surface only (D20, lethal-telegraphed) | Approach opens (L13+) | **Endgame (D20→D23)** | §19 |

> **The endgame is vertical, under Hollowmere.** No surface region is the keystone or the Court's seat. Far regions are breadth and corroboration; the climax is depth-in-place.

---

## "What Do I Run Here?" — Fast Router

For each region the arc pack provides a self-contained pack. Use this priority when the player arrives:

1. Read the region's **Arrival Situation** aloud-adaptable (player-safe).
2. Surface the **most pressing Playable Situation** (the one with a live clock).
3. Hand a **hook** toward a Relevant Quest Chain or Dungeon at the player's level.
4. If the player lingers, fire an **Escalation Event** (clock advances).
5. Track everything in runtime state; advance regional + master clocks at session end.

---

## Tier-Path Files (cross-region playbooks)

When the player is following a *thread* rather than sitting in a region, use the tier-path files instead of (or alongside) the arc packs:

- **Tier 2 (5–10):** `TIER_2_PLAYABLE_PATHS_LEVELS_5_10.md` — 5 step-by-step paths (Faction, Mystery, Dungeon, City, Travel).
- **Tier 3 (11–16):** `TIER_3_PLAYABLE_PATHS_LEVELS_11_16.md` — 6 step-by-step paths.
- **Tier 4 (17–20):** `TIER_4_PLAYABLE_PATHS_LEVELS_17_20.md` — 9 endgame playbooks.

## Companion Stage 15B Files

| Concern | File |
|---|---|
| Concrete per-region arc packs (all 19) | `REGIONAL_ARC_PACKS_LEVEL_5_TO_20.md` |
| How to move between regions | `REGION_TO_REGION_TRANSITION_GUIDE.md` |
| Named events if the player ignores the arc | `CONTINENTAL_PRESSURE_TIMELINE.md` |
| Per-tier world changes if arc ignored | `PLAYER_IGNORES_MAIN_ARC_GUIDE.md` |
| Early/late region arrival handling | `PLAYER_GOES_ANYWHERE_GUIDE.md` |
| Per-region Tier 4 endgame state | `ENDGAME_REGION_PLAYBOOK.md` |
| REV_007–010 paths, redundancy, endings | `FINAL_REVELATION_AND_ENDING_PATHS.md` |
| Cross-tier concrete faction behavior | `FACTION_ESCALATION_PATHS.md` (Stage 15B section) |

## Related Files

- [`REGIONAL_ARC_PACKS_LEVEL_5_TO_20.md`](REGIONAL_ARC_PACKS_LEVEL_5_TO_20.md)
- [`LEVEL_5_TO_20_OVERVIEW.md`](LEVEL_5_TO_20_OVERVIEW.md)
- [`../11_mysteries_and_secrets/REVELATION_MAP.md`](../11_mysteries_and_secrets/REVELATION_MAP.md)
- [`../02_runtime_state/WORLD_CLOCKS.md`](../02_runtime_state/WORLD_CLOCKS.md)
