# HETHEWALD_FREE_HOLDS_QUESTS.md — Developed Quests (Stage 10)

---
type: quest
secrecy: mixed
status: static
region: The Hethewald Free Holds
factions: [Mourners' Circle, Cinder Ledger, Concord Remnant, Gravecallers]
level_range: 7-12
related: [../../08_npcs/by_region/HETHEWALD_FREE_HOLDS_NPCS.md, ../../04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md, ../hooks_and_rumors/fc_HETHEWALD_FREE_HOLDS_HOOKS.md, ../MAJOR_CAMPAIGN_QUESTS.md]
tags: [type:quest, far-continent, stage-10, region:hethewald, level:7-12, secrecy:mixed]
---

## AI Use

Seven developed quests for the Hethewald Free Holds (Tollwood writ large; forest free-holds, river-tolls, outlaws, deep Concord ruins; Lvl 7–12). Cast from `08_npcs/by_region/HETHEWALD_FREE_HOLDS_NPCS.md`. The crisis reads here as failing *forest-bargains* (the pagan cousin of the Mourners' songs and the official faith's failing rites). Feeds Q_MAJOR_017 (Bargain in the Deep Wood), Q_MAJOR_027 (Free Holds Vote). The Old Holds are surface-Concord ruins, NOT the keystone. Anchors: Hethemoot, Greenward, Tollreach, the Old Holds.

---

# Q_HFH_001_THE_WOODS_LAW — The Wood's Law

**Quest Type:** Negotiation / social infiltration / faction favor. **Level Range:** 7–9; solo danger: moderate. **Secrecy:** mixed.
**Likely Checks/DCs:** Persuasion DC 16 (Bram Hethe / the welcomer); Survival DC 16 (the deep wood); Insight DC 15 (the wood's law); Nature DC 15.
**Starting Hook:** To pass through the Hethewald at all, the player must earn the holds' welcome from Hold-Speaker Bram Hethe — who measures outsiders "against the wood's own law."
**Location:** Hethemoot (the great gathering-hold); the forest approaches.
**Primary NPCs:** Bram Hethe (giver/gatekeeper), Welcomer Mab Tarn (the social gateway), Hold-Elder Doss Greenward (distrusts outsiders), Moot-Warden Sera Hethe.
**Factions:** Independent (free-hold confederacy).
**Surface Problem:** Win the holds' welcome and safe passage.
**Hidden Truth (DM):** Bram secretly wants anyone who can tell him *why the old forest-bargains are failing* (the crisis in a pagan idiom). Earning the wood's law opens the region and seeds the bargain-failure thread (Q_MAJOR_017). No apex truth.
**Objectives:** 1) Win Mab Tarn's hospitality and Bram's trust. 2) Prove respect for the wood's law. 3) Earn safe passage.
**Approaches:** Honor forest-custom; win the welcomer; help a hold with a small problem; impress the moot.
**Obstacles:** The holds' suspicion of outsiders (Doss Greenward); the wood's law; the deep forest's dangers.
**Important Scenes:** Bram's slow, weighing courtesy; Mab Tarn deciding who eats at the hold-fire; a hostile elder won over.
**Clues:** The forest-bargains "going wrong" (M5-pagan, oblique — seeds Q_MAJOR_017); the Old Holds as forbidden ground.
**Combat Options:** Forest hazards or a wary hold-patrol (**Scout/Archer-like**) if the player blunders — avoidable by respect.
**Noncombat Options:** Custom, hospitality, persuasion, helping — combat avoidable.
**Solo Safety Valves:** Welcome is winnable peacefully; Mab Tarn and Brann the Guide aid; the player can withdraw; danger telegraphed.
**Rest/Time Pressure:** Hold-sanctuary for rests; no hard clock.
**Rewards:** The holds' welcome and safe passage (gateway to all Hethewald quests); Bram's trust; forest-guides; the bargain-failure thread.
**Consequences:** Earning the wood's law opens the forest. Offending the holds bars the region (no safe passage east). Ignored — the Hethewald stays closed.
**Failure State:** Refused welcome — the player is escorted out (not killed); reopen via a smaller hold or Brann; no dead end.
**Follow-Up Hooks:** Q_HFH_002 (the failing bargains); Q_HFH_004 (the Ledger); Q_MAJOR_017/027.
**Scaling Notes:** L7 — a welcome-trial. L9 — the holds' suspicion sharper as the bargains fail.
**State Updates:** FACTION_STATE (holds attitude), RELATIONSHIPS (Bram, Mab Tarn), NPC_MEMORY.
**Related:** `MAJOR_CAMPAIGN_QUESTS.md` (Q_MAJOR_017/027).

