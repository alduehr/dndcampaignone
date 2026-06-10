# The Whispering Cairn

---
type: dungeon
secrecy: mixed
status: static
region: Sundering Reach
settlement: Candlewick
factions: [Concord Remnant, Cinder Ledger, Ashen Wardens]
level_range: 1-3
related: [../06_settlements/CANDLEWICK.md, ../05_regions/wilderness/MIREWEND_AND_ROADS_SITES.md, ../03_canon/LANGUAGES.md]
tags: [type:ruin, secrecy:mixed, region:sundering-reach, level:1-3, function:clue, function:exploration]
---

## AI Use

Load for "The Scholar's Request" (Hook 8) and any Concord Script clue-gate scene. A Concord archive-cairn on the South Road between Candlewick and Hollowmere — a small, low-combat ruin built around reading, escorting, and protecting a scholar. **Low solo danger (level 1–3); the primary tension is a timed protect-and-translate, not a slugfest.**

## One-Sentence Identity

A roadside Concord archive-cairn dense with carved old script, where the dead's records were kept — and where a scholar can begin teaching the player to read the truth.

## History

Publicly: an old Concord road-cairn, one of several, carved with the "dead language." **Truly (DM):** an archive-marker that recorded the local harvest's tally — a census of the dead taken by the network. Its inscriptions, read, are a fair M6/M9 seed (the Concord "kept the pattern of the dead"). It is intact because it sits on firm South Road ground, away from the drowning.

## Entrance

A low stone mound off the South Road, its entrance a star-carved lintel half-buried in turf. **Telegraphed:** Candlewick folk know it; Briss (or a Remnant scholar) leads the player here in Hook 8. Open and obvious — this is an exploration/social site, not a sealed vault.

## Solo Danger Rating

**Low (level 1–3).** A scavenger ambush or a single Remembrance is the only combat, both telegraphed and avoidable. The real challenge is protecting a fragile NPC scholar and managing a translation clock.

## Zone / Room List

1. **The Lintel Hall** — the entry passage, walls dense with Concord Script. Safe; the reading begins here.
2. **The Tally Chamber** — the main vault: a great carved census-wall (**C-M6/M9 fragment**, language-gated) and stone record-coffers. The translation set-piece.
3. **The Collapsed Annex** — a partly fallen side-room with salvage and a possible scavenger or animal lair.
4. **The Sealed Niche** — a star-marked recess holding a single intact record-relic (a minor Remembrance relic; M3 hook) behind a simple Concord lock-glyph (puzzle).

## Encounter List

- **The Lintel Hall / Tally Chamber:** none by default — a reading scene. *Pressure* comes from rivals: **Remnant agents or Ledger salvagers may arrive** mid-translation to seize the cairn (social/stealth/combat choice; telegraphed by tracks or a distant cart).
- **The Collapsed Annex:** **1–2 scavengers** (**bandit/scout-like**, CR 1/8) or a **fen predator** (CR 1/4) — telegraphed by spoor.
- **The Sealed Niche (climax-lite):** if the lock-glyph is forced rather than solved, a warding **minor Remembrance** (specter-like, AC 12, ~17 HP) manifests once — telegraphed by the glyph's warning, and avoidable by solving the puzzle.

## Traps / Hazards (DCs)

- **Unstable Annex ceiling:** DC 13 Perception/Dex to avoid a minor collapse (1d6, blocks a passage; never seals the exit).
- **Lock-glyph (Sealed Niche):** not a trap if solved; forcing it (Thieves' Tools/Strength DC 15) triggers the warding Remembrance.
- **No lethal traps** — this is a clue site, not a killbox.

## Puzzle / Clue Checks

- **The Census-Wall (Tally Chamber):** the centerpiece. **Concord Script gate.** With the language (or Briss reading aloud, or Comprehend Languages), Investigation DC 12 yields an M6/M9 fragment: the Concord *recorded and kept the dead's patterns*. With Briss present, this becomes the player's **first Concord Script lesson** (a downtime/teaching beat — they begin to learn the language themselves).
- **The Lock-Glyph (Sealed Niche):** a readable Concord puzzle — translate the star-sequence (Concord Script, or Investigation DC 14 with a rubbing) to open it cleanly. Clever alternate solutions accepted (e.g., a Mourner's knowledge of the old star-order).

## Resting Constraints

Safe short and long rests inside if no rivals are inbound; the cairn is dry and defensible. Candlewick is half a day off for full recovery and the Threshold chapel's healing.

## Treasure

- Concord salvage in the coffers and Annex (~30 gp value; the Ledger and Remnant both want it).
- The Sealed Niche record-relic (minor Remembrance relic; M3 study-object).
- The **census-wall rubbing** — a portable M6/M9 clue and a teaching aid for Concord Script (the real prize).

## Boss / Climax Mechanics

There is no boss by design. The "climax" is a **choice and a clock:** finish the translation/escort before rivals arrive, and decide what to do when they do (negotiate, hide the find, fight, or hand it over). If the warding Remembrance is triggered, it is a single, layable specter (true rite, Religion DC 13), not a fight to the death.

## Retreat Options

Open exit to the South Road throughout; the player and scholar can leave with a partial translation at any time. Rivals can be avoided by leaving early (at the cost of a complete reading).

## Scaling Notes

- **Level 1:** remove rival pressure; make it a pure, gentle teaching scene.
- **Level 3–4:** rivals arrive as a coordinated Remnant snatch-team (Veska Dunn or similar; AC 13–14, ~16–30 HP); the warding Remembrance becomes a real specter (AC 13, ~22 HP) if the niche is forced.

## Consequences If Ignored

If the cairn is left unread, the Concord Script gate is still reachable via Briss elsewhere, but the Remnant or Ledger may loot and erase the cairn (removing an accessible M6/M9 seed and strengthening the Reclamation/Monopoly clocks). Candlewick loses a piece of its heritage.

## State Update Triggers

- If translated: mark C-M6/M9 fragment in `KNOWN_CLUES.md`; note Concord Script progress in `PLAYER_CHARACTER.md`.
- If rivals contested it: update `FACTION_STATE.md` (Remnant/Ledger attitude) and `RELATIONSHIPS.md` (Briss trust ↑ if protected).
- If the relic is taken: update `INVENTORY_AND_REWARDS.md`.

## Related Files

- [`../06_settlements/CANDLEWICK.md`](../06_settlements/CANDLEWICK.md)
- [`../03_canon/LANGUAGES.md`](../03_canon/LANGUAGES.md)
- [`../07_factions/major_factions/CONCORD_REMNANT.md`](../07_factions/major_factions/CONCORD_REMNANT.md)
- [`../11_mysteries_and_secrets/MYSTERY_WEB.md`](../11_mysteries_and_secrets/MYSTERY_WEB.md)
