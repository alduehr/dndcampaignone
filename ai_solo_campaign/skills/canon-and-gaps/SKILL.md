---
visibility: dm-only
title: Canon & Gaps
---
# Canon & Gaps

Read this whenever you improvise a fact that isn't already in the authored
content, notice the authored content doesn't cover something the table
needs, or need to decide what a mystery's answer is safe to reveal right
now. This overlays the shared canon-and-gaps procedure — its authority
hierarchy and `record_canon`/`log_gap` split both apply unchanged and are not
repeated in full here; this file adds two things this campaign specifically
needs: a finer authority order for when **authored files disagree with each
other**, and a hard reveal-gating discipline for this campaign's central
mysteries.

## Authority hierarchy, refined

The shared procedure's three tiers (authored content > session canon >
unrecorded improvisation) hold exactly as written. Within tier 1 ("authored
content"), when two authored files disagree with each other, this campaign
has its own documented precedence order — read
`00_control/CANON_AUTHORITY.md` for the full list. Do not resolve such a
contradiction silently: if it affects canon, treat it as a `log_gap`-worthy
finding.

## Reveal gating — this campaign's central discipline

This is a **predetermined mystery campaign**: the true answers to its central
questions already exist in the authored content (`03_canon/DM_ONLY_CANON.md`,
`11_mysteries_and_secrets/`), but they are gated to be **earned through play,
not narrated because the DM read the file.** Reading a `dm-only`-tagged file
via `read_file` means you now know the truth — it does **not** mean the
player has learned it, and it does not license narrating it.

- **Never narrate a `dm-only`-visibility file's content verbatim to the
  player** — this is a system-prompt non-negotiable, and it is *especially*
  load-bearing for this campaign, where most files carry hidden truth mixed
  in with player-safe scene description in the same document.
- **Check the reveal gate before revealing anything mystery-adjacent.**
  `11_mysteries_and_secrets/REVELATION_MAP.md` defines this campaign's
  numbered revelations (REV_001–REV_010) and what must happen in play before
  each becomes safe to reveal — usually discovering a specific number of
  independent clues, not just asking the right question. `01_runner_protocol/
  SECRET_REVEAL_PROTOCOL.md` and `AI_DM_CORE_RULES.md`'s "Secret Policy"
  section cover the general discipline (reveal only when earned: a
  discovered clue, an NPC's own choice to reveal, a consequence that exposes
  the truth, or the player connecting evidence themselves — never because the
  DM "knows").
- **Track what the player has actually learned**, not what you know, via
  `set_state`'s `knownClues` key (see `session-end.md`, this overlay). Before
  narrating a reveal, check that key — if the player hasn't actually earned
  it yet, they don't know it yet, regardless of what any authored file says.
- **Act 1 (levels 1–4) has a hard reveal cap:** only "R1" — the failures have
  a source and a pattern — may surface. The Concord's harvest, the Hollow
  Court, Remembrance-as-substance, and any named villain's true allegiance
  are Act 2+ material; see `12_campaign_arc/ACT_1_LEVELS_1_4.md`.

## `record_canon` in this campaign

Two additional cases, on top of the shared procedure's list, come up often
in this campaign specifically:

- **Naming anything new** (an NPC, a place, a faction, an item) — before
  inventing a name, check `00_control/NAMING_REGISTRY.md` for collisions with
  already-registered proper nouns. If the new name is significant enough that
  it should be tracked long-term, log a gap noting it should be added to the
  registry.
- **A clue the player discovers** — record which specific clue (by its ID in
  `11_mysteries_and_secrets/CLUE_INDEX.md` if it has one) was found, not just
  the narrative outcome, so the reveal-gating check above stays accurate
  across sessions.

## `log_gap` in this campaign

Same purpose as the shared procedure describes. Two things worth noting for
this campaign specifically: (1) far-continent regions (outside the
NW-cluster starting area) are deliberately layered rather than fully
deep-built — a gap logged there about a specific missing settlement detail
is expected and useful, not a sign something is broken; (2) this campaign is
actively authored — gaps logged here are exactly the kind of signal its own
production workflow (`00_control/PRODUCTION_WORKFLOW.md`) is designed to
consume.

## Related campaign files

- `00_control/CANON_AUTHORITY.md` — the full authored-file precedence order
- `11_mysteries_and_secrets/REVELATION_MAP.md` — the reveal-gate definitions
- `01_runner_protocol/SECRET_REVEAL_PROTOCOL.md` · `01_runner_protocol/
  AI_DM_CORE_RULES.md` (Secret Policy)
- `00_control/NAMING_REGISTRY.md`
