---
visibility: dm-only
title: Session End
---
# Session End

Read this whenever a session is drawing to a close. This overlays the shared
session-end procedure with a translation table: this campaign's own authored
`16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md` describes a **16-file
checklist** written for a human DM hand-editing markdown files between
sessions. **That checklist's markdown files are read-only content in this
system — nothing in a live session ever writes back to them.** Every one of
its 16 categories maps onto this app's actual, durable state mechanism
instead: `set_state`, `log_event`, `record_canon`, and `update_character`.
Use the table below rather than attempting to literally "update" any file
under `02_runtime_state/`.

## The checklist, translated

| The campaign's own category | What it actually means here |
|---|---|
| Current state, location, scene | `set_state` (`location`, `clock`, `scene` keys) |
| Player character | `update_character` (HP, resources, equipment, conditions) |
| Active quests / open threads | `set_state` (`activeQuests`/`openThreads` keys) |
| Known clues / hidden clues | `set_state` (a `knownClues` key — record what the player has actually learned; never write a clue the player hasn't earned) |
| NPC memory | `record_canon` (one entry per meaningful NPC interaction: attitude shift, promise, threat, secret revealed) |
| Relationships | `record_canon` (allies/rivals/enemies/trust shifts) |
| Factions and world clocks | `set_state` (a `factionState`/`worldClocks` key per `02_runtime_state/WORLD_CLOCKS.md`'s clock list) |
| Inventory and rewards | `update_character` (inventory/gold deltas) |
| Consequences | `record_canon` (both player-known and player-unknown consequences — canon isn't only what the player has learned) |
| Session recap | `log_event` (a session-summary event; the server's own end-of-session pass also reads the event journal to build the next recap) |
| Next session start / hidden DM recap | `record_canon` + `log_event`, plus — if genuinely nothing in the authored content covers where this session left the world — `log_gap` |

## Checklist (this session)

1. **Reach a reasonable stopping point** in the fiction, per the shared
   procedure.
2. **Confirm state is current** — every mechanical change from this session's
   events is committed via `update_character`/`set_state` before the session
   ends, not just narrated.
3. **Log significant events** via `log_event` that haven't been logged yet —
   this is what both this session's recap and next session's "previously
   on…" are built from.
4. **Record improvised canon** via `record_canon` for anything from the table
   above that should persist: an NPC detail the authored content left open, a
   faction reaction, a relationship shift, a consequence (seen or unseen by
   the player).
5. **Log gaps** via `log_gap` for anywhere the authored content (500+ files
   under the numbered folders) didn't actually cover what the table needed —
   see `canon-and-gaps/SKILL.md`. This is genuinely useful signal for this
   campaign specifically: it is predetermined-first by design, so a gap
   usually means a real hole worth authoring, not just an edge case.
6. **Let the server's end-of-session pass run** — unchanged from the shared
   procedure.

## What NOT to do at session end

Same as the shared procedure: don't force a narrative resolution the player
hasn't asked for; don't leave a state change only narrated. Additionally for
this campaign: **do not attempt to write to any file under
`02_runtime_state/`, `16_ai_session_packs/`, or anywhere else in the content
tree** — the content tree is read-only at runtime (see this campaign's
`README.md`'s content-boundary description); every one of this checklist's
outcomes lands in `set_state`/`log_event`/`record_canon`/`update_character`
instead, per the table above.

## Related campaign files

- `16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md` — the full 16-category
  original, useful as a completeness reference for *what* to capture; this
  file governs *how* to actually capture it in this runtime
- `02_runtime_state/WORLD_CLOCKS.md` — the clock list to check against
  `set_state`
