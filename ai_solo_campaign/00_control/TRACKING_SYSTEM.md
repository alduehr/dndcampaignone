# TRACKING_SYSTEM.md

## Purpose

Defines how to track what has been created, what remains unfinished, and how ready the campaign is for AI-run solo play. The tracking files listed below are self-documenting — open them to see their formats and rules.

---

## Core Tracking Files

| File | Purpose |
|---|---|
| `00_control/PROGRESS_LOG.md` | Chronological production history |
| `00_control/TODO.md` | Prioritized actionable work queue |
| `00_control/CONTENT_INDEX.md` | Global inventory of all campaign files |
| `00_control/TAG_INDEX.md` | Retrieval tags and file membership |
| `00_control/OPEN_QUESTIONS.md` | Unresolved design decisions |
| `00_control/CONSISTENCY_AUDIT.md` | Known continuity and AI-readiness issues |
| `17_generation_backlog/EXPANSION_PLAN.md` | Forward-looking development roadmap |
| `17_generation_backlog/CONTENT_GAPS.md` | Missing or underdeveloped content by category |
| `18_audits/*.md` | Formal audit reports |

---

## Definition of Done

### File-Level Done

A content file is done when:
- It has a metadata block with type, secrecy, status, and tags.
- It has an AI Use section.
- It separates player-facing and DM-only content where needed.
- It links to related files.
- It has play function.
- It is indexed in CONTENT_INDEX.md and TAG_INDEX.md.
- It does not contradict CANON.md.
- It does not assume a four-person party unless explicitly marked.
- It has no remaining TBD, placeholder, unnamed, or fill-in areas.

### Stage-Level Done

A stage is done when:
- Required outputs exist.
- Completion criteria from DEVELOPMENT_STAGES.md are met.
- Indexes are updated.
- Canon is updated.
- State files are updated if needed.
- PROGRESS_LOG.md has an entry.
- TODO.md reflects remaining work.
- No critical audit issues remain for that stage.

### Campaign-Ready Done

The campaign is ready to begin play when:
- Stages 0, 1, and 2 are complete.
- Stage 3 is at least 75% complete.
- Stage 5 is at least 75% complete.
- Pre-play audit has no critical issues.
- Starting scene is ready.
- Runtime state is ready.
- First 10–20 sessions have enough authored material.
- Hidden truths are protected.
- The first mystery has multiple clue paths.
- Factions have clocks.
- The AI DM has a clean start prompt.

---

## Stage Completion Scale

Use rough percentages only.

- 0% — not started
- 25% — skeleton exists
- 50% — substantial content but gaps remain
- 75% — usable, needs audit or minor fixes
- 90% — audit complete, only minor gaps remain
- 100% — meets all completion criteria in DEVELOPMENT_STAGES.md

Do not mark a stage 100% complete without meeting its criteria.

---

## Suggested Prompts

### Status check
```
Read TRACKING_SYSTEM.md, DEVELOPMENT_STAGES.md, PROGRESS_LOG.md, TODO.md, CONTENT_INDEX.md, CONTENT_GAPS.md, and CONSISTENCY_AUDIT.md. Produce a current project status report. Identify the current stage, what is complete, what is incomplete, what is blocked, what should be done next, and which files need to be updated. Do not create new campaign content unless needed to fix tracking.
```

### Next work
```
Read TRACKING_SYSTEM.md, DEVELOPMENT_STAGES.md, TODO.md, CONTENT_GAPS.md, and PROGRESS_LOG.md. Choose the highest-priority unblocked task for the current development stage. Make a concise plan, complete the task, update all relevant indexes/canon/state/tracking files, then summarize what changed.
```

### Audit
```
Read AUDIT_STANDARDS.md, DEVELOPMENT_STAGES.md, TRACKING_SYSTEM.md, CANON.md, DM_ONLY_CANON.md, PLAYER_SAFE_CANON.md, CONTENT_INDEX.md, TAG_INDEX.md, and all files relevant to the current stage. Run an AI-readiness and continuity audit. Do not rewrite major canon yet. Produce an audit report in /18_audits and update CONSISTENCY_AUDIT.md, TODO.md, and CONTENT_GAPS.md.
```

---

## Final Rule

Tracking is part of the product. If content exists but the AI cannot find it, load it, distinguish secrets from player-safe facts, or know what remains incomplete — the campaign is not AI-ready.
