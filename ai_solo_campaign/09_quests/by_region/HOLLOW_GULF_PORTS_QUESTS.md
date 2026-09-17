# HOLLOW_GULF_PORTS_QUESTS.md — Developed Quests (Stage 10)

---
type: quest
secrecy: mixed
status: static
region: The Hollow Gulf Ports
factions: [Cinder Ledger, Mourners' Circle, Concord Remnant, Sallowmarch Protectorate]
level_range: 10-15
related: [../../08_npcs/by_region/HOLLOW_GULF_PORTS_NPCS.md, ../../04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md, ../hooks_and_rumors/fc_HOLLOW_GULF_PORTS_HOOKS.md, ../MAJOR_CAMPAIGN_QUESTS.md]
tags: [type:quest, far-continent, stage-10, region:hollow-gulf-ports, level:10-15, secrecy:mixed]
---

## AI Use

Eight developed quests for the Hollow Gulf Ports (the warm maritime south; rival port city-states; the door overseas to Surren; Lvl 10–15). Cast from `08_npcs/by_region/HOLLOW_GULF_PORTS_NPCS.md`. The Gulf is the campaign's most *normal* region — the crisis is essentially unknown; keep failure-themes faint/oblique. Feeds Q_MAJOR_010 (Sea Gives Back Its Dead) and Q_MAJOR_022 (Door Overseas). Anchors: Calderport, Saltgate, the Reach Lanes, the Foreign Quarter, the Mardenmouth.

---

# Q_HGP_001_THE_PORT_MISTRESS_FAVOR — The Port-Mistress's Favor

**Quest Type:** Faction favor / negotiation. **Level Range:** 10–12; solo danger: low. **Secrecy:** player-safe.
**Likely Checks/DCs:** Persuasion DC 16; Insight DC 16 (Calder's real aim); Investigation DC 15 (a rival's deal); Deception DC 17 if running deniable work.
**Starting Hook:** Port-Mistress Ive Calder needs a bold, deniable outsider to settle a delicate matter her own people can't be seen touching — and rewards usefulness with the south's greatest harbor.
**Location:** Calderport; the harbor; a rival's counting-house.
**Primary NPCs:** Ive Calder (giver), Harbor-Master Brann Calder, Counting-House Mistress Doll Reach, Southern-Factor Iss Mallorn (Ledger).
**Factions:** Independent (Calderport), Cinder Ledger (southern arm).
**Surface Problem:** Do Calder a deniable favor (recover a hijacked cargo / settle a trade-dispute / assess a rival).
**Hidden Truth (DM):** Calder is the player's gateway overseas (Q_MAJOR_022) and proof the crisis is contained to the north. She'd suppress any failure-rumor for the market's sake; she will never spend a copper on a "northern ghost story." No harvest content.
**Objectives:** 1) Take Calder's commission. 2) Resolve it (force, guile, or trade). 3) Bank her favor.
**Approaches:** Recover the cargo by negotiation, stealth, or a brief fight; play Calder's rivalry with Saltgate; expose the Ledger's hand.
**Obstacles:** Calderport's tangled rivalries; the Ledger's southern reach; deniability (failure can't touch Calder).
**Important Scenes:** Calder's counting-house terrace over a thousand ships; a tense dockside recovery; Iss Mallorn's smooth interference.
**Clues:** The Ledger's southern arm (M3 scale, oblique); the door to Surren (Q_MAJOR_022 seed).
**Combat Options:** Dockside: 3–4 **Bandit/Guard-like** hijackers (AC 13–14) — avoidable by stealth/negotiation.
**Noncombat Options:** Negotiation, stealth, rivalry-play, trade.
**Solo Safety Valves:** Multiple resolution paths; Brann Calder and Doll Crow (if befriended) assist; retreat by sea always possible.
**Rest/Time Pressure:** Safe rests at the Drowned Anchor; soft clock — the deal slips if delayed.
**Rewards:** Calder's powerful maritime patronage; harbor access; overseas-passage standing; ~150–250 gp.
**Consequences:** Calder's favor opens the Gulf and the way overseas. Failing publicly costs her face (she withdraws). Crossing her closes the south's greatest harbor.
**Failure State:** A blown commission embarrasses Calder but she still values nerve; reopen via Saltgate or a smaller favor.
**Follow-Up Hooks:** Q_HGP_002 (Saltgate rivalry); Q_HGP_007 (overseas); Q_MAJOR_022.
**Scaling Notes:** L10 — minor cargo. L14 — a fleet-scale dispute and a Ledger counter-move.
**State Updates:** FACTION_STATE (Calderport ↑), RELATIONSHIPS (Calder), NPC_MEMORY, INVENTORY.
**Related:** `MAJOR_CAMPAIGN_QUESTS.md` (Q_MAJOR_022).

---

# Q_HGP_002_TWO_HARBORS_ONE_KNIFE — Two Harbors, One Knife

**Quest Type:** Faction race / political leverage. **Level Range:** 11–14; solo danger: moderate. **Secrecy:** mixed.
**Likely Checks/DCs:** Persuasion/Deception DC 17 (playing the ports); Insight DC 16 (Vesk Mallorn's double-game); Stealth DC 16; Investigation DC 17.
**Starting Hook:** Saltgate Port-Lord Doss Saltgate courts the player against Ive Calder — "which side of Calderport's fall would you rather be on?"
**Location:** Saltgate and Calderport; the Reach Lanes between.
**Primary NPCs:** Doss Saltgate (giver), Harbor-Mistress Sera Saltgate, Sub-Factor Vesk Mallorn (Ledger double-agent), Shipwright-Master Holt Saltgate.
**Factions:** Independent (Saltgate vs. Calderport), Cinder Ledger (playing both).
**Surface Problem:** Help Saltgate gain an edge over Calderport (or refuse and warn Calder).
**Hidden Truth (DM):** The Gulf's two poles are fully playable against each other; the Ledger (via Vesk Mallorn) is stoking the rivalry for profit. A clean political sandbox; no central-mystery content.
**Objectives:** 1) Take or refuse Saltgate's commission. 2) Tilt (or expose) the rivalry. 3) Survive both ports' notice.
**Approaches:** Aid Saltgate; double-deal; expose Vesk Mallorn's game to one or both ports; broker a truce; warn Calder for a counter-reward.
**Obstacles:** Vesk Mallorn's double-dealing; either port discovering the player's hand; sea-lane danger.
**Important Scenes:** Doss Saltgate's cold pitch; catching Vesk Mallorn playing both; a sea-lane crossing under watch.
**Clues:** The Ledger profiting from the rivalry (M3-oblique).
**Combat Options:** A sea-lane interception by a privateer or port-guards (**Veteran/Bandit-like**) — avoidable by guile or Roke Mallin's escort.
**Noncombat Options:** Intrigue, double-dealing, exposure, brokering.
**Solo Safety Valves:** Multiple sides to take; truce option; turnable contacts (Holt Saltgate, Doll Crow); sea-escape.
**Rest/Time Pressure:** Safe rests in either port; a deal-window deadline.
**Rewards:** A second maritime patron (Saltgate) as a base against Calder; coin; political leverage over the Gulf.
**Consequences:** Tilting the rivalry shifts Gulf power. Exposing Vesk Mallorn hurts the Ledger's south. A truce calms the Gulf but pleases no port-lord.
**Failure State:** Caught double-dealing — one port bars the player; the other welcomes them; play continues.
**Follow-Up Hooks:** Q_HGP_001; a Ledger reprisal; Roke Mallin's wild card.
**Scaling Notes:** L11 — port-intrigue. L14 — open trade-war risk; Roke Mallin's leash-slipping (Q_HGP_005) intersects.
**State Updates:** FACTION_STATE (Calderport/Saltgate/Ledger), RELATIONSHIPS, CONSEQUENCES.
**Related:** `../../08_npcs/by_region/HOLLOW_GULF_PORTS_NPCS.md`.

---

# Q_HGP_003_THE_SALT_CROWS_WAGER — The Salt Crow's Wager

**Quest Type:** Escort / smuggling / rogue ally. **Level Range:** 11–14; solo danger: high at sea. **Secrecy:** mixed.
**Likely Checks/DCs:** Persuasion DC 16 (Mallin respects nerve); Survival/Vehicles(water) DC 16; Insight DC 16 (Mallin's leash-slipping); Athletics/Acrobatics DC 15 in a sea-fight.
**Starting Hook:** Privateer-Captain Roke Mallin offers fast passage or a fat prize — "sail with me or sail careful." The player needs the sea, and Mallin wants a bold crew.
**Location:** The Reach Lanes; the *Salt Crow*; a target ship or the Drowned Steps.
**Primary NPCs:** Roke Mallin (giver/ally), Privateer-Mate Doll Crow (steady conscience), Salvage-Captain Mab Reach (if the Drowned Steps tempt), a rival privateer.
**Factions:** Independent (privateers), Calderport (Mallin's chafing marque).
**Surface Problem:** Run a daring sea-job with Mallin (passage, a prize, or a salvage).
**Hidden Truth (DM):** Mallin is the rare far-region NPC who *might believe* the frontier crisis (sailors trade in true-strange tales) — a potential late-game bridge to alarm the maritime world (Q_MAJOR_010/022). Keep his "north gone wrong" knowledge as vague sailor's-rumor.
**Objectives:** 1) Win Mallin's wager/job. 2) Manage the risk (and Mallin's wildness). 3) Decide whether to plant the frontier truth with him.
**Approaches:** Crew the raid/salvage; out-sail a rival; talk Mallin's leash-slipping down via Doll Crow; share the frontier truth (he's one of the few who'd believe).
**Obstacles:** Sea-danger; Mallin straining Calder's leash; the Drowned Steps "not wanting to be dived."
**Important Scenes:** A wager struck on the *Crow*'s deck; a running sea-fight or a tense dive; Mallin half-believing a "north gone wrong" tale.
**Clues:** Faint sailor's-rumor of "the north gone wrong" (do NOT confirm); the Drowned Steps as a far-south Concord-sea-ruin (M2/M5-oblique).
**Combat Options:** A sea-battle: rival crew of **Bandit/Veteran-like** sailors + Mallin's crew aiding — high danger; escapable by speed/guile.
**Noncombat Options:** Charm, wager, out-sail, hire — fighting is one option among many.
**Solo Safety Valves:** Mallin's crew fights alongside the player (ally support); fast retreat by sea; the dive can be declined.
**Rest/Time Pressure:** Rests aboard ship; sea-weather/"the season" as soft pressure.
**Rewards:** Fast sea-passage anywhere on the Gulf or to Surren; a roguish maritime ally; prize-coin; a potential late-game truth-bridge.
**Consequences:** Allying Mallin gains the lanes. If he slips Calder's leash, the Gulf erupts (a clock). Planting the frontier truth makes him a possible far-region believer.
**Failure State:** A botched job — Mallin shrugs it off if the player showed nerve; a lost prize, not a dead end.
**Follow-Up Hooks:** Q_HGP_001/002 (Mallin's leash); Q_HGP_008 (Drowned Steps); Q_MAJOR_010/022.
**Scaling Notes:** L11 — a smuggling run. L14 — a full sea-battle and the Drowned Steps' real danger.
**State Updates:** RELATIONSHIPS (Mallin, Doll Crow), FACTION_STATE (Calder leash-clock), CONSEQUENCES.
**Related:** `MAJOR_CAMPAIGN_QUESTS.md` (Q_MAJOR_010/022).

---

# Q_HGP_004_THE_DOOR_OVERSEAS — The Door Overseas

**Quest Type:** Trade / world-horizon / negotiation. **Level Range:** 12–15; solo danger: low. **Secrecy:** mixed.
**Likely Checks/DCs:** Persuasion DC 17; History DC 18 (Surren lore — gated, oblique); Insight DC 16; Investigation DC 16.
**Starting Hook:** Foreign-Factor Hadiz of Surren — cultured, amused by Orrun's parochialism — offers the player a glimpse of the world beyond the sea, and wants "stories of the north's ruins" for his collection.
**Location:** The Foreign Quarter, Calderport; aboard a Surren-bound ship.
**Primary NPCs:** Hadiz of Surren (giver), Foreign-Quarter Host Mira, Surren-Captain Zayd, Crown-Customs Legate Vorr (Sallowmarch obstacle).
**Factions:** Independent (overseas), Sallowmarch Protectorate (customs).
**Surface Problem:** Broker an inland deal or carry a cargo/message overseas for Hadiz; trade him Orrun lore.
**Hidden Truth (DM):** Hadiz embodies the world *beyond* Orrun and carries the campaign's faintest, most optional hint that harvest-like history may not be Orrun's alone — keep EXTREMELY oblique; never confirm or develop; never pull focus from Hollowmere. Primarily a colorful overseas gateway (Q_MAJOR_022).
**Objectives:** 1) Win Hadiz's trust/business. 2) Complete his commission (deal/cargo/message). 3) Optionally trade Orrun lore for a glimpse of Surren's "old tales."
**Approaches:** Honest brokering; a daring overseas run (with Zayd/Mallin); trading the player's own Orrun history for Surren lore.
**Obstacles:** Crown-Customs Legate Vorr's tariffs/obstruction; the Gulf rivalries catching Hadiz's house; the long sea-lanes.
**Important Scenes:** Hadiz's Foreign-Quarter salon of "gods and goods no Orrun-born has names for"; Vorr's customs-wall; a sealed overture overseas.
**Clues:** "Surren has tales not unlike it" — the world-horizon hint (deeply gated, never developed).
**Combat Options:** Avoid; if a customs clash turns ugly, Vorr's fever-thinned **Guard/Veteran-like** soldiers — better bribed or out-talked.
**Noncombat Options:** Trade, knowledge, passage, diplomacy — the whole quest.
**Solo Safety Valves:** No combat gate; the overseas run is optional; allies (Hadiz, Zayd, Host Mira); customs is bribable.
**Rest/Time Pressure:** Safe rests in the Foreign Quarter; sailing-season pressure if going overseas.
**Rewards:** Overseas goods/knowledge; passage toward Surren (a door to the wider world); Hadiz as a far-future horizon-ally; coin.
**Consequences:** Cultivating Hadiz opens the world beyond Orrun (late-game reach). Crossing him loses overseas access.
**Failure State:** A failed commission costs Hadiz's business but not his courtesy; reopen via Host Mira or Zayd.
**Follow-Up Hooks:** Q_HGP_003 (Mallin's passage); Q_MAJOR_022 (Door Overseas); a Surren horizon-thread (far future).
**Scaling Notes:** L12 — a coastal deal. L15 — a true overseas voyage and imperial customs-politics.
**State Updates:** RELATIONSHIPS (Hadiz, Zayd), FACTION_STATE (overseas reach), INVENTORY.
**Related:** `MAJOR_CAMPAIGN_QUESTS.md` (Q_MAJOR_022).

---

# Q_HGP_005_THE_PRIVATEERS_LEASH — The Privateer's Leash

**Quest Type:** Moral dilemma / faction (Calderport) / hunt. **Level Range:** 12–15; solo danger: high. **Secrecy:** mixed.
**Likely Checks/DCs:** Insight DC 17 (Calder vs. Mallin); Persuasion DC 18; Vehicles(water) DC 16; Investigation DC 16.
**Starting Hook:** Ive Calder asks the player to rein in (or eliminate) Privateer-Captain Roke Mallin, who is slipping his marque toward open sea-lordship.
**Location:** Calderport; the Reach Lanes; the *Salt Crow*.
**Primary NPCs:** Ive Calder (giver), Roke Mallin (target/possible ally), Doll Crow (the crew's conscience), Tide-Mother Sera Mardenmouth (a sea-Mourner who'd warn Mallin the north's tales are true).
**Factions:** Calderport (Calder's authority), independent (Mallin).
**Surface Problem:** Bring Mallin to heel for Calder.
**Hidden Truth (DM):** This pits the player between Calder's order and Mallin's potential as a far-region believer/bridge for the frontier truth (Q_MAJOR_010). Killing Mallin removes a possible ally; turning him both ways is the clever path. No harvest content surfaces.
**Objectives:** 1) Find Mallin's true intent. 2) Choose: rein him in, free him, broker a peace, or take him down. 3) Manage the Gulf fallout.
**Approaches:** Negotiate Mallin back to the marque; help him win a clean independence; broker Calder/Mallin terms via Doll Crow; or hunt him (a deadly sea-fight).
**Obstacles:** Mallin's wildness; Calder's expectation; a sea-battle if it comes to force.
**Important Scenes:** Calder's cold commission; Doll Crow pleading for the crew; a parley on the *Crow*'s deck; (optional) a running battle.
**Clues:** Mallin's half-belief in "the north gone wrong" (a bridge for Q_MAJOR_010, kept oblique).
**Combat Options:** A full sea-battle vs. Mallin's crew (**Veteran/Bandit-like** + a Pirate-Captain-tier Mallin, AC 16 ~75 HP) — high danger; only one resolution among several.
**Noncombat Options:** Negotiation, brokering, leverage — combat is avoidable.
**Solo Safety Valves:** Non-violent resolutions exist; Doll Crow is a turnable lever; retreat by sea; the fight is telegraphed and optional.
**Rest/Time Pressure:** Rests in port; a leash-clock deadline before the Gulf erupts.
**Rewards:** Calder's deep favor (if reined in) OR Mallin as a free ally (if freed); coin; a stabilized or transformed Gulf.
**Consequences:** Killing Mallin removes a far-region truth-bridge and a wild card. Freeing him strains Calder. Brokering peace is hardest and best.
**Failure State:** A botched hunt — Mallin escapes as an enemy on every lane; Calder is displeased; play continues with a Gulf-clock advance.
**Follow-Up Hooks:** Q_HGP_003; Q_MAJOR_010 (the sea-truth bridge); a Gulf trade-war.
**Scaling Notes:** L12 — a parley. L15 — a deadly fleet engagement.
**State Updates:** FACTION_STATE (Calder, Gulf leash-clock), RELATIONSHIPS (Mallin, Calder, Doll Crow), CONSEQUENCES.
**Related:** `MAJOR_CAMPAIGN_QUESTS.md` (Q_MAJOR_010).

---

# Q_HGP_006_THE_SEAS_OWN_DEAD — The Sea's Own Dead

**Quest Type:** Death-rite failure (faint) / investigation / clue trail. **Level Range:** 11–14; solo danger: low–moderate. **Secrecy:** mixed.
**Likely Checks/DCs:** Religion DC 16 (sea-rites); Insight DC 17 (Sera's correlation); Investigation DC 16; Persuasion DC 15.
**Starting Hook:** Tide-Mother Sera Mardenmouth — the Gulf's lone believer — has connected sailors' "north gone wrong" rumors to the old songs, and the wharf-rites are *faintly* slipping. She seeks a frontier traveler who knows the truth.
**Location:** The Mardenmouth wharves; the delta-edge; the sea-shrines.
**Primary NPCs:** Sera Mardenmouth (giver/ally), Sea-Singer Coll Mardenmouth (first faint failure-signs), Sea-saint-wife Mab, Far-sailor "Three-Seas" (a "north" rumor).
**Factions:** Mourners' Circle (southern/maritime).
**Surface Problem:** Help the faltering sea-rites and learn why they slip — at the warm far south, where no one believes.
**Hidden Truth (DM):** Sera is the southernmost old-songs network anchor and the Gulf's only believer; she could carry the frontier warning to the maritime world via Mallin (Q_MAJOR_010). Her "grey hands took the dead" is M6-oblique folk-memory ONLY — no mechanism, no Court, no keystone. The Gulf's failures are the faintest of any region.
**Objectives:** 1) Confirm the faint failures. 2) Settle a slipping sea-rite. 3) Decide whether to help Sera sound the alarm.
**Approaches:** Help the sea-rite; correlate sailors' rumors with Sera; bring frontier truth to her; enlist Mallin to spread the warning by sea.
**Obstacles:** The Gulf's total disbelief; the failures so faint they're deniable; the official sea-faith's complacency (Father Ode Calder).
**Important Scenes:** Sera connecting the rumors to the century-old songs; a wharf-rite that "doesn't quite take"; a sailor's "north gone wrong" tale.
**Clues:** Faint sea-rite slippage (M5, far-south faintest); Sera's oblique "grey hands" fragment (M6-oblique); the old-songs network thread.
**Combat Options:** A single sea-drowned Remembrance manifestation (scaled, AC 11) at a shrine — settle-able by rite; telegraphed and rare.
**Noncombat Options:** Rite, investigation, alliance — combat avoidable.
**Solo Safety Valves:** Non-violent settling; Sera and Coll assist; retreat to the wharves; the threat is faint.
**Rest/Time Pressure:** Safe rests; no hard clock (the Gulf is far from the edge).
**Rewards:** Sera's trust (southern network-key, far later); a rare far-region believer-ally; the chance to seed the maritime alarm; Mourner goodwill.
**Consequences:** Helping Sera plants the seed of the maritime world believing (Q_MAJOR_010). Ignored — the south stays oblivious and Sera grieves alone.
**Failure State:** If a rite isn't settled, a faint wharf-crisis hook opens; the Mourner thread persists — no dead end.
**Follow-Up Hooks:** Q_HGP_005 (Mallin as the bridge); Q_MAJOR_010; the continental old-songs network.
**Scaling Notes:** L11 — one faint sign. L14 — the failures spread and Sera's alarm becomes actionable.
**State Updates:** HIDDEN_CLUES (M5/M6-oblique south), RELATIONSHIPS (Sera, Coll), FACTION_STATE (Mourners), NPC_MEMORY.
**Related:** `MAJOR_CAMPAIGN_QUESTS.md` (Q_MAJOR_010), `../../11_mysteries_and_secrets/CLUE_INDEX.md`.

