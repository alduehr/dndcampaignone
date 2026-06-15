# OPEN_QUESTIONS.md

## Purpose

Track unresolved design questions that cannot be resolved by making a standard creative decision. Use this only for genuine uncertainty — not as a substitute for acting.

## Current Status

Stages 0–14 complete (Stage 14 Treasure, Artifacts, and Rewards: 2026-06-14). Stage 15 (Level 5–20 Arc Expansion) is next. No blocking open questions currently recorded. Future unresolved design questions should be added here only when they cannot be resolved through a standard creative decision.

---

## Active Questions

### Should the Ravenloft: The Horrors Within (RtHW) supplement be integrated into the bestiary once it releases?
- Context: *Ravenloft: The Horrors Within* (RtHW) releases **June 16, 2026** — after Stage 13 completion. Stage 13's horror bestiary already uses **Van Richten's Guide to Ravenloft (VRGtR, 2021)** as a Track-A, copyright-safe gothic-horror source (name + source reference only, no stat blocks, no imported setting lore). RtHW would add ~25–28 thematically apt creatures (memory/grief/preserved-body horror) that mirror the campaign's Remembrance/harvest cosmology.
- Why it matters: several RtHW creatures (Mist Horror, Gallows Speaker, Waxworks, Necrichor, Strahd Skeleton, Brain in a Jar, Carrionette, etc.) map cleanly onto the harvest/grief themes and would enrich `HORROR_AND_CURSE_THREATS.md` and the deep-node regional tables. The book was not yet available at Stage 13 completion, so only a placeholder pending-section exists.
- Related files: `13_encounters_and_bestiary/CREATURE_SOURCE_REFERENCE.md` (Horror Expansion Supplement — Pending section), `HORROR_AND_CURSE_THREATS.md`, `BESTIARY_INDEX.md`, `MYSTERY_ENCOUNTERS.md`, and the deep-horror regional files (SUNDERING_REACH, CONCORD_HEARTLANDS, MARROWDOWNS, SALTMERE_REACHES, DROWNED_STEPS, HETHEWALD).
- Options:
  1. Run a small Stage 13 supplement pass once RtHW is accessible — add the apt creatures as Track-A references (no stat blocks, no Domains-of-Dread/darklord/named-NPC lore), reskinned to the Remembrance cosmology, only where a site's horror theme already fits.
  2. Skip RtHW entirely — VRGtR already covers the horror needs.
  3. Defer indefinitely.
- Recommended answer: **Option 1** — run a focused RtHW supplement pass after June 16, 2026, following the same Track-A discipline already used for VRGtR (the campaign world Vael/Orrun is original and is NOT Ravenloft; only published *creature* references are borrowed, never setting lore). Logged as a low-priority TODO and a CONTENT_GAPS entry.
- Blocking status: non-blocking (Stage 14 can proceed; RtHW integration is enrichment, gated on book release).

### Confirmed-answered (this pass): is official-monster sourcing copyright-safe?
- Answer: **Yes.** The two-track approach (Track A = official creatures named + source-referenced with original placement/tactics/solo notes, no stat blocks copied; Track B = campaign originals with abbreviated prose summaries) is documented in `CREATURE_SOURCE_REFERENCE.md` and matches `RULESET_ASSUMPTIONS.md` / `DND_MECHANICS_REQUIREMENTS.md`. Source shorthands (2024 MM, 2014 MM, MotM, MToF, VGtM, VRGtR, FToD, XGtE, TCoE) are mapped in `BESTIARY_INDEX.md`. A few entries are marked "source check needed" where the exact book is genuinely uncertain.

---

## Answered Questions

*None yet.*

---

## Rules

- Prefer making a decision over adding a question.
- Mark whether a question blocks progress.
- When resolved, move to Answered Questions.
- Update canon if the answer establishes world truth.

### Question Template

```md
### [Question]
- Context:
- Why it matters:
- Related files:
- Options:
  1. ...
  2. ...
  3. ...
- Recommended answer:
- Blocking status: blocking | non-blocking
```
