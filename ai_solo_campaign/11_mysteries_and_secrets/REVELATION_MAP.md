# REVELATION_MAP.md

---
type: mystery
secrecy: dm-only
status: static
level_range: 1-20
tags: [revelation, pacing, secrets, acts, rev-ids, three-clue-rule]
related: [MYSTERY_WEB.md, CLUE_INDEX.md, SECRET_INDEX.md, FALSE_LEADS_AND_MISDIRECTIONS.md, DISCOVERY_PATHS.md, SECRET_PROTECTION_MATRIX.md, ../12_campaign_arc/MAIN_ARC_OVERVIEW.md]
---

## Purpose

**DM-ONLY.** The sequence and timing of revelations, and the formal **revelation map**: every major revelation (REV-ID), its secrecy, its phase/level gate, its prerequisite chain, and its **three or more independent clue sources** drawn from different regions, NPCs, factions, and approaches. Use to pace secrets, guarantee no single point of failure, and avoid revealing the central truth too early. Never quote to the player.

## AI Use

Before delivering a major clue or revelation:
1. Find the REV-ID it feeds (below).
2. Confirm the current campaign phase/level is at or past the REV's gate.
3. Confirm any prerequisite REVs are already confirmed by the player.
4. Deliver only what the clue earns; check "What Must Not Be Revealed Yet."
5. After the player confirms a REV, log it in `KNOWN_CLUES.md` / `PLAYER_SAFE_CANON.md` and update the mystery-state tracker.

The legacy **R1-R8** labels (used across older files) map 1:1 onto the REV-IDs and are kept in each entry for compatibility. The **M-codes** (M0-M10) are the mystery threads in `MYSTERY_WEB.md`.

---

## Revelation Timeline (Phase Gates)

| Phase | Act | Levels | What the player may confirm | Hard ceiling (do not exceed) |
|---|---|---|---|---|
| Early | Act 1 | 1-4 | The failures have a **source and pattern** centered on the basin (REV_001). | No Remembrance-as-substance, no Concord sin, no Court, no steering-employer. |
| Mid | Act 2 | 5-8 | **Remembrance is a substance someone collects** (REV_002); a **human conspiracy** (REV_003 Reke; REV_004 steering). | The conspiracy is contemporary/human; NOT yet a century-old machine; NOT the Court. |
| Deep | Act 3 | 9-12 | **The Concord harvested the dead** (REV_005); **the Quietfall was deliberate** (REV_006); the afterlife is finite (REV_009). | The surviving Custodians/Court are hinted only, never named/confirmed. |
| Apex | Act 4 | 13-16 | **The Hollow Court lives and is restarting the harvest** (REV_007); meet Veyl; Maire's heresy (REV_010). | — |
| Choice | Act 5 | 17-20 | The full cost-set of every ending (REV_008). | — |

> **Phase is gated by revelation progress, not strictly by level.** A fast player who confirms the prerequisites early may advance a phase; a slow/passive player gets the truth delivered by the world clocks at a slower pace (no REV strictly *requires* the player to chase it). Use level bands as the default, prerequisites as the real lock.

---

## Major Revelations (REV-IDs)

Each REV lists: statement (DM-only where it is a hidden truth), secrecy, phase/level gate, what the player may safely infer before confirmation, prerequisite REVs, **3+ independent clue sources** (region / NPC / approach varied), supporting NPCs / quests / locations / objects, false interpretations, what changes after, what must not be revealed yet.

---

### REV_001 — The Failures Have a Source and a Pattern
*(legacy R1; mysteries M1, M5, M2-shape)*

