# CREATURE_SOURCE_REFERENCE.md — How Monster Sources Are Handled

---
type: encounter
secrecy: mixed
status: static
region: Orrun
level_range: 1-20
related: [BESTIARY_INDEX.md, ENCOUNTER_INDEX.md, ../00_control/RULESET_ASSUMPTIONS.md, ../00_control/DND_MECHANICS_REQUIREMENTS.md]
tags: [type:encounter, secrecy:mixed, function:bestiary, source-handling, copyright-safe]
---

> **Secrecy note (DM):** This file is **mixed** — the creature-handling rules are player-safe, but the thematic-link notes name DM-only arc terms (the harvest, the Hollow Court, the Custodians, the Concord Deep) as AI-DM guidance for which creatures mirror hidden truths. Do not surface those links to the player; they are DM-side placement cues.

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
- **Official chassis anchor (required as of 2026-07-07):** the published D&D stat block the creature is mechanically built on, stated as "use [creature] ([book]), modified: …". Every campaign-original creature must be runnable from a real published stat block plus stated modifications — no creature exists on invented mechanics alone. The master anchor table lives in `BESTIARY_INDEX.md` §"Track-B Official-Chassis Anchors".
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
| **VRGtR** | Van Richten's Guide to Ravenloft (2021) — the project's published gothic-horror source (32 monster stat blocks) |
| **FToD** | Fizban's Treasury of Dragons (2021) |
| **XGtE** | Xanathar's Guide to Everything (2017) |
| **TCoE** | Tasha's Cauldron of Everything (2020) |
| **GoS** | Ghosts of Saltmarsh (2019) — source of the drowned-dead series (Drowned Ascetic/Assassin/Blade/Master) |
| **ToA** | Tomb of Annihilation (2017) — appendix monsters (e.g. Assassin Vine) |
| **RtHW** | Ravenloft: The Horrors Within (2026) — **verified and integrated 2026-07-07** (released June 16 2026; 51 monster stat blocks, CR 1/2–21, largely VRGtR creatures updated to 2024 rules plus new cosmic-horror entries; see the Horror Expansion section below) |
| **source check needed** | Used in the bestiary where the exact official book is genuinely uncertain — a deliberate placeholder, never a guess |
| **(custom)** | Campaign-original; full Track-B summary given in the bestiary — **must name an official chassis anchor** (see Track B) |
| **(variant)** | A campaign reskin of an official chassis; Track-A reference + the changed behavior noted |

**Edition-preference rule:** if a creature appears in both an older book and the 2024 MM, prefer **2024 MM**. Only cite an older book when the creature is *not* in the 2024 MM. Many VGtM/MToF creatures are reprinted in **MotM (2022)**; when in doubt, cite the original book — the AI DM can use either printing.

**Citation-integrity rule (2026-07-07 verification pass):** cite **book only, never page numbers**, unless a page has been verified against the physical/digital book — earlier drafts carried invented page citations, which have been removed. Every Track-A creature name and book attribution in this repo was re-verified in the 2026-07-07 pass; do not add a new official-creature reference without confirming the creature actually appears in the named book. If it cannot be confirmed, use `source check needed` or anchor a Track-B original to a verified chassis instead.

The AI DM is assumed to have access to the referenced books. The campaign files never substitute for owning the rules; they tell the DM **what to use, where, and how to tune it for solo play**.

## Gothic-Horror Source: Van Richten's Guide to Ravenloft (VRGtR)

**VRGtR is a published, copyrighted D&D 5e sourcebook (2021), referenced here exactly like the Monster Manual — Track A only.** The campaign world (Vael / Orrun) is **original**; it is **not** Ravenloft, the Domains of Dread, or any proprietary setting. No Ravenloft place, darklord, character, deity, or domain lore is imported. We borrow only **published creature stat references** where the campaign's *own* horror themes — the Remembrance harvest, the consumed dead, grief-saturated sites, memory-loss, hollow/thin-born people — already call for that kind of creature.

**Source correction (2026-07-07 verification pass):** several gothic-horror creatures previously misattributed to VRGtR are actually **Mordenkainen's Tome of Foes (MToF)** or **Volo's Guide to Monsters (VGtM)** creatures, and one ("Caller in Darkness") **does not exist in any official 5e book** (it is a 3rd-edition psionics monster) — it has been replaced by the Sorrowsworn. The corrected reference list:

Published gothic-horror creatures that fit this campaign's themes (a Track-A reference list, **not** stat-block reproduction):