---

# Q_HFH_002_THE_FAILING_BARGAINS — The Failing Bargains

**Quest Type:** Investigation / death-rite failure (pagan idiom) / clue trail. **Level Range:** 8–11; solo danger: moderate. **Secrecy:** mixed.
**Likely Checks/DCs:** Religion/Nature DC 16 (grove-rites); Investigation DC 17 (the failing sites); Insight DC 16 (Onn's fragment); Survival DC 16.
**Starting Hook:** Forest-Mother Onn Greenward's grove-rites are slipping and the deep wood is "waking" — the old bargains that kept the dead quiet are failing, and no one knows why.
**Location:** Greenward (Onn's grove-village); failing deep-wood sites.
**Primary NPCs:** Onn Greenward (giver/oblique keeper), Grave-Singer Coll Greenward (failing graves), Grove-Warden Brann Oak (the wood "watching back"), Hold-Elder Doss Greenward (M5 witness).
**Factions:** Mourners' Circle (Onn), independent (the holds).
**Surface Problem:** Help the failing grove-rites and learn why the bargains slip.
**Hidden Truth (DM):** The crisis read through forest-paganism — the pagan cousin of the Mourners' songs. Onn is the EASTERN node of the old-songs network; her "the grey hands took the dead" is M6-oblique folk-memory ONLY (no mechanism). The Old Holds are where "the grey hands worked" — surface-Concord ruins, NOT the keystone.
**Objectives:** 1) Confirm the bargains are failing. 2) Help honor/restore a failing grove-rite. 3) Decide what to do about the waking deep wood.
**Approaches:** Grove-rite with Onn/Coll; investigate a failing deep-wood site; consult Brann Oak; correlate with the player's frontier knowledge.
**Obstacles:** The waking deep wood; the holds' pagan dread; the Old Holds' forbidden status.
**Important Scenes:** A grove-grave that "won't keep"; the deep wood "watching back"; Onn's grave, song-laced fragment.
**Clues:** Failing forest-bargains (M5-pagan); Onn's oblique "grey hands" fragment (M6-oblique); the Old Holds named (oblique, surface-Concord).
**Combat Options:** A deep-wood manifestation / a "woken" grove-dead (scaled L8–11, telegraphed) — settle-able by rite; retreat possible.
**Noncombat Options:** Rite, investigation, correlation — combat avoidable.
**Solo Safety Valves:** Non-violent settling; Onn, Coll, Brann Oak assist; retreat from the deep wood; telegraphed danger.
**Rest/Time Pressure:** Hold-sanctuary rests; a soft bargain-failure clock.
**Rewards:** Onn's trust (eastern network-key, far later); the forest's grief-lore; a pagan-idiom corroboration of the crisis; Mourner/hold goodwill.
**Consequences:** Helping the rites eases the wood and proves the crisis's reach. Ignored — the bargains fail worse and the deep wood wakes (links Q_HFH_006/Q_MAJOR_017).
**Failure State:** A failing rite unsettled → a hold-crisis hook; the Mourner thread persists; no dead end.
**Follow-Up Hooks:** Q_HFH_006 (the Old Holds); the continental old-songs network; Q_MAJOR_017.
**Scaling Notes:** L8 — one failing grove. L11 — the deep wood waking region-wide.
**State Updates:** HIDDEN_CLUES (M5-pagan, M6-oblique), RELATIONSHIPS (Onn, Coll), FACTION_STATE (Mourners/holds), NPC_MEMORY.
**Related:** `MAJOR_CAMPAIGN_QUESTS.md` (Q_MAJOR_017), `../../11_mysteries_and_secrets/CLUE_INDEX.md`.

---

# Q_HFH_003_THE_TOLL_OF_THE_HETHE — The Toll of the Hethe

