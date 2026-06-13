# CLUE_INDEX.md

---
type: index
secrecy: dm-only
status: static
tags: [index, clues, dm-only, three-clue-rule]
related: [MYSTERY_WEB.md, REVELATION_MAP.md, SECRET_INDEX.md, ../02_runtime_state/HIDDEN_CLUES.md]
---

## Purpose

**DM-ONLY.** Master index of every authored clue in the campaign. The AI DM uses this to track the full clue landscape and to find clues for a given mystery, location, or discovery method quickly. Clues are extracted from `MYSTERY_WEB.md` (clue paths per mystery) and pacing-checked against `REVELATION_MAP.md`. Never summarize to the player.

## Current Status

**Stage 11 expanded.** Populated from the Stage 1 mystery web, then expanded with a **region-coded clue layer** (`C_SR_*`/`C_CAR_*`/`C_AV_*`/`C_TW_*`/`C_PC_*`/`C_FC_*`) cross-referenced to the formal `REV_*` revelations in `REVELATION_MAP.md`, plus the Stage 3/4 region anchors and the far-continent echo clues. All clues are authored and currently **hidden** — the player has discovered nothing at campaign start. As play progresses, update each clue's status here and mirror discovered clues into `../02_runtime_state/KNOWN_CLUES.md` (remove or mark them in `../02_runtime_state/HIDDEN_CLUES.md`).

Clue IDs use two compatible patterns: the original `C-<mystery>-<n>` (e.g. `C-M1-2`, the canonical per-mystery clues) and the Stage 11 region-coded `C_<REGION>_<nnn>` (e.g. `C_SR_001`, `C_CAR_011`, `C_FC_001`) used by the revelation map. Many region-coded clues are the same authored clue as a C-M* under a region ID; new ones extend redundancy. Several mysteries are solved by **convergence** of other mysteries rather than by net-new clues; those are noted as convergence clues. Full runnable per-clue detail lives in the regional trail files `by_region/*_CLUES.md`.

---

## Clue Index