- **Oblex** (adult/spawn; **MToF**, reprinted MotM) — an ooze that **absorbs and mimics the memories** of those it consumes. The single best mechanical mirror of the Harvest in published 5e. Belongs in Remembrance-leak ruins and memory-scarred fen.
- **Allip** (**MToF**) — an incorporeal undead driven mad by a **terrible secret** it must share. A perfect Hollow-Court / harvest-secret echo.
- **Sorrowsworn** (**MToF** — the Lost CR 7, the Wretched CR 1/4, the Angry CR 13, the Hungry CR 11, the Lonely CR 9) — **grief, loss, and despair given flesh**; the published embodiment of exactly what this campaign's mass-death sites produce. The Lost fills the grief-swarm role at drift-lines and drowned towns; the Wretched hunt in pitiable packs. *(Replaces the non-official "Caller in Darkness.")*
- **Soul Monger** (**MToF**) — devours the **life force and memories** of victims; a thematic mirror of the Custodians at high tier.
- **Bodak** (**VGtM**) — soul-drained undead that spread death by gaze; a deep-node / Custodian-touched horror.
- **Deathlock** (**MToF** — Deathlock CR 4, Deathlock Wight CR 3, Deathlock Mastermind CR 8) — undead caster bound to a dark patron; reskins as a Concord-bound or Gravecaller-bound dead caster.
- **Gloom Weaver / Gray Render** (**MToF**) — shadow-realm dread and a grief-bonded brute; drawn on only where the matching theme already exists.
- **Reborn** (VRGtR, character lineage) — used **only as flavor** for thin-born / returned-wrong NPCs; not a stat block. *(Replaces the earlier "Hollow One" note — that option is from a setting book this project does not reference.)*
- **Loup garou** (VRGtR, CR 13; updated in RtHW) — pack-lord werewolf; an apex beast option for deep wilderness, used sparingly and only where lycanthrope-horror fits.
- **VRGtR's own bestiary** (verified 2021 roster) — **Death's Head** (CR 1/2), **Carrionette** (CR 1), **Jiangshi**, **Necrichor**, **Boneless**, **Bagman**, **Zombie Clot**, **Wereraven**, **Priest of Osybus**, **Dullahan**, **Gremishka**, **Strigoi**, **Nosferatu**, **Star Spawn Emissary**, **Brain in a Jar**, **Carrion Stalker** — plus **vampire spawn variants, ghost variants, will-o'-wisp (grief-flavored)** from the 2024 MM — drawn on **only** where a region's encounter design already has the matching theme; never forced.

**Track-A discipline still applies:** name + source + page (if known) + type + CR + habitat fit + encounter role + campaign thematic link + solo danger + prose tactics. **No ability lines, no verbatim action blocks, no copied trait text.** Reskins (e.g. "an oblex re-skinned as a Concord harvest-residue") state the changed theme/behavior on top of the referenced chassis.

**Do not force-fit.** A VRGtR creature is only added to a region whose existing design already carries horror, grief, memory-drain, soul-consumption, or shadow/darkness themes. Bright, mundane, or purely martial encounters stay as they were.

## Horror Expansion — Ravenloft: The Horrors Within (RtHW) — INTEGRATED

**Status: VERIFIED AND INTEGRATED (2026-07-07).** *Ravenloft: The Horrors Within* (`RtHW`) released **June 16, 2026** and has been verified as a real published sourcebook: **51 monster stat blocks (CR 1/2–21)**, the large majority being **VRGtR (2021) creatures updated to the 2024 rules**, plus a handful of new cosmic-horror entries. The earlier pre-release placeholder list in this section has been replaced with the verified roster below; unverifiable placeholder entries were **removed** per the campaign's no-invented-monsters rule.

