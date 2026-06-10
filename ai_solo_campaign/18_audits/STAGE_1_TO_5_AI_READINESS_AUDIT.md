# Audit Report: Stage 1–5 AI-Readiness Audit (Stage 6 First Full Audit)

---
type: audit
secrecy: dm-only
status: static
date: 2026-06-10
auditor: canon-continuity-auditor
related: [../00_control/CONSISTENCY_AUDIT.md, ../00_control/AUDIT_STANDARDS.md, ../00_control/DEVELOPMENT_STAGES.md]
tags: [audit, stage-6, ai-readiness, continuity]
---

## Scope

Full AI-readiness and continuity audit of Stages 1–5 (Campaign Foundation, AI Runtime, Starting Region Deep Build, First Major City Deep Build, Level 1–4 Play Arc), per `DEVELOPMENT_STAGES.md` Stage 6 and `AUDIT_STANDARDS.md`. All ten audit categories checked.

Files/folders reviewed: `03_canon/` (CANON, DM_ONLY_CANON, PLAYER_SAFE_CANON), `00_control/` indexes (CONTENT_INDEX, TAG_INDEX, RETRIEVAL_GUIDE, NAMING_REGISTRY, CONSISTENCY_AUDIT, TODO), `11_mysteries_and_secrets/` (MYSTERY_WEB, CLUE_INDEX, ACT_1_CLUE_TRAILS), `07_factions/FACTION_INDEX` + HOLLOW_COURT, `08_npcs/` (NPC_INDEX, MAJOR_NPCS, ACT_1_NPC_GUIDE), `09_quests/` (HOOKS_TABLE + glob of all quest files + sample act_1 quest), `12_campaign_arc/` (ACT_1_LEVELS_1_4, ACT_1_MILESTONES, ACT_1_FAILURE_STATES), `13_encounters_and_bestiary/ACT_1_THREATS`, `02_runtime_state/` (CURRENT_STATE, ACTIVE_QUESTS, FACTION_STATE, WORLD_CLOCKS, HIDDEN_CLUES). Quest-file existence verified against disk by glob.

## Summary

**The Stage 1–5 foundation is sound and AI-ready.** Canon is internally consistent, secret separation is rigorously maintained (player-safe vs. DM-only is clean across every file sampled, with the apex secret — the Hollow Court — correctly never named in any Act 1 / player-facing content), mysteries satisfy the three-clue rule with multi-route redundancy, factions all have clocks and proactive ignore-behavior, solo-play safety is exemplary (telegraphing, noncombat outs, retreat, no cheap death), state tracking is thorough with per-quest State Update instructions, and indexes are comprehensive and current.

**No Critical findings.** One High finding: the Act 1 arc spine (`ACT_1_LEVELS_1_4.md`) cross-referenced two quest files that do not exist on disk — a broken-link defect in the DM's primary Act 1 map. This was within the audit's small-cleanup remit and has been **fixed inline** (both rows repointed to the real authored content). The remaining findings are Medium/Low gaps already largely tracked, plus polish items.

**Scaling to Stage 7 is CLEAR.** No critical issues block outward expansion. The High finding is resolved.

---

## Critical Findings

| Issue | File(s) | Why It Matters | Recommended Fix |
|---|---|---|---|
| *(none)* | — | — | — |

## High Findings

| Issue | File(s) | Why It Matters | Recommended Fix |
|---|---|---|---|
| Arc spine pointed to two nonexistent quest files: Door 4 cited `Q_ACT1_INDEPENDENT_WHAT_THE_FENS_CARRY` and Door 7 cited `Q_ACT1_COURT_THE_COUNCILORS_ERRAND`. Only 6 `act_1_quests/` files exist on disk; neither of these is among them. | `12_campaign_arc/ACT_1_LEVELS_1_4.md` (lines 34, 60) | This is the DM's primary Act 1 map. A broken pointer to a "prepared content" file would send the AI DM looking for material that does not exist, breaking the predetermined-first contract at the exact moment of play. | **FIXED INLINE.** Door 4 repointed to Hook 6 + the existing `Q_SASHES_WARNING.md`. Door 7 repointed to Hook 4 in `HOOKS_TABLE.md` with an explicit note that the Court has no `act_1_quests/` file by design (consistent with ACT_1_NPC_GUIDE, ACT_1_CLUE_TRAILS, ACTIVE_QUESTS). |

