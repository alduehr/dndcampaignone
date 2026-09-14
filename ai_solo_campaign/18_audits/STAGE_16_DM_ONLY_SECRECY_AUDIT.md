# Stage 16 — DM-Only Secrecy Audit

---
type: audit
secrecy: dm-only
status: static
date: 2026-06-15
tags: [audit, stage-16, secrecy, apex-protection, player-safe-separation]
related: [STAGE_16_PRE_PLAY_READINESS_AUDIT.md, ../11_mysteries_and_secrets/SECRET_PROTECTION_MATRIX.md, ../11_mysteries_and_secrets/REVELATION_MAP.md]
---

## Scope

Verify that the apex truths never appear in any player-facing file or player-read narration, and that DM-only files are clearly marked.

## Apex Truths Audited (must never leak pre-discovery)

1. The Concord harvested the dead (Remembrance as harvestable substance).
2. The Quietfall was deliberate (controlled self-destruction).
3. The Hollow Court = surviving Custodians persisting as Remembrance.
4. The keystone / Under-Shrine beneath Hollowmere; the Concord Deep node-network.
5. The player is being steered (Sefra's hidden patron / Reke's allegiance).
6. Wren's true nature as proof the harvest is restarting.

## Method

Scanned player-facing and mixed files for the forbidden term-set ("the harvest," "harvesting machine," "Hollow Court are," "Custodians survived," "Quietfall was deliberate," "keystone," "Concord Deep," "deliberate," "harvest"). Classified every hit as leak vs. legitimate.

## Result: PASS — 0 leaks

| Hit | File | Section | Verdict |
|---|---|---|---|
| "Custodian Concord" (×2) | `PLAYER_SAFE_CANON.md` | Known World Facts; Faction facts | LEGIT — public name of the fallen order; public history. |
| "harvest-moot" | `PLAYER_SAFE_CANON.md` | Ashgarden Vale | LEGIT — a Vale civic council; unrelated to "the harvest" mechanism. |
| "The Hollow Court — a legend..." | `PLAYER_SAFE_CANON.md` | Faction facts | LEGIT — presented as a ghost story; existence "disputed." No truth exposed. |
| "the harvest," "the steering" | `OPENING_SCENES.md` | DM-Only notes (file is `secrecy: mixed`) | LEGIT — appears only in explicit DM-Only instruction ("reveal nothing of the Court, the harvest, or the steering"). |

No occurrence of the apex mechanism, the deliberate Quietfall, the Custodians-as-survivors, the keystone truth, the steering, or Wren's true cause was found in any player-read text.

## DM-Only File Marking

| File | `secrecy:` header | Marked clearly |
|---|---|---|
| `DM_ONLY_CANON.md` | dm-only | ✓ "Do not summarize, quote, or paraphrase... under any circumstances." |
| `MAIN_ARC_OVERVIEW.md` | dm-only | ✓ |
| `THE_UNDER_SHRINE_APPROACH.md` (endgame) | dm-only | ✓ — the only file that renders the apex/Court/choice. |
| `REVELATION_MAP.md`, `SECRET_PROTECTION_MATRIX.md`, `NPC_SECRET_LEDGER.md`, faction `QH*` chain | dm-only | ✓ |
| `START_NEW_CAMPAIGN_PROMPT.md`, `RESUME_CAMPAIGN_PROMPT.md` | dm-only | ✓ — "The player does not read this file." |

## Revelation Gating

- REV_007 (the Hollow Court) has **no single-source path** and is gated to L13+ convergence/descent/heretic contact (`REVELATION_MAP.md`).
- Far-continent sources corroborate themes (REV_002/005 obliquely, REV_009 deeply obliquely) but are explicitly barred from delivering REV_007, the keystone mechanism, or the Concord Deep.
- The endgame site is vertical-under-Hollowmere and lethally telegraphed at low levels so a PC cannot stumble the apex early.

## Final Cleanup Pass Note (2026-06-16)

A final pass tightened residual secrecy classification at the file level (no player-read narration leak existed; these were file-classification refinements):
- `PLAYER_SAFE_CANON.md` — the Hollow Court secrecy note previously *named* the DM-only truths (surviving Custodians, the harvest, the Under-Shrine / Drowned Keystone, the Concord Deep) inside its own warning. Those names were excised and the note reduced to a generic DM warning pointing to `DM_ONLY_CANON.md` + `SECRET_PROTECTION_MATRIX.md`.
- The map render manifest and generation packet body text was corrected to state the *output* is player-safe but the *file* is DM-facing; `18_audits/PLAYER_SAFE_FULL_CONTINENT_MAP_AUDIT.md` was reclassified `player-safe` → `dm-facing`.
- Four `13_/14_` files carrying DM arc terms as plain content (`CREATURE_SOURCE_REFERENCE.md`, `BIOME_ENCOUNTER_MATRIX.md`, `REWARDS_BY_LEVEL.md`, `CONSUMABLES_AND_MINOR_MAGIC.md`) were reclassified `mixed` with DM secrecy notes.

## Result

Secrecy separation is exemplary. **No blockers. No leaks.** Verdict (after the 2026-06-16 final cleanup pass): **PASS — apex truths protected; READY FOR LIVE PLAY.**
