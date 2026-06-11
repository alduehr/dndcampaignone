# The Buried Cloister

---
type: dungeon
secrecy: mixed
status: static
region: Ashgarden Vale
settlement: Orchardmere
factions: [Concord Remnant, Cinder Ledger, Mourners' Circle]
level_range: 2-4
related: [../05_regions/wilderness/ASHGARDEN_VALE_SITES.md, ../06_settlements/ORCHARDMERE.md, ../07_factions/major_factions/CONCORD_REMNANT.md]
tags: [type:ruin, secrecy:mixed, region:ashgarden-vale, level:2-4, function:exploration, function:clue]
---

## AI Use

Load for the Vale's accessible mid-low Concord ruin — a collapsed wayside cloister sunk under a hillside orchard south of Orchardmere, where the Remnant's scholar-pilgrims have begun digging. The "what did the Concord build" delve for levels 2–4, short of the great tomb: Concord Script, minor relics, a rival-scholar dynamic, and a gentle haunting. M2/M6 *fragment* and M3.

## One-Sentence Identity

A Concord wayside cloister swallowed by an orchard hillside, where scholar-pilgrims dig for the old script and the cloister's last brothers still keep a sorrowful, century-old vigil.

## History

Publicly: an old ruined cloister, good for cut stone and curiosities, locally thought haunted. **Truly (DM):** a Concord wayside house attached to the regional shrine-network — a place that "settled travelers' dead" and kept Script-records. It collapsed in the Quietfall and the orchard grew over it. Its records and minor relics survive; so do the bound Remembrances of the brothers who died keeping it.

## Entrance

A dig-shaft and a collapsed cloister-arch on a wooded orchard slope, an hour south of Orchardmere. The Remnant's survey-camp (Oneth Vael's two scholars) sits at the mouth. **Telegraphed:** the dig is known and discussed in Orchardmere; the Remnant will let a useful player in, bargain, or compete.

## Solo Danger Rating

**Low-to-moderate (level 2–4).** Unstable ruin, a sorrowful haunting, and a possible rivalry with the Remnant diggers. No lethal gauntlet; built as a comfortable second-tier Vale delve.

## Zone / Room List

1. **The Dig-Mouth** — the Remnant's camp and the collapsed arch; the social gate (deal, join, or compete with the scholars).
2. **The Cloister Walk** — a half-collapsed colonnade; unstable footing; minor salvage and the first Script.
3. **The Scriptorium** — the cloister's record-room, partly intact: Concord Script texts (M2/M6 fragment; the Vale's accessible Script-clue).
4. **The Settling Cells** — niche-cells where travelers' dead were "settled"; minor Remembrance relics (M3) and the bound brothers.
5. **The Sunk Chapel** — the deepest room, flooded ankle-deep; the cloister's altar and the climactic vigil-Remembrance.

## Encounter List

- **Cloister Walk:** unstable masonry (hazard); a fen-style scavenger possible (giant rat-swarm / badger-like, CR 1/8–1/4), telegraphed.
- **Scriptorium:** none by default; possible tension with a Remnant scholar if the player is competing for the records.
- **Settling Cells / Sunk Chapel (climax):** the **Vigil-Brother** — a Remembrance of the cloister's last keeper, flavor a **specter/ghost-like** (AC 12, ~26 HP); sorrowful, **non-hostile unless the relics are looted disrespectfully**; asks to be released or to have his vigil "ended kindly." Layable by a true rite (Religion DC 13) or parley (Insight/Persuasion DC 12).

## Traps / Hazards (DCs)

- **Unstable ruin (Cloister Walk):** DC 13 Perception to spot weak vault; DC 13 Dex save or take 1d6 from falling stone / be briefly pinned (Athletics DC 12).
- **Flooded chapel:** slick footing (Acrobatics DC 11); foul air at the back (Con DC 12, minor).
- **Thin-touch (Settling Cells):** Con DC 14 near raw relics; reversible.
- No lethal traps.

## Puzzle / Clue Checks

- **The Scriptorium texts:** Concord Script (Comprehend Languages or a reader) — the cloister "settled the dead and kept their record for the shrine on the hill" (M2/M6 **fragment**: ties the Vale's ruins to a *network* and points at Saint Veddow's — act-paced; no harvest reveal pre-Act-3).
- **The Settling-Cell relics:** Arcana/Religion DC 13, or experiential — they store the dead (M3).
- **The Vigil-Brother's testimony:** speaking with him (no roll to start) — "we kept them for the Keepers... they never came back for them" — a human, tragic M6 *seed* (carefully capped).

## Resting Constraints

Short rest safe in the Dig-Mouth or Cloister Walk; long rest safe at the Remnant camp (if on good terms) or back in Orchardmere. No haunting-danger to a respectful party at rest.

## Treasure

- Minor Concord salvage (~30 gp) and 1–2 Remembrance relics (M3; moral choice as ever).
- A near-complete **Script-codex page** (the Remnant pays ~50 gp; Mother Combe wants it; a real clue-object).
- The Vigil-Brother's keepsake (roleplay weight; Mourners' goodwill if returned to his kin's grave).

## Boss / Climax Mechanics

No combat boss by design. The **Vigil-Brother** is the emotional climax — a choice about releasing a century-bound servant of the Concord, and whether to hand his cloister's secrets to the Remnant (who will use them), the Mourners (who will bury them), or keep them. If attacked, he defends weakly (AC 12, ~26 HP, chill touch ~1d6 necrotic) and begs release. Scaling: L2 → ~18 HP, gentler; L4 → ~34 HP, add a second bound brother and a Remnant scholar already at the Scriptorium (a race/ethics complication).

## Retreat Options

Open throughout; the orchard slope back to Orchardmere is short and safe. The Remnant camp is a fallback.

## Scaling Notes

- **L2:** a soft Script-and-haunting delve.
- **L3 (intended):** as written.
- **L4:** more leakage (a second Remembrance), a sharper Remnant rivalry, a thin-touch relic in the cells.

## Consequences If Ignored

If the player leaves it to the Remnant, the scholars strip the Scriptorium and carry its Script south to Caradril (advancing their reconstruction and their interest in Saint Veddow's), and the Vigil-Brother keeps his hopeless vigil. The Ledger may later quarry the relics. A clear Vale M2/M3 fragment-source passes to a faction instead of the player.

## State Update Triggers

- Script/relic clues: mark M2/M3/M6 **fragment** IDs in `KNOWN_CLUES.md` (act-capped).
- Records disposition (Remnant / Mourners / kept): `FACTION_STATE.md`, `CONSEQUENCES.md`.
- Vigil-Brother released vs. fought: `RELATIONSHIPS.md` (Mourners), `WORLD_CLOCKS.md` (minor node-leakage).

## Related Files

- [`../05_regions/wilderness/ASHGARDEN_VALE_SITES.md`](../05_regions/wilderness/ASHGARDEN_VALE_SITES.md)
- [`../06_settlements/ORCHARDMERE.md`](../06_settlements/ORCHARDMERE.md)
- [`../07_factions/major_factions/CONCORD_REMNANT.md`](../07_factions/major_factions/CONCORD_REMNANT.md)
- [`../11_mysteries_and_secrets/MYSTERY_WEB.md`](../11_mysteries_and_secrets/MYSTERY_WEB.md)
