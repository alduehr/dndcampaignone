# SETTLEMENT_TOLLSTONE_CROSS_MAP.md — Settlement Map Packet

---
type: settlement
secrecy: mixed
status: static
region: Tollwood
settlement: Tollstone Cross
level_range: 2-5
related: [../../05_regions/TOLLWOOD.md, ../../06_settlements/TOLLSTONE_CROSS.md, ../../07_factions/major_factions/CINDER_LEDGER.md, ../../08_npcs/SECONDARY_NPCS.md]
tags: [type:map, secrecy:mixed, function:cartography, settlement-map, map-packet, tollstone-cross, tollwood, tollmen]
---

> **Secrecy classification:** Mixed. The Tollstone Cross hamlet and Tollmen toll-station are player-safe. Cady Renn's turnability and the Tollmen's true connection to the Ledger are DM-only until discovered.

## Settlement: Tollstone Cross (Tollwood — East Road toll-station / Tollmen hamlet)

- **Local grid:** 0–100 (X east, Y south); (0,0) = NW corner. A crossroads hamlet where the **East Road** meets a deep-wood track south toward Coldhearth. The Tollmen — a fractious band of road-toll extortionists — have made it their base. The structure is rough: a tollhouse, a crude alehouse, a stable, a few lean-tos for the band. Travelers who pay face few problems; those who don't may not reach Hartfell.
- **Full-continent position:** render-grid (34,25).
- **Population / scale:** ~25–40 Tollmen plus a few permanent residents (smith, toll-clerk). A tense, transactional settlement.
- **Water/road relationship:** sits on the **East Road** between Hartfell (1.5 hrs W) and the deeper Tollwood interior (no Concord settlement E); the deep-wood track goes S toward Coldhearth (1.5 hrs).

## Layout / Notable Areas

| Area | Local | Notes |
|---|---|---|
| The Tollhouse | (40,45) | the main barrier structure across the East Road; Cady Renn holds court here during the day; has a rough map of the road and toll-records |
| The Cross Alehouse | (55,40) | the Tollmen's drinking hall; also where travelers wait while their toll is assessed; Toll-clerk Wenny at the door |
| The Stable | (65,55) | horses and confiscated goods; a back-way out if things go badly |
| Skell's Post | (30,60) | the rough camp where Skell's more murderous sub-group bunks; watch for them at night |
| The Hanging Tree | (50,20) | a large oak N of the tollhouse with old rope-marks; warning piece; travelers who didn't pay and didn't leave |
| Smith Doune's Smithy | (70,40) | the settlement's one genuine craftsman; non-Tollman; keeps a nervous neutrality |

## Entrances / Exits

| Exit | Local edge | Leads to |
|---|---|---|
| West (East Road) | (0,45) | Hartfell (1.5 hrs W); the safe direction |
| East (East Road) | (100,45) | Tollwood interior / Greenward Toll-Station dungeon approach (2+ hrs; increasingly dangerous) |
| South (deep-wood track) | (45,100) | Coldhearth (1.5 hrs S) — dangerous if Skell's group is active |
| North (forest edge) | (45,0) | The Charcoal Burns / Mast-Beasts' Range (dangerous; no settlement) |

## Services

| Service | Where | Details |
|---|---|---|
| Rest | Cross Alehouse (55,40) | 3cp/night; but Tollmen may search packs; uneasy rest (Perception DC 12 to detect it) |
| Resupply | Stable / Alehouse | fodder, cheap provisions, rope; all at extortionate prices (150% normal) |
| Healing | none | no healer in residence; Smith Doune will cauterize a wound (1 HP stabilization; free; DC 12) |
| Information | Tollhouse / Cady Renn | road conditions and what's east (DC 11); Renn is genuinely knowledgeable about the Tollwood; Skell's movements (DC 14 Deception/Persuasion with Renn) |
| Toll | Tollhouse (40,45) | standard toll: 5sp/traveler; 1gp/wagon; Cady Renn sets it; Skell's sub-group enforces it |

## Law and Threat DCs