| Clue ID | Mystery | Type | Where Found | Discovery Method | Status |
|---|---|---|---|---|---|
| C-M1-1 | M1 — Wren's failed rite | Social | Speaking with Wren (in town) | Social (Insight/Persuasion, roleplay) | hidden |
| C-M1-2 | M1 — Wren's failed rite | Indirect | A Warden examining Wren | Magic/Ritual (Religion/Medicine) | hidden |
| C-M1-3 | M1 — Wren's failed rite | Symbolic | Mourners' eldest and the old songs | Social (folk knowledge) | hidden |
| C-M1-4 | M1 — Wren's failed rite | Physical | Wren's grave on the town cemetery | Exploration (Investigation/Survival) | hidden |
| C-M2-1 | M2 — The drowned shrine | Direct | The basin shore / a surfacing ruin | Exploration (Concord Script; needs a reader/Comprehend Languages) | hidden |
| C-M2-2 | M2 — The drowned shrine | Indirect | The fen-guide's map of the drifting dead | Social/Document (testimony) | hidden |
| C-M2-3 | M2 — The drowned shrine | Document | Compact survey records (records office) | Document (Investigation) | hidden |
| C-M2-4 | M2 — The drowned shrine | Symbolic | The Gravecaller speaker's channeled dead | Magic/Forbidden (social contact) | hidden |
| C-M3-1 | M3 — What is Remembrance? | Magic | A Remembrance relic | Magic (Arcana/Religion) | hidden |
| C-M3-2 | M3 — What is Remembrance? | Direct | The Gravecallers' teaching | Social (forbidden contact) | hidden |
| C-M3-3 | M3 — What is Remembrance? | Direct | The Ledger's Hollowmere vault relic | Document/Magic (via a turned factor or a heist) | hidden |
| C-M3-4 | M3 — What is Remembrance? | Document | Concord Script texts (Remnant scholar) | Document (scholarly; language gate) | hidden |
| C-M4-1 | M4 — Who pushes the basin scheme? | Indirect | The reeve's suspicions + the council votes | Social/Investigation (Insight) | hidden |
| C-M4-2 | M4 — Who pushes the basin scheme? | Document | The fabricated "water rights" filings | Document (Investigation) | hidden |
| C-M4-3 | M4 — Who pushes the basin scheme? | Physical | Tailing the councilor to the basin shore at night | Exploration (Stealth/Perception) | hidden |
| C-M4-4 | M4 — Who pushes the basin scheme? | Indirect | The Ledger factor's grumbling about funding | Social | hidden |
| C-M5-1 | M5 — The dead's drift | Indirect | The fen-guide's observations | Social (testimony) | hidden |
| C-M5-2 | M5 — The dead's drift | Physical | Wren's grave drifting waterward | Exploration (Investigation/Survival) | hidden |
| C-M5-3 | M5 — The dead's drift | Symbolic | Gravecaller lore | Social (forbidden contact) | hidden |
| C-M5-4 | M5 — The dead's drift | Indirect | A Warden noticing rites fail worse near the basin | Magic/Ritual (observation) | hidden |
| C-M6-1 | M6 — The Concord's true purpose | Document | Caradril Concord archives | Document (Remnant access; clearest proof) | hidden |
| C-M6-2 | M6 — The Concord's true purpose | Direct | A senior Warden breaking her oath | Social (late; trust-gated confession) | hidden |
| C-M6-3 | M6 — The Concord's true purpose | Direct | A channeled Quietfall-era witness | Magic/Forbidden (the dead testify) | hidden |
| C-M6-4 | M6 — The Concord's true purpose | Symbolic | The fully-decoded old songs | Social (earn Mourners' trust) | hidden |
| C-M7-1 | M7 — The Hollow Court | Physical | The under-shrine (late-arc) | Exploration (dangerous descent) | hidden |
| C-M7-2 | M7 — The Hollow Court | Convergence | Assemble M4 + M6 + M9 | Investigation/inference (convergence) | hidden |
| C-M7-3 | M7 — The Hollow Court | Direct | A heretic Court member reaches out / channeled dead name "the ones who would not pass" | Social/Forbidden (contact) | hidden |
| C-M8-1 | M8 — Why is the PC here? | Social | Pressing the fixer who made first contact | Social (Insight/Persuasion; confession) | hidden |
| C-M8-2 | M8 — Why is the PC here? | Document | Tracing the patron's payments to a cutout | Document (Investigation; follow the coin) | hidden |
| C-M8-3 | M8 — Why is the PC here? | Indirect | Pattern: the PC keeps being pointed at the shrine | Player-driven realization (DM confirms) | hidden |
| C-M9-1 | M9 — The deliberate Quietfall | Document | Caradril archives | Document (Remnant access) | hidden |
| C-M9-2 | M9 — The deliberate Quietfall | Direct | A senior Warden's confession | Social (trust-gated) | hidden |
| C-M9-3 | M9 — The deliberate Quietfall | Direct | A channeled Quietfall-era witness | Magic/Forbidden (the dead testify) | hidden |
| C-M9-4 | M9 — The deliberate Quietfall | Symbolic | Concord Script inscriptions at the shrine | Exploration/Document (language gate) | hidden |
| C-M10-1 | M10 — What to do about it | Consequence | Gravecaller warning: destroying it risks catastrophe | Social (forbidden contact) | hidden |
| C-M10-2 | M10 — What to do about it | Consequence | Warden warning: sealing ends resurrection | Social (trust-gated) | hidden |
| C-M10-3 | M10 — What to do about it | Consequence | The Court leader's case for controlled restart | Social (apex contact) | hidden |
| C-M10-4 | M10 — What to do about it | Consequence | The Court heretic's synthesis argument | Social (apex contact) | hidden |

---

## Stage 3 Clue Access Points (Region Anchors)