**Track-A discipline applies (same as VRGtR):** name + source (`RtHW`, or `VRGtR / RtHW` where the creature exists in both printings) + habitat fit + encounter role + campaign thematic link + solo danger + prose tactics. **No ability lines, no verbatim action blocks, no copied trait text. No imported Ravenloft setting lore** (no Domains of Dread, darklords, domains, or the book's named NPCs as setting canon). The campaign world (Vael / Orrun) remains **original** and is **not** Ravenloft. A creature is added **only** where a site's horror theme already calls for it (no force-fitting).

### Verified RtHW/VRGtR roster in campaign use

| Creature | Verified source | Campaign thematic link | Where integrated |
|---|---|---|---|
| **Gallows Speaker** | RtHW (confirmed in the published bestiary) | **bound dead that speaks** — the harvested who "remember"; gated M5/M6 dread-vector | HORROR #H10, MYSTERY_ENCOUNTERS, Marrowdowns/Heartlands |
| **Mist Horror** | RtHW (new entry) | **memory-mist threat** — published pairing for the Mind-fog Lurker / drift-line fog | HORROR #H13, Sundering Reach, Drowned Steps |
| **Necrichor** | VRGtR / RtHW | **death-fluid horror** — "blood of the taken" at harvest-leak and curse sites | HORROR #H11, deep nodes |
| **Bodytaker Plant + Podling** | RtHW (confirmed); VRGtR-era | body-snatcher horror; the "wrong" returned | HORROR #H12 note, Hethewald deep wood |
| **Boneless** | VRGtR / RtHW | collapsed/unmade dead | HORROR #H12, drowned towns |
| **Jiangshi** | VRGtR / RtHW | hopping preserved dead; preservation-horror kin of the Salt-Mummy | HORROR #H12, Saltmere |
| **Carrionette** | VRGtR (Construct, CR 1) / RtHW | preserved-body / puppet horror | HORROR #H12, Caradril Ashmarket, Glassmere |
| **Brain in a Jar** | VRGtR / RtHW | preserved mind — the harvest's stored identity made monstrous | HORROR #H12, Concord vaults (gated) |
| **Carrion Stalker** | VRGtR / RtHW | grave/charnel predator near barrows and drowned towns | Marrowdowns, Saltmere regional tables |
| **Death's Head** | VRGtR (Undead, CR 1/2, petrifying bite) / RtHW | death-omen horror at deep nodes | regional deep-site tables |
| **Dullahan** | VRGtR / RtHW | headless herald of death; barrow/Heartlands omen | Marrowdowns, Heartlands |
| **Gremishka** | VRGtR / RtHW | minor anti-magic pest (sparing wilderness use) | optional wilderness color |
| **Loup Garou** | VRGtR (CR 13) / RtHW | apex lycanthrope; deep-wilderness only | HORROR #H9 (unchanged) |
| **Nightgaunt** | RtHW (confirmed; cosmic-horror entry) | silent flying dread (night travel; deepest ruins) — **DM-gated** | HORROR #H13 |
| **Gug** | RtHW (confirmed; cosmic-horror entry) | deep-cavern aberrant brute (Karran deeps / Drowned Steps) — **DM-gated** | HORROR #H13 |
| **Shoggoth** | RtHW (confirmed; cosmic-horror entry) | apex deep aberration — **DM-gate hard**; Drowned Steps / Concord Deep outer reach | HORROR #H13 |
| **Greater Star Spawn Emissary** | RtHW (confirmed; Star Spawn Emissary also VRGtR) | apex cosmic herald — **DM-gate hard**; tier-4 deep-horror only | HORROR #H13 |

**Exact type/CR for RtHW-only entries:** the AI DM pulls these from the published book (Track A). Where a CR is stated above it is verified from the 2021 VRGtR printing.

### Entries removed in the 2026-07-07 verification pass

The pre-release placeholder list contained entries that could **not** be verified against the published book and have been **removed from campaign use** (per the no-invented-monsters rule): *Elder Thing, Mi-Go, Yithian, Waxworks, "Strahd Skeleton," "Mordenheim's Monster," "Death's Head (Aberrant)," "Death's Head Tree," and "Mist Wanderer" (verified as an RtHW **background**, not a creature).* The three NPC placeholders (*Ez d'Avenir, Madame Eva, Rudolph Van Richten*) were removed outright — importing named setting characters would violate the campaign's originality rules regardless of stat-block availability. If a future owner of the physical book confirms any removed creature, it may be re-added under standard Track-A discipline; do not re-add on memory or secondhand claims.

## Variant / Reskin Handling

Many campaign creatures are a **reskin** of an official chassis (e.g. "use a Specter-like profile, recolored as a mournful drifting Remembrance"). For these:
- Reference the chassis (Track A: "Specter-like").
- State the **changed behavior, theme, and any tweaked numbers** as campaign-original notes (Track B-lite).
- Do not transcribe the chassis stat block; the reskin notes ride on top of the referenced creature.

This is how the signature Remembrance dead are handled: a published incorporeal-undead chassis, retuned (mournful not malicious, bound to a node, resolvable by rite) into something the campaign owns thematically.

## Copyright-Safety Confirmation

**Confirmed for Stage 13 (incl. the VRGtR supplement) and re-confirmed in the 2026-07-07 verification/RtHW pass:** No file in `13_encounters_and_bestiary/` reproduces a full official stat block — including the VRGtR and RtHW horror entries. Official creatures from all referenced books (2024 MM, 2014 MM, VRGtR, RtHW, MotM, MToF, VGtM, FToD, GoS, ToA) are **named and source-referenced** with original placement/tactics/solo notes only, and every name-and-book attribution was re-verified in the 2026-07-07 pass (misattributions corrected; one non-official creature replaced; invented page numbers removed). Original creatures carry **abbreviated prose summaries anchored to a named official chassis**, not reproduced layouts. No proprietary *setting* lore (Ravenloft domains, darklords, named NPCs/deities) is imported — only published creature references, used where the campaign's own Remembrance-horror themes already call for them. This matches `RULESET_ASSUMPTIONS.md` ("Do not copy official stat blocks verbatim. Use abbreviated D&D-compatible stat profiles.") and `DND_MECHANICS_REQUIREMENTS.md` ("Avoid copying official stat blocks verbatim").

## Related Files

- [`BESTIARY_INDEX.md`](BESTIARY_INDEX.md)
- [`ENCOUNTER_INDEX.md`](ENCOUNTER_INDEX.md)
- [`STAGE_12_ADVERSARIES.md`](STAGE_12_ADVERSARIES.md) (model Track-B file)
- [`../00_control/RULESET_ASSUMPTIONS.md`](../00_control/RULESET_ASSUMPTIONS.md)
- [`../00_control/DND_MECHANICS_REQUIREMENTS.md`](../00_control/DND_MECHANICS_REQUIREMENTS.md)