- **Paying the toll without incident:** no roll; Renn accepts, notes the traveler, moves on.
- **Negotiating the toll down:** Persuasion DC 13 (Renn is businesslike; DC 14 if Skell is watching); success = 50% reduction.
- **Refusing the toll or attempting to pass:** Renn gives one warning; Skell's group appears (3–5 Bandits, CR 1/4 + 1/2; morale breaks at 50% losses or if Skell falls); see combat encounter below.
- **Turning Renn against Skell:** Cady Renn is turnable — he wants a quieter operation and fears Skell's violence will draw Compact attention. DC 15 Persuasion (lower by 2 if the player has leverage: Compact warrant, Ledger contact, evidence of Skell's murders). If turned, Renn provides safe passage and may become an informant.
- **Threatening Smith Doune:** he cooperates; noncombatant; will hide travelers in the smithy if asked (DC 11; he hates the Tollmen but can't leave).

## Key NPC Links

| NPC | Role | Location | Notes |
|---|---|---|---|
| Toll-Boss Cady Renn | Tollmen leader; turnable | Tollhouse (40,45) | DC 15 to turn; businesslike; afraid of the Compact seeing Skell's body count; his voice: flat, watchful, tired of Skell's extremism |
| Skell | Tollmen lieutenant; murderous | Skell's Post (30,60) | NOT turnable; morale breaks only at 50% losses or Renn's order; his removal is the only way to fully pacify the Cross |
| Toll-clerk Wenny | minor NPC; Tollmen bookkeeper | Cross Alehouse (55,40) | DC 11; nervous; will pass a secret note to a traveler if Renn isn't watching |
| Smith Doune | minor NPC; neutral craftsman | Doune's Smithy (70,40) | DC 12; noncombatant; knows how many Tollmen there are and where they sleep |

## Quest Hooks

- **The toll problem:** Hartfell merchants and Compact road-wardens want the Tollmen gone. Renn can be turned or the Cross can be taken by force. Partial success (turning Renn; removing Skell) is the optimal outcome for the Tollwood quest chain (L2–4; Q_TOLLWOOD_001 or adjacent; feeds Tollwood regional stability clock T1).
- **What Renn knows:** if turned, Renn reveals that the Tollmen were "encouraged" by a Cinder Ledger factor to set up the toll — the Ledger wanted Compact attention on the East Road diverted (M3 oblique; DC 15 Persuasion to get this).
- **Skell's camp:** Skell's lean-to contains a list of travelers he killed who "didn't pay." One name on it is a Compact messenger; the Compact doesn't know. This can be used as leverage or handed to Road-Warden Brannoch in Hartfell (L3; Compact political thread; DC 13 to find the list).

## Encounter / Treasure References

- Encounter: **Cady Renn** uses Bandit Captain profile (AC 15, HP 65, multiattack +4/+4 short-swords; morale: fights to the end if no out is offered; retreats if Skell is dead and Renn has less than 20 HP). **Skell** uses Veteran profile (AC 15, HP 58; aggressive; will attack without provocation if Skell's alone and the player looks weak). Rank-and-file Tollmen: Bandit CR 1/8 (3–8 present; half at Tollhouse, half at Skell's post). **Solo danger: MEDIUM at L2; HIGH if Skell is present; manageable if Renn is turned first.**
- Treasure: `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` Tier 1 — Tollmen coffers (2d6 gp if raided; Compact pays 10gp reward for Skell dead or captured and Renn turned); Skell's murder list (quest item); Renn's ledger (intelligence value re: Ledger connection; M3).

## Player-Safe Layer

Crossroads in the Tollwood; a rope across the road; the Hanging Tree; Cady Renn at the tollhouse door with a ledger and a sword-hand. Travelers pay or face the tree. The alehouse is tense. Smith Doune's hammer rings at the edge of the settlement. The wood is close on all sides.

## DM-Only Layer (NEVER on player map)

- Cady Renn is turnable: he wants the operation quieter and fears Skell will get them all killed or arrested. He can become an informant or even a minor ally if handled well (Tollwood clock T1 advances toward stability when Renn is turned and Skell removed).
- The Ledger connection: a Ledger factor (Hesk Dorr in Hartfell) quietly encouraged the Tollmen's establishment to redirect Compact road-patrols away from the Ledger's logging-camp operation further east. Renn knows this but won't say so until DC 15 turned.
- Toll-clerk Wenny is Renn's sister's son — he's here because he had nowhere else to go. He'll give the player a note about Skell's plans if he thinks Renn won't be hurt.

## Related Files

- Region: [`../../05_regions/TOLLWOOD.md`](../../05_regions/TOLLWOOD.md)
- Settlement: [`../../06_settlements/TOLLSTONE_CROSS.md`](../../06_settlements/TOLLSTONE_CROSS.md)
- Faction: [`../../07_factions/major_factions/CINDER_LEDGER.md`](../../07_factions/major_factions/CINDER_LEDGER.md)
- Dungeon: [`../../10_dungeons_and_ruins/THE_GREENWARD_TOLL_STATION.md`](../../10_dungeons_and_ruins/THE_GREENWARD_TOLL_STATION.md)
- NPCs: [`../../08_npcs/SECONDARY_NPCS.md`](../../08_npcs/SECONDARY_NPCS.md)