Stage 3 **did not create new mysteries or new clues** — it gave the existing M1–M9 clue paths concrete *places and NPCs* in the deep-built region, strengthening the three-clue rule by anchoring each path to authored content. Cross-reference for the AI DM (all still `hidden` at start):

| Mystery / Clue | New Authored Access Point (Stage 3) | File |
|---|---|---|
| C-M2-1 (shrine Script) | The Surfacing Ruin (basin shore); Roofless Hall / Cold Cairns (Heights); the Whispering Cairn census-wall | wilderness + `THE_WHISPERING_CAIRN.md` |
| C-M2-2/3/4 (shrine) | Sunken Tollhouse Script; Bly's river-salvage; the Drowned Blind's channeled dead | `THE_SUNKEN_TOLLHOUSE.md`, `KETTLE_BRIDGE.md`, `GREYFENS_SITES.md` |
| C-M3-1/3 (Remembrance relic) | Peat Chapel altar relic; Ledger Vault relic; "old glass" in the Deep Adit / Marlow's cellar | `THE_PEAT_CHAPEL.md`, `THE_LEDGER_VAULT.md`, `THE_DEEP_ADIT.md`, `SALTMARGIN.md` |
| C-M4-2/3/4 (basin scheme) | Pevin Oss's doctored filings; tail Reke at the basin shore; Bly/Marlow funding grumbles; the Reed Holms land-grab | `KETTLE_BRIDGE.md`, `BASIN_SHORE_AND_HOLMS_SITES.md`, `Q_THE_REED_HOLMS.md` |
| C-M5-1/2/4 (the drift) | The Drift-Line (Sashe); grave-drift at Greywater & Kettle Bridge (Bann Oester); rites fail worse near water (Pell); Reedford's grey woman | `GREYFENS_SITES.md`, `GREYWATER_HOLM.md`, `Q_PELLS_DOUBT.md`, `Q_THE_GREY_WOMAN_AT_THE_FORD.md` |
| C-M6/M9 fragments (Act 3 gate) | Whispering Cairn census-wall; Deep Adit Relay-Vault; Candlewick archive-stone; Barrow of Nine Doors layered glyphs; the Tallow Man at Mother Tongue Pool | cairn/adit/barrow dungeons + `CANDLEWICK.md` |

**Gate reminder:** M6/M9/M7 access points give *fragments* in Act 1–2; the apex truth stays gated to Act 3–4 per `REVELATION_MAP.md`.

## Stage 4 Clue Access Points (Caradril City Anchors)

Stage 4 **created no new mysteries and no new clues** — it anchored existing M2/M3/M4/M6/M8/M9 paths to the first major city, deepening the three-clue rule. All still `hidden` at start. **Act guardrail: Caradril never names the Hollow Court (M7); it delivers M6/M9 at Act 3 / L9–12 and fragments earlier.**