---

# Q_HGP_007_THE_DROWNED_STEPS — The Drowned Steps

**Quest Type:** Ruin salvage / monster problem / mystery (oblique). **Level Range:** 12–15; solo danger: high. **Secrecy:** mixed.
**Likely Checks/DCs:** Vehicles(water)/Survival DC 17 (the dive); Athletics DC 16; Arcana/Religion DC 18 (what the ruin is — gated); Investigation DC 17.
**Starting Hook:** Salvage-Captain Mab Reach (or a port-lord) wants the rumored Drowned Steps dived — a submerged Concord sea-ruin off the delta the port-lords covet and the sea-Mourners dread.
**Location:** The Drowned Steps (offshore submerged ruin); the delta-mouth.
**Primary NPCs:** Mab Reach (giver/guide), Salvage-mate Brann ("won't dive past the third step"), Tide-Mother Sera (warns against it), Pilot-Master Sef Tide (navigation).
**Factions:** Calderport/Saltgate (covet the salvage), Mourners' Circle (warn).
**Surface Problem:** Reach and salvage the Drowned Steps.
**Hidden Truth (DM):** The Drowned Steps are a far-south Concord sea-node (M2/M5-oblique) — a peripheral work, NOT the keystone, NOT the Court's seat. The dead/wrongness there corroborate the crisis's continental reach without explaining it. Keep the deepest steps unexplained and dangerous.
**Objectives:** 1) Reach the Steps. 2) Salvage/investigate (and decide how deep to go). 3) Survive what stirs there.
**Approaches:** A careful dive with Mab Reach; heed Sera's warning and go cautious; turn back at the "third step"; a relic-recovery for a port-lord.
**Obstacles:** The deadly dive; the ruin "not wanting to be dived"; stirring sea-dead in the deeps.
**Important Scenes:** The Steps rising from the green dark; Brann refusing the third step; a stirring deep-ruin presence (oblique, unexplained).
**Clues:** A far-south Concord node "waking" (M2 continental); the dead stirring at its oldest deeps (M5-oblique); never the mechanism.
**Combat Options:** Sea-drowned guardians / a stirring presence (scaled to L12–15; telegraphed) — escapable by retreat; deeper = deadlier.
**Noncombat Options:** Careful salvage, retreat, rite (settle rather than fight); the deep is optional.
**Solo Safety Valves:** Clear retreat at every "step"; Mab Reach and Sef Tide guide; Sera's warning telegraphs danger; turning back is rewarded with survival.
**Rest/Time Pressure:** Rests aboard ship; tide-windows constrain the dive (time pressure).
**Rewards:** Concord sea-salvage (coin + possibly a relic [STAGE_14_FINALIZE]); a continental M2 data-point; port-lord favor by choice.
**Consequences:** Going too deep risks death and may "wake" the Steps further (a regional consequence). A cautious dive yields salvage and a clean clue. Ignored — a port-lord hires someone worse.
**Failure State:** Forced retreat — the player escapes with partial salvage and the knowledge that the south, too, has a "waking" ruin; no dead end.
**Follow-Up Hooks:** Q_HGP_006 (Sera's dread confirmed); Q_HGP_001/002 (port-lord salvage politics).
**Scaling Notes:** L12 — shallow salvage. L15 — the deep ruin's full danger; a real guardian-boss at the lowest steps.
**State Updates:** HIDDEN_CLUES (M2/M5 far-south), INVENTORY, FACTION_STATE (port-lords), CONSEQUENCES.
**Related:** `../../11_mysteries_and_secrets/CLUE_INDEX.md`, `MAJOR_CAMPAIGN_QUESTS.md`.

---

# Q_HGP_008_THE_CROWNS_CUT — The Crown's Cut

**Quest Type:** Smuggling / trade dispute / low-mid stakes. **Level Range:** 11–14; solo danger: moderate. **Secrecy:** mixed.
**Likely Checks/DCs:** Deception/Persuasion DC 16 (customs); Stealth DC 16 (the run); Insight DC 15 (Vorr's leverage); Investigation DC 15.
**Starting Hook:** Crown-Customs Legate Vorr taxes the Gulf's delta trade for an absent crown; a free port (or a smuggler) hires the player to break, dodge, or expose the customs squeeze.
**Location:** The delta customs-posts; the Mardenmouth; the Fever Channels' edge.
**Primary NPCs:** Crown-Customs Legate Vorr, Dock-Boss "Anchor" Voss (squeezed docker), Smuggler-wife Senna, Crown-clerk Vesk (bribable), Crown-guard Sera (homesick, turnable).
**Factions:** Sallowmarch Protectorate (customs), Calderport/Saltgate (free ports), independent smugglers.
**Surface Problem:** Get a cargo past (or break) the crown's customs.
**Hidden Truth (DM):** Introduces the Sallowmarch crown's reach into the Gulf (a foreign-power thread; links Q_HGP_004 and the Sallowmarch region). Pure trade/politics; no central-mystery content.
**Objectives:** 1) Assess the customs squeeze. 2) Run, bribe, or expose it. 3) Avoid an imperial incident.
**Approaches:** Bribe Vesk/Sera; smuggle via Senna; expose Vorr's over-reach to the free ports; negotiate a fair tariff.
**Obstacles:** Vorr's cold authority; fever-thinned but real garrison; the free ports' rivalry.
**Important Scenes:** Vorr's stiff customs-wall; a tense night-run; turning homesick Crown-guard Sera.
**Clues:** The Sallowmarch crown's reach into the Gulf (foreign-power thread).
**Combat Options:** Customs soldiers (**Guard/Veteran-like**, fever-weakened) if a run is blown — avoidable by guile/bribery.
**Noncombat Options:** Bribery, smuggling, exposure, negotiation.
**Solo Safety Valves:** Multiple paths; turnable guards; the Channels offer escape; no forced fight.
**Rest/Time Pressure:** Safe rests in port; a cargo-window deadline.
**Rewards:** Free-port or smuggler favor; coin; a door toward the Sallowmarch (links Q_SP quests); contacts in the delta underworld.
**Consequences:** Breaking the squeeze pleases the ports and angers the crown. Exposing Vorr may get him recalled. Ignored — the squeeze tightens.
**Failure State:** Caught — a fine/detention by Vorr (not death); the player can buy or scheme out; play continues.
**Follow-Up Hooks:** Q_HGP_004; Q_SP quests (Sallowmarch); a crown grudge.
**Scaling Notes:** L11 — a bribe-and-run. L14 — an imperial-incident risk and a garrison crackdown.
**State Updates:** FACTION_STATE (Protectorate/ports), RELATIONSHIPS (Vorr, smugglers), CONSEQUENCES.
**Related:** `../../08_npcs/by_region/SALLOWMARCH_PROTECTORATE_NPCS.md`, `../../08_npcs/by_region/HOLLOW_GULF_PORTS_NPCS.md`.

---

## Related Files
- [`../../08_npcs/by_region/HOLLOW_GULF_PORTS_NPCS.md`](../../08_npcs/by_region/HOLLOW_GULF_PORTS_NPCS.md)
- [`../MAJOR_CAMPAIGN_QUESTS.md`](../MAJOR_CAMPAIGN_QUESTS.md) · [`../hooks_and_rumors/fc_HOLLOW_GULF_PORTS_HOOKS.md`](../hooks_and_rumors/fc_HOLLOW_GULF_PORTS_HOOKS.md)
