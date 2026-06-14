# CREATURE_SOURCE_REFERENCE.md — How Monster Sources Are Handled

---
type: encounter
secrecy: player-safe
status: static
region: Orrun
level_range: 1-20
related: [BESTIARY_INDEX.md, ENCOUNTER_INDEX.md, ../00_control/RULESET_ASSUMPTIONS.md, ../00_control/DND_MECHANICS_REQUIREMENTS.md]
tags: [type:encounter, secrecy:player-safe, function:bestiary, source-handling, copyright-safe]
---

## AI Use

Load this once to understand **how the bestiary references creatures**. Every other Stage 13 file follows the conventions defined here. This file is the project's written decision on copyright-safe monster handling. Read it before adding any new creature to any encounter table.

## The Two-Track Decision

The campaign uses **two tracks** for adversaries, both D&D 5e / 2024-compatible (`RULESET_ASSUMPTIONS.md`), and **neither reproduces a full stat block**.

### Track A — Official-Monster Source Reference

For mundane and standard fantasy creatures that already exist in published 5e books, the bestiary **names the creature and points to a source**, then gives only the play-relevant notes the AI DM needs. It does **not** transcribe the stat block.

**Required fields for a Track A entry:**
- **Name** (the published creature name)
- **Source reference** — the book it appears in, in shorthand (see source key below)
- **Type, CR** (these are facts/labels, not the protected stat-block text)
- **Habitat fit** — why it belongs in the region/biome it is placed in
- **Encounter role** — skirmisher, ambusher, brute, controller, lurker, swarm, social, etc.
- **Solo-PC danger notes** — how dangerous it is to a lone PC by level band
- **Encounter tactics** — how it behaves, its morale, how to telegraph it
- **Solo adjustment** — how to add/remove bodies or scale for one PC

**Example (the approved format):**
> **Wolf** (2024 MM, Beast, CR 1/4) — pack hunter; fits Tollwood/Hethewald forests and the Wender Steppe; solo danger: low at L1, trivial at L3+. Tactics: pack tactics, tries to drop one target then harry; flees when half the pack falls. Solo adjustment: 2–3 wolves is a real L1 fight; a lone wolf is a warning sign, not a threat.

> **Wight** (2024 MM, Undead, CR 3) — fits Remembrance-corrupted burial sites (Marrowdowns barrows, Greyfens drift-line); solo danger: moderate at L3–4. Tactics: drains Constitution (life-drain), can command lesser undead, fights to "completion" not self-preservation. Telegraph: cold, a wrongly-preserved corpse, lesser dead that defer to it. Solo adjustment: run it alone (no minion pack) below L4.

**What a Track A entry must NEVER contain:**
- Full ability score lines (e.g. "STR 15 (+2), DEX 14 (+2)...")
- The full action block as printed (attack bonus, damage dice, and reach all transcribed verbatim)
- Verbatim trait text copied from the book

A single referenced number (e.g. "moderate AC, ~45 HP, multiattack for ~2d6+3") given as DM guidance is acceptable as a **paraphrased difficulty cue**, but the AI DM should pull the actual numbers from the published book if it has access. The campaign files supply *placement, role, tactics, and solo tuning* — not the publisher's stat block.

### Track B — Campaign-Original Creature / Variant

For creatures unique to the world (Remembrance-linked dead, Concord constructs, memory-echo threats, salt-desiccated undead, etc.) the bestiary gives a **full campaign-original abbreviated mechanical summary**. These are our own creations, written in an abbreviated, non-formatted style (so they are clearly original work, not a reproduced layout).

**Required fields for a Track B entry:**
- Name, type, size, CR/level band, habitat, encounter role
- Behavior, tactics, morale/retreat
- Solo danger rating
- Noncombat options
- Warning signs before the encounter
- Treasure / remains
- Linked faction / quest / mystery
- **Abbreviated D&D 5e-compatible mechanical summary:** AC, HP range, key abilities/saves, primary attacks (written in prose-abbreviated form, e.g. "AC 13, ~36 HP, fly/hover, life-drain touch ~2d6 necrotic, immune to the usual incorporeal-undead conditions") — **not** a fully formatted stat block.

`STAGE_12_ADVERSARIES.md` is the canonical example of Track B style and is the model all original creatures follow.

## Source Key (shorthand used across the bestiary)