| Mystery / Clue | Caradril Access Point (Stage 4) | File |
|---|---|---|
| C-M2-1 (the network) | The Sunken Wards' warming + in-situ Concord Script — proof the harvest-network is continental (*fragment*) | `caradril_districts/THE_SUNKEN_WARDS.md`, `Q_BELOW_THE_STILLING.md` |
| C-M3-1/3 (Remembrance relic) | Ashmarket quiet-coin relic; Crucible smelting "incidents"; Ledger deep-vault refined relic; a dormant Wards relic | `THE_ASHMARKET.md`, `THE_CRUCIBLE.md`, `THE_COUNTING_QUAYS.md`, `THE_SUNKEN_WARDS.md`, `Q_QUIET_COIN.md`, `Q_THE_SMELTING.md` |
| C-M4-2 (basin scheme funding) | The misfiled charter-registry record tying Ledger money to "Reach water-rights works" (a Caradril-side echo) | `THE_MAGISTERIUM.md`, `Q_THE_SEALED_LETTER.md` |
| C-M6-1 (Concord's purpose) | The **Sealed Archive** (clearest written proof); Highmourn's institutional folk-memory; Wards Script fragments; the Vyre–Quorrin deal-pages (via Coll Riis) | `THE_LANTERN_REACH.md`, `Q_THE_SEALED_ARCHIVE.md`, `THE_COUNTING_QUAYS.md`, `Q_THE_QUAY_CHARTER.md`, `HIGHMOURN.md` |
| C-M8-1/2 (why is the PC here?) | The Magisterium correspondent thread (Reke writes to someone seated here — *lead only*, never a named second agent); the Hush sells fragments | `THE_MAGISTERIUM.md`, `THE_SILL.md`, `Q_THE_SEALED_LETTER.md`, `Q_THE_BELLMANS_PRICE.md` |
| C-M9-1 (deliberate Quietfall) | The **Sealed Archive** (the planned, signed Quietfall) | `THE_LANTERN_REACH.md`, `Q_THE_SEALED_ARCHIVE.md` |
| C-M1/M5 (city echoes) | Highmourn's covered-up raise-dead failures and a hushed wrong-come-back; Renna Sill's sheltered revenant; the thin-born refugees (M10 local) | `HIGHMOURN.md`, `THE_SILL.md`, `Q_THE_FUNERAL_THAT_WOULDNT_TAKE.md` |

City part-truth NPCs: Quorrin Vane (M3/M6/M9), Briss (M6 via Archive once disillusioned — Secret 13), Mother Ysarra (city M1/M5 failures, covered up), Lon Quayle (turnable witness), Coll Riis (deal-proof = M3/M6), the Bellman (sells M3/M6/M8/Wards fragments), Renna Sill (M10 local + a city Wren-echo).

**Gate reminder:** the Sealed Archive (C-M6-1, C-M9-1) is Act 3 / L9–12. Wards/Ashmarket/Crucible give M2/M3 *fragments and demonstrations* earlier. Never surface M7 (the Hollow Court) in Caradril.

## Clue Counts and Three-Clue-Rule Check

| Mystery | Authored Clue Paths | Meets 3+ Rule | Notes |
|---|---|---|---|
| M1 | 4 | yes | social / ritual / folk / physical |
| M2 | 4 | yes | exploration / testimony / document / forbidden |
| M3 | 4 | yes | magic / teaching / mercantile / scholarly |
| M4 | 4 | yes | political / paper trail / surveillance / money |
| M5 | 4 | yes | testimony / physical / lore / ritual observation |
| M6 | 4 | yes | archives / confession / dead witness / songs |
| M7 | 3 | yes | physical / convergence / heretic — gate before Act 4 |
| M8 | 3 | yes | fixer / follow-the-money / pattern |
| M9 | 4 | yes | archives / confession / dead witness / inscriptions |
| M10 | 4 | yes | consequence knowledge from four factions (a choice, not a truth) |
| M0 | (central) | n/a | solved by assembling M2 + M3 + M6 + M7; no net-new clues |

---

## Stage 11 — Region-Coded Clue Layer (REV-ID cross-reference)

Stage 11 adds a **region-coded clue ID layer** (`C_SR_*` Sundering Reach, `C_CAR_*` Caradril, `C_AV_*` Ashgarden Vale, `C_TW_*` Tollwood, `C_PC_*` Pale Coast, `C_FC_*` far-continent echoes) so each `REV_*` in `REVELATION_MAP.md` has its 3+ independent sources addressably tracked. **These do not replace the C-M* clues above** — many are the same authored clue under a region-coded ID for revelation-map cross-reference; new ones extend redundancy. All `hidden` at start. Each row: ID · player-facing form · actual meaning (brief DM) · REV(s) supported · source type · approach · redundancy/fallback · false-read risk · secrecy · fixed/movable.

> **Format note (per file size):** full per-clue prose (who can interpret, exact NPCs/locations/quests, DC bands, alt-paths, fallback) lives in the **regional clue-trail files** `by_region/*_CLUES.md`. This index is the master cross-reference; load the regional file for the runnable detail.

### Sundering Reach (`C_SR_*`)

| ID | Player-facing form | Actual meaning (DM) | REV | Source type | False-read risk | Secrecy |
|---|---|---|---|---|---|---|
| C_SR_001 | Wren clings to "something unfinished"; remembers dying | Partial Remembrance-revenant; shrine pulled at her | REV_001 | NPC conversation | "a normal ghost / haunting" | discoverable |
| C_SR_004 | Grave-soil turned from beneath, drifting waterward | The basin pulls the buried dead | REV_001 | Site/physical | "grave-robbers / erosion" | discoverable |
| C_SR_005 | Old Sashe's map: the dead drift basin-ward for years | The keystone pulls leaked Remembrance | REV_001 | Document/testimony | "fen currents / animal trails" | clue-gated (Sashe's trust) |
| C_SR_010 | Rites fail worse the nearer the water | Proximity to the reawakening keystone | REV_001 | Religious/rite observation | "the fens are cursed" | discoverable |
| C_SR_011 | A relic is cold-wrong; shows a dead face | It *stores a person* (substance) | REV_002 | Object/magic | "a creepy antique" | dm-only -> player on study |
| C_SR_012 | Gravecallers: "the dead know things; the relics are full" | Remembrance is harvestable identity | REV_002 | Faction/forbidden | "cult raving" | clue-gated (cult contact) |
| C_SR_013 | The Ledger vault relic "remembers" a dead person | Someone collects the substance on purpose | REV_002 | Object/heist or turned factor | "valuable salvage only" | clue-gated |
| C_SR_014 | The reeve: "the basin push doesn't add up" | A cover to reopen the shrine | REV_003 | Social/investigation | "ordinary council politics" | discoverable |
| C_SR_015 | The water-rights filings are fabricated | The stated reason is false | REV_003 | Document | "clerical error" | clue-gated (protect Pevin Oss) |
| C_SR_016 | Reke visits the basin shore alone at night | Personal, secret interest in the shrine | REV_003 | Exploration/surveillance | "an affair / smuggling" | discoverable |
| C_SR_017 | The factor: "it's not really about water" | Ledger money behind the works | REV_003 | Social | "factor gossip" | discoverable |
| C_SR_018 | Sela Coalmont: the Compact is "steered against the Reach" | Infiltration steering policy | REV_003 | Faction/authority | "frontier neglect, not a plot" | clue-gated |
| C_SR_019 | Sefra is uneasy about her patron's money | She was a paid cutout | REV_004 | NPC confession | "she's just shifty" | clue-gated (trust/press) |
| C_SR_020 | The patron's payments trace to a cutout | The player was steered | REV_004 | Document/follow-the-money | "a rival faction hired me" | clue-gated |
| C_SR_021 | The player keeps being pointed at the shrine | Deliberate steering | REV_004 | Pattern (player-driven) | "coincidence" | dm-confirms |
| C_SR_022 | A senior Warden breaks her oath | The Concord harvested the dead | REV_005 | NPC confession | — (direct) | dm-only (Act 3 gate) |
| C_SR_023 | A channeled Quietfall-era witness testifies | Firsthand harvest + pause account | REV_005/REV_006 | Forbidden/the dead | "a lying spirit" | dm-only (Act 3 gate) |
| C_SR_024 | Wend's old songs, fully decoded | "The Concord ate the dead" (folk-truth) | REV_005 | Song/folk | "old superstition" | dm-only (Act 3 gate) |
| C_SR_025 | Othetha: the Wardens were seeded to keep a pause | The Quietfall was deliberate | REV_006 | NPC confession | — | dm-only (Act 3 gate) |
| C_SR_026 | Shrine Concord Script states "the pause" | The self-destruction was planned | REV_006 | Document/inscription (Script) | mistranslation | dm-only (Act 3 gate) |
| C_SR_027 | The under-shrine; preserved memory-beings | The Hollow Court | REV_007 | Exploration (lethal-telegraphed) | — (apex) | dm-only (Act 4 gate) |
| C_SR_028 | The only explanation that fits all proof | Surviving Custodians restarting the harvest | REV_007 | Convergence | "the Remnant is the apex" | dm-only (Act 4 gate) |
| C_SR_029 | "The ones who would not pass" / Maire reaches out | The Court is real and present | REV_007 | Forbidden/heretic | "metaphor" | dm-only (Act 4 gate) |
| C_SR_030 | Gravecaller warning: breaking it = catastrophe | Destroy-ending cost | REV_008 | Faction/forbidden | "cult fear-mongering" | dm-only (Act 4-5) |
| C_SR_031 | Warden warning: sealing ends resurrection | Seal-ending cost | REV_008 | Faction/trust | "Warden conservatism" | dm-only (Act 4-5) |
| C_SR_032 | Veyl's case for a controlled restart | Restart-ending cost (stability+horror) | REV_008 | Apex contact | "villain lies" | dm-only (apex) |
| C_SR_033 | Maire: the dead could choose | Synthesis-ending possibility | REV_008/REV_010 | Apex contact | — | dm-only (apex) |
| C_SR_034 | "Thin" Harrowgast miners; thin-born | Living evidence the afterlife thinned | REV_009 | Site/social | "miner's disease" | discoverable (effects) |
| C_SR_035 | The dead name "the empty country" | The Quiet Country is finite/drained | REV_009 | Forbidden/the dead | "spirit metaphor" | dm-only (Act 3+ gate) |
| C_SR_036 | Maire reaches out directly | The Court could end itself | REV_010 | Apex contact | — | dm-only (endgame) |
| C_SR_037 | Orre's hawkishness vs. Maire's doubt | Court internal split | REV_010 | Apex observation | — | dm-only (endgame) |
| C_SR_038 | Gravecaller fragments on freeing the dead | A consensual system is conceivable | REV_010 | Forbidden | "chaos / catastrophe only" | dm-only (endgame) |