**Quest Type:** Escort / turnable outlaw / moral dilemma. **Level Range:** 8–11; solo danger: moderate–high. **Secrecy:** mixed.
**Likely Checks/DCs:** Persuasion DC 16 (turning Greenfinger); Stealth DC 16; Insight DC 16 (splitting him from Skell-the-Younger); Survival/Vehicles(water) DC 15.
**Starting Hook:** Toll-Lord "Greenfinger" Maddoc taxes the Hethe with mock-courtesy and an easy grin — but his cruel lieutenant Skell-the-Younger wants the tolls turned to slaughter. The player must deal with the river-toll.
**Location:** Tollreach (the outlaw toll-camp); the Hethe.
**Primary NPCs:** "Greenfinger" Maddoc (outlaw/possible ally), Skell-the-Younger (the dark mirror), River-Pilot Mossa Hethe, Smuggler-Wife Doll Tull.
**Factions:** Independent (Greenfinger's crew), Cinder Ledger (his prey, via Hesk Dorr's trains).
**Surface Problem:** Deal with the Hethe's toll — pay, fight, or turn Greenfinger.
**Hidden Truth (DM):** Greenfinger is the Hethewald's Cady Renn — a robber with a line he hasn't crossed, turnable; Skell-the-Younger is the Skell-role dark mirror. He's also a grey-network witness to which deep-wood is "going wrong." No central-mystery content beyond an oblique "bad wood" note.
**Objectives:** 1) Resolve the toll (pay, fight, or turn Greenfinger). 2) Optionally split Greenfinger from Skell-the-Younger. 3) Protect the river-trade or the poor he claims to spare.
**Approaches:** Pay the toll; turn Greenfinger against a Ledger train; split him from his cruel lieutenant; expose the camp to the holds (betrayal).
**Obstacles:** Greenfinger's hidden camp; Skell-the-Younger's bloodlust; the "bad wood" disrupting ambushes.
**Important Scenes:** Greenfinger's mock-courteous robbery; Skell-the-Younger itching for blood; turning the lord against his lieutenant.
**Clues:** Which deep-wood is "going wrong" (M5-oblique grey-network witness).
**Combat Options:** Greenfinger's outlaws (**Bandit/Scout-like**, AC 15) in a forest ambush — avoidable by parley; Skell-the-Younger is the real threat if he rises.
**Noncombat Options:** Payment, alliance, splitting the lieutenant, betrayal — combat avoidable.
**Solo Safety Valves:** Greenfinger prefers toll to murder; turnable; Mossa Hethe for river-retreat; multiple resolutions.
**Rest/Time Pressure:** Rests at a hold; a cargo-deadline if escorting.
**Rewards:** Safe river-passage; a roguish ally (if turned); the outlaw-network's intelligence; coin.
**Consequences:** Turning Greenfinger gains a river-ally and curbs Skell-the-Younger. Letting Skell rise turns the tolls murderous (a regional clock). Betraying the camp burns a grey-network.
**Failure State:** A failed turn / lost cargo — Greenfinger is a recurring nuisance, not an enemy-for-life; no dead end.
**Follow-Up Hooks:** Q_HFH_004 (the Ledger trains); Q_HFH_002 (the bad wood); the Hethe underworld.
**Scaling Notes:** L8 — a toll-ambush. L11 — Skell-the-Younger's bid for the lordship and a river-war.
**State Updates:** RELATIONSHIPS (Greenfinger, Skell-the-Younger), FACTION_STATE (Tollreach/Ledger), CONSEQUENCES.
**Related:** `../../08_npcs/by_region/HETHEWALD_FREE_HOLDS_NPCS.md`.

---

# Q_HFH_004_THE_LOGGERS_PUSH — The Logger's Push