| Shorthand | Refers to |
|---|---|
| **2024 MM** | The 2024 core Monster Manual (current edition; the default for any classic monster updated in 2024) |
| **2014 MM** | The 2014 core Monster Manual (or **MM** when a creature is not updated in 2024 and exists only there) |
| **MotM** | Mordenkainen Presents: Monsters of the Multiverse (2022) |
| **MToF** | Mordenkainen's Tome of Foes (2018) |
| **VGtM** | Volo's Guide to Monsters (2016) |
| **VRGtR** | Van Richten's Guide to Ravenloft (2021) — the project's published gothic-horror source |
| **FToD** | Fizban's Treasury of Dragons (2021) |
| **XGtE** | Xanathar's Guide to Everything (2017) |
| **TCoE** | Tasha's Cauldron of Everything (2020) |
| **RtHW** | Ravenloft: The Horrors Within (2026) — **pending; not yet integrated** (releases June 16 2026; see the Horror Expansion Supplement section below) |
| **source check needed** | Used in the bestiary where the exact official book is genuinely uncertain — a deliberate placeholder, never a guess |
| **(custom)** | Campaign-original; full Track-B summary given in the bestiary |
| **(variant)** | A campaign reskin of an official chassis; Track-A reference + the changed behavior noted |

**Edition-preference rule:** if a creature appears in both an older book and the 2024 MM, prefer **2024 MM**. Only cite an older book when the creature is *not* in the 2024 MM.

The AI DM is assumed to have access to the referenced books. The campaign files never substitute for owning the rules; they tell the DM **what to use, where, and how to tune it for solo play**.

## Gothic-Horror Source: Van Richten's Guide to Ravenloft (VRGtR)

**VRGtR is a published, copyrighted D&D 5e sourcebook (2021), referenced here exactly like the Monster Manual — Track A only.** The campaign world (Vael / Orrun) is **original**; it is **not** Ravenloft, the Domains of Dread, or any proprietary setting. No Ravenloft place, darklord, character, deity, or domain lore is imported. We borrow only **published creature stat references** where the campaign's *own* horror themes — the Remembrance harvest, the consumed dead, grief-saturated sites, memory-loss, hollow/thin-born people — already call for that kind of creature.

Why VRGtR fits this campaign's themes (a Track-A reference list, **not** stat-block reproduction):

- **Oblex** (adult/spawn; VRGtR) — an ooze that **absorbs and mimics the memories** of those it consumes. The single best mechanical mirror of the Harvest in published 5e. Belongs in Remembrance-leak ruins and memory-scarred fen.
- **Allip** (VRGtR) — an incorporeal undead driven mad by a **terrible secret** it must share. A perfect Hollow-Court / harvest-secret echo.
- **Caller in Darkness** (VRGtR) — a swarm of **tormented, collected souls**; the literal grief-swarm of a mass-death site (drift-lines, drowned towns).
- **Soul Monger** (VRGtR) — devours the **life force and memories** of victims; a thematic mirror of the Custodians at high tier.
- **Bodak** (VRGtR / MToF) — soul-drained undead that spread death by gaze; a deep-node / Custodian-touched horror.
- **Deathlock** (VRGtR / MToF) — undead caster bound to a dark patron; reskins as a Concord-bound or Gravecaller-bound dead caster.
- **Hollow One** (VRGtR, character option) — used **only as flavor** for thin-born / hollow-interior NPCs; not a stat block.
- **Loup garou** (VRGtR, CR 13) — pack-lord werewolf; an apex beast option for deep wilderness, used sparingly and only where lycanthrope-horror fits.
- **Nosferatu / vampiric mist / vampire spawn variants, ghost variants, will-o'-wisp (grief-flavored), gloom weaver, gray render, dullahan, death's head** (VRGtR) — drawn on **only** where a region's encounter design already has the matching theme; never forced.

**Track-A discipline still applies:** name + source + page (if known) + type + CR + habitat fit + encounter role + campaign thematic link + solo danger + prose tactics. **No ability lines, no verbatim action blocks, no copied trait text.** Reskins (e.g. "an oblex re-skinned as a Concord harvest-residue") state the changed theme/behavior on top of the referenced chassis.

**Do not force-fit.** A VRGtR creature is only added to a region whose existing design already carries horror, grief, memory-drain, soul-consumption, or shadow/darkness themes. Bright, mundane, or purely martial encounters stay as they were.