> `C_SR_001`-`C_SR_017` map onto the Act-1/2 C-M1/M2/M3/M4/M5/M8 clues above (region-coded for REV cross-ref). `C_SR_022`-`C_SR_038` map onto C-M6/M7/M9/M10. **Redundancy/fallback for every REV is the 3+ sources listed in `REVELATION_MAP.md`; the regional trail files hold the per-clue alt-paths and "what if missed."**

### Caradril (`C_CAR_*`)

| ID | Player-facing form | Actual meaning (DM) | REV | Source type | Secrecy |
|---|---|---|---|---|---|
| C_CAR_004 | A studied relic stores a person | Remembrance substance (city magic path) | REV_002 | Object/magic | dm-only -> player on study |
| C_CAR_005 | Ashmarket quiet-coin "holds the dead" | Commercial relic trade | REV_002 | Mercantile | discoverable |
| C_CAR_006 | Crucible smelting "incidents" | Relics resist destruction (substance) | REV_002 | Site/hazard | clue-gated |
| C_CAR_007 | Concord Script: "the keeping of the dead's pattern" | The substance, scholarly | REV_002 | Document (Script) | clue-gated (Script gate) |
| C_CAR_008 | Misfiled charter record: Ledger -> "Reach water-rights" | Caradril-side basin-scheme echo | REV_003 | Document | clue-gated |
| C_CAR_009 | Patron payment trail (city banking) | Steering cutout | REV_004 | Document/follow-the-money | clue-gated |
| C_CAR_010 | The Hush sells the correspondent fragment | Reke writes to someone seated here | REV_004 | Faction/broker (costly) | clue-gated |
| C_CAR_011 | The Sealed Archive: the harvest, written | The Concord harvested the dead | REV_005 | Archive (Script) | dm-only (Act 3 gate) |
| C_CAR_012 | The Sealed Archive: the signed, planned Quietfall | Deliberate self-destruction | REV_006 | Archive (Script) | dm-only (Act 3 gate) |
| C_CAR_013 | Node-site Concord Script (Sunken Wards) | The pause, inscribed | REV_006 | Document/inscription | dm-only (Act 3 gate) |
| C_CAR_014 | Deep study of resurrection failure + relic analysis | The afterlife is finite | REV_009 | Magic/research | dm-only (gated) |
| C_CAR_015 | Thin-born refugees in the Sill | Living thinning evidence | REV_009 | Social/site | discoverable |