**Quest Type:** Faction conflict (Ledger) / protection / sabotage. **Level Range:** 8–11; solo danger: moderate. **Secrecy:** mixed.
**Likely Checks/DCs:** Persuasion DC 16; Stealth DC 16 (sabotage); Investigation DC 15; Insight DC 15.
**Starting Hook:** Factor Hesk Dorr drives the Cinder Ledger's logging and "old wood" trade into the sacred deep forest; Bram Hethe and the holds need help driving off the incursion before the wood is gutted.
**Location:** A Ledger logging-camp; the deep wood's edge; Hethemoot.
**Primary NPCs:** Factor Hesk Dorr (Ledger antagonist), Bram Hethe (ally), Grove-Warden Brann Oak, Moot-Warden Sera Hethe.
**Factions:** Cinder Ledger (logging/relic trade) vs. the free holds.
**Surface Problem:** Stop the Ledger's logging incursion into the sacred wood.
**Hidden Truth (DM):** Hesk Dorr's crews are "spooked by the deep wood" (the bargains failing where they cut) — an oblique link to Q_HFH_002. The "old wood"/relic angle ties the Ledger's continental reach (Q_MAJOR_004). No central-mystery content beyond oblique notes.
**Objectives:** 1) Assess the logging push. 2) Drive it off (negotiate, sabotage, or rally the holds). 3) Protect the sacred sites.
**Approaches:** Negotiate Dorr down; sabotage the logging-camp; rally the holds for a show of force; expose Dorr's relic-skim to the holds or a rival.
**Obstacles:** Dorr's relentless acquisition; the Ledger's resources; the deep wood spooking both sides.
**Important Scenes:** Dorr's cold, ledger-eyed acquisition; a logging-camp at a sacred grove's edge; the holds rallying.
**Clues:** The deep wood "spooking" the loggers (M5-oblique link to Q_HFH_002); the Ledger's "old wood"/relic trade (M3).
**Combat Options:** Logging-camp guards (**Guard/Veteran-like**) if force is used — avoidable by sabotage/negotiation.
**Noncombat Options:** Negotiation, sabotage, rallying, exposure — combat avoidable.
**Solo Safety Valves:** Multiple paths; hold-folk as allies; retreat into the wood; the player can avoid open battle.
**Rest/Time Pressure:** Hold rests; a logging-season deadline.
**Rewards:** The holds' deep trust; Bram Hethe's friendship; a blow to the Ledger's reach (Q_MAJOR_004); the sacred wood preserved.
**Consequences:** Driving off Dorr earns the holds' loyalty. Failing guts the wood and worsens the bargains (links Q_HFH_002/006). Exposing the relic-skim hurts the Ledger.
**Failure State:** The logging proceeds → the wood is gutted and the holds embittered; reopen via a deeper hold; no dead end.
**Follow-Up Hooks:** Q_HFH_002 (the bargains); Q_HFH_007 (the free holds vote); Q_MAJOR_004/017.
**Scaling Notes:** L8 — a small camp. L11 — a major Ledger push and a hold-mobilization.
**State Updates:** FACTION_STATE (Ledger/holds), RELATIONSHIPS (Bram, Hesk Dorr), CONSEQUENCES.
**Related:** `MAJOR_CAMPAIGN_QUESTS.md` (Q_MAJOR_004/017).

---

# Q_HFH_005_THE_FEUD_OF_THE_HOLDS — The Feud of the Holds