- **Statement (player-reachable surface):** The dead are not lingering at random. Rites fail worse the nearer the drowned basin, the dead drift *toward* the water, and Wren's rite failed because *something held her.* The crisis has a center.
- **Secrecy:** discoverable (this is the intended Act 1 frame).
- **Gate:** Early / Act 1 / Lvl 1-4.
- **Safe early inference:** "It's a curse / decay / bad luck" is the wrong-but-fine starting read; the right read is "there is a pattern pointing at the basin."
- **Prerequisites:** none.
- **3+ independent clue sources (different regions/NPCs/approaches):**
  1. **Social/personal (Reach/Hollowmere):** Wren herself — C_SR_001 (she clings to "something unfinished"; she remembers dying).
  2. **Testimony/wilderness (Reach/Greyfens):** Old Sashe's drift-map — C_SR_005 (the dead consistently move basin-ward for years).
  3. **Ritual-observation (Reach, cross-settlement):** a Warden noting rites fail *worse* near water — C_SR_010 (Greywater Holm worst; Candlewick "holds" at the edge of the pull).
  4. **Physical (Reach/cemetery):** grave-soil drifting waterward — C_SR_004.
  5. **Regional corroboration (Ring 1):** honest M5 windows at Tilbrook, Coldhearth, Cobble Strand confirm the failures *radiate outward from the Reach* (C_AV_*/C_TW_*/C_PC_* M5 windows).
- **Supporting NPCs:** Wren, Tomas Brevin, Old Sashe, Grandmother Wend, Bann Oester, Warden Pell/Hale, Mam Tace (Vale), Mabon Crale (Coast).
- **Supporting quests:** Q_MAJOR_001, Q_THE_FAILING_FUNERAL, Q_SASHES_WARNING, Q_THE_HOLM_THAT_WONT_BURY_ITS_DEAD; Ring 1 M5 windows.
- **Supporting locations/objects:** Mourner's Green; the Drift-Line; the basin shore; the surfacing ruin (shape only).
- **False interpretations:** "a curse on Hollowmere"; "the Mourners are doing it"; "the Gravecallers are doing it." All fair, all correctable in Act 2.
- **Changes after:** turns horror into a solvable mystery; the basin becomes the obvious center.
- **Must not reveal yet:** the substance (REV_002), the Concord (REV_005), the Court (REV_007), the steering (REV_004).

---

### REV_002 — Someone Is Collecting the Dead (Remembrance Is a Substance)
*(legacy R2; mystery M3)*

