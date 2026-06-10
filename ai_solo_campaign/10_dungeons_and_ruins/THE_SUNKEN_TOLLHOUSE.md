# The Sunken Tollhouse

---
type: dungeon
secrecy: mixed
status: static
region: Sundering Reach
settlement: Kettle Bridge
factions: [Reachward Compact, Cinder Ledger, Gravecallers]
level_range: 2-3
related: [../06_settlements/KETTLE_BRIDGE.md, ../05_regions/wilderness/MIREWEND_AND_ROADS_SITES.md, ../11_mysteries_and_secrets/MYSTERY_WEB.md]
tags: [type:dungeon, secrecy:mixed, region:sundering-reach, level:2-3, function:exploration, function:clue]
---

## AI Use

Load when the player investigates the Kettle Bridge river-drownings ("The Broken Arch" hook). A small, flooded Concord ruin under the bridge's collapsed fourth arch — a minor harvest node, leaking. **Solo-safe small dungeon (level 2–3); the climax is a single telegraphed Remembrance, resolvable without combat.** A clean early M2/M5 clue site.

## One-Sentence Identity

A drowned Concord toll-shrine sunk under the bridge's broken arch, half-flooded and leaking the dead into the river.

## History

Publicly: an old toll-house that collapsed into the Mirewend generations ago. **Truly (DM):** a minor Concord relay-node where the road-conduit met the river. The Quietfall cracked it; it sank. Now, as the harvest reawakens, it leaks — and its leakage is what drowns the boatmen at the broken arch (M5) and seeds Reedford's haunting downstream.

## Entrance

Reached by boat from the Wet Ward, or by diving at low water from the broken arch. The flooded entry-stair descends from the arch's footing into the murk. **Telegraphed:** Bargemaster Tibb or a frightened boatman can describe (and, paid/persuaded, guide to) the entrance; the cold and the "wrong" water warn the player before they descend.

## Solo Danger Rating

**Low-to-moderate (level 2–3).** Hazards are environmental (flooding, cold, drowning) more than combat. One real fight is possible at the climax but is telegraphed and avoidable. Strong retreat options throughout.

## Zone / Room List

1. **The Flooded Stair** — descends from the arch into chest-deep water. Cold (Con DC 12 or 1 exhaustion on a long stay). Current hazard.
2. **The Toll-Hall** — a half-drowned chamber, Concord Script on the walls (**C-M2 fragment**, language-gated). Submerged toll-coffers (salvage; Quenna Bly has already looted the easy ones).
3. **The Relay-Room** — the node itself: a cracked Concord relay-stone, leaking visibly (faint grey light, cold dread). **C-M5 clue:** the dead drown here and drift downstream/basinward. Re-settling the stone (a true rite, Religion DC 14, or a Warden) eases the drownings.
4. **The Silt Vault** — a collapsed side-room with a mislabeled salvage crate (a low-value Remembrance relic — **C-M3 hook**) and a drowned bargeman's body (grief-clue; ties to a Wet Ward family).

## Encounter List

- **The Flooded Stair:** current/cold hazard; possibly **1 fen predator** (eel/snake-like, CR 1/8) disturbed by the intrusion (telegraphed by movement in the water).
- **The Toll-Hall:** none by default; rising water if the player lingers (clock pressure, not combat).
- **The Relay-Room (climax):** **1 drowned Remembrance** — a boatman the river took — flavor **specter-like** (AC 12, ~22 HP, can move through water freely). **Telegraphed** (cold, weeping, the grey light). **Non-combat resolution primary:** speak with it (Insight/Persuasion DC 13) or lay it with a true rite (Religion DC 14); it attacks only if attacked or if the player tries to take the relay-stone.
- **The Silt Vault:** none; a body and a relic.

## Traps / Hazards (DCs)

- **Drowning/current:** in deep-water rooms, Athletics DC 13 to move against the current; failure = swept toward the stair (no damage, lost progress) or, in the Relay-Room, pulled toward the leak (Wisdom DC 13 vs. grave-touched).
- **Rising water:** if the player lingers (each ~10 min), the tide/flood rises a stage; after 3 stages the lower rooms flood fully — a clock, not a death-trap (the stair stays open).
- **Cracked floor (Silt Vault):** DC 13 Perception to spot; DC 12 Dex save or drop into a silt-pit (Athletics DC 13 to climb out; non-lethal).

## Puzzle / Clue Checks

- **Concord Script (Toll-Hall, Relay-Room):** language-gated. With Concord Script or Comprehend Languages, Investigation DC 13 yields an M2 fragment ("the road carries them to the door under the water") — a real, fair clue pointing at the basin shrine, without naming the Court.
- **Reading the leak (Relay-Room):** Arcana/Religion DC 14 recognizes this as a *smaller version of something larger* (M5/M2 inference).

## Resting Constraints

No safe rest inside (cold, water, rising tide). Retreat to the Wet Ward / Drowned Kettle inn at Kettle Bridge for a long rest. Short rests possible on the dry upper stair between dives.

## Treasure

- Submerged toll-coffers: ~25 gp in old, water-blackened Concord coin (mostly already looted by Bly — finding more implicates her skimming).
- The Silt Vault relic: a minor Remembrance relic (M3 study-object; the Ledger, Remnant, and Gravecallers all want it — a choice).
- A drowned bargeman's signet (returns to a grieving Wet Ward family; goodwill, a follow-up hook).

## Boss / Climax Mechanics

The drowned Remembrance in the Relay-Room. **Primary win = release, not kill.** If spoken to or laid, it gives the M5 clue freely (it "remembers being pulled toward the water"). If fought: AC 12, ~22 HP, one chilling touch attack (~1d6+2 necrotic, no multiattack), can submerge to break line of sight. Morale: it cannot leave the node; if reduced or out-argued, it begs release. **No cheap death:** it telegraphs, can be fled, and prefers grief to violence.

## Retreat Options

The flooded stair stays open throughout; the player can leave at any time (Tibb's boat waits, or swim up). The rising-water clock pressures but never seals the exit.

## Scaling Notes

- **Level 1:** reduce the Remembrance to ~15 HP; soften the cold DC to 10.
- **Level 4–5:** add a second drowned Remembrance and make the relay-stone's leak a recurring grave-touched aura (DC 14 each round in the Relay-Room) to keep tension; raise relic value.

## Consequences If Ignored

The drownings spread upriver, Reedford's haunting worsens, and the Sunken Tollhouse's leak grows until the broken arch must be abandoned — closing the Reach's main crossing. Bly keeps fishing relics out of it for sale.

## State Update Triggers

- If the relay-stone is re-settled: log a brief easing of Kettle Bridge/Reedford hauntings (player-visible win); note the Court will counter over time.
- If the relic is taken: update `INVENTORY_AND_REWARDS.md` and the relevant faction's interest (`FACTION_STATE.md`).
- Mark C-M2 / C-M5 clues discovered in `KNOWN_CLUES.md` if read.

## Related Files

- [`../06_settlements/KETTLE_BRIDGE.md`](../06_settlements/KETTLE_BRIDGE.md)
- [`../05_regions/wilderness/MIREWEND_AND_ROADS_SITES.md`](../05_regions/wilderness/MIREWEND_AND_ROADS_SITES.md)
- [`../11_mysteries_and_secrets/MYSTERY_WEB.md`](../11_mysteries_and_secrets/MYSTERY_WEB.md)
- [`../13_encounters_and_bestiary/SUNDERING_REACH_ENCOUNTERS.md`](../13_encounters_and_bestiary/SUNDERING_REACH_ENCOUNTERS.md)