**Quest Type:** Negotiation / family conflict / council dispute. **Level Range:** 8–11; solo danger: moderate. **Secrecy:** mixed.
**Likely Checks/DCs:** Persuasion DC 17 (mediating); Insight DC 16; Investigation DC 16 (the feud's root); History/Nature DC 15.
**Starting Hook:** Two free-holds are feuding — worse now that the bargains fail and tempers fray — and Moot-Warden Sera Hethe asks the player to mediate before it turns to blood at the moot.
**Location:** Hethemoot; the feuding holds.
**Primary NPCs:** Moot-Warden Sera Hethe (giver), Bram Hethe (the confederacy's unity at stake), the two feuding hold-elders, Welcomer Mab Tarn.
**Factions:** Independent (the free-hold confederacy).
**Surface Problem:** Mediate a hold-feud before it shatters the confederacy.
**Hidden Truth (DM):** The feud is worsened by the failing bargains fraying everyone's nerves (oblique link to Q_HFH_002) and by the confederacy's always-fragile unity (links Q_MAJOR_027). A clean social/mediation quest; no central-mystery content.
**Objectives:** 1) Uncover the feud's true root. 2) Broker a peace the moot accepts. 3) Keep the confederacy whole.
**Approaches:** Mediate; uncover and address the feud's hidden cause; appeal to the wood's law; use Bram's authority; expose a manipulator.
**Obstacles:** Old grudges; frayed nerves (the bargains failing); the holds' pride; a possible outside manipulator (Ledger? outlaw?).
**Important Scenes:** Sera Hethe arbitrating; the two elders at the moot-fire; a feud nearly turning to blood.
**Clues:** The bargains' failure fraying the holds (oblique link to Q_HFH_002); the confederacy's fragility (Q_MAJOR_027).
**Combat Options:** A feud erupting to blows (**Scout/Archer-like** hold-folk) if mediation fails — avoidable.
**Noncombat Options:** Mediation, investigation, persuasion, exposure — the whole quest.
**Solo Safety Valves:** No combat gate; multiple resolutions; Sera Hethe and Bram assist; the player can withdraw.
**Rest/Time Pressure:** Hold rests; a moot-deadline before blood is shed.
**Rewards:** The holds' goodwill; a strengthened confederacy (helps Q_MAJOR_027); Sera Hethe and Mab Tarn as allies.
**Consequences:** A brokered peace strengthens the holds against outside pressure. A failed feud weakens the confederacy (links Q_HFH_004/Q_MAJOR_027).
**Failure State:** The feud turns to blood → a weakened confederacy and a regional grievance; play continues.
**Follow-Up Hooks:** Q_HFH_007 (the free holds vote); Q_HFH_004 (the Ledger exploiting disunity).
**Scaling Notes:** L8 — a contained feud. L11 — a confederacy-splitting crisis with an outside hand.
**State Updates:** FACTION_STATE (holds unity), RELATIONSHIPS (Sera Hethe, the elders), CONSEQUENCES.
**Related:** `MAJOR_CAMPAIGN_QUESTS.md` (Q_MAJOR_027).

---

# Q_HFH_006_THE_OLD_HOLDS — The Old Holds

**Quest Type:** Ruin / mystery (gated, oblique) / monster problem. **Level Range:** 10–12; solo danger: high. **Secrecy:** mixed.
**Likely Checks/DCs:** Religion/Arcana DC 18 (the Old Holds — gated); Survival DC 17 (deep wood); Stealth DC 17; Persuasion DC 16.
**Starting Hook:** Bram Hethe needs the failing of the bargains investigated at its worst — a deep-wood Old Holds ruin where "the grey hands worked" and the dead now stir, threatening the surrounding holds.
**Location:** The Old Holds (deep-wood Concord ruins); the sacred deep forest.
**Primary NPCs:** Bram Hethe (giver), Grove-Warden Brann Oak (guide to the threshold), Onn Greenward (the rite), Sub-Lector Wenn Vael (reckless Remnant breacher).
**Factions:** Independent (holds), Concord Remnant (covets the ruins), Mourners' Circle, Gravecallers (DM-watch — drawn by failing dead).
**Surface Problem:** Settle the stirring dead at a deep-wood Old Holds ruin before it threatens the holds.
**Hidden Truth (DM):** The Old Holds are SURFACE-Concord ruins (the Tollwood "Old Mast" logic, writ large) where "the grey hands worked" — a resonant echo, NOT the keystone. The stirring corroborates the crisis. Onn's rite can settle it (the bargain-logic). Wenn Vael's reckless dig risks waking it worse. NEVER confirm the mechanism.
**Objectives:** 1) Reach the Old Holds ruin. 2) Settle the stirring dead (rite or sealing). 3) Stop the reckless Remnant dig.
**Approaches:** Onn's grove-rite to settle it; honor the bargains (the pagan logic); stop or redirect Wenn Vael; seal the ruin.
**Obstacles:** The deep wood's dangers; the stirring dead; the Old Holds' forbidden power; Wenn Vael's recklessness.
**Important Scenes:** Brann Oak at the forbidden threshold; the Old Holds "humming" in the deep dark; Onn's settling-rite; Wenn Vael digging where he shouldn't.
**Clues:** The Old Holds as where "the grey hands worked" (oblique, surface-Concord — never the mechanism); the stirring dead (M5); the Remnant's reckless reach (Q_MAJOR_012/017).
**Combat Options:** Stirring dead / a deep-wood Old Holds presence (scaled L10–12, telegraphed) — settle-able by rite; retreat possible.
**Noncombat Options:** Rite, sealing, persuasion (stop Wenn Vael), retreat — combat is one path.
**Solo Safety Valves:** Settling > slaying; Brann Oak and Onn guide/aid; clear retreat; the deepest ruin is avoidable.
**Rest/Time Pressure:** Hold rests at the wood's edge; a stirring-clock before the dead threaten the holds.
**Rewards:** The holds' deep gratitude; the bargain-rite mastery (settle the failing dead); an oblique corroboration; a Remnant-direction clue.
**Consequences:** Settling it eases the holds and proves the crisis's reach. Wenn Vael's dig (if unchecked) wakes it worse (a regional disaster). Ignored — the deep wood wakes and the holds suffer (Q_MAJOR_017).
**Failure State:** The ruin wakes worse → a regional threat the player can later help contain; the apex truth is NOT revealed; no campaign-ending dead end.
**Follow-Up Hooks:** Q_HFH_002 (the bargains); Q_HFH_007 (the vote); Q_MAJOR_017 (Bargain in the Deep Wood); Q_MAJOR_012 (Remnant).
**Scaling Notes:** L10 — a contained stirring. L12 — the Old Holds fully waking; a boss-tier presence.
**State Updates:** HIDDEN_CLUES (oblique surface-Concord), FACTION_STATE (holds/Remnant/Gravecallers), WORLD_CLOCKS (deep-wood clock), CONSEQUENCES.
**Related:** `MAJOR_CAMPAIGN_QUESTS.md` (Q_MAJOR_017/012), `../../03_canon/DM_ONLY_CANON.md`.