## Medium Findings

| Issue | File(s) | Why It Matters | Recommended Fix |
|---|---|---|---|
| Caradril NPC density (~40 useful city NPCs) is below the Stage 4 target band (75–100). | `08_npcs/SECONDARY_NPCS.md`, `MINOR_NPCS.md`, `caradril_districts/` | The city is a long-term mid-game hub; thin NPC coverage will force improvisation once city play begins in earnest. | Expand toward target in Stage 9 (already a TODO). Not blocking — quality coverage exists for all 8 districts and all city factions. |
| No standalone full bestiary; adversary stats live only inside zone/city encounter tables + the 5 Act 1 threat profiles. | `13_encounters_and_bestiary/` | Mid/high-tier (Acts 2–5) threats are not yet mechanically usable; the AI DM has no statted antagonist vocabulary above ~level 6. | Build the bestiary in Stage 13 (tracked). Act 1–early play is fully covered. |
| No `REWARDS_BY_LEVEL.md` / treasure-by-level; dungeon and quest rewards reference "level-appropriate items" without concrete itemization. | `10_dungeons_and_ruins/`, quest files | The AI DM must improvise reward specifics, risking under/over-rewarding a solo PC. | Build treasure/rewards in Stage 14 (tracked). |
| No standalone act files for Acts 2–5; the arc above level 4 exists as shape only. | `12_campaign_arc/` | Play beyond level 4 is not yet runnable in detail. | Build in Stage 15 (tracked). Expected at this stage of development. |

## Low Findings

| Issue | File(s) | Why It Matters | Recommended Fix |
|---|---|---|---|
| No individual per-clue files; clues tracked in index/runtime rows only. | `11_mysteries_and_secrets/CLUE_INDEX.md` | Coarser retrieval than per-file; fine for current scale. | Optional in Stage 11 (tracked). |
| `/15_random_tables/` empty (no travel/weather/event tables). | `15_random_tables/` | Slightly higher improvisation burden during travel/downtime; zone encounter tables partly cover this. | Populate when convenient (tracked, low). |
| `NPC_RELATIONSHIP_WEB.md`, `NPC_SECRET_LEDGER.md`, `NPC_VOICE_GUIDE.md` not created; relationship/secret data currently lives in MAJOR_NPCS + FACTION_INDEX. | `08_npcs/` | QoL tooling for a large roster; data is not lost, just not consolidated. | Create in Stage 9 (tracked). |
| No dedicated `QUEST_INDEX.md`; quests indexed inline in CONTENT_INDEX/TAG_INDEX. | `09_quests/` | Slower lookup by level/region/faction as the library grows. | Create in Stage 10 (tracked). |
| The "Magisterium correspondent" thread (Reke ↔ a Caradril magister) is an intentionally unresolved lead. | `THE_MAGISTERIUM.md`, `HIDDEN_CLUES.md` | By design; must stay a lead, never a named second Court agent. Flagged only so it is not mistaken for a gap. | Resolve through play in Stage 15. No action now. |

---

## Orphaned Content

None found. Every NPC sampled has a location, motive, faction tie or independent role, and play function. Every quest links to NPCs/factions/locations/clues. Every faction has named members, a clock, resources, and ignore-behavior. The two broken arc-file pointers (now fixed) were the only "dangling reference to nonexistent content" detected — and they pointed *outward* to missing files, not orphaned files lying unreferenced. All 36 quest files, 8 district files, 6 dungeons, 4 wilderness zones, and 7 major faction files are referenced by the indexes and the retrieval guide.

## Missing Index Entries

None material. CONTENT_INDEX, TAG_INDEX, RETRIEVAL_GUIDE, NPC_INDEX, FACTION_INDEX, CLUE_INDEX, and NAMING_REGISTRY are all current through Stage 5. The 6 Act 1 quests, 5 Act 1 threats, Act 1 clue-trails, Act 1 NPC guide, and the three Act 1 arc files are all indexed and tagged (`act:1`). Quest-file glob matches the index listings exactly (6 act_1 + 11 city + 14 regional + hooks/rumors tables).

