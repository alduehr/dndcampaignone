# PRODUCTION_WORKFLOW.md

## Default Workflow For Major Production Passes

For any major production pass:

1. **Read context**
   - Read relevant control files.
   - Read relevant canon files.
   - Read relevant indexes.
   - Read relevant existing content files.

2. **Determine current state**
   - What already exists?
   - What canon is binding?
   - What is missing?
   - What should not be contradicted?

3. **Make a concise plan**
   - List files to create or edit.
   - List expected canon/state/index updates.
   - Identify any risks.

4. **Create or edit content**
   - Use structured markdown.
   - Add retrieval tags.
   - Separate player-facing and DM-only content.
   - Cross-link related files.

5. **Update canon and state**
   - If new world facts were created, update canon.
   - If runtime state changed, update state files.
   - If secrets were created, store them in DM-only files.

6. **Update indexes**
   - Add new content to the relevant index.
   - Update CONTENT_INDEX.md.
   - Update TAG_INDEX.md when tags change.

7. **Update project tracking**
   - Update PROGRESS_LOG.md.
   - Update TODO.md.
   - Update CONTENT_GAPS.md if gaps were identified.

8. **Run a small consistency check**
   - Did any new fact contradict CANON.md?
   - Did any player-facing file expose DM-only truth?
   - Did new content get indexed and tagged?
   - Did new lore connect to play?
   - Did any solo encounter assume a full party?
   - Did any mystery rely on only one clue?
   - Did any faction remain passive with no clock?
   - Did state need updating?

9. **Report**
   - Files created or changed.
   - Major canon established.
   - Indexes updated.
   - State files updated, if any.
   - What remains incomplete.
   - Recommended next production pass.

---

## Stage Requirements and Expansion Passes

For per-stage required outputs, content targets, and completion criteria, see `DEVELOPMENT_STAGES.md`.

---

## Progress Log Format

```md
## YYYY-MM-DD — Pass Name

### Stage
Stage number and name.

### Summary
One short paragraph.

### Files Created
- `path/to/file.md` — description

### Files Changed
- `path/to/file.md` — description

### Canon Established
- ...

### Indexes Updated
- ...

### Gaps Identified
- ...

### Next Recommended Pass
- ...
```

---

## TODO Format

```md
## Critical
- [ ] Task
  - Why it matters:
  - Related files:
  - Suggested agent:
  - Stage:

## High / Medium / Low
- [ ] Task

## Completed Recently
- [x] Task — date
```

Do not leave vague TODOs like "add more stuff." Write actionable tasks.