---

# Q_HFH_007_THE_FREE_HOLDS_VOTE — The Free Holds Vote

**Quest Type:** Council dispute / political leverage / faction race. **Level Range:** 9–12; solo danger: low–moderate. **Secrecy:** mixed.
**Likely Checks/DCs:** Persuasion DC 17 (the moot); Insight DC 16; Investigation DC 16; Deception DC 16 (countering a manipulator).
**Starting Hook:** The holds gather at Hethemoot to decide the confederacy's course — resist the Ledger and the outside world, or bend — and the vote could swing on the player's word.
**Location:** Hethemoot (the great gathering).
**Primary NPCs:** Bram Hethe (the Speaker), Welcomer Mab Tarn, Hold-Elder Doss Greenward, Factor Hesk Dorr (outside pressure), the feuding/wavering elders.
**Factions:** Independent (the confederacy), Cinder Ledger (pressure).
**Surface Problem:** Influence the holds' great vote on their future course.
**Hidden Truth (DM):** The vote is the confederacy's future (Q_MAJOR_027) — whether the free holds resist the outside world (Ledger/League/crown) or bend. A clean political-leverage quest reflecting the player's prior Hethewald actions. The failing bargains shadow the debate (oblique). No apex truth.
**Objectives:** 1) Understand the factions at the moot. 2) Build a coalition for the player's preferred course. 3) Counter the outside manipulator (Hesk Dorr).
**Approaches:** Rally the holds to resist; broker a measured opening; expose Hesk Dorr's manipulation; leverage the player's prior deeds (Q_HFH_002/004/005).
**Obstacles:** The holds' division; the Ledger's pressure; the failing bargains stoking fear; a wavering moot.
**Important Scenes:** The moot-fire debate; Hesk Dorr's outside pressure exposed; the vote itself.
**Clues:** The confederacy's future course (Q_MAJOR_027); the failing bargains shadowing the debate (oblique).
**Combat Options:** None expected; if a manipulator's agents turn to force, **Guard/Bandit-like** — avoidable.
**Noncombat Options:** Politics, coalition, exposure, leverage — the whole quest.
**Solo Safety Valves:** No combat gate; multiple courses; the player's prior allies weigh in; the vote is winnable several ways.
**Rest/Time Pressure:** Hold rests; the moot is the deadline.
**Rewards:** A confederacy aligned to the player's influence (helps or hinders future regional play); the holds' lasting regard; a blow to or boon for the Ledger.
**Consequences:** The vote shapes the Hethewald's future (Q_MAJOR_027) — resistance, opening, or fracture. The player's prior deeds carry weight. A manipulated vote serves the Ledger.
**Failure State:** A fractured or manipulated vote → a weakened/co-opted confederacy; the thread persists; no dead end.
**Follow-Up Hooks:** Q_MAJOR_027 (Free Holds Vote); the Ledger's continental reach; future Hethewald play.
**Scaling Notes:** L9 — a contained vote. L12 — a confederacy-defining decision with continental stakes.
**State Updates:** FACTION_STATE (confederacy course), RELATIONSHIPS (Bram, the elders, Hesk Dorr), CONSEQUENCES.
**Related:** `MAJOR_CAMPAIGN_QUESTS.md` (Q_MAJOR_027).

---

## Related Files
- [`../../08_npcs/by_region/HETHEWALD_FREE_HOLDS_NPCS.md`](../../08_npcs/by_region/HETHEWALD_FREE_HOLDS_NPCS.md)
- [`../MAJOR_CAMPAIGN_QUESTS.md`](../MAJOR_CAMPAIGN_QUESTS.md) · [`../hooks_and_rumors/fc_HETHEWALD_FREE_HOLDS_HOOKS.md`](../hooks_and_rumors/fc_HETHEWALD_FREE_HOLDS_HOOKS.md)