## Exposed Secrets

**None.** Secret separation is clean across every file sampled:
- `PLAYER_SAFE_CANON.md` contains only public faces, common knowledge, and the genuinely-unknown surface mystery. No harvest, no Hollow Court, no Remembrance-as-substance, no Reke allegiance, no steering.
- `DM_ONLY_CANON.md`, `MYSTERY_WEB.md`, `CLUE_INDEX.md`, `ACT_1_CLUE_TRAILS.md`, and `HOLLOW_COURT.md` carry the dm-only headers and warnings; all are tagged `secrecy:dm-only`.
- The apex secret (Hollow Court / M7) is correctly **never named** in any Act 1, player-facing, or Caradril-public content. The reveal cap of **R1 for all of Act 1** is stated and enforced in every Act 1 file (arc spine, milestones, failure states, threats, clue trails, NPC guide, the sampled faction quest).
- Mixed-secrecy files (NPCs, quests, settlements) consistently segregate Player-Facing from DM-Only / Hidden Truth sections.
- The Act 1 quest sampled (`Q_ACT1_WARDEN_THE_TRUE_RITE`) holds its hidden truth to a clearly marked DM-Only section and caps the clue ceiling at R1/seed level.

## Solo-Play Risks

**None significant.** Solo-play safety is a clear strength:
- Every Act 1 threat profile telegraphs before any fight, offers at least one noncombat resolution, allows retreat, gives morale/goals (enemies don't fight to the death), and provides explicit level-scaling for one PC. No four-PC assumptions found.
- The signature early threat is a roleplay/rite scene by default, not a fight; cheap death is structurally prevented by the telegraph rule.
- The starting safety net (companion, fen-guide, safe base, patron, sanctuary waystation) and the "Safe Re-Entry Points" table backstop a lost or stranded solo player.
- Failure states all redirect rather than end the campaign, with an explicit "solo-play floor" (no failure may strand the player with zero leads/allies/level-paths).

## Mystery / Clue Risks

**None significant.** The three-clue rule is satisfied with margin:
- Every mystery M1–M10 has 3–4 independent authored clue paths spanning social/exploration/ritual/scholarly/mercantile/forbidden approaches; the CLUE_INDEX includes an explicit three-clue-rule check table.
- Act 1's single required conclusion (R1) has 4 independent routes; the player needs only ~2, and the clocks deliver R1 even to a fully passive player.
- Caradril deepens but never gates the deep-history mysteries (M3/M6/M9 remain reachable in the Reach), so a player who never visits the city is never blocked.
- Late clues (C-M6-*, C-M7-*, C-M9-*) are act/level-gated in both CLUE_INDEX and HIDDEN_CLUES with pacing reminders. No mystery depends on a single roll, a single NPC, or a single faction.

---

## Recommended Fix Order

1. **(DONE — High)** Repoint the two broken Act 1 arc-spine quest references. *Fixed inline during this audit.*
2. **(Medium, Stage 9)** Expand Caradril NPC roster toward the 75–100 target before heavy city play.
3. **(Medium, Stage 13)** Build the standalone bestiary (mid/high tiers) so Acts 2+ are mechanically usable.
4. **(Medium, Stage 14)** Build `REWARDS_BY_LEVEL.md` / treasure-by-level and stat the referenced dungeon rewards.
5. **(Medium, Stage 15)** Build Acts 2–5 standalone arc files + villain-escalation / endgame-states.
6. **(Low, Stages 9–11)** Create `QUEST_INDEX.md`, NPC relationship/secret/voice tools, optional per-clue files, and populate `/15_random_tables/`.

None of items 2–6 block Stage 7 (Regional Expansion Ring 1). They are expected forward-stage work already tracked in TODO/CONTENT_GAPS.

## Verdict

Stage 6 complete. Foundation verified sound. **Outward scaling to Stage 7 is approved.**
