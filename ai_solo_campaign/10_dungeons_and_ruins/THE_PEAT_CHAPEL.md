# The Peat Chapel

---
type: dungeon
secrecy: mixed
status: static
region: Sundering Reach
settlement: Hollowmere
factions: [Cinder Ledger, Gravecallers, Mourners' Circle]
level_range: 1-2
related: [../06_settlements/HOLLOWMERE.md, ../05_regions/wilderness/GREYFENS_SITES.md, ../09_quests/hooks_and_rumors/SUNDERING_REACH_HOOKS.md]
tags: [type:ruin, secrecy:mixed, region:sundering-reach, level:1-2, function:exploration, function:clue]
---

## AI Use

Load for "A Quiet Job for the Ledger" (Hook 3) — the small, near-Hollowmere ruin where Domic Sael sends the player to fetch salvage. A half-sunk Concord wayside chapel in the fen, perfect as the player's **first dungeon** at level 1: tiny, telegraphed, escapable, with a single clear threat and a relic prize. The salvage here is a Remembrance relic (M3 seed).

## One-Sentence Identity

A small Concord wayside chapel half-swallowed by the peat, where a piece of "salvage" the Ledger wants turns out to remember a dead man's face.

## History

Publicly: an old roadside chapel, abandoned and sinking, full of scavengeable Concord stone. **Truly (DM):** a minor wayside shrine of the old network — a place travelers' dead were "settled" on the road. Its altar-relic is a genuine Remembrance relic. Sinking and leaking, but minor; a safe first taste of the campaign's central horror.

## Entrance

A leaning, turf-grown chapel a few hours' walk into the fen from Hollowmere, reachable on a firm finger of ground (no guide strictly needed, but Old Sashe or a local can point the way). **Telegraphed:** the tilted star-spire is visible across the fen; Domic's job-description warns of "fen-damp and maybe a beast."

## Solo Danger Rating

**Low (level 1–2).** One telegraphed threat, environmental damp, and a moral choice about the relic. Designed as a confidence-building first delve.

## Zone / Room List

1. **The Tilted Nave** — the main chapel, floor canted into the peat, pews rotted, a hole where the floor gave way. Atmospheric; minor salvage.
2. **The Sunk Vestry** — a flooded side-room (knee-deep), with the scavenger/animal lair and some salvage.
3. **The Altar Recess** — the intact star-altar holding the **salvage Domic wants: a Remembrance relic** (a smooth grey stone that, held, shows the face of a long-dead traveler). The clue and the choice.
4. **The Floor-Hole** — a drop into a tiny crypt-space below (optional), with a traveler's bones and a second, broken relic.

## Encounter List

- **The Tilted Nave:** none by default; the floor-hole is a fall hazard.
- **The Sunk Vestry:** **1 fen predator** (giant snake/frog/giant rat-swarm-like, CR 1/8–1/4) lairing in the damp — **telegraphed** by tracks, smell, and disturbed water. Avoidable (skip the vestry) or fightable easily at level 1.
- **The Altar Recess (climax-lite):** taking the relic stirs a **faint Remembrance** — the dead traveler whose face it holds — flavor a **weak specter/ghost** (AC 12, ~13 HP), sorrowful, **non-hostile unless attacked**. It asks, wordlessly, to be remembered or released (Insight/Persuasion DC 11; or a true rite, Religion DC 12). A gentle first encounter with the campaign's theme.

## Traps / Hazards (DCs)

- **Rotten floor / floor-hole:** DC 12 Perception to spot weak boards; DC 11 Dex save or fall into the crypt-space (1d6, climb out Athletics DC 10).
- **Cold damp (Sunk Vestry):** lingering = Con DC 10 or minor fatigue; trivial.
- **No lethal traps.**

## Puzzle / Clue Checks

- **The Relic (Altar Recess):** Arcana/Religion DC 13 (or simply holding it and paying attention) reveals it *stores a dead person* — the player's **first concrete brush with M3** ("Remembrance is a thing you can hold"). No language gate; this is an experiential clue.
- **The Faint Remembrance:** speaking with it (no roll to start) gives a human, tragic frame for the whole crisis — a clue to *feeling*, not facts.

## Resting Constraints

Safe short rest in the Tilted Nave; Hollowmere is a few hours back for a long rest. No in-dungeon long-rest danger.

## Treasure

- **The altar Remembrance relic** — Domic will pay ~40 gp for it (Hook 3 reward). **But:** giving it to the Ledger feeds the monopoly clock; giving it to the Mourners (to release the dead) or keeping it (to study, M3) are live alternatives with consequences.
- Minor Concord salvage (~15 gp) in the nave and vestry.
- The broken second relic in the crypt-space (study-only; a damaged M3 clue).

## Boss / Climax Mechanics

No true boss. The faint Remembrance is the emotional climax, not a fight. If attacked, it defends weakly (AC 12, ~13 HP, one chill touch ~1d4 necrotic) and flees/begs release. **The real "boss" is the moral choice** about what to do with the relic and the dead man it holds — setting up the player's stance toward the Ledger, the Mourners, and the harvest.

## Retreat Options

Open exit throughout; the firm-ground path back to Hollowmere is short and unguarded.

## Scaling Notes

- **Level 1 (intended):** exactly as written — a soft, safe first delve.
- **Level 3+:** add a second fen predator and make the faint Remembrance a full specter (AC 12, ~22 HP); add a competing scavenger or Gravecaller already at the altar (a race/social complication).

## Consequences If Ignored

If skipped, Domic finds another hand for the job (the relic reaches the Ledger anyway, advancing the Monopoly clock), and the player misses an easy, low-risk M3 introduction. A Gravecaller scout may later claim the relic instead.

## State Update Triggers

- Relic disposition: update `INVENTORY_AND_REWARDS.md` and the receiving faction's interest (`FACTION_STATE.md`).
- If the dead man is released/studied: mark C-M3 (experiential) in `KNOWN_CLUES.md`; note Mourners' goodwill if released (`RELATIONSHIPS.md`).

## Related Files

- [`../06_settlements/HOLLOWMERE.md`](../06_settlements/HOLLOWMERE.md)
- [`../07_factions/major_factions/CINDER_LEDGER.md`](../07_factions/major_factions/CINDER_LEDGER.md)
- [`../09_quests/hooks_and_rumors/SUNDERING_REACH_HOOKS.md`](../09_quests/hooks_and_rumors/SUNDERING_REACH_HOOKS.md)
- [`../03_canon/MAGIC_RULES.md`](../03_canon/MAGIC_RULES.md)