- **Statement:** The lingering of the dead is a *substance* — a person's memory/identity — that can be stored in relics and that someone is deliberately collecting.
- **Secrecy:** dm-only until earned (then player-known once confirmed in Act 2).
- **Gate:** Mid / Act 2 / Lvl 5-8. (Act 1 gives only the *uncanny fragment* — relics feel "wrong," someone wants them — never the mechanism.)
- **Safe early inference:** "these relics are wrong and someone is buying them up."
- **Prerequisites:** REV_001 (helpful, not strict).
- **3+ independent clue sources:**
  1. **Magic (Reach or Caradril):** study a Remembrance relic — C_SR_011 / C_CAR_004 (it *stores a person*).
  2. **Forbidden/teaching (Reach/Greyfens):** the Gravecallers explain what the dead taught them — C_SR_012.
  3. **Mercantile (Reach/Caradril):** the Ledger vault relic / Ashmarket quiet-coin / Crucible smelting "incidents" — C_SR_013 / C_CAR_005 / C_CAR_006 (someone is *collecting on purpose*).
  4. **Scholarly (Caradril):** Concord Script texts describe "the keeping of the dead's pattern" — C_CAR_007 (Script-gated).
  5. **Far-continent corroboration (Emberfell/Karran):** "old glass" / "humming iron" relic-sources prove the substance and the trade exist continent-wide — C_FC_004 / C_FC_010 (oblique; never the mechanism's origin).
- **Supporting NPCs:** the Tallow Man, Domic Sael, Tallytooth Ren, Iss Marlow, "Tidewife" Sorrel, Beck Harrow, Cassia Mourn, Doss Ashfast (far), Mully Karr (far).
- **Supporting quests:** Q_MAJOR_004, Q_QUIET_COIN, Q_THE_SMELTING, QL3_WHAT_THE_VAULT_REMEMBERS, Q_SAINTS_BONES (Vale), Q_THE_SALT_PRICE (Coast), Q_ET_003/Q_KM_004 (far echoes).
- **Supporting locations/objects:** the Peat Chapel altar relic; the Ledger vault relic; "old glass" from the Deep Adit; Ashmarket quiet-coin.
- **False interpretations:** "it's just valuable salvage / antiquities"; "it's a Ledger scam, nothing supernatural." Correctable by a relic demonstration.
- **Changes after:** reframes the crisis as a conspiracy with profit/power motives; implicates the Ledger and Remnant.
- **Must not reveal yet:** the machine's *age* (keep it contemporary); the Court.

---

### REV_003 — A Trusted Authority Is Steering the Basin Reopening
*(legacy R3; mystery M4 — Reke)*

- **Statement:** The basin "water-rights" scheme is a cover to *reopen the drowned shrine*; Councilor Reke is pushing it for a hidden reason and serves a hidden master.
- **Secrecy:** dm-only until earned. Act 1 banks *suspicion only*.
- **Gate:** Mid / Act 2 / Lvl 5-8. (Act 1: "Reke is hiding something" / "the scheme is a cover" — never "he's a traitor serving the Court.")
- **Safe early inference:** "the basin push doesn't add up; someone wants the water gone."
- **Prerequisites:** REV_001.
- **3+ independent clue sources:**
  1. **Political (Reach):** Reeve Coalmont's suspicions + the council votes — C_SR_014.
  2. **Paper trail (Reach/Caradril):** the fabricated water-rights filings (Pevin Oss) + a misfiled charter-registry record in Caradril (Ledger -> "Reach water-rights works") — C_SR_015 / C_CAR_008.
  3. **Surveillance (Reach):** tail Reke to the basin shore at night — C_SR_016.
  4. **Money (Reach):** the Ledger factor's grumbling that "it's not really about water" — C_SR_017.
  5. **Lawful authority (Reach):** Magister-Reeve Sela Coalmont suspects the Compact is *steered against the Reach* (can't yet name Reke) — C_SR_018.
- **Supporting NPCs:** Reeve Coalmont, Sela Coalmont, Pevin Oss, Sergeant Hesk, Domic Sael, Halla Coalmont, Otho Brail (Caradril council bribe-tally).
- **Supporting quests:** Q_MAJOR_002, Q_ACT1_COMPACT_THE_REEVES_DOUBT, QC2_THE_DOCTORED_SURVEY, Q_THE_REED_HOLMS, Q_THE_SEALED_LETTER (Caradril echo).
- **Supporting locations/objects:** the Compact records office; the basin shore at night; the Reed Holms eviction trail.
- **False interpretations:** "Reke is just ambitious / corrupt for money"; "the Ledger alone is behind it." Fair Act 2 reads; corrected when his master surfaces (REV_007 territory).
- **Changes after:** names a human antagonist; raises the basin-clock stakes.
- **Must not reveal yet:** that Reke's master is the Court (reveal only "someone above him").

---

### REV_004 — You Were Steered Here
*(legacy R4; mystery M8)*

- **Statement:** Sefra Quick was paid by a "wrong-money" patron to point the player at the failed rite/shrine; the player is an unwitting probe.
- **Secrecy:** dm-only until earned (then a personal player-known shock).
- **Gate:** Mid / Act 2-3 / Lvl 5-12 (flexible — may land early as a shock; keep the *ultimate* employer hidden).
- **Safe early inference:** "Sefra's job was odd / her money was strange" (Act 1 unease only).
- **Prerequisites:** none strict; lands best after REV_001.
- **3+ independent clue sources:**
  1. **Social/confession (Reach):** press Sefra — C_SR_019 (she's uneasy about the money; she confesses she doesn't know whom she served).
  2. **Follow-the-money (Reach/Caradril):** trace the patron's payments to a cutout — C_SR_020 / C_CAR_009.
  3. **Pattern (player-driven):** the player notices how conveniently they keep being pointed at the shrine — C_SR_021 (DM confirms what they can prove).
  4. **Broker (Caradril):** the Hush sells a fragment of the correspondent thread — C_CAR_010 (costly; lead only).
- **Supporting NPCs:** Sefra Quick, Halla Coalmont, the Bellman, Halloran Voss (compromised correspondent conduit).
- **Supporting quests:** Q_MAJOR_007, Q_THE_BELLMANS_PRICE, Q_THE_SEALED_LETTER, Q_THE_OPEN_CHARTER.
- **Supporting locations/objects:** Sefra's lodgings; the patron's payment trail; the Magisterium correspondent thread (lead only — never a named second Court agent).
- **False interpretations:** "Sefra set me up for a rival faction"; "the Ledger hired me." Fair; the true (Court-adjacent) employer stays murky.
- **Changes after:** a trust crisis; personal stakes; the player questions every "lucky" lead.
- **Must not reveal yet:** the cutout traces to the Hollow Court (keep it Reke-adjacent and murky).

---

### REV_005 — The Concord Harvested the Dead
*(legacy R5; mystery M6)*

- **Statement:** The Concord's "keeping the dead at peace" was a *harvest*. Its golden age was powered by consuming the dead's Remembrance.
- **Secrecy:** dm-only. The apex-historical truth.
- **Gate:** Deep / Act 3 / Lvl 9-12.
- **Safe early inference (pre-Act 3):** "the Concord wasn't kind"; "the dead are angry at the old order" (atmosphere only).
- **Prerequisites:** REV_002 (substance) and REV_001; ideally exposure to a Concord ruin/Script.
- **3+ independent clue sources:**
  1. **Archives/documentary (Caradril):** the Sealed Archive — C_CAR_011 (the clearest written proof; Script-gated, Act 3).
  2. **Confession (Reach):** Warden Othetha breaks her oath — C_SR_022 (late, trust-gated).
  3. **The dead testify (Reach/Greyfens):** a channeled Quietfall-era witness via the Tallow Man — C_SR_023.
  4. **Song/folk (Reach + Ring 1):** Wend's fully decoded old songs ("the Concord ate the dead") — C_SR_024 — corroborated by the **old-songs network**: Ezrith Combe (Vale), Salt-Mother Bryd (Coast), Goodwife Sennet (Tollwood), and far anchors (Wenna Lowwater/Sela Reed/Tess Brackhold/Senna Crale) — C_FC_011 (folk-fragment only, far).
  5. **Far surface-proof (Concord Heartlands):** the Ruin'd Crown / Sealed-equivalent records corroborate the Concord's true scale and sin — C_FC_001 (NEVER implies the live machine/keystone is there).
- **Supporting NPCs:** Quorrin Vane, Lector Briss (once disillusioned), Othetha, the Tallow Man, Wend, the old-songs network, Wessel Dree (Archive lock), Tamsin Orr (Script gate), Hollin Vane (far, apex-adjacent — never confirms the Court).
- **Supporting quests:** Q_MAJOR_003, Q_MAJOR_011, Q_MAJOR_012, Q_THE_SEALED_ARCHIVE, QR3_THE_IDEALIST_AND_THE_ARCHIVIST, Q_CH_002 (Into the Crown).
- **Supporting locations/objects:** the Sealed Archive; the Whispering Cairn census-wall; the Barrow of Nine Doors glyphs; the Ruin'd Crown record-vault (far).
- **False interpretations:** "the Concord fell because it was decadent"; "it was punished by the gods." Corrected by the documentary + dead-witness convergence.
- **Changes after:** destroys the noble-fallen-order myth; recontextualizes all history; implicates the Wardens (unwitting guardians) and the Remnant (would-be heirs).
- **Must not reveal yet:** the Court's *survival* (still only hinted).

---

### REV_006 — The Quietfall Was Deliberate
*(legacy R6; mystery M9)*

- **Statement:** The inner Custodians destroyed their own order on purpose to *pause* the harvest and let the drained afterlife refill.
- **Secrecy:** dm-only.
- **Gate:** Deep / Act 3 / Lvl 9-12 (pairs with REV_005; do not separate by more than an act).
- **Safe early inference:** none before Act 3 beyond "the Quietfall is stranger than the histories say."
- **Prerequisites:** REV_005.
- **3+ independent clue sources:**
  1. **Archives (Caradril):** the Sealed Archive's planned, signed Quietfall — C_CAR_012.
  2. **Confession (Reach):** Othetha's confession (the Wardens were seeded to keep the pause) — C_SR_025.
  3. **The dead testify (Reach):** the Tallow Man's Quietfall-era witness — C_SR_023 (shared with REV_005, distinct content).
  4. **Inscription (Reach/Caradril/far):** Concord Script inscriptions at the shrine and node-sites stating the pause — C_SR_026 / C_CAR_013 (Script-gated).
- **Supporting NPCs:** Quorrin Vane, Othetha, the Tallow Man, Wessel Dree, Sabine Ferrant (far/Remnant true believer — frames it as "holy restoration").
- **Supporting quests:** Q_MAJOR_011, Q_THE_SEALED_ARCHIVE, Q_MAJOR_006 (Warden seal).
- **Supporting locations/objects:** the Sealed Archive; shrine inscriptions; node-site Script.
- **False interpretations:** "the Quietfall was an accident the Concord caused by overreach." Close but wrong; the *intent* (a controlled pause) is the key.
- **Changes after:** reframes the world's founding trauma; explains the "age of healing"; directly sets up the Court.
- **Must not reveal yet:** that the Custodians who did it *still exist* (REV_007).

---

### REV_007 — The Hollow Court Lives and Is Restarting the Harvest
*(legacy R7; mystery M7 — APEX)*

- **Statement:** The original Custodians survive as preserved Remembrance beneath the basin — the Hollow Court — and are restarting the harvest "to save everyone" from the slow thinning.
- **Secrecy:** **dm-only — the campaign's keystone reveal.** Highest protection. See `SECRET_PROTECTION_MATRIX.md`.
- **Gate:** Apex / Act 4 / Lvl 13-16. Before this, the Court is a *legend only*; no clue, NPC, or site names it as real.
- **Safe early inference:** none. Earlier clues must point at Reke / the Remnant / the Ledger first.
- **Prerequisites:** REV_003 (Reke serves someone) AND REV_005 (the Concord harvested) AND ideally REV_006 (deliberate Quietfall).
- **3+ independent clue sources:**
  1. **Physical (Reach/Under-Shrine):** descend to the under-shrine and meet them — C_SR_027 (late-arc, lethal-telegraphed).
  2. **Convergence (cross-region):** assemble REV_003 + REV_005 + REV_006 into the only explanation that fits — C_SR_028 (inference, DM confirms).
  3. **Heretic/forbidden (Reach):** Custodian Maire reaches out, OR the Tallow Man's dead name "the ones who would not pass" — C_SR_029.
- **Supporting NPCs:** Custodian Veyl, Custodian Maire, Custodian Orre, Councilor Reke (the link), the Tallow Man.
- **Supporting quests:** Q_MAJOR_014 (DM-only), Q_MAJOR_028 (faction war converges), Q_MAJOR_002 (basin culmination).
- **Supporting locations/objects:** the Under-Shrine / Drowned Keystone (beneath Hollowmere); convergence of all prior proof.
- **False interpretations:** "Quorrin/the Remnant is the apex"; "Reke is the top." Both are *deliberately* the player's likely Act 3 guess; the Court is the true apex above them.
- **Changes after:** names the apex power; makes the antagonist a *person with an argument* (Veyl); opens the endgame choice (REV_008).
- **Must not reveal earlier:** anything that confirms the Court is real, located beneath Hollowmere, or composed of surviving Custodians. Keep it a ghost story until the gate.

---

### REV_008 — The Choice and Its Costs
*(legacy R8; mystery M10)*

- **Statement:** Every ending for the Remembrance has a terrible price; a *synthesis* (consensual system) is possible but hard.
- **Secrecy:** dm-only until apex; the *choice* becomes player-known in Act 4-5.
- **Gate:** Choice / Act 4-5 / Lvl 13-20.
- **Prerequisites:** REV_007.
- **3+ independent clue sources (consequence-knowledge, not truth-clues):**
  1. **Gravecaller warning (Reach):** destroying the shrine = catastrophe — C_SR_030.
  2. **Warden warning (Reach):** sealing = end of resurrection — C_SR_031.
  3. **The Court's case (Under-Shrine):** Veyl's argument for a controlled restart = stability + horror — C_SR_032.
  4. **The heretic's synthesis (Under-Shrine):** Maire's case that the dead could *choose* — C_SR_033; corroborated by the **far hopeful contrast** (Sunmark's working grove-faith) — C_FC_012.
- **Supporting NPCs:** the Tallow Man, Cole Ashby, Othetha, Veyl, Maire, Sael Sunmark / Sun-Singer Doll (far hopeful echo).
- **Supporting quests:** Q_MAJOR_015 (The Fate of the Remembrance), Q_MAJOR_026 (the grove that will not harvest).
- **Endings:** seal / restart-controlled / seize / destroy / transform (see `MAIN_ARC_OVERVIEW.md`).
- **Changes after:** turns the climax into an informed moral decision, not a reflex.
- **Must not reveal yet:** nothing further — this is the final layer; the epilogue reflects what the player knew and chose.

---

### REV_009 — The Afterlife Is Finite and Was Nearly Drained
*(supporting cosmological; mysteries M3/M6/M7)*

- **Statement:** The Quiet Country is finite; centuries of harvest nearly emptied it; this is why resurrection is dangerous and why "thin-born" people exist.
- **Secrecy:** dm-only.
- **Gate:** Deep / Act 3 / Lvl 9-14 (lands with or after REV_005/REV_006; can deepen into Act 4).
- **Safe early inference:** "resurrection has gotten harder and more dangerous since the Quietfall" (this is public/player-safe already); the *cause* is gated.
- **Prerequisites:** REV_002; ideally REV_005.
- **3+ independent clue sources:**
  1. **Magic/research (Caradril/Reach):** deep study of resurrection failure + relic analysis — C_CAR_014.
  2. **The thin-born (Caradril/Reach):** the thin-born refugees in the Sill and "thin" Harrowgast miners as living evidence — C_SR_034 / C_CAR_015.
  3. **The dead/Court testify (Reach/Under-Shrine):** Veyl's case rests on it; the Tallow Man's witness names "the empty country" — C_SR_035.
  4. **Far cosmic echo (Wender Steppe/Sunmark):** Wind-Singer Esha's "the Sky has gone thin in the south" / Sun-Singer Doll's "a far root aches" — C_FC_013 (deeply oblique; never names the Quiet Country/harvest).
- **Supporting NPCs:** Onaia Veen (clinical), Mother Ysarra (city failures), Renna Sill (thinning local), Veyl, the Tallow Man, Wind-Singer Esha (far), Sun-Singer Doll (far).
- **Supporting quests:** Q_THE_FUNERAL_THAT_WOULDNT_TAKE, Q_MAJOR_024 (steppe), Q_MAJOR_026 (Sunmark).
- **False interpretations:** "resurrection is hard because magic is fading generally." Corrected by tying it to the harvest.
- **Changes after:** raises the stakes of every ending (sealing/restarting both touch the afterlife's survival).
- **Must not reveal yet:** that the Court caused it deliberately (folds into REV_005/REV_007).

---

### REV_010 — Maire's Heresy: The Court Could End Itself
*(supporting; mysteries M7/M10 — synthesis key)*

- **Statement:** Custodian Maire secretly believes the Court should let itself end and the dead should choose — the key to the "transform/synthesis" ending.
- **Secrecy:** dm-only; endgame only.
- **Gate:** Apex / Act 4-5 / Lvl 14-20.
- **Prerequisites:** REV_007.
- **3+ independent clue sources:**
  1. **Apex contact (Under-Shrine):** Maire reaches out directly — C_SR_036.
  2. **Court internal tension (Under-Shrine):** the player perceives Orre's hawkishness vs. Maire's doubt — C_SR_037.
  3. **The synthesis evidence (cross-region):** the far hopeful contrast (Sunmark) + Gravecaller fragments suggest a consensual system is conceivable — C_FC_012 / C_SR_038.
- **Supporting NPCs:** Custodian Maire, Custodian Orre, Veyl (foil), Sael Sunmark (far hopeful contrast).
- **Supporting quests:** Q_MAJOR_015.
- **Changes after:** unlocks the hardest, best-outcome ending; requires uniting unlikely allies.
- **Must not reveal yet:** nothing later — this is endgame-only.

---

## Revelation Dependency Graph (DM)

```
REV_001 (source/pattern)
   |-> REV_002 (substance) -> REV_005 (Concord harvested) -> REV_006 (deliberate Quietfall)
   |-> REV_003 (Reke steers)                |                        |
   |-> REV_004 (you were steered)           +----> REV_009 (finite afterlife)
                                            |
   REV_003 + REV_005 + REV_006  ==========> REV_007 (Hollow Court lives) [APEX]
                                                     |
                                                     +-> REV_008 (the choice & costs)
                                                     +-> REV_010 (Maire's heresy / synthesis)
```

- REV_007 has **no single-source path**: it requires convergence of three independent prior REVs *or* a lethal-telegraphed physical descent *or* a heretic/forbidden contact — never one NPC, one document, or one roll.
- Every REV above has **>=3 independent clue sources** spanning different regions, NPCs, factions, and approaches (verified in `CLUE_INDEX.md`).

---

## Pacing Guard Rails

- Keep Act 1 *small and personal* (REV_001/Wren), Act 2 *conspiratorial and contemporary* (REV_002/REV_003/REV_004), Act 3 *historical and shattering* (REV_005/REV_006/REV_009), Act 4 *apex* (REV_007/REV_010), Act 5 *choice* (REV_008).
- If the player rushes (e.g., dives the shrine at level 4), do **not** dump REV_007 — gate it: the upper shrine is dangerous, the Court is dormant/sealed, and the player gets *fragments* (more clues), not the apex truth. Telegraph lethal danger.
- The world clocks advance the truth toward a passive player, so no revelation strictly *requires* the player to chase it — but chasing is always faster and safer.
- **Never let a far-continent source deliver REV_007 or the keystone mechanism.** Far echoes corroborate the *theme* (REV_002/REV_005 obliquely, REV_009 deeply obliquely) but never name the Court, the keystone, or the Concord Deep.

## Related Files

- [`MYSTERY_WEB.md`](MYSTERY_WEB.md)
- [`CLUE_INDEX.md`](CLUE_INDEX.md)
- [`SECRET_INDEX.md`](SECRET_INDEX.md)
- [`FALSE_LEADS_AND_MISDIRECTIONS.md`](FALSE_LEADS_AND_MISDIRECTIONS.md)
- [`DISCOVERY_PATHS.md`](DISCOVERY_PATHS.md)
- [`SECRET_PROTECTION_MATRIX.md`](SECRET_PROTECTION_MATRIX.md)
- [`../12_campaign_arc/MAIN_ARC_OVERVIEW.md`](../12_campaign_arc/MAIN_ARC_OVERVIEW.md)
- [`../01_runner_protocol/SECRET_REVEAL_PROTOCOL.md`](../01_runner_protocol/SECRET_REVEAL_PROTOCOL.md)