## Horror Expansion Supplement (Pending) — Ravenloft: The Horrors Within (RtHW)

**Status: PENDING. Not yet integrated.** *Ravenloft: The Horrors Within* (`RtHW`) releases **June 16, 2026** — **after** Stage 13 completion (2026-06-14). At Stage 13 completion the full RtHW bestiary was **not yet available**, so no RtHW creature has been placed in any encounter table yet. This section is a **placeholder list** so a later supplement pass can integrate the apt creatures quickly and safely.

**Why RtHW fits this campaign:** like VRGtR, RtHW is a published D&D 5e gothic-horror sourcebook. Several of its creatures mirror the campaign's **Remembrance / harvest** cosmology — memory-mist, bound dead who speak, preserved-body horror, death-fluid seeping from old wounds, undead that will not stay down. These map directly onto the world's themes of grief, forgetting, the consumed dead, and the thin-born/hollow.

**Same Track-A discipline as VRGtR will apply on integration:** name + source (`RtHW`) + type + CR + habitat fit + encounter role + campaign thematic link + solo danger + prose tactics. **No ability lines, no verbatim action blocks, no copied trait text. No imported Ravenloft setting lore** (no Domains of Dread, darklords, domains, or the book's named NPCs as setting canon). The campaign world (Vael / Orrun) remains **original** and is **not** Ravenloft. Add a creature **only** where a site's horror theme already calls for it (do not force-fit).

### Confirmed partial RtHW creature list (from pre-release reviews — placeholders only)

Each is marked **(source check needed — RtHW)** because exact type/CR/page must be confirmed against the printed book before use. NPC entries are flagged; they would be used (if at all) **only as published-creature references**, never as imported setting characters.

| Creature (placeholder) | Status | Likely campaign thematic link |
|---|---|---|
| Bodytaker Plant | source check needed — RtHW | body-snatcher horror; the "wrong" returned |
| Bodytaker Podling | source check needed — RtHW | lesser body-snatcher; infiltration dread |
| Boneless | source check needed — RtHW | collapsed/unmade dead |
| Brain in a Jar | source check needed — RtHW | preserved mind; the harvest's stored identity made monstrous |
| Carrion Stalker | source check needed — RtHW | grave/charnel predator near barrows and drowned towns |
| Carrionette | source check needed — RtHW | preserved-body / puppet horror (Waxworks family) |
| Death's Head (Aberrant) | source check needed — RtHW | death-omen horror at deep nodes |
| Death's Head (Petrifying) | source check needed — RtHW | death-gaze variant for deep harvest-scarred sites |
| Death's Head Tree | source check needed — RtHW | grief-fed flora (mirrors the custom Grave-Bloom) |
| Dullahan | source check needed — RtHW | headless herald of death; barrow/Heartlands omen |
| Elder Thing | source check needed — RtHW | deep-cosmic aberration (Drowned Steps / deepest nodes) |
| Ez d'Avenir **(NPC)** | source check needed — RtHW | reference only if ever used; not imported as setting canon |
| **Gallows Speaker** | source check needed — RtHW | **bound dead that speaks** — fits the harvested who "remember"; M5/M6 dread-vector |
| Gremishka | source check needed — RtHW | minor anti-magic pest (sparing wilderness use) |
| Gug | source check needed — RtHW | deep-cavern aberrant brute (Karran deeps / Drowned Steps) |
| Jiangshi | source check needed — RtHW | hopping preserved dead; preservation-horror like the Salt-Mummy |
| Loup Garou | source check needed — RtHW (also VRGtR) | apex lycanthrope; deep-wilderness only (already in VRGtR list) |
| Madame Eva **(NPC)** | source check needed — RtHW | reference only if ever used; not imported as setting canon |
| Mi-Go | source check needed — RtHW | brain-harvesting aberration; uncanny mirror of the harvest (deep/gated) |
| **Mist Horror** | source check needed — RtHW | **memory-mist threat** — strong mirror of the Memory-Echo Haunt / Mind-fog Lurker |
| Mist Wanderer | source check needed — RtHW | mist-bound lost dead; drift-line / fog flavor |
| Mordenheim's Monster | source check needed — RtHW | stitched-dead horror (deep-cult / Emberfell heresy) |
| **Necrichor** | source check needed — RtHW | **death-fluid seeping from old wounds** — fits harvest-leak ooze/curse sites |
| Nightgaunt | source check needed — RtHW | silent flying dread (night travel; deep ruins) |
| Rudolph Van Richten **(NPC)** | source check needed — RtHW | reference only if ever used; not imported as setting canon |
| Shoggoth | source check needed — RtHW | apex deep aberration (DM-gate hard; Drowned Steps / Concord Deep outer reach) |
| **Strahd Skeleton** | source check needed — RtHW | **undead that won't stay down** — fits the relentless harvest-dead |
| **Waxworks** | source check needed — RtHW | **preserved-body horror** — direct mirror of the harvest's kept dead |
| Yithian | source check needed — RtHW | mind-swapping aberration (deep/gated; harvest-of-identity echo) |

**Strongest thematic fits (prioritize on integration):** **Mist Horror** (memory-mist), **Gallows Speaker** (bound dead that speaks), **Waxworks** / **Carrionette** / **Jiangshi** (preserved-body horror), **Necrichor** (death-fluid from old wounds), **Strahd Skeleton** (the dead that won't stay down), **Brain in a Jar** (stored identity). These align tightly with the Remembrance/harvest/grief spine.

### Where a later RtHW pass should add entries

When the book is accessible, run a focused supplement pass and add the apt creatures (Track-A) to:
- `HORROR_AND_CURSE_THREATS.md` — the primary home for reskinned RtHW horror (alongside the VRGtR §).
- `BESTIARY_INDEX.md` — index rows with `A · RtHW` source shorthands.
- `MYSTERY_ENCOUNTERS.md` — for any RtHW creature that delivers a clue fragment (e.g. a Gallows Speaker / Mist Horror as an M5/M6 vector; keep fragments gated).
- Deep-horror regional files: `SUNDERING_REACH_ENCOUNTERS.md`, `CONCORD_HEARTLANDS_ENCOUNTERS.md`, `MARROWDOWNS_ENCOUNTERS.md`, `SALTMERE_REACHES_ENCOUNTERS.md`, `DROWNED_STEPS_ENCOUNTERS.md`, `HETHEWALD_ENCOUNTERS.md`.

This pass is logged as a low-priority item in `TODO.md` / `CONTENT_GAPS.md` and as an `OPEN_QUESTIONS.md` entry, gated on the June 16 2026 release.

## Variant / Reskin Handling

Many campaign creatures are a **reskin** of an official chassis (e.g. "use a Specter-like profile, recolored as a mournful drifting Remembrance"). For these:
- Reference the chassis (Track A: "Specter-like").
- State the **changed behavior, theme, and any tweaked numbers** as campaign-original notes (Track B-lite).
- Do not transcribe the chassis stat block; the reskin notes ride on top of the referenced creature.

This is how the signature Remembrance dead are handled: a published incorporeal-undead chassis, retuned (mournful not malicious, bound to a node, resolvable by rite) into something the campaign owns thematically.

## Copyright-Safety Confirmation

**Confirmed for Stage 13 (incl. the VRGtR supplement):** No file in `13_encounters_and_bestiary/` reproduces a full official stat block — including the Van Richten's Guide to Ravenloft entries added in the horror supplement. Official creatures from all referenced books (2024 MM, VRGtR, MotM, MToF, VGtM, FToD) are **named and source-referenced** with original placement/tactics/solo notes only. Original creatures carry **abbreviated prose summaries**, not reproduced layouts. No proprietary *setting* lore (Ravenloft domains, darklords, named NPCs/deities) is imported — only published creature references, used where the campaign's own Remembrance-horror themes already call for them. This matches `RULESET_ASSUMPTIONS.md` ("Do not copy official stat blocks verbatim. Use abbreviated D&D-compatible stat profiles.") and `DND_MECHANICS_REQUIREMENTS.md` ("Avoid copying official stat blocks verbatim").

## Related Files

- [`BESTIARY_INDEX.md`](BESTIARY_INDEX.md)
- [`ENCOUNTER_INDEX.md`](ENCOUNTER_INDEX.md)
- [`STAGE_12_ADVERSARIES.md`](STAGE_12_ADVERSARIES.md) (model Track-B file)
- [`../00_control/RULESET_ASSUMPTIONS.md`](../00_control/RULESET_ASSUMPTIONS.md)
- [`../00_control/DND_MECHANICS_REQUIREMENTS.md`](../00_control/DND_MECHANICS_REQUIREMENTS.md)
