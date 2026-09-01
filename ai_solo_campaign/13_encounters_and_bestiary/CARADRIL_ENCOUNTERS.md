# CARADRIL_ENCOUNTERS.md — City Encounter & Social Scene Tables

---
type: encounter
secrecy: mixed
status: static
region: Orrun
settlement: Caradril
factions: [all]
level_range: 3-14
related: [../06_settlements/CARADRIL.md, ../06_settlements/caradril_districts/, ../01_runner_protocol/SOCIAL_SCENE_PROTOCOL.md, ../01_runner_protocol/COMBAT_PROTOCOL.md]
tags: [type:encounter, secrecy:mixed, region:caradril, function:social, function:solo-safety, level:5-12]
---

## AI Use

Solo-tuned encounter and **social-scene** tables for Caradril, by district. The city's "encounters" are overwhelmingly **social, political, and investigative** — Caradril is a safe-rest hub where danger is leverage, exposure, and the underworld, not random violence. Combat-capable threats are concentrated in the **Sunken Wards** (a graded dungeon) and in *telegraphed* faction reprisals. Roll d10 by district or pick to fit the scene/clocks. Stat references use D&D 5e/2024-compatible baselines (no copied stat blocks); scale per Scaling Notes. Always telegraph danger; always offer a non-combat path (`SOCIAL_SCENE_PROTOCOL.md`, `COMBAT_PROTOCOL.md`, `SOLO_PLAY_PRINCIPLES.md`).

