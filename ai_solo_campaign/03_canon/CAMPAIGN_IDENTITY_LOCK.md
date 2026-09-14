# CAMPAIGN_IDENTITY_LOCK.md

---
type: canon
secrecy: dm-only
status: static
---

## Purpose

**DM-ONLY.** Locks the core campaign identity once established during Stage 1. These decisions — premise, central conflict, hidden truth, tone, world name, starting region — are foundational. They should not be changed casually or accidentally overwritten during content generation passes.

Before changing anything recorded in this file, consult `CANON_AUTHORITY.md` and document the revision in `CANON.md`'s revision log.

## Current Status

**LOCKED — Stage 1 complete (2026-06-09).** Core campaign identity is finalized and locked. Do not change locked fields without explicit user instruction and a revision entry in `CANON.md`.

## AI Use

Load this file when beginning any major content generation pass to confirm you are working within the locked identity. If new content contradicts anything here, stop and flag it in `CONSISTENCY_AUDIT.md` before proceeding.

---

## Locked Campaign Identity

*To be established during Stage 1. Do not modify without a formal revision entry in CANON.md.*

| Field | Value | Locked |
|---|---|---|
| Campaign name | The Long Remembering | yes |
| World name | Vael (continent: Orrun) | yes |
| Premise (one sentence) | A century after the fall of the order that "kept the dead at peace," death-rites are failing across the ruin-haunted Sundering Reach, and a frontier newcomer is drawn into why the boundary between the living and the remembered is breaking. | yes |
| Central conflict | Multiple powers race to control the Remembrance — the lingering of the dead as preservable memory — each certain only they can save or rule the world by mastering it. | yes |
| Hidden truth | DM only. The Custodian Concord secretly harvested the dead; the Quietfall was a deliberate pause; surviving Custodians (the Hollow Court) are now restarting the harvest. See `DM_ONLY_CANON.md`. | yes |
| Tone | Grounded folk-horror frontier fantasy: eerie, mysterious, morally weighty, but hopeful — not nihilistic. | yes |
| Core themes | Memory vs. truth; grief and letting go; who owns the dead; the cost of being remembered; renewal after collapse. | yes |
| Starting region | The Sundering Reach | yes |
| Starting settlement | Hollowmere | yes |
| Level 1 opening situation | Newcomer arrives in Hollowmere as a death-rite fails publicly; a body that should rest does not, and the town is frightened. | yes |
| Campaign end condition | The fate of the Remembrance is decided — sealed, freed, controlled, or transformed — determining whether the dead can finally rest. | yes |

---

## What "Locked" Means

Once a field is marked `yes`:

- It cannot be changed by a content generation pass.
- It cannot be overridden by an NPC, quest, faction, or region file.
- Changes require explicit user instruction and a revision entry in `CANON.md`.
- An AI DM running the campaign treats locked fields as permanent facts.

---

## Revision Log

| Date | Field Changed | Old Value | New Value | Reason |
|---|---|---|---|---|
| 2026-06-09 | All fields | TBD | (see table above) | Stage 1 Campaign Foundation established and locked |

---

## Related Files

- [`CANON.md`](CANON.md)
- [`DM_ONLY_CANON.md`](DM_ONLY_CANON.md)
- [`../00_control/CANON_AUTHORITY.md`](../00_control/CANON_AUTHORITY.md)
- [`../00_control/CONSISTENCY_AUDIT.md`](../00_control/CONSISTENCY_AUDIT.md)