### Ring 1 (`C_AV_*` Vale · `C_TW_*` Tollwood · `C_PC_*` Coast) and Far-Continent (`C_FC_*`)

These are corroboration/echo clues. They **confirm the pattern from outside the Reach** and (far) **confirm the theme is bigger than the NW** — but never deliver the keystone mechanism or name the Court. Full per-clue detail in `by_region/ASHGARDEN_VALE_CLUES.md`, `by_region/TOLLWOOD_CLUES.md`, `by_region/PALE_COAST_CLUES.md`, and `by_region/FAR_CONTINENT_ECHO_CLUES.md`.

| ID | Region | Player-facing form | REV | Ceiling |
|---|---|---|---|---|
| C_AV_001 | Vale | Honest M5 window (Tilbrook/Mam Tace): rites starting to fail here too | REV_001 | radiates from the Reach; no mechanism |
| C_AV_002 | Vale | "Saint's-bones" relics are Remembrance relics | REV_002 | substance demo; no Concord-sin |
| C_AV_003 | Vale | Ezrith Combe's old songs (folk-fragment) | REV_005 | folk-truth only, Act 3 gate |
| C_TW_001 | Tollwood | Coldhearth honest M5 window; deep wood "gone wrong" | REV_001 | radiates outward; no mechanism |
| C_TW_002 | Tollwood | "Grey lords took the dead before the roads fell" (oblique) | REV_005 | pre-Concord half-memory; gated; never the Court |
| C_PC_001 | Coast | Cobble Strand honest M5/M2 window; the "drowned-tide" | REV_001 | radiates outward; no mechanism |
| C_PC_002 | Coast | Salt-Mother Bryd: "Lamps kept the drowned for the Concord" | REV_005 | coastal folk-fragment; Act 3 gate |
| C_PC_003 | Coast | Sea-relic trade (Maris Cole's salvage-ledger) | REV_002 | maritime substance trade |
| C_FC_001 | Concord Heartlands | The Ruin'd Crown's harvest-record | REV_005 | the Concord's true scale/sin; NEVER the live machine/keystone |
| C_FC_004 | Emberfell | "Old glass" sold against the Pyre's law; "ash-touched" crews | REV_002 | southern relic source; no meaning/origin |
| C_FC_010 | Karran | "Humming old iron"; deep crews "come back changed" | REV_002 | NE relic source; no meaning/origin |
| C_FC_011 | (network) | The continental old-songs fragment: "the grey hands took the dead" | REV_005 | folk-fragment only; never the mechanism/Court |
| C_FC_012 | Sunmark | A faith whose rites *still hold the dead* | REV_008/REV_010 | hopeful contrast; synthesis is conceivable |
| C_FC_013 | Steppe/Sunmark | "The Sky has gone thin"; "a far root aches" | REV_009 | deeply oblique cosmic echo; never names Quiet Country/harvest |

---

## Stage 11 — Per-REV Three-Source Verification

Each major revelation is backed by **>=3 independent clue sources from different regions/NPCs/approaches** (no single point of failure). Counts include the C-M* and region-coded layers; far echoes are *corroboration*, never the sole path.

| REV | Independent sources | Approaches spanned | >=3? | Single-point-of-failure? |
|---|---|---|---|---|
| REV_001 | C_SR_001, _004, _005, _010 + Ring1 windows | social / physical / testimony / rite / regional | 5+ | none |
| REV_002 | C_SR_011, _012, _013 + C_CAR_004/005/006/007 + C_FC_004/010 + C_PC_003 | magic / forbidden / mercantile / scholarly / far | 8+ | none |
| REV_003 | C_SR_014, _015, _016, _017, _018 + C_CAR_008 | political / paper / surveillance / money / authority | 6 | none |
| REV_004 | C_SR_019, _020, _021 + C_CAR_009/010 | confession / follow-money / pattern / broker | 5 | none |
| REV_005 | C_CAR_011 + C_SR_022, _023, _024 + C_FC_001/011 + C_AV_003/C_PC_002 | archive / confession / dead / song / far | 7+ | none |
| REV_006 | C_CAR_012 + C_SR_025, _023, _026 + C_CAR_013 | archive / confession / dead / inscription | 5 | none |
| REV_007 | C_SR_027, _028, _029 | physical / convergence / heretic | 3 | none (convergence requires 3 prior REVs) |
| REV_008 | C_SR_030, _031, _032, _033 + C_FC_012 | faction warnings (4 sources) / far contrast | 5 | none |
| REV_009 | C_CAR_014/015 + C_SR_034, _035 + C_FC_013 | research / social / dead / far | 5 | none |
| REV_010 | C_SR_036, _037, _038 + C_FC_012 | apex contact / observation / forbidden / far | 4 | none |

## Clue Type Reference

| Type | Description |
|---|---|
| Direct | Clearly points to the conclusion |
| Indirect | Suggests without stating; requires inference |
| Symbolic | Metaphorical or visual; requires interpretation |
| Damaged | Incomplete; gives partial information |
| Misleading | Points toward a false lead, but can be disproven |
| Partial | One piece of a larger clue chain |
| Convergence | Not a net-new clue; the conclusion emerges from assembling other mysteries |
| Consequence | Not a truth-clue; knowledge of an outcome's cost (used for the M10 choice) |

---

## Discovery Method Reference

| Method | Description |
|---|---|
| Social | Conversation, persuasion, insight, folk knowledge, confession |
| Investigation | Following leads, surveillance, paper trails (player-skill or check) |
| Exploration | Going to a place and finding/observing physical evidence |
| Document | Reading records, archives, filings, inscriptions (may need a language gate) |
| Magic | Arcana/Religion study, relic examination, ritual observation |
| Forbidden | Gravecaller contact, channeled dead — dangerous/illegal sources |

---

## Discovery Status Reference

| Status | Meaning |
|---|---|
| hidden | In the world but not found |
| in play | Player has been to the location but didn't find it |
| discovered | Player has the clue |
| misinterpreted | Player has it but drew the wrong conclusion |
| confirmed | Player has it and understood it correctly |
| missed | Opportunity has passed |

---

## AI Use

- Before delivering a clue, confirm the act/level is appropriate via `REVELATION_MAP.md`. Several late clues (C-M6-*, C-M7-*, C-M9-*) must not surface before their act.
- If the player is stuck on a conclusion, this index shows the alternate paths available so no single failed roll, dead NPC, or skipped faction blocks the truth.
- When a clue is discovered: set its status here, add it to `KNOWN_CLUES.md` with the player's interpretation, and update `HIDDEN_CLUES.md`.
- DM-only. Never expose clue IDs, locations, or the convergence logic to the player.

---

## Related Files

- [`MYSTERY_WEB.md`](MYSTERY_WEB.md)
- [`REVELATION_MAP.md`](REVELATION_MAP.md)
- [`SECRET_INDEX.md`](SECRET_INDEX.md)
- [`../02_runtime_state/KNOWN_CLUES.md`](../02_runtime_state/KNOWN_CLUES.md)
- [`../02_runtime_state/HIDDEN_CLUES.md`](../02_runtime_state/HIDDEN_CLUES.md)