## Encounter Type Legend
- **[Social]** = a person/scene to talk through (the city's default); social DCs apply.
- **[Intrigue]** = a faction maneuver, lead, or surveillance beat; mostly investigation/stealth.
- **[Clue]** = a breadcrumb toward a mystery (deliver fragments; never the apex).
- **[Hazard]** = environmental (mostly the Wards/Crucible); a check, not a fight.
- **[Threat]** = a telegraphed danger that *can* turn to combat; always with a non-combat out.
- **[Dead]** = a Remembrance/apparition (Sunken Wards / Highmourn failures); resolvable by rite/parley.

## Citywide Adversary Stat Reference (for reprisals/Wards)
- **Tide-Watch guard:** Guard-like (AC 16, ~11 HP). **Watch sergeant:** Veteran-like (AC 17, ~58 HP). **Captain Kade:** Knight/Veteran-like (AC 18, ~90 HP, Leadership) — never a default fight.
- **Ledger/House hireling:** Thug/Spy-like (AC 13–14, ~30–40 HP; intimidation over killing).
- **Salt Syndicate crew:** Bandit/Thug-like (AC 12–14, ~11–30 HP); **Sorrel:** Spy/Assassin-like (AC 15, ~55 HP; leverage over blades).
- **Reclaimer agent:** Spy/Mage-like (AC 13–14, ~40–60 HP; Hold Person, Counterspell, Remembrance one-offs); **Quorrin Vane:** Tier-1 Mage/Archmage-like (never a cheap ambush).
- **Remembrance apparition (Wards/Highmourn):** Specter/Ghost-like (AC 12, ~22–40 HP, incorporeal, life/Remembrance drain); telegraphed, often resolvable without combat (a true rite Religion DC 13, a name, a blessing, or withdrawal). 1–2 at a time, never a swarm.

---

## The Magisterium (Lvl 4–10) — political/social

| d10 | Encounter | Type | Solo Danger | Notes / Stat Reference |
|---|---|---|---|---|
| 1 | A charter-hearing the player can influence | [Social][Intrigue] | none | Persuasion DC 17; `Q_THE_OPEN_CHARTER` |
| 2 | Sefa Dann seeking an honest outsider | [Social][Clue] | none | reform lever; the Reach warning |
| 3 | Tolm's "friendly" overture (using the player vs. the Ledger) | [Social][Intrigue] | none | treacherous patron; Insight DC 14 |
| 4 | The Watch stops the player over visible weapons/armor | [Threat] | low | talk past DC 12, or a charter-sponsor; Guard-like |
| 5 | A frightened Compact courier, ignored by all but the player | [Social][Clue] | none | the Reach plea; `Q_THE_SEALED_LETTER` |
| 6 | A clerk hints a registry record can be "lost" for coin | [Intrigue][Clue] | none | C-M4 city echo; Sile |
| 7 | Voss, anxious over a Reach letter, says too much | [Clue] | none | correspondent thread (lead only) |
| 8 | A bribe offered to sway the player's testimony | [Social][Intrigue] | none | Insight DC 13 reads the true cost |
| 9 | Kade quietly recruits the player off-record | [Social] | none | `Q_THE_TIDE_TURNS`; deputization |
| 10 | A House's hireling "warns" the player off a vote | [Threat] | low | Thug/Spy-like; flee/talk/bribe; telegraphed |

## The Counting-Quays (Lvl 5–12) — money/conspiracy

| d10 | Encounter | Type | Solo Danger | Notes / Stat Reference |
|---|---|---|---|---|
| 1 | Vyre's audience: a warm offer with a clause | [Social] | none | `Q_THE_QUAY_CHARTER`; Vyre |
| 2 | Coll Riis nearly confessing in the Last Tally | [Social][Clue] | none | the deal-proof (M3/M6); Persuasion DC 14 |
| 3 | A Remnant courier slipping into the Keep at night | [Intrigue][Clue] | low | tail Stealth DC 13; the deal |
| 4 | A debt-collection that's also a moral test | [Social][Intrigue] | low | Ledger hireling backup (Thug/Spy) |
| 5 | Smugglers landing a "quiet" crate at a quay | [Intrigue][Clue] | low | Syndicate; `Q_THE_TIDE_TURNS` |
| 6 | A blacklisted debtor begs the player's help | [Social][Clue] | none | Ledger leverage; a hook |
| 7 | The deep vault "talks" (overheard rumor made real) | [Clue] | none | the refined relic (M3; L8+) |
| 8 | Provost Vell tests the player with a hard errand | [Social][Intrigue] | low | Vell; trust-building |
| 9 | A Ledger hireling tails the player | [Threat][Intrigue] | low | spot Perception DC 13; lose/confront |
| 10 | A botched job → capture-not-kill by Ledger muscle | [Threat] | mod | flee/bargain; never lethal by default |

## The Lantern Reach (Lvl 4–12) — scholarship/secrets

| d10 | Encounter | Type | Solo Danger | Notes / Stat Reference |
|---|---|---|---|---|
| 1 | Briss teaching Concord Script, lighting up | [Social][Clue] | none | `Q_THE_LANTERN_AND_THE_LAMP` |
| 2 | Tamsin Orr tutoring late, strings-free | [Social] | none | clean Script path |
| 3 | Wessel Dree barring the Archive stair, all courtesy | [Social][Intrigue] | none | the Sealed Archive gate |
| 4 | Quorrin "happening by," reading the player | [Social][Intrigue] | low | Quorrin's evaluation; never a fight here |
| 5 | A copyist who saw too much, frightened | [Social][Clue] | none | M6 fragment; Hale-of-Lampgate |
| 6 | A Stacks text yields an M2/M3 fragment (gated) | [Clue] | none | Investigation DC 13 + Script |
| 7 | A Reclaimer agent shadows the player | [Threat][Intrigue] | low | Spy/Mage-like; turn-back, not kill |
| 8 | Briss troubled, half-doubting his own order | [Social][Clue] | none | Secret 13 lever |
| 9 | The Archive break-in (if attempted) | [Intrigue][Threat] | mod | DC 18–20 multi-path; `Q_THE_SEALED_ARCHIVE` |
| 10 | A Reclaimer "turn-back" confrontation | [Threat] | mod | telegraphed; non-combat out always |

## The Ashmarket (Lvl 4–9) — relics/black market

| d10 | Encounter | Type | Solo Danger | Notes / Stat Reference |
|---|---|---|---|---|
| 1 | A back-room quiet-coin sale; the relic murmurs a name | [Clue][Hazard] | low | M3; thin-touch risk; `Q_QUIET_COIN` |
| 2 | Mooren the appraiser, unnerved by a relic | [Social][Clue] | none | M3; honest read DC 14 |
| 3 | Sorrel offering discreet work | [Social][Intrigue] | low | Syndicate jobs |
| 4 | A buyer who "went strange" after a relic | [Clue][Hazard] | low | M3 horror; thin-touch case |
| 5 | Clergy protesting the relic-trade | [Social][Clue] | none | moral fault line; M6 echo |
| 6 | A fence offering to move the player's salvage | [Social] | none | quiet-coin trade |
| 7 | A relic that "reads wrong" handed to the player | [Hazard][Clue] | low | handle DC 14 or thin-touch |
| 8 | Syndicate runners shadowing a deal | [Intrigue][Threat] | low | Bandit/Thug-like; avoidable |
| 9 | A bidding-war between Ledger and Syndicate buyers | [Intrigue][Clue] | none | the relic flow; exploitable |
| 10 | A Syndicate "lesson" for a crosser | [Threat] | mod | telegraphed; flee/negotiate; Sorrel prefers leverage |

## Highmourn (Lvl 4–8) — faith/death/cover-up

| d10 | Encounter | Type | Solo Danger | Notes / Stat Reference |
|---|---|---|---|---|
| 1 | A civic funeral that falters — and is hushed | [Clue][Social] | none | Secret 7; `Q_THE_FUNERAL...` |
| 2 | Quayle showing a grave that "won't keep" | [Clue][Social] | none | M1/M5 city echo |
| 3 | Sister Onae (Warden), grateful anyone will listen | [Social][Clue] | none | ignored Wardens; Othetha path |
| 4 | Mother Ysarra, gracious and stonewalling | [Social][Intrigue] | none | the cover-up; DC 18 to crack |
| 5 | A charter family's failed raise-dead | [Social][Clue] | none | resurrection risk; the failures |
| 6 | A hushed-up wrong-come-back in a sealed tomb | [Dead][Clue] | low | revenant (AC 12, ~30 HP); rite resolves; non-default combat |
| 7 | Vass's ledger of re-dug graves | [Clue] | none | Investigation DC 15; the cover-up |
| 8 | The bells toll for a rite that "didn't take" | [Clue] | none | Tomm; pattern of failures |
| 9 | Healing/sanctuary offered freely | [Social] | none | solo-safety; rest/heal |
| 10 | A grieving family seeks the player's help to let go | [Social][Clue] | none | a humane Wren-echo |

## The Crucible (Lvl 5–8) — craft/smelting hazard

| d10 | Encounter | Type | Solo Danger | Notes / Stat Reference |
|---|---|---|---|---|
| 1 | A night-shift smelt screaming in a human voice | [Clue][Hazard] | low | M3 by accident; `Q_THE_SMELTING` |
| 2 | Beck Harrow, scared, asking what she's melted | [Social][Clue] | none | M3 witness |
| 3 | A slag-yard cast that murmurs when lifted | [Clue][Hazard] | low | thin-touch warning |
| 4 | Soot the apprentice hiding his thin-touch | [Social][Clue] | none | the workers' plight |
| 5 | Ordo diverting a crate to a Remnant courier | [Intrigue][Clue] | none | proxy-war; tail DC 13 |
| 6 | A foundry heat/slag hazard in the player's path | [Hazard] | low | Dex/Con DC 13; 2d6 fire if careless |
| 7 | A gear commission scene (upgrade) | [Social] | none | Phane; quality goods |
| 8 | Guild toughs warn the player off the foundry | [Threat] | low | Guard/Thug-like; telegraphed |
| 9 | Workers' unrest spilling toward the Sill | [Social][Clue] | none | Renna link |
| 10 | A deeper foundry "incident" (M3 climax) | [Clue][Hazard] | mod | thin-touch-heavy; escapable |

## The Sill (Lvl 4–9) — underworld/refugees

| d10 | Encounter | Type | Solo Danger | Notes / Stat Reference |
|---|---|---|---|---|
| 1 | The Bellman, never quite seen, naming a price | [Social][Intrigue] | none | `Q_THE_BELLMANS_PRICE` |
| 2 | Thin-born refugees on the boards | [Social][Clue] | none | M10 local; Renna |
| 3 | Renna pleading the refugees' case | [Social][Clue] | none | humane lever |
| 4 | A thin-born child who "remembers wrong" | [Clue][Social] | none | the thinning, made unbearable |
| 5 | Cutpurses sizing up an upper-city visitor | [Threat] | low | Thug/Bandit-like; avoidable |
| 6 | Old Pater Dunk at the Sealgate, lantern lit | [Social][Clue] | none | the Sunken Wards |
| 7 | A Hush-runner with an offer (or a warning) | [Intrigue] | none | the Hush's reach |
| 8 | A smuggler drop in the backwater channels | [Intrigue][Clue] | low | Syndicate; avoidable |
| 9 | Renna's sheltered wrong-come-back | [Dead][Clue] | low | a city Wren-echo; rite resolves |
| 10 | A Syndicate vs. Hush flashpoint | [Threat][Intrigue] | mod | `Q_THE_TIDE_TURNS`; flee/broker |

## The Sunken Wards (Lvl 6–14) — the city's dungeon

| d10 | Encounter | Type | Solo Danger | Notes / Stat Reference |
|---|---|---|---|---|
| 1 | A flooded hall on a rising-water cycle | [Hazard] | low-mod | Athletics/Con DC 13; read cycle DC 14 |
| 2 | A drifting Remembrance up a drowned passage | [Dead] | mod | Specter/Ghost-like; avoidable/parley DC 13 |
| 3 | Concord Script on a drowned lintel (M2 fragment) | [Clue] | none | Investigation DC 13 + Script |
| 4 | Collapsing Concord stone | [Hazard] | low-mod | Perception DC 13 / Dex DC 14; reroutable |
| 5 | A thin-touch zone near a warming relic | [Hazard][Clue] | mod | telegraphed; reversible; M3 |
| 6 | Syndicate runners using the dry upper Wards | [Threat][Intrigue] | low | Bandit/Thug-like; avoidable/bribable |
| 7 | The hidden door to the Sealed Archive's lower way | [Intrigue][Clue] | none | the back-way (`Q_THE_SEALED_ARCHIVE`) |
| 8 | A dormant relic in a drowned shrine-niche (M3) | [Clue][Hazard] | mod | thin-touch care; a better relic deeper |
| 9 | Reclaimer guards near the back-way | [Threat] | mod | Spy/Mage-like; turn-back, not kill |
| 10 | A deeper flooded hall, a stronger apparition + better relic (L12+) | [Dead][Hazard][Clue] | mod-high | telegraphed; non-combat out; retreat to the Sill |

---

## Scaling Notes

- **Levels 3–5 (city on-ramp):** favor [Social]/[Clue] results; reprisals are warnings, not fights; the Wards stay shallow (rows 1–5).
- **Levels 5–9 (core city play):** full faction intrigue; reprisals telegraphed and survivable; the Wards' middle depth; Reclaimer/Syndicate maneuvers active.
- **Levels 9–12 (Archive/endgame threads):** the Archive break-in, the deep vault, the Wards' lower flood, a Quorrin confrontation (social first) — all retreat-rich, never damage-races.
- **Solo rule:** Caradril is a safe-rest hub. The DM should resolve most city "encounters" socially; reserve combat for the Sunken Wards, telegraphed reprisals the player provokes, and the optional revenant scenes — always with a non-combat path and a retreat.

## Solo-Safety Pillars in the City
- **Rest/healing:** Highmourn (Cathedral, Quiet Houses), the Pale Star, Ledger letters of credit, hireling protection.
- **Guides/allies:** Old Pater Dunk (Wards), Sister Onae (Wardens), Renna Sill (the Sill), Captain Kade (lawful backup), Tamsin Orr (Script).
- **Retreat:** every district adjoins safe ground; the Wards always retreat up the Sealgate.

## Related Files

- [`../06_settlements/CARADRIL.md`](../06_settlements/CARADRIL.md)
- [`../06_settlements/caradril_districts/THE_SUNKEN_WARDS.md`](../06_settlements/caradril_districts/THE_SUNKEN_WARDS.md)
- [`../01_runner_protocol/SOCIAL_SCENE_PROTOCOL.md`](../01_runner_protocol/SOCIAL_SCENE_PROTOCOL.md)
- [`SUNDERING_REACH_ENCOUNTERS.md`](SUNDERING_REACH_ENCOUNTERS.md)
